# Comparing `tmp/noaa_coops-0.2.1.tar.gz` & `tmp/noaa_coops-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noaa_coops-0.2.1.tar", max compression
+gzip compressed data, was "noaa_coops-0.2.2.tar", max compression
```

## Comparing `noaa_coops-0.2.1.tar` & `noaa_coops-0.2.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35141 2023-02-06 03:59:54.090196 noaa_coops-0.2.1/LICENSE
--rw-r--r--   0        0        0     5499 2023-02-06 03:59:54.090196 noaa_coops-0.2.1/README.md
--rw-r--r--   0        0        0      101 2023-02-06 03:59:54.090196 noaa_coops-0.2.1/noaa_coops/__init__.py
--rw-r--r--   0        0        0    37849 2023-02-06 03:59:54.090196 noaa_coops-0.2.1/noaa_coops/station.py
--rw-r--r--   0        0        0     1564 2023-02-06 03:59:54.090196 noaa_coops-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     6504 1970-01-01 00:00:00.000000 noaa_coops-0.2.1/setup.py
--rw-r--r--   0        0        0     6385 1970-01-01 00:00:00.000000 noaa_coops-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    35141 2023-02-05 16:17:34.880061 noaa_coops-0.2.2/LICENSE
+-rw-r--r--   0        0        0     5499 2023-02-07 01:49:14.952908 noaa_coops-0.2.2/README.md
+-rw-r--r--   0        0        0      101 2023-04-17 06:04:01.773060 noaa_coops-0.2.2/noaa_coops/__init__.py
+-rw-r--r--   0        0        0    35861 2023-04-17 06:04:01.773911 noaa_coops-0.2.2/noaa_coops/station.py
+-rw-r--r--   0        0        0     1564 2023-04-17 06:04:01.774618 noaa_coops-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     6504 1970-01-01 00:00:00.000000 noaa_coops-0.2.2/setup.py
+-rw-r--r--   0        0        0     6385 1970-01-01 00:00:00.000000 noaa_coops-0.2.2/PKG-INFO
```

### Comparing `noaa_coops-0.2.1/LICENSE` & `noaa_coops-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `noaa_coops-0.2.1/README.md` & `noaa_coops-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `noaa_coops-0.2.1/noaa_coops/station.py` & `noaa_coops-0.2.2/noaa_coops/station.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,29 @@
 
 import pandas as pd
 import requests
 import zeep
 from pandas import json_normalize
 
 
+class COOPSAPIError(Exception):
+    """Raised when a NOAA CO-OPS API request returns an error."""
+
+    def __init__(self, message: str, error: dict) -> None:
+        """Initialize COOPSAPIError.
+
+        Args:
+            message (str): The error message.
+            error (dict): The error dict returned by the NOAA CO-OPS API.
+        """
+        self.message = message
+        self.error = error
+        super().__init__(self.message)
+
+
 def get_stations_from_bbox(
     lat_coords: list[float, float],
     lon_coords: list[float, float],
 ) -> list[str]:
     """Return a list of stations IDs found within a bounding box.
 
     Args:
@@ -96,21 +111,17 @@
             "datainventory/wsdl/DataInventory.wsdl"
         )
         client = zeep.Client(wsdl=wsdl)
         response = client.service.getDataInventory(self.id)["parameter"]
         names = [x["name"] for x in response]
         starts = [x["first"] for x in response]
         ends = [x["last"] for x in response]
-
-        unique_names = []
-        for name in names:
-            if name not in unique_names:
-                unique_names.append(name)
-
+        unique_names = list(set(names))
         inventory_dict = {}
+
         for name in unique_names:
             idxs = [i for i, x in enumerate(names) if x == name]
             inventory_dict[name] = {
                 "start_date": [starts[i] for i in idxs][0],
                 "end_date": [ends[i] for i in idxs][-1],
             }
 
@@ -128,22 +139,19 @@
             "nearby,bins,deployments,currentpredictionoffsets,"
             "floodlevels"
         )
         units_for_url = "?units=" + self.units
         metadata_url = (
             metadata_base_url + self.id + extension + metadata_expand + units_for_url
         )
-
-        # Get response from Metadata API
         response = requests.get(metadata_url)
         json_dict = response.json()
         station_metadata = json_dict["stations"][0]
 
-        # Determine station type, then assign class attributes accordingly from
-        # metadata
+        # Set class attributes base on provided metadata
         if "datums" in station_metadata:  # if True --> water levels
             self.metadata = station_metadata
             self.affiliations = station_metadata["affiliations"]
             self.benchmarks = station_metadata["benchmarks"]
             self.datums = station_metadata["datums"]
             # self.details = station_metadata['details']  # Only 4 water levels
             self.disclaimers = station_metadata["disclaimers"]
@@ -227,26 +235,26 @@
             self.affiliations = station_metadata["affiliations"]
             self.ports_code = station_metadata["portscode"]
             self.products = station_metadata["products"]
             self.disclaimers = station_metadata["disclaimers"]
             self.notices = station_metadata["notices"]
             self.tide_type = station_metadata["tideType"]
 
-    def _build_query_url(
+    def _build_request_url(
         self,
         begin_date: str,
         end_date: str,
         product: str,
         datum: Optional[str] = None,
         bin_num: Optional[int] = None,
         interval: Optional[Union[str, int]] = None,
         units: Optional[str] = "metric",
         time_zone: Optional[str] = "gmt",
     ) -> str:
-        """Build query URL for NOAA CO-OPS API.
+        """Build a request URL for the NOAA CO-OPS API.
 
         See: https://tidesandcurrents.noaa.gov/api/
 
         Args:
             begin_date (str): Start date of the data to be fetched.
             end_date (str): End date of the data to be fetched.
             product (str): Data product to be fetched.
@@ -258,269 +266,220 @@
             time_zone (str, optional): Time zone used when returning fetched data.
                 Defaults to "gmt".
 
         Raises:
             ValueError: One of the specified arguments is invalid.
 
         Returns:
-            str: Query URL for NOAA CO-OPS API.
+            str: Request URL for NOAA CO-OPS API.
         """
         base_url = "https://api.tidesandcurrents.noaa.gov/api/prod/datagetter?"
 
-        # If the data product is water levels, check that a datum is specified
         if product == "water_level":
             if datum is None:
                 raise ValueError(
                     "No datum specified for water level data. See"
                     " https://tidesandcurrents.noaa.gov/api/#datum "
                     "for list of available datums"
                 )
             else:
-                # Compile parameter string for use in URL
                 parameters = {
                     "begin_date": begin_date,
                     "end_date": end_date,
                     "station": self.id,
                     "product": product,
                     "datum": datum,
                     "units": units,
                     "time_zone": time_zone,
                     "application": "noaa_coops",
                     "format": "json",
                 }
 
+                if interval is not None:
+                    parameters["interval"] = interval
+
         elif product == "hourly_height":
             if datum is None:
                 raise ValueError(
                     "No datum specified for water level data. See"
                     " https://tidesandcurrents.noaa.gov/api/#datum "
                     "for list of available datums"
                 )
             else:
-                # Compile parameter string for use in URL
                 parameters = {
                     "begin_date": begin_date,
                     "end_date": end_date,
                     "station": self.id,
                     "product": product,
                     "datum": datum,
                     "units": units,
                     "time_zone": time_zone,
                     "application": "noaa_coops",
                     "format": "json",
                 }
+
         elif product == "high_low":
             if datum is None:
                 raise ValueError(
                     "No datum specified for water level data. See"
                     " https://tidesandcurrents.noaa.gov/api/#datum "
                     "for list of available datums"
                 )
             else:
-                # Compile parameter string for use in URL
                 parameters = {
                     "begin_date": begin_date,
                     "end_date": end_date,
                     "station": self.id,
                     "product": product,
                     "datum": datum,
                     "units": units,
                     "time_zone": time_zone,
                     "application": "noaa_coops",
                     "format": "json",
                 }
 
         elif product == "predictions":
-            # If no interval provided, return 6-min predictions data
-            if interval is None:
-                # Compile parameter string for use in URL
-                parameters = {
-                    "begin_date": begin_date,
-                    "end_date": end_date,
-                    "station": self.id,
-                    "product": product,
-                    "datum": datum,
-                    "units": units,
-                    "time_zone": time_zone,
-                    "application": "noaa_coops",
-                    "format": "json",
-                }
+            parameters = {
+                "begin_date": begin_date,
+                "end_date": end_date,
+                "station": self.id,
+                "product": product,
+                "datum": datum,
+                "units": units,
+                "time_zone": time_zone,
+                "application": "noaa_coops",
+                "format": "json",
+            }
 
-            else:
-                # Compile parameter string, including interval, for use in URL
-                parameters = {
-                    "begin_date": begin_date,
-                    "end_date": end_date,
-                    "station": self.id,
-                    "product": product,
-                    "datum": datum,
-                    "interval": interval,
-                    "units": units,
-                    "time_zone": time_zone,
-                    "application": "noaa_coops",
-                    "format": "json",
-                }
+            if interval is not None:
+                parameters["interval"] = interval
 
-        # If the data product is currents, check that a bin number is specified
         elif product == "currents":
             if bin_num is None:
                 raise ValueError(
                     "No bin specified for current data. Bin info can be "
                     "found on the station info page"
                     " (e.g., https://tidesandcurrents.noaa.gov/cdata/StationInfo?id=PUG1515)"  # noqa
                 )
             else:
-                # Compile parameter string for use in URL
                 parameters = {
                     "begin_date": begin_date,
                     "end_date": end_date,
                     "station": self.id,
                     "product": product,
                     "bin": str(bin_num),
                     "units": units,
                     "time_zone": time_zone,
                     "application": "noaa_coops",
                     "format": "json",
                 }
 
-        # For all other data types (e.g., meteoroligcal conditions)
-        else:
-            # If no interval provided, return 6-min met data
-            if interval is None:
-                # Compile parameter string for use in URL
-                parameters = {
-                    "begin_date": begin_date,
-                    "end_date": end_date,
-                    "station": self.id,
-                    "product": product,
-                    "units": units,
-                    "time_zone": time_zone,
-                    "application": "noaa_coops",
-                    "format": "json",
-                }
-            else:
-                # Compile parameter string, including interval, for use in URL
-                parameters = {
-                    "begin_date": begin_date,
-                    "end_date": end_date,
-                    "station": self.id,
-                    "product": product,
-                    "interval": interval,
-                    "units": units,
-                    "time_zone": time_zone,
-                    "application": "noaa_coops",
-                    "format": "json",
-                }
+        else:  # All other data types (e.g., meteoroligcal conditions)
+            parameters = {
+                "begin_date": begin_date,
+                "end_date": end_date,
+                "station": self.id,
+                "product": product,
+                "interval": interval,
+                "units": units,
+                "time_zone": time_zone,
+                "application": "noaa_coops",
+                "format": "json",
+            }
+
+            if interval is not None:
+                parameters["interval"] = interval
 
-        # Build URL with requests library
-        query_url = requests.Request("GET", base_url, params=parameters).prepare().url
+        request_url = requests.Request("GET", base_url, params=parameters).prepare().url
 
-        return query_url
+        return request_url
 
     def _url2pandas(
         self, data_url: str, product: str, num_request_blocks: int
     ) -> pd.DataFrame:
-        """Fetch data from NOAA CO-OPS API based on URL. Returns as Pandas DataFrame.
+        """Request data from CO-OPS API and handle response. Return data in DataFrame.
+
+        Handles 4 scenarios based on the original request from the end user:
+            1. Single 'block' request, no error in response from API
+            2. Single 'block' request, error in response from API
+            3. Multiple 'block' request, no error in response from API
+            4. Multiple 'block' request, error in response from API
 
         Args:
             data_url (str): The URL to fetch data from.
             product (str): The data product being fetched.
             num_request_blocks (int): The number of blocks of data requested.
 
         Raises:
-            ValueError: An error occurred when fetching data from the NOAA CO-OPS API.
+            COOPSAPIError: Error occurred while fetching data from the NOAA CO-OPS API.
 
         Returns:
             DataFrame: Pandas DataFrame containing data from NOAA CO-OPS API.
         """
-        response = requests.get(data_url)  # Get JSON data from URL
-        json_dict = response.json()  # Create a dictionary from JSON data
-
-        df = pd.DataFrame()  # Initialize a empty DataFrame
-
-        # Error when the requested begin_date and/or end_date doesn't have data
-        large_data_gap_error = (
+        df = pd.DataFrame()
+        response = requests.get(data_url)
+        json_dict = response.json()
+        no_data_error = (  # Error message when no data is found
             "No data was found. This product may not be "
             "offered at this station at the "
             "requested time."
         )
 
-        # Handle .get_data() request size & errors from CO-OPS API, cases below:
-        # 1. .get_data() makes a large request (i.e. >1 block requests)
-        #    and an error occurs in one of the individual blocks of data
-
-        # 2. .get_data() makes a large request (i.e. >1 block requests) and
-        #    an error does not occur in one of the individual blocks of data
-
-        # 3. .get_data() makes a small request (i.e. 1 request)
-        #    and an error occurs in the data requested
-
-        # 4. .get_data() makes a small request (i.e. 1 request)
-        #    and an error does not occur in the data requested
-
-        # Case 1
-        if (num_request_blocks > 1) and ("error" in json_dict):
-            error_message = json_dict["error"].get("message", "Error retrieving data")
-            error_message = error_message.lstrip()
-            error_message = error_message.rstrip()
-
-            if error_message == large_data_gap_error:
-                return df  # Return the empty DataFrame
-            else:
-                raise ValueError(
-                    json_dict["error"].get("message", "Error retrieving data")
-                )
-
-        # Case 2
-        elif (num_request_blocks > 1) and ("error" not in json_dict):
-            if product == "predictions":
-                key = "predictions"
-            else:
-                key = "data"
-
-            df = json_normalize(json_dict[key])  # Parse JSON dict to dataframe
+        if "error" not in json_dict:  # Case 1 or 3 (no error in response)
+            key = "predictions" if product == "predictions" else "data"
+            df = json_normalize(json_dict[key])
 
             return df
 
-        # Case 3
-        elif (num_request_blocks == 1) and ("error" in json_dict):
-            raise ValueError(json_dict["error"].get("message", "Error retrieving data"))
-
-        # Case 4
-        else:
-            if product == "predictions":
-                key = "predictions"
+        else:  # Case 2 or 4 (error in response)
+            if num_request_blocks == 1:
+                error_message = (
+                    json_dict["error"]
+                    .get("message", "Error retrieving data")
+                    .lstrip()
+                    .rstrip()
+                )
+                raise COOPSAPIError(error_message, json_dict["error"])
             else:
-                key = "data"
-
-            df = json_normalize(json_dict[key])  # Parse JSON dict to dataframe
-
-            return df
+                if json_dict["error"]["message"] == no_data_error:
+                    return df
+                else:
+                    error_message = (
+                        json_dict["error"]
+                        .get("message", "Error retrieving data")
+                        .lstrip()
+                        .rstrip()
+                    )
+                    raise COOPSAPIError(error_message, json_dict["error"])
 
     def _parse_known_date_formats(self, dt_string: str):
-        """Parse known date formats.
+        """Parse known date formats and return a datetime object.
 
         Args:
             dt_string (str): The date string to parse.
 
         Raises:
             ValueError: Invalid date format was provided.
 
         Returns:
             datetime: The parsed date.
         """
         for fmt in ("%Y%m%d", "%Y%m%d %H:%M", "%m/%d/%Y", "%m/%d/%Y %H:%M"):
             try:
                 return datetime.strptime(dt_string, fmt)
             except ValueError:
-                raise ValueError(
-                    "No valid date format found."
-                    "See https://tidesandcurrents.noaa.gov/api/ "
-                    "for list of accepted date formats."
-                )
+                match = False  # Flag indicating no match for current format
+                pass
+
+        if not match:  # No match after trying all formats
+            raise ValueError(
+                f"Invalid date format '{dt_string}' provided."
+                "See https://tidesandcurrents.noaa.gov/api/ "
+                "for list of accepted date formats."
+            )
 
     def get_data(
         self,
         begin_date: str,
         end_date: str,
         product: str,
         datum: Optional[str] = None,
@@ -542,131 +501,107 @@
             units (str, optional): Units of fetched data. Defaults to "metric".
             time_zone (str, optional): Time zone used when returning fetched data.
                 Defaults to "gmt".
 
         Returns:
             DataFrame: Pandas DataFrame containing data from NOAA CO-OPS API.
         """
-        # Convert dates to datetime objects so deltas can be calculated
         begin_datetime = self._parse_known_date_formats(begin_date)
         end_datetime = self._parse_known_date_formats(end_date)
         delta = end_datetime - begin_datetime
 
-        # If the length of our data request is less or equal to 31 days,
-        # we can pull the data from API in one request
+        # If the length of the data request is less or equal to 31 days,
+        # make a single request to the API
         if delta.days <= 31:
-            data_url = self._build_query_url(
+            data_url = self._build_request_url(
                 begin_datetime.strftime("%Y%m%d %H:%M"),
                 end_datetime.strftime("%Y%m%d %H:%M"),
                 product,
                 datum,
                 bin_num,
                 interval,
                 units,
                 time_zone,
             )
 
             df = self._url2pandas(data_url, product, num_request_blocks=1)
 
-        # If the length of the user specified data request is < 365 days
-        # AND the product is hourly_height or high_low, we can pull data
-        # directly from the API in one request
+        # If the length of the data request is < 365 days AND the product is
+        # hourly_height or high_low, make a single request to the API
         elif delta.days <= 365 and (
             product == "hourly_height" or product == "high_low"
         ):
-            data_url = self._build_query_url(
+            data_url = self._build_request_url(
                 begin_date,
                 end_date,
                 product,
                 datum,
                 bin_num,
                 interval,
                 units,
                 time_zone,
             )
-
             df = self._url2pandas(data_url, product, num_request_blocks=1)
 
-        # If the length of the user specified data request is greater than 365
-        # days AND the product is hourly_height or high_low, we need to load
-        # data from the API in 365 day blocks.
+        # If the data request is greater than 365 days AND the product is
+        # hourly_height or high_low, make multiple requests to the API in 365 day blocks
         elif product == "hourly_height" or product == "high_low":
-            # Find the number of 365 day blocks in our desired period,
-            # constrain the upper limit of index in the for loop to follow
+            df = pd.DataFrame([])
             num_365day_blocks = int(math.floor(delta.days / 365))
 
-            df = pd.DataFrame([])  # Empty dataframe for data from API requests
-
-            # Loop through in 365 day blocks,
-            # adjust the begin_datetime and end_datetime accordingly,
-            # make a request to the NOAA CO-OPS API
+            # Loop through 365 day blocks, update request params accordingly
             for i in range(num_365day_blocks + 1):
                 begin_datetime_loop = begin_datetime + timedelta(days=(i * 365))
                 end_datetime_loop = begin_datetime_loop + timedelta(days=365)
-
-                # If end_datetime_loop of the current 365 day block is greater
-                # than end_datetime specified by user, use end_datetime
-                if end_datetime_loop > end_datetime:
-                    end_datetime_loop = end_datetime
-
-                # Build url for each API request as we proceed through the loop
-                data_url = self._build_query_url(
+                end_datetime_loop = (
+                    end_datetime
+                    if end_datetime_loop > end_datetime
+                    else end_datetime_loop
+                )
+                data_url = self._build_request_url(
                     begin_datetime_loop.strftime("%Y%m%d"),
                     end_datetime_loop.strftime("%Y%m%d"),
                     product,
                     datum,
                     bin_num,
                     interval,
                     units,
                     time_zone,
                 )
+                df_block = self._url2pandas(data_url, product, num_365day_blocks)
+                df = pd.concat([df, df_block])
 
-                # Get dataframe for block and append to time series df
-                df_new = self._url2pandas(data_url, product, num_365day_blocks)
-                df = pd.concat([df, df_new])
-
-        # If the length of the user specified data request is greater than 31
-        # days for any other products, we need to load data from the API in 31
-        # day blocks
+        # If any other product is requested for >31 days, make multiple requests to the
+        # API in 31 day blocks
         else:
-            # Find the number of 31 day blocks in our desired period,
-            # constrain the upper limit of index in the for loop to follow
+            df = pd.DataFrame([])
             num_31day_blocks = int(math.floor(delta.days / 31))
 
-            df = pd.DataFrame([])  # Empty dataframe for data from API requests
-
-            # Loop through in 31 day blocks,
-            # adjust the begin_datetime and end_datetime accordingly,
-            # make a request to the NOAA CO-OPS API
             for i in range(num_31day_blocks + 1):
                 begin_datetime_loop = begin_datetime + timedelta(days=(i * 31))
                 end_datetime_loop = begin_datetime_loop + timedelta(days=31)
-
-                # If end_datetime_loop of the current 31 day block is greater
-                # than end_datetime specified by user, use end_datetime
-                if end_datetime_loop > end_datetime:
-                    end_datetime_loop = end_datetime
-
-                # Build URL for each API request as we proceed through the loop
-                data_url = self._build_query_url(
+                end_datetime_loop = (
+                    end_datetime
+                    if end_datetime_loop > end_datetime
+                    else end_datetime_loop
+                )
+                data_url = self._build_request_url(
                     begin_datetime_loop.strftime("%Y%m%d"),
                     end_datetime_loop.strftime("%Y%m%d"),
                     product,
                     datum,
                     bin_num,
                     interval,
                     units,
                     time_zone,
                 )
+                df_block = self._url2pandas(data_url, product, num_31day_blocks)
+                df = pd.concat([df, df_block])
 
-                # Get dataframe for block and append to time series df
-                df_new = self._url2pandas(data_url, product, num_31day_blocks)
-                df = pd.concat([df, df_new])
-
-        # Rename output dataframe columns based on requested product
+        # Rename output DataFrame columns based on requested product
         # and convert to useable data types
         if product == "water_level":
             # Rename columns for clarity
             df.rename(
                 columns={
                     "f": "flags",
                     "q": "QC",
@@ -687,15 +622,15 @@
         elif product == "hourly_height":
             # Rename columns for clarity
             df.rename(
                 columns={
                     "f": "flags",
                     "s": "sigma",
                     "t": "date_time",
-                    "v": "water_level",
+                    "v": "hourly_height",
                 },
                 inplace=True,
             )
 
             # Convert columns to numeric values
             data_cols = df.columns.drop(["flags", "date_time"])
             df[data_cols] = df[data_cols].apply(pd.to_numeric, axis=1, errors="coerce")
@@ -711,15 +646,15 @@
                     "ty": "high_low",
                     "t": "date_time",
                     "v": "water_level",
                 },
                 inplace=True,
             )
 
-            # Separate to high and low dataframes
+            # Separate to high and low DataFrames
             df_HH = df[df["high_low"] == "HH"].copy()
             df_HH.rename(
                 columns={
                     "date_time": "date_time_HH",
                     "water_level": "HH_water_level",
                 },
                 inplace=True,
@@ -764,15 +699,15 @@
             df_H["date_time"] = dates_H
             df_H.index = df_H["date_time"]
             df_L["date_time"] = dates_L
             df_L.index = df_L["date_time"]
             df_LL["date_time"] = dates_LL
             df_LL.index = df_LL["date_time"]
 
-            # Remove flags and combine to single dataframe
+            # Remove flags and combine to single DataFrame
             df_HH = df_HH.drop(columns=["flags", "high_low"])
             df_H = df_H.drop(columns=["flags", "high_low", "date_time"])
             df_L = df_L.drop(columns=["flags", "high_low", "date_time"])
             df_LL = df_LL.drop(columns=["flags", "high_low", "date_time"])
 
             # Keep only one instance per date (based on max/min)
             maxes = df_HH.groupby(df_HH.index).HH_water_level.transform(max)
@@ -807,30 +742,30 @@
             df["date_time_L"] = pd.to_datetime(df["date_time_L"])
             df["date_time_LL"] = pd.to_datetime(df["date_time_LL"])
 
         elif product == "predictions":
             if interval == "h" or interval is None:
                 # Rename columns for clarity
                 df.rename(
-                    columns={"t": "date_time", "v": "predicted_wl"},
+                    columns={"t": "date_time", "v": "predictions"},
                     inplace=True,
                 )
 
                 # Convert columns to numeric values
                 data_cols = df.columns.drop(["date_time"])
                 df[data_cols] = df[data_cols].apply(
                     pd.to_numeric, axis=1, errors="coerce"
                 )
 
             elif interval == "hilo":
                 # Rename columns for clarity
                 df.rename(
                     columns={
                         "t": "date_time",
-                        "v": "predicted_wl",
+                        "v": "predictions",
                         "type": "hi_lo",
                     },
                     inplace=True,
                 )
 
                 # Convert columns to numeric values
                 data_cols = df.columns.drop(["date_time", "hi_lo"])
@@ -863,16 +798,16 @@
         elif product == "wind":
             # Rename columns for clarity
             df.rename(
                 columns={
                     "d": "dir",
                     "dr": "compass",
                     "f": "flags",
-                    "g": "gust_spd",
-                    "s": "spd",
+                    "g": "gust_speed",
+                    "s": "wind_speed",
                     "t": "date_time",
                 },
                 inplace=True,
             )
 
             # Convert columns to numeric values
             data_cols = df.columns.drop(["date_time", "flags", "compass"])
@@ -880,43 +815,43 @@
 
             # Convert date & time strings to datetime objects
             df["date_time"] = pd.to_datetime(df["date_time"])
 
         elif product == "air_pressure":
             # Rename columns for clarity
             df.rename(
-                columns={"f": "flags", "t": "date_time", "v": "air_press"},
+                columns={"f": "flags", "t": "date_time", "v": "air_pressure"},
                 inplace=True,
             )
 
             # Convert columns to numeric values
             data_cols = df.columns.drop(["date_time", "flags"])
             df[data_cols] = df[data_cols].apply(pd.to_numeric, axis=1, errors="coerce")
 
             # Convert date & time strings to datetime objects
             df["date_time"] = pd.to_datetime(df["date_time"])
 
         elif product == "air_temperature":
             # Rename columns for clarity
             df.rename(
-                columns={"f": "flags", "t": "date_time", "v": "air_temp"},
+                columns={"f": "flags", "t": "date_time", "v": "air_temperature"},
                 inplace=True,
             )
 
             # Convert columns to numeric values
             data_cols = df.columns.drop(["date_time", "flags"])
             df[data_cols] = df[data_cols].apply(pd.to_numeric, axis=1, errors="coerce")
 
             # Convert date & time strings to datetime objects
             df["date_time"] = pd.to_datetime(df["date_time"])
 
         elif product == "water_temperature":
             # Rename columns for clarity
             df.rename(
-                columns={"f": "flags", "t": "date_time", "v": "water_temp"},
+                columns={"f": "flags", "t": "date_time", "v": "water_temperature"},
                 inplace=True,
             )
 
             # Convert columns to numeric values
             data_cols = df.columns.drop(["date_time", "flags"])
             df[data_cols] = df[data_cols].apply(pd.to_numeric, axis=1, errors="coerce")
 
@@ -933,35 +868,73 @@
 
         df.drop_duplicates()  # Handle duplicates due to overlapping requests
         self.data = df
         return df
 
 
 if __name__ == "__main__":
-    from pprint import pprint as pp
-
     # DEBUGGING
-    seattle = Station(id="9447130")  # water levels
+    # from pprint import pprint
+
+    # import noaa_coops as nc
+
+    # station = nc.Station("8771510")
+
+    # print(f"CO-OPS MetaData API Station ID: {station.id}")
+    # print(f"CO-OPS MetaData API Station Name: {station.name}")
+    # print("CO-OPS MetaData API Station Products: ")
+    # pprint(station.products, indent=4)
+    # print("\n")
+
+    # data1 = station.get_data(
+    #     begin_date="19951201 00:00",
+    #     end_date="19960131 00:00",
+    #     product="water_level",
+    #     datum="MSL",
+    #     interval="h",
+    #     units="english",
+    #     time_zone="gmt",
+    # )
+    # pprint(data1)
+    # print("\n")
+
+    # data2 = station.get_data(
+    #     begin_date="19951201 00:00",
+    #     end_date="19951210 00:00",
+    #     product="water_level",
+    #     datum="MSL",
+    #     interval="h",
+    #     units="english",
+    #     time_zone="gmt",
+    # )
+    # pprint(data2)
+    # print("\n")
+
+    # print(
+    #     "CO-OPS SOAP Data Inventory: ",
+    # )
+    # pprint(station.data_inventory, indent=4, compact=True, width=100)
+    # print("\n")
+
+    # seattle = Station(id="9447130")  # water levels
+    # print("Test that metadata is working:")
+    # pprint(seattle.metadata)
+    # print("\n" * 2)
+    # print("Test that attributes are populated from metadata:")
+    # pprint(seattle.sensors)
+    # print("\n" * 2)
+    # print("Test that data_inventory is working:")
+    # pprint(seattle.data_inventory)
+    # print("\n" * 2)
+    # print("Test water level station request:")
+    # sea_data = seattle.get_data(
+    #     begin_date="20150101",
+    #     end_date="20150331",
+    #     product="water_level",
+    #     datum="MLLW",
+    #     units="metric",
+    #     time_zone="gmt",
+    # )
+    # pprint(sea_data.head())
+    # print("\n" * 2)
 
-    print("Test that metadata is working:")
-    pp(seattle.metadata)
-    print("\n" * 2)
-
-    print("Test that attributes are populated from metadata:")
-    pp(seattle.sensors)
-    print("\n" * 2)
-
-    print("Test that data_inventory is working:")
-    pp(seattle.data_inventory)
-    print("\n" * 2)
-
-    print("Test water level station request:")
-    sea_data = seattle.get_data(
-        begin_date="20150101",
-        end_date="20150331",
-        product="water_level",
-        datum="MLLW",
-        units="metric",
-        time_zone="gmt",
-    )
-    pp(sea_data.head())
-    print("\n" * 2)
+    pass
```

### Comparing `noaa_coops-0.2.1/pyproject.toml` & `noaa_coops-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "noaa-coops"
-version = "0.2.1"
+version = "0.2.2"
 description = "Python wrapper for NOAA Tides & Currents Data and Metadata."
 authors = ["Greg Clunies <greg.clunies@gmail.com>"]
 license = "GNU GPL"
 readme = "README.md"
 repository = "https://github.com/GClunies/noaa_coops"
 keywords = ["noaa", "coops", "tides", "currents", "weather", "api"]
 packages = [{include = "noaa_coops"}]
```

### Comparing `noaa_coops-0.2.1/setup.py` & `noaa_coops-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['numpy>=1.24.1,<2.0.0',
  'pandas>=1.5.3,<2.0.0',
  'requests>=2.28.2,<3.0.0',
  'zeep>=4.2.1,<5.0.0']
 
 setup_kwargs = {
     'name': 'noaa-coops',
-    'version': '0.2.1',
+    'version': '0.2.2',
     'description': 'Python wrapper for NOAA Tides & Currents Data and Metadata.',
     'long_description': '# noaa_coops\n\n[![Build Status](https://travis-ci.org/GClunies/noaa_coops.svg?branch=master)](https://travis-ci.org/GClunies/noaa_coops)\n[![PyPI](https://img.shields.io/pypi/v/noaa_coops.svg)](https://pypi.python.org/pypi/noaa-coops)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/noaa_coops.svg)](https://pypi.python.org/pypi/noaa-coops)\n\nA Python wrapper for the NOAA CO-OPS Tides &amp; Currents [Data](https://tidesandcurrents.noaa.gov/api/)\nand [Metadata](https://tidesandcurrents.noaa.gov/mdapi/latest/) APIs.\n\n## Installation\nThis package is distributed through [pip](https://pypi.org/project/noaa-coops/) and can be installed to an environment via `pip install noaa-coops`.\n\n## Getting Started\n\n### Stations\nData is accessed via `Station` class objects. Each station is uniquely identified by an `id`. To initialize a `Station` object, run:\n\n```python\n>>> from noaa_coops import Station\n>>> seattle = Station(id="9447130")  # Create Station object for Seattle (ID = 9447130)\n```\n\nStations can be found with the Tides & Currents [mapping interface](https://tidesandcurrents.noaa.gov/) or the `get_stations_from_bbox` function, which searches a bounding box for stations and returns their IDs (if found).\n```python\n>>> from pprint import pprint\n>>> from noaa_coops import Station, get_stations_from_bbox\n>>> stations = get_stations_from_bbox(lat_coords=[40.389, 40.9397], lon_coords=[-74.4751, -73.7432])\n>>> pprint(stations)\n[\'8516945\', \'8518750\', \'8519483\', \'8531680\']\n>>> station_one = Station(id="8516945")\n>>> pprint(station_one.name)\n\'Kings Point\'\n```\n\n#### Metadata\nStation metadata is stored in the `.metadata` attribute of a `Station` object. Additionally, the keys of the metadata attribute dictionary are also assigned as attributes of the station object itself.\n\n```python\n>>> from pprint import pprint\n>>> from noaa_coops import Station\n>>> seattle = Station(id="9447130")\n>>> pprint(list(seattle.metadata.items())[:5])                   # Print first 3 items in metadata\n[(\'tidal\', True), (\'greatlakes\', False), (\'shefcode\', \'EBSW1\')]  # Metadata dictionary can be very long\n>>> pprint(seattle.lat_lon[\'lat\'])                               # Print latitude\n47.601944\n>>> pprint(seattle.lat_lon[\'lon\'])                               # Print longitude\n-122.339167\n```\n\n#### Data Inventory\nA description of a Station\'s data products and available dates can be accessed via the `.data_inventory` attribute of a `Station` object.\n\n```python\n>>> from noaa_coops import Station\n>>> from pprint import pprint\n>>> seattle = Station(id="9447130")\n>>> pprint(seattle.data_inventory)\n{\'Air Temperature\': {\'end_date\': \'2019-01-02 18:36\',\n                     \'start_date\': \'1991-11-09 01:00\'},\n \'Barometric Pressure\': {\'end_date\': \'2019-01-02 18:36\',\n                         \'start_date\': \'1991-11-09 00:00\'},\n \'Preliminary 6-Minute Water Level\': {\'end_date\': \'2023-02-05 19:54\',\n                                      \'start_date\': \'2001-01-01 00:00\'},\n \'Verified 6-Minute Water Level\': {\'end_date\': \'2022-12-31 23:54\',\n                                   \'start_date\': \'1995-06-01 00:00\'},\n \'Verified High/Low Water Level\': {\'end_date\': \'2022-12-31 23:54\',\n                                   \'start_date\': \'1977-10-18 02:18\'},\n \'Verified Hourly Height Water Level\': {\'end_date\': \'2022-12-31 23:00\',\n                                        \'start_date\': \'1899-01-01 00:00\'},\n \'Verified Monthly Mean Water Level\': {\'end_date\': \'2022-12-31 23:54\',\n                                       \'start_date\': \'1898-12-01 00:00\'},\n \'Water Temperature\': {\'end_date\': \'2019-01-02 18:36\',\n                       \'start_date\': \'1991-11-09 00:00\'},\n \'Wind\': {\'end_date\': \'2019-01-02 18:36\', \'start_date\': \'1991-11-09 00:00\'}}\n```\n\n#### Data\nStation data can be fetched using the `.get_data` method on a `Station` object. Data is returned as Pandas DataFrames for ease of use and analysis. Available data products can be found in [NOAA CO-OPS Data API](https://tidesandcurrents.noaa.gov/api/#products) docs.\n\n`noaa_coops` currently supports the following data products:\n- Currents\n- Observed water levels\n- Observed daily high and low water levels (use `product="high_low"`)\n- Predicted water levels\n- Predicted high and low water levels\n- Winds\n- Air pressure\n- Air temperature\n- Water temperature\n\nThe example below fetches water level data from the Seattle station for a 3 month period.\n\n```python\n>>> from noaa_coops import Station\n>>> seattle = Station(id="9447130")\n>>> df_water_levels = seattle.get_data(\n...     begin_date="20150101",\n...     end_date="20150331",\n...     product="water_level",\n...     datum="MLLW",\n...     units="metric",\n...     time_zone="gmt")\n>>> df_water_levels.head()\n                     water_level  sigma    flags QC\ndate_time\n2015-01-01 00:00:00        1.799  0.023  0,0,0,0  v\n2015-01-01 00:06:00        1.718  0.018  0,0,0,0  v\n2015-01-01 00:12:00        1.639  0.013  0,0,0,0  v\n2015-01-01 00:18:00        1.557  0.012  0,0,0,0  v\n2015-01-01 00:24:00        1.473  0.014  0,0,0,0  v\n\n```\n\n## Development\n\n### Requirements\nThis package and its dependencies are managed using [poetry](https://python-poetry.org/). To install the development environment for `noaa_coops`, first install poetry, then run (inside the repo):\n\n```bash\npoetry install\n```\n\n### TODO\nClick [here](https://github.com/GClunies/noaa_coops/issues) for a list of existing issues and to submit a new one.\n\n### Contribution\nContributions are welcome, feel free to submit a pull request.\n',
     'author': 'Greg Clunies',
     'author_email': 'greg.clunies@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/GClunies/noaa_coops',
```

### Comparing `noaa_coops-0.2.1/PKG-INFO` & `noaa_coops-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noaa-coops
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python wrapper for NOAA Tides & Currents Data and Metadata.
 Home-page: https://github.com/GClunies/noaa_coops
 License: GNU GPL
 Keywords: noaa,coops,tides,currents,weather,api
 Author: Greg Clunies
 Author-email: greg.clunies@gmail.com
 Requires-Python: >=3.8,<4.0
```

