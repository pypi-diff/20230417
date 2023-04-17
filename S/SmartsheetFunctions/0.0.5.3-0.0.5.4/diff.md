# Comparing `tmp/SmartsheetFunctions-0.0.5.3.tar.gz` & `tmp/SmartsheetFunctions-0.0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SmartsheetFunctions-0.0.5.3.tar", last modified: Mon Apr 17 21:03:50 2023, max compression
+gzip compressed data, was "SmartsheetFunctions-0.0.5.4.tar", last modified: Mon Apr 17 21:15:06 2023, max compression
```

## Comparing `SmartsheetFunctions-0.0.5.3.tar` & `SmartsheetFunctions-0.0.5.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 21:03:50.228917 SmartsheetFunctions-0.0.5.3/
--rw-rw-rw-   0        0        0     1092 2023-04-06 14:51:56.000000 SmartsheetFunctions-0.0.5.3/LICENSE
--rw-rw-rw-   0        0        0     5064 2023-04-17 21:03:50.227919 SmartsheetFunctions-0.0.5.3/PKG-INFO
--rw-rw-rw-   0        0        0     4659 2023-04-06 16:20:52.000000 SmartsheetFunctions-0.0.5.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 21:03:50.207917 SmartsheetFunctions-0.0.5.3/SmartsheetFunctions/
--rw-rw-rw-   0        0        0        0 2023-03-08 20:38:06.000000 SmartsheetFunctions-0.0.5.3/SmartsheetFunctions/__init__.py
--rw-rw-rw-   0        0        0    23338 2023-04-17 21:02:30.000000 SmartsheetFunctions-0.0.5.3/SmartsheetFunctions/smartsheet.py
-drwxrwxrwx   0        0        0        0 2023-04-17 21:03:50.224921 SmartsheetFunctions-0.0.5.3/SmartsheetFunctions.egg-info/
--rw-rw-rw-   0        0        0     5064 2023-04-17 21:03:50.000000 SmartsheetFunctions-0.0.5.3/SmartsheetFunctions.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-04-17 21:03:50.000000 SmartsheetFunctions-0.0.5.3/SmartsheetFunctions.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 21:03:50.000000 SmartsheetFunctions-0.0.5.3/SmartsheetFunctions.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-17 21:03:50.000000 SmartsheetFunctions-0.0.5.3/SmartsheetFunctions.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-04-17 21:03:50.000000 SmartsheetFunctions-0.0.5.3/SmartsheetFunctions.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 21:03:50.229916 SmartsheetFunctions-0.0.5.3/setup.cfg
--rw-rw-rw-   0        0        0      763 2023-04-17 21:03:08.000000 SmartsheetFunctions-0.0.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 21:15:06.169198 SmartsheetFunctions-0.0.5.4/
+-rw-rw-rw-   0        0        0     1092 2023-04-06 14:51:56.000000 SmartsheetFunctions-0.0.5.4/LICENSE
+-rw-rw-rw-   0        0        0     5064 2023-04-17 21:15:06.168198 SmartsheetFunctions-0.0.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4659 2023-04-06 16:20:52.000000 SmartsheetFunctions-0.0.5.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 21:15:06.150201 SmartsheetFunctions-0.0.5.4/SmartsheetFunctions/
+-rw-rw-rw-   0        0        0        0 2023-03-08 20:38:06.000000 SmartsheetFunctions-0.0.5.4/SmartsheetFunctions/__init__.py
+-rw-rw-rw-   0        0        0    23631 2023-04-17 21:14:49.000000 SmartsheetFunctions-0.0.5.4/SmartsheetFunctions/smartsheet.py
+drwxrwxrwx   0        0        0        0 2023-04-17 21:15:06.166199 SmartsheetFunctions-0.0.5.4/SmartsheetFunctions.egg-info/
+-rw-rw-rw-   0        0        0     5064 2023-04-17 21:15:06.000000 SmartsheetFunctions-0.0.5.4/SmartsheetFunctions.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-04-17 21:15:06.000000 SmartsheetFunctions-0.0.5.4/SmartsheetFunctions.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 21:15:06.000000 SmartsheetFunctions-0.0.5.4/SmartsheetFunctions.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-17 21:15:06.000000 SmartsheetFunctions-0.0.5.4/SmartsheetFunctions.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-04-17 21:15:06.000000 SmartsheetFunctions-0.0.5.4/SmartsheetFunctions.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 21:15:06.170200 SmartsheetFunctions-0.0.5.4/setup.cfg
+-rw-rw-rw-   0        0        0      763 2023-04-17 21:14:48.000000 SmartsheetFunctions-0.0.5.4/setup.py
```

### Comparing `SmartsheetFunctions-0.0.5.3/LICENSE` & `SmartsheetFunctions-0.0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `SmartsheetFunctions-0.0.5.3/PKG-INFO` & `SmartsheetFunctions-0.0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SmartsheetFunctions
-Version: 0.0.5.3
+Version: 0.0.5.4
 Summary: SmartSheet Functions for development
 Author: Derek Bantel
 Author-email: derekbantel@outlook.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `SmartsheetFunctions-0.0.5.3/README.md` & `SmartsheetFunctions-0.0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `SmartsheetFunctions-0.0.5.3/SmartsheetFunctions/smartsheet.py` & `SmartsheetFunctions-0.0.5.4/SmartsheetFunctions/smartsheet.py`

 * *Files 0% similar despite different names*

```diff
@@ -403,98 +403,98 @@
         api_url = f"{self.api_url}sheets/{self.sheet_id}/columns"
         payload = json.dumps(payload, default=json_decode_handler)
         r = requests.post(api_url, headers=self.std_header, data=payload)
         if r.status_code != 200:
             print(r.status_code, r.text)
         return r.json()
     
-def add_rows_payload_creater(self, data: list, column_headers: list, add_row_position: str, additional_settings: dict) -> list:
-        """
-        Creates a payload for adding new rows to a Smartsheet.
-
-        Args:
-            data (list): A list of data to be added to the sheet. Each element of the list represents a new row.
-            column_headers (list): A list of the column headers in the order they appear in the sheet.
-            add_row_position (str): A string indicating whether new rows should be added at the top or bottom of the sheet.
-            additional_settings (dict): A dictionary containing additional settings for the new rows, such as formatting or cell linking.
-
-        Returns:
-            list: A list of dictionaries containing the new row data.
-
-        """
-        # Make a copy of the data so we can modify it without changing the original list.
-        new_data = []
-        for row in data:
-            new_data.append(list(row))
-        
-        # Get the IDs of the columns in the sheet, so we can map column headers to column IDs later.
-        col_names = self.column_names()
-        col_ids = self.sheet_column_ids()
-        col_dict = self.column_dictionary(col_names, col_ids)
-
-        add_payload = []
-        rows_payload = []
-        counter = 0
-
-        # Regular expressions for matching decimal and percentage values in cells.
-        decimal_regex = re.compile(r"\d+\.\d+")
-        percent_pattern = re.compile(r"\d+%")
-
-        # Loop over the rows of data, creating a payload for each row.
-        for row in new_data:
-            if counter != 0:
-                col_counter = 0
-                for col in column_headers:
+    def add_rows_payload_creator(self, data: list, column_headers: list, add_row_position: str, additional_settings: dict) -> list:
+            """
+            Creates a payload for adding new rows to a Smartsheet.
+
+            Args:
+                data (list): A list of data to be added to the sheet. Each element of the list represents a new row.
+                column_headers (list): A list of the column headers in the order they appear in the sheet.
+                add_row_position (str): A string indicating whether new rows should be added at the top or bottom of the sheet.
+                additional_settings (dict): A dictionary containing additional settings for the new rows, such as formatting or cell linking.
+
+            Returns:
+                list: A list of dictionaries containing the new row data.
+
+            """
+            # Make a copy of the data so we can modify it without changing the original list.
+            new_data = []
+            for row in data:
+                new_data.append(list(row))
+            
+            # Get the IDs of the columns in the sheet, so we can map column headers to column IDs later.
+            col_names = self.column_names()
+            col_ids = self.sheet_column_ids()
+            col_dict = self.column_dictionary(col_names, col_ids)
+
+            add_payload = []
+            rows_payload = []
+            counter = 0
+
+            # Regular expressions for matching decimal and percentage values in cells.
+            decimal_regex = re.compile(r"\d+\.\d+")
+            percent_pattern = re.compile(r"\d+%")
+
+            # Loop over the rows of data, creating a payload for each row.
+            for row in new_data:
+                if counter != 0:
+                    col_counter = 0
+                    for col in column_headers:
+                        
+                        # Check if the cell value is a decimal or percentage value, and convert it if necessary.
+                        decimal_regex_test = decimal_regex.search(str(row[col_counter]))
+                        datetime_test = isinstance(row[col_counter], datetime.datetime)
+
+                        if decimal_regex_test and not datetime_test:
+                            percent_test = percent_pattern.search(str(row[col_counter]))
+                            if percent_test:
+                                # Convert percentage value to decimal.
+                                new_per_value = float(str(row[col_counter]).replace("%", ""))
+                                rows_payload.append({"columnId": col_dict[col], "value": new_per_value})
+                            else: 
+                                # Convert decimal value to float.
+                                new_dec_value = float(row[col_counter])
+                                rows_payload.append({"columnId": col_dict[col], "value": new_dec_value})
+
+                        # Check if the cell value is a datetime object, and format it if necessary.
+                        if datetime_test:
+                            new_value = row[col_counter].strftime("%m/%d/%Y")
+                            rows_payload.append({"columnId": col_dict[col], "value": new_value})
+
+                        # Otherwise, just add the cell value as-is.
+                        elif not decimal_regex_test and not datetime_test:
+                            rows_payload.append({"columnId": col_dict[col], "value": row[col_counter]})
+                        col_counter += 1
+                        
+                    # Create a dictionary with the row data and additional settings, if any.
+                    payload_dict = {
+                        add_row_position: True,
+                        "cells": rows_payload,
+                    }
+                        
+                    if len(additional_settings) > 0:
+                        add_payload.append({
+                            **payload_dict,
+                            **additional_settings
+                        })
+                    else:
+                        add_payload.append({
+                            **payload_dict
+                        })
                     
-                    # Check if the cell value is a decimal or percentage value, and convert it if necessary.
-                    decimal_regex_test = decimal_regex.search(str(row[col_counter]))
-                    datetime_test = isinstance(row[col_counter], datetime.datetime)
-
-                    if decimal_regex_test and not datetime_test:
-                        percent_test = percent_pattern.search(str(row[col_counter]))
-                        if percent_test:
-                            # Convert percentage value to decimal.
-                            new_per_value = float(str(row[col_counter]).replace("%", ""))
-                            rows_payload.append({"columnId": col_dict[col], "value": new_per_value})
-                        else: 
-                            # Convert decimal value to float.
-                            new_dec_value = float(row[col_counter])
-                            rows_payload.append({"columnId": col_dict[col], "value": new_dec_value})
-
-                    # Check if the cell value is a datetime object, and format it if necessary.
-                    if datetime_test:
-                        new_value = row[col_counter].strftime("%m/%d/%Y")
-                        rows_payload.append({"columnId": col_dict[col], "value": new_value})
-
-                    # Otherwise, just add the cell value as-is.
-                    elif not decimal_regex_test and not datetime_test:
-                        rows_payload.append({"columnId": col_dict[col], "value": row[col_counter]})
-                    col_counter += 1
-                    
-                # Create a dictionary with the row data and additional settings, if any.
-                payload_dict = {
-                    add_row_position: True,
-                    "cells": rows_payload,
-                }
-                    
-                if len(additional_settings) > 0:
-                    add_payload.append({
-                        **payload_dict,
-                        **additional_settings
-                    })
-                else:
-                    add_payload.append({
-                        **payload_dict
-                    })
-                   
-                rows_payload = []
-
-            counter += 1 
-        
-        return add_payload
+                    rows_payload = []
+
+                counter += 1 
+            
+            return add_payload
 
 
 class SmartFolder:
     """
     A class for interacting with Smartsheet folders using the Smartsheet API.
 
     Attributes:
```

### Comparing `SmartsheetFunctions-0.0.5.3/SmartsheetFunctions.egg-info/PKG-INFO` & `SmartsheetFunctions-0.0.5.4/SmartsheetFunctions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SmartsheetFunctions
-Version: 0.0.5.3
+Version: 0.0.5.4
 Summary: SmartSheet Functions for development
 Author: Derek Bantel
 Author-email: derekbantel@outlook.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `SmartsheetFunctions-0.0.5.3/setup.py` & `SmartsheetFunctions-0.0.5.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="SmartsheetFunctions",
-    version="0.0.5.3",
+    version="0.0.5.4",
     author="Derek Bantel",
     author_email="derekbantel@outlook.com",
     description="SmartSheet Functions for development",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="MIT",
     packages=["SmartsheetFunctions"],
```

