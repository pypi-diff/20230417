# Comparing `tmp/actiapi-0.2.0.tar.gz` & `tmp/actiapi-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "actiapi-0.2.0.tar", max compression
+gzip compressed data, was "actiapi-0.2.1.tar", max compression
```

## Comparing `actiapi-0.2.0.tar` & `actiapi-0.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35149 2023-02-15 09:47:59.060844 actiapi-0.2.0/LICENSE.md
--rw-r--r--   0        0        0      581 2023-02-15 09:47:59.060844 actiapi-0.2.0/README.rst
--rw-r--r--   0        0        0      438 2023-02-15 09:47:59.060844 actiapi-0.2.0/actiapi/__init__.py
--rw-r--r--   0        0        0     3129 2023-02-15 09:47:59.060844 actiapi-0.2.0/actiapi/v2.py
--rw-r--r--   0        0        0     4240 2023-02-15 09:47:59.060844 actiapi-0.2.0/actiapi/v3.py
--rw-r--r--   0        0        0      764 2023-02-15 09:47:59.060844 actiapi-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1359 1970-01-01 00:00:00.000000 actiapi-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-17 14:06:53.008112 actiapi-0.2.1/LICENSE.md
+-rw-r--r--   0        0        0      581 2023-04-17 14:06:53.008112 actiapi-0.2.1/README.rst
+-rw-r--r--   0        0        0      438 2023-04-17 14:06:53.008112 actiapi-0.2.1/actiapi/__init__.py
+-rw-r--r--   0        0        0     3129 2023-04-17 14:06:53.008112 actiapi-0.2.1/actiapi/v2.py
+-rw-r--r--   0        0        0     4706 2023-04-17 14:06:53.008112 actiapi-0.2.1/actiapi/v3.py
+-rw-r--r--   0        0        0      764 2023-04-17 14:06:53.008112 actiapi-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1359 1970-01-01 00:00:00.000000 actiapi-0.2.1/PKG-INFO
```

### Comparing `actiapi-0.2.0/LICENSE.md` & `actiapi-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `actiapi-0.2.0/README.rst` & `actiapi-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `actiapi-0.2.0/actiapi/v2.py` & `actiapi-0.2.1/actiapi/v2.py`

 * *Files identical despite different names*

### Comparing `actiapi-0.2.0/actiapi/v3.py` & `actiapi-0.2.1/actiapi/v3.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Client for API V2.
 
 See https://github.com/actigraph/CentrePoint3APIDocumentation.
 """
 import logging
-from typing import Any, Dict, List, Union
+from typing import Any, Dict, List, Union, Optional
 
 import requests
 
 from actiapi import ActiGraphClient
 
 
 class ActiGraphClientV3(ActiGraphClient):
@@ -45,30 +45,45 @@
                 "No access token! Make sure you have API_ACCESS_KEY and API_SECRET_KEY!"
             )
 
     def get_files(
         self,
         user: Union[int, str],
         study_id: int,
+        start: Optional[str] = None,
+        end: Optional[str] = None,
     ) -> List[str]:
         """Return download URLs to raw AVRO files.
 
         Parameters
         ----------
         user:
             User id
         study_id:
             Id of the study
+        start:
+            Start timestamp string in ISO8601 format
+        end:
+            End timestamp string in ISO8601 format
         """
         token = self._get_access_token(
             "DataAccess",
         )
-        results = self._get_paginated(
+
+        request_string = (
             f"/dataaccess/v3/files/studies/{study_id}/subjects/{user}"
-            f"/raw-accelerometer?fileFormat=avro&",
+            f"/raw-accelerometer?fileFormat=avro"
+        )
+        if start is not None:
+            request_string += f"&startDate={start}"
+        if end is not None:
+            request_string += f"&endDate={end}"
+        request_string += "&"
+        results = self._get_paginated(
+            request_string,
             token,
         )
 
         results = [x["downloadUrl"] for x in results]
 
         return results
```

### Comparing `actiapi-0.2.0/pyproject.toml` & `actiapi-0.2.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "actiapi"
-version = "0.2.0"
+version = "0.2.1"
 description = "A python package for accessing ActiGraph data through the official ActiGraph API"
 authors = ["ActiGraph Data Science Team <science@theactigraph.com>"]
 maintainers = ["ActiGraph Data Science Team <science@theactigraph.com>"]
 repository = "https://github.com/actigraph/actiapi"
 readme = "README.rst"
 license = "GPL-3.0-only"
```

### Comparing `actiapi-0.2.0/PKG-INFO` & `actiapi-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: actiapi
-Version: 0.2.0
+Version: 0.2.1
 Summary: A python package for accessing ActiGraph data through the official ActiGraph API
 Home-page: https://github.com/actigraph/actiapi
 License: GPL-3.0-only
 Author: ActiGraph Data Science Team
 Author-email: science@theactigraph.com
 Maintainer: ActiGraph Data Science Team
 Maintainer-email: science@theactigraph.com
```

