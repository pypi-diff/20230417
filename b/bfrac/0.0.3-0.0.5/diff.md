# Comparing `tmp/bfrac-0.0.3.tar.gz` & `tmp/bfrac-0.0.5.tar.gz`

## Comparing `bfrac-0.0.3.tar` & `bfrac-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bfrac-0.0.3/example_config.ini
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 bfrac-0.0.3/bfrac/__about__.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 bfrac-0.0.3/bfrac/__init__.py
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 bfrac-0.0.3/bfrac/app_config.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 bfrac-0.0.3/bfrac/match_info_object.py
--rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 bfrac-0.0.3/bfrac/query_context.py
--rw-r--r--   0        0        0    10302 2020-02-02 00:00:00.000000 bfrac-0.0.3/bfrac/riot_api_caller.py
--rw-r--r--   0        0        0     4726 2020-02-02 00:00:00.000000 bfrac-0.0.3/bfrac/riot_api_helper.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 bfrac-0.0.3/tests/context.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 bfrac-0.0.3/tests/simple_test.py
--rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 bfrac-0.0.3/tests/tester.ipynb
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 bfrac-0.0.3/.gitignore
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 bfrac-0.0.3/LICENSE
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 bfrac-0.0.3/README.md
--rw-r--r--   0        0        0     3296 2020-02-02 00:00:00.000000 bfrac-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 bfrac-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bfrac-0.0.5/example_config.ini
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 bfrac-0.0.5/bfrac/__about__.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 bfrac-0.0.5/bfrac/__init__.py
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 bfrac-0.0.5/bfrac/app_config.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 bfrac-0.0.5/bfrac/match_info_object.py
+-rw-r--r--   0        0        0     7826 2020-02-02 00:00:00.000000 bfrac-0.0.5/bfrac/query_context.py
+-rw-r--r--   0        0        0    10284 2020-02-02 00:00:00.000000 bfrac-0.0.5/bfrac/riot_api_caller.py
+-rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 bfrac-0.0.5/bfrac/riot_api_helper.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 bfrac-0.0.5/tests/context.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 bfrac-0.0.5/tests/simple_test.py
+-rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 bfrac-0.0.5/tests/tester.ipynb
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 bfrac-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 bfrac-0.0.5/LICENSE
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 bfrac-0.0.5/README.md
+-rw-r--r--   0        0        0     3296 2020-02-02 00:00:00.000000 bfrac-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 bfrac-0.0.5/PKG-INFO
```

### Comparing `bfrac-0.0.3/bfrac/app_config.py` & `bfrac-0.0.5/bfrac/app_config.py`

 * *Files identical despite different names*

### Comparing `bfrac-0.0.3/bfrac/riot_api_caller.py` & `bfrac-0.0.5/bfrac/riot_api_caller.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     def __init__(self, in_status_code, in_text):
         self.status_code = in_status_code
         self.text = in_text
         msg = f"Request returned an error: {in_status_code} -> {in_text}."
         super().__init__(msg)
 
 
-class BadRequest(RequestError):
+class BadRequest(Exception):
     """
     BadRequest is an Exception
     Raised when the RiotAPI sends error code 400
     """
 
     def __init__(self, in_status_code, in_text):
         self.status_code = in_status_code
@@ -35,15 +35,15 @@
             "Common Reasons:\n" \
             "\t A provided parameter is in the wrong format (e.g., a string instead of an integer).\n" \
             "\t A provided parameter is invalid (e.g., beginTime and startTime specify a time range that is too large).\n" \
             "\t A required parameter was not provided.\n"
         super().__init__(msg + info)
 
 
-class Unauthorized(RequestError):
+class Unauthorized(Exception):
     """
     Unauthorized is an Exception
     Raised when the RiotAPI sends error code 401
     """
 
     def __init__(self, in_status_code, in_text):
         self.status_code = in_status_code
@@ -51,15 +51,15 @@
         msg = f"Request returned a error code 401 (Unauthorized) -> {in_text}.\n"
         info = "Authentication error.\n" \
             "Common Reasons:\n" \
             "\t An API key has not been included in the request.\n"
         super().__init__(msg + info)
 
 
-class Forbidden(RequestError):
+class Forbidden(Exception):
     """
     Forbidden is an Exception
     Raised when the RiotAPI sends error code 403
     """
 
     def __init__(self, in_status_code, in_text):
         self.status_code = in_status_code
@@ -69,15 +69,15 @@
             "Common Reasons:\n" \
             "\t An invalid API key was provided with the API request.\n" \
             "\t A blacklisted API key was provided with the API request.\n" \
             "\t The API request was for an incorrect or unsupported path.\n"
         super().__init__(msg + info)
 
 
-class NotFound(RequestError):
+class NotFound(Exception):
     """
     NotFound is an Exception
     Raised when the RiotAPI sends error code 404
     """
 
     def __init__(self, in_status_code, in_text):
         self.status_code = in_status_code
@@ -87,15 +87,15 @@
             "Common Reasons:\n" \
             "\t The ID or name provided does not match any existing resource " \
                "(e.g., there is no Summoner matching the specified ID).\n" \
             "\t There are no resources that match the parameters specified.\n"
         super().__init__(msg + info)
 
 
-class UnsupportedMediaType(RequestError):
+class UnsupportedMediaType(Exception):
     """
     UnsupportedMediaType is an Exception
     Raised when the RiotAPI sends error code 415
     """
 
     def __init__(self, in_status_code, in_text):
         self.status_code = in_status_code
@@ -103,15 +103,15 @@
         msg = f"Request returned a error code 415 (Unsupported Media Type) -> {in_text}.\n"
         info = "Server is refusing to service the request because the body of the request is in a format that is not supported.\n" \
             "Common Reasons:\n" \
             "\t The Content-Type header was not appropriately set.\n"
         super().__init__(msg + info)
 
 
-class RateLimitExceeded(RequestError):
+class RateLimitExceeded(Exception):
     """
     RateLimitExceeded is an Exception
     Raised when the RiotAPI sends error code 429
     """
 
     def __init__(self, in_status_code, in_text):
         self.status_code = in_status_code
```

### Comparing `bfrac-0.0.3/bfrac/riot_api_helper.py` & `bfrac-0.0.5/bfrac/riot_api_helper.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+from typing import Literal
+from bfrac.bfrac import RiotAPICaller
+
+
 class RiotAPIHelper:
     """
     Helper class containing static methods for calling common riot api endpoints.
     """
     LOL_SERVERS = ["br1", "eun1", "euw1", "jp1", "kr", "la1", "la2", "na1", "oc1", "ph2", "ru", "sg2", "th2", "tr1",
                    "tw2", "vn2"]
     LOL_CONTINENTS = ["americas", "asia", "europe", "sea"]
@@ -13,46 +17,68 @@
     The AMERICAS routing value serves NA, BR, LAN and LAS.
     The ASIA routing value serves KR and JP.
     The EUROPE routing value serves EUNE, EUW, TR and RU.
     The SEA routing value serves OCE, PH2, SG2, TH2, TW2 and VN2.
     """
 
     @staticmethod
-    def url_summoner_by_name(in_region_server, in_summoner_name):
+    def url_summoner_by_name(in_region_server: Literal["br1", "eun1", "euw1", "jp1", "kr", "la1", "la2", "na1", "oc1",
+                                                       "ph2", "ru", "sg2", "th2", "tr1", "tw2", "vn2"],
+                             in_summoner_name: str):
         return f"https://{in_region_server}.api.riotgames.com/lol/summoner/v4/summoners/by-name/{in_summoner_name}"
 
     @staticmethod
-    def url_summoner_by_puuid(in_region_server, in_encrypted_puuid):
+    def url_summoner_by_puuid(in_region_server: Literal["br1", "eun1", "euw1", "jp1", "kr", "la1", "la2", "na1", "oc1",
+                                                        "ph2", "ru", "sg2", "th2", "tr1", "tw2", "vn2"],
+                              in_encrypted_puuid: str):
         return f"https://{in_region_server}.api.riotgames.com/lol/summoner/v4/summoners/by-puuid/{in_encrypted_puuid}"
 
     @staticmethod
-    def url_match_list_by_summoner_puuid(in_region_continent, in_puuid):
+    def url_match_list_by_summoner_puuid(in_region_continent: Literal["americas", "asia", "europe", "sea"], in_puuid):
         return f"https://{in_region_continent}.api.riotgames.com/lol/match/v5/matches/by-puuid/{in_puuid}/ids"
 
     @staticmethod
-    def url_match_info(in_region_continent, in_match_id):
+    def url_match_info(in_region_continent: Literal["americas", "asia", "europe", "sea"], in_match_id):
         return f"https://{in_region_continent}.api.riotgames.com/lol/match/v5/matches/{in_match_id}"
 
     @staticmethod
-    def url_match_timeline(in_region_continent, in_match_id):
+    def url_match_timeline(in_region_continent: Literal["americas", "asia", "europe", "sea"], in_match_id):
         return f"https://{in_region_continent}.api.riotgames.com/lol/match/v5/matches/{in_match_id}/timeline"
 
     @staticmethod
-    def get_summoner_by_name(in_riot_api_caller, in_region_server, in_summoner_name):
+    def get_summoner_by_name(in_riot_api_caller: RiotAPICaller,
+                             in_region_server: Literal["br1", "eun1", "euw1", "jp1", "kr", "la1", "la2", "na1", "oc1",
+                                                       "ph2", "ru", "sg2", "th2", "tr1", "tw2", "vn2"],
+                             in_summoner_name: str) -> dict:
         url = RiotAPIHelper.url_summoner_by_name(in_region_server, in_summoner_name)
         return in_riot_api_caller.call_riot_api(url, {})
 
     @staticmethod
-    def get_matches_list(in_riot_api_caller, in_region_continent, in_summoner_puuid, in_count,
-                         in_type="", in_queue=None, in_start_time=0, in_end_time=0, in_start=0):
+    def get_summoner_by_puuid(in_riot_api_caller: RiotAPICaller,
+                              in_region_server: Literal["br1", "eun1", "euw1", "jp1", "kr", "la1", "la2", "na1", "oc1",
+                                                        "ph2", "ru", "sg2", "th2", "tr1", "tw2", "vn2"],
+                              in_encrypted_puuid: str) -> dict:
+        url = RiotAPIHelper.url_summoner_by_puuid(in_region_server, in_encrypted_puuid)
+        return in_riot_api_caller.call_riot_api(url, {})
+
+    @staticmethod
+    def get_matches_list(in_riot_api_caller: RiotAPICaller,
+                         in_region_continent: Literal["americas", "asia", "europe", "sea"],
+                         in_summoner_puuid: str,
+                         in_count: int,
+                         in_type: Literal["ranked", "normal", "tourney", "tutorial"] = "",
+                         in_queue: int = None,
+                         in_start_time: int = 0,
+                         in_end_time: int = 0,
+                         in_start: int = 0):
         """
 
         Parameters
         ----------
-        in_riot_api_caller : RiotAPICaller
+        in_riot_api_caller
             A valid RiotAPICaller object that could be used to call the endpoint.
         in_region_continent : str
             One of region values from {"americas", "asia", "europe", "sea"}
             This is the region for this query.
         in_summoner_puuid : str
             PUUID of the summoner
         in_count : int
@@ -88,15 +114,19 @@
         if in_start_time > 0:
             params["startTime"] = in_start_time
         if in_end_time > 0:
             params["endTime"] = in_end_time
         return in_riot_api_caller.call_riot_api(url, params)
 
     @staticmethod
-    def get_match_info(in_riot_api_caller, in_region_continent, in_match_id):
+    def get_match_info(in_riot_api_caller: RiotAPICaller,
+                       in_region_continent: Literal["americas", "asia", "europe", "sea"],
+                       in_match_id: str):
         url = RiotAPIHelper.url_match_info(in_region_continent, in_match_id)
         return in_riot_api_caller.call_riot_api(url, {})
 
     @staticmethod
-    def get_match_timeline(in_riot_api_caller, in_region_continent, in_match_id):
+    def get_match_timeline(in_riot_api_caller: RiotAPICaller,
+                           in_region_continent: Literal["americas", "asia", "europe", "sea"],
+                           in_match_id: str):
         url = RiotAPIHelper.url_match_timeline(in_region_continent, in_match_id)
         return in_riot_api_caller.call_riot_api(url, {})
```

### Comparing `bfrac-0.0.3/tests/tester.ipynb` & `bfrac-0.0.5/tests/tester.ipynb`

 * *Files identical despite different names*

### Comparing `bfrac-0.0.3/.gitignore` & `bfrac-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `bfrac-0.0.3/LICENSE` & `bfrac-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bfrac-0.0.3/pyproject.toml` & `bfrac-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bfrac-0.0.3/PKG-INFO` & `bfrac-0.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bfrac
-Version: 0.0.3
+Version: 0.0.5
 Summary: Beginner Friendly Riot API Caller is a simple wrapper for RiotAPI with rate maintenance built in.
 Project-URL: Documentation, https://github.com/deamonpog/bfrac#readme
 Project-URL: Issues, https://github.com/deamonpog/bfrac/issues
 Project-URL: Source, https://github.com/deamonpog/bfrac
 Author-email: deamonpog <pog666@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
```

