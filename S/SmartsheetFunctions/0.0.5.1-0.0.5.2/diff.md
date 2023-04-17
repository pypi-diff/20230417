# Comparing `tmp/SmartsheetFunctions-0.0.5.1.tar.gz` & `tmp/SmartsheetFunctions-0.0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SmartsheetFunctions-0.0.5.1.tar", last modified: Thu Apr  6 16:22:22 2023, max compression
+gzip compressed data, was "SmartsheetFunctions-0.0.5.2.tar", last modified: Mon Apr 17 15:39:36 2023, max compression
```

## Comparing `SmartsheetFunctions-0.0.5.1.tar` & `SmartsheetFunctions-0.0.5.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 16:22:22.254241 SmartsheetFunctions-0.0.5.1/
--rw-rw-rw-   0        0        0     1092 2023-04-06 14:51:56.000000 SmartsheetFunctions-0.0.5.1/LICENSE
--rw-rw-rw-   0        0        0     5064 2023-04-06 16:22:22.253243 SmartsheetFunctions-0.0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     4659 2023-04-06 16:20:52.000000 SmartsheetFunctions-0.0.5.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-06 16:22:22.229242 SmartsheetFunctions-0.0.5.1/SmartsheetFunctions/
--rw-rw-rw-   0        0        0        0 2023-03-08 20:38:06.000000 SmartsheetFunctions-0.0.5.1/SmartsheetFunctions/__init__.py
--rw-rw-rw-   0        0        0     8945 2023-03-08 20:38:06.000000 SmartsheetFunctions-0.0.5.1/SmartsheetFunctions/smartsheet.py
-drwxrwxrwx   0        0        0        0 2023-04-06 16:22:22.250244 SmartsheetFunctions-0.0.5.1/SmartsheetFunctions.egg-info/
--rw-rw-rw-   0        0        0     5064 2023-04-06 16:22:22.000000 SmartsheetFunctions-0.0.5.1/SmartsheetFunctions.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-04-06 16:22:22.000000 SmartsheetFunctions-0.0.5.1/SmartsheetFunctions.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 16:22:22.000000 SmartsheetFunctions-0.0.5.1/SmartsheetFunctions.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-06 16:22:22.000000 SmartsheetFunctions-0.0.5.1/SmartsheetFunctions.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-04-06 16:22:22.000000 SmartsheetFunctions-0.0.5.1/SmartsheetFunctions.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-06 16:22:22.254241 SmartsheetFunctions-0.0.5.1/setup.cfg
--rw-rw-rw-   0        0        0      763 2023-04-06 16:22:04.000000 SmartsheetFunctions-0.0.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 15:39:36.001331 SmartsheetFunctions-0.0.5.2/
+-rw-rw-rw-   0        0        0     1092 2023-04-06 14:51:56.000000 SmartsheetFunctions-0.0.5.2/LICENSE
+-rw-rw-rw-   0        0        0     5064 2023-04-17 15:39:35.999330 SmartsheetFunctions-0.0.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4659 2023-04-06 16:20:52.000000 SmartsheetFunctions-0.0.5.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 15:39:35.979329 SmartsheetFunctions-0.0.5.2/SmartsheetFunctions/
+-rw-rw-rw-   0        0        0        0 2023-03-08 20:38:06.000000 SmartsheetFunctions-0.0.5.2/SmartsheetFunctions/__init__.py
+-rw-rw-rw-   0        0        0     9284 2023-04-17 15:36:32.000000 SmartsheetFunctions-0.0.5.2/SmartsheetFunctions/smartsheet.py
+drwxrwxrwx   0        0        0        0 2023-04-17 15:39:35.996333 SmartsheetFunctions-0.0.5.2/SmartsheetFunctions.egg-info/
+-rw-rw-rw-   0        0        0     5064 2023-04-17 15:39:35.000000 SmartsheetFunctions-0.0.5.2/SmartsheetFunctions.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-04-17 15:39:35.000000 SmartsheetFunctions-0.0.5.2/SmartsheetFunctions.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 15:39:35.000000 SmartsheetFunctions-0.0.5.2/SmartsheetFunctions.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-17 15:39:35.000000 SmartsheetFunctions-0.0.5.2/SmartsheetFunctions.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-04-17 15:39:35.000000 SmartsheetFunctions-0.0.5.2/SmartsheetFunctions.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 15:39:36.001331 SmartsheetFunctions-0.0.5.2/setup.cfg
+-rw-rw-rw-   0        0        0      763 2023-04-17 15:36:30.000000 SmartsheetFunctions-0.0.5.2/setup.py
```

### Comparing `SmartsheetFunctions-0.0.5.1/LICENSE` & `SmartsheetFunctions-0.0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `SmartsheetFunctions-0.0.5.1/PKG-INFO` & `SmartsheetFunctions-0.0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SmartsheetFunctions
-Version: 0.0.5.1
+Version: 0.0.5.2
 Summary: SmartSheet Functions for development
 Author: Derek Bantel
 Author-email: derekbantel@outlook.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `SmartsheetFunctions-0.0.5.1/README.md` & `SmartsheetFunctions-0.0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `SmartsheetFunctions-0.0.5.1/SmartsheetFunctions/smartsheet.py` & `SmartsheetFunctions-0.0.5.2/SmartsheetFunctions/smartsheet.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Declare smartsheet functions
 import requests
 import json
+from decimal import Decimal
 #####################
 
 #Initialize smartsheet class
 class SmartSheet():
 
     def __init__(self, sheet_id, api_token):
         self.api_url =  "https://api.smartsheet.com/2.0/"
@@ -19,15 +20,15 @@
         if r.status_code != 200:
             print(r.status_code, r.text)
         return r.json()
 
 
     def add_smartsheet_row(self, payload):
         api_url = f"{self.api_url}sheets/{self.sheet_id}/rows"
-        payload = json.dumps(payload)
+        payload = json.dumps(payload, default=json_decode_handler)
         r = requests.post(api_url, headers=self.std_header, data=payload)
         if r.status_code != 200:
             print(r.status_code, r.text)
         return r.json()
 
 
     def delete_smartsheet_row(self, row_id):
@@ -114,15 +115,15 @@
         if r.status_code != 200:
             print(r.status_code, r.text)
         return r.json()
 
 
     def update_row(self, payload):
         api_url = f"{self.api_url}sheets/{self.sheet_id}/rows"
-        payload = json.dumps(payload)
+        payload = json.dumps(payload, default=json_decode_handler)
         r = requests.put(api_url, headers=self.std_header, data=payload)
         if r.status_code != 200:
             print(r.status_code, r.text)
         return r.json()
 
 
     def upload_attachment(self, row_id, attachment, filename):
@@ -184,15 +185,15 @@
         #creates a dictionary that allows referencing columns by name to get id
         dictionary = dict(zip(column_names, column_ids))
         return dictionary
 
     
     def add_columns(self, payload):
         api_url = f"{self.api_url}sheets/{self.sheet_id}/columns"
-        payload = json.dumps(payload)
+        payload = json.dumps(payload, default=json_decode_handler)
         r = requests.post(api_url, headers=self.std_header, data=payload)
         if r.status_code != 200:
             print(r.status_code, r.text)
         return r.json()
 
 
 class SmartFolder():
@@ -219,18 +220,25 @@
             print(r.status_code, r.text)
 
 
 def create_smartsheet(folderid, api_token, name):
     api_url = f"https://api.smartsheet.com/2.0/folders/{folderid}/sheets"
     header =  {"Authorization": f"Bearer {api_token}", "Content-Type": "application/json"}
     payload = {"name": name, "columns": [{"title": "Primary Column", "primary": True, "type": "TEXT_NUMBER"}]}
-    payload = json.dumps(payload)
+    payload = json.dumps(payload, default=json_decode_handler)
     r = requests.post(api_url, headers=header, data = payload)
     if r.status_code != 200:
         print(r.status_code, r.text)
 
 
 def create_dictionary_fr_list(first_list, second_list):
     #creates a dictionary that allows referencing columns by name to get id
     dictionary = dict(zip(first_list, second_list))
     return dictionary
-#################
+#################
+
+
+
+def json_decode_handler(obj):
+    if isinstance(obj, Decimal):
+        return float(obj)
+    raise TypeError("Object of type {} is not JSON serializable".format(type(obj).__name__))
```

### Comparing `SmartsheetFunctions-0.0.5.1/SmartsheetFunctions.egg-info/PKG-INFO` & `SmartsheetFunctions-0.0.5.2/SmartsheetFunctions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SmartsheetFunctions
-Version: 0.0.5.1
+Version: 0.0.5.2
 Summary: SmartSheet Functions for development
 Author: Derek Bantel
 Author-email: derekbantel@outlook.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `SmartsheetFunctions-0.0.5.1/setup.py` & `SmartsheetFunctions-0.0.5.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="SmartsheetFunctions",
-    version="0.0.5.1",
+    version="0.0.5.2",
     author="Derek Bantel",
     author_email="derekbantel@outlook.com",
     description="SmartSheet Functions for development",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="MIT",
     packages=["SmartsheetFunctions"],
```

