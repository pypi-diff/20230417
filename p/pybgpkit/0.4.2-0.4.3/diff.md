# Comparing `tmp/pybgpkit-0.4.2.tar.gz` & `tmp/pybgpkit-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybgpkit-0.4.2.tar", last modified: Sun Apr  9 06:13:07 2023, max compression
+gzip compressed data, was "pybgpkit-0.4.3.tar", last modified: Mon Apr 17 21:35:39 2023, max compression
```

## Comparing `pybgpkit-0.4.2.tar` & `pybgpkit-0.4.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mingwei    (501) staff       (20)        0 2023-04-09 06:13:07.501584 pybgpkit-0.4.2/
--rw-r--r--   0 mingwei    (501) staff       (20)     1063 2022-01-31 02:29:25.000000 pybgpkit-0.4.2/LICENSE
--rw-r--r--   0 mingwei    (501) staff       (20)     7643 2023-04-09 06:13:07.501472 pybgpkit-0.4.2/PKG-INFO
--rw-r--r--   0 mingwei    (501) staff       (20)     7389 2023-03-30 05:13:34.000000 pybgpkit-0.4.2/README.md
-drwxr-xr-x   0 mingwei    (501) staff       (20)        0 2023-04-09 06:13:07.500617 pybgpkit-0.4.2/bgpkit/
--rw-r--r--   0 mingwei    (501) staff       (20)       98 2022-04-05 23:11:20.000000 pybgpkit-0.4.2/bgpkit/__init__.py
--rw-r--r--   0 mingwei    (501) staff       (20)     2081 2022-04-27 15:55:01.000000 pybgpkit-0.4.2/bgpkit/bgpkit_broker.py
--rw-r--r--   0 mingwei    (501) staff       (20)       34 2022-04-27 15:54:49.000000 pybgpkit-0.4.2/bgpkit/bgpkit_parser.py
--rw-r--r--   0 mingwei    (501) staff       (20)     2012 2022-04-05 22:19:49.000000 pybgpkit-0.4.2/bgpkit/bgpkit_roas.py
--rw-r--r--   0 mingwei    (501) staff       (20)     1273 2022-04-27 15:56:16.000000 pybgpkit-0.4.2/bgpkit/test_integration.py
-drwxr-xr-x   0 mingwei    (501) staff       (20)        0 2023-04-09 06:13:07.501325 pybgpkit-0.4.2/pybgpkit.egg-info/
--rw-r--r--   0 mingwei    (501) staff       (20)     7643 2023-04-09 06:13:07.000000 pybgpkit-0.4.2/pybgpkit.egg-info/PKG-INFO
--rw-r--r--   0 mingwei    (501) staff       (20)      316 2023-04-09 06:13:07.000000 pybgpkit-0.4.2/pybgpkit.egg-info/SOURCES.txt
--rw-r--r--   0 mingwei    (501) staff       (20)        1 2023-04-09 06:13:07.000000 pybgpkit-0.4.2/pybgpkit.egg-info/dependency_links.txt
--rw-r--r--   0 mingwei    (501) staff       (20)       49 2023-04-09 06:13:07.000000 pybgpkit-0.4.2/pybgpkit.egg-info/requires.txt
--rw-r--r--   0 mingwei    (501) staff       (20)        7 2023-04-09 06:13:07.000000 pybgpkit-0.4.2/pybgpkit.egg-info/top_level.txt
--rw-r--r--   0 mingwei    (501) staff       (20)      103 2022-02-01 17:35:12.000000 pybgpkit-0.4.2/pyproject.toml
--rw-r--r--   0 mingwei    (501) staff       (20)       38 2023-04-09 06:13:07.501617 pybgpkit-0.4.2/setup.cfg
--rw-r--r--   0 mingwei    (501) staff       (20)      709 2023-04-09 06:12:48.000000 pybgpkit-0.4.2/setup.py
+drwxr-xr-x   0 mingwei    (501) staff       (20)        0 2023-04-17 21:35:39.971783 pybgpkit-0.4.3/
+-rw-r--r--   0 mingwei    (501) staff       (20)     1063 2022-01-31 02:29:25.000000 pybgpkit-0.4.3/LICENSE
+-rw-r--r--   0 mingwei    (501) staff       (20)     7643 2023-04-17 21:35:39.971657 pybgpkit-0.4.3/PKG-INFO
+-rw-r--r--   0 mingwei    (501) staff       (20)     7389 2023-03-30 05:13:34.000000 pybgpkit-0.4.3/README.md
+drwxr-xr-x   0 mingwei    (501) staff       (20)        0 2023-04-17 21:35:39.970776 pybgpkit-0.4.3/bgpkit/
+-rw-r--r--   0 mingwei    (501) staff       (20)       98 2022-04-05 23:11:20.000000 pybgpkit-0.4.3/bgpkit/__init__.py
+-rw-r--r--   0 mingwei    (501) staff       (20)     2322 2023-04-17 21:35:29.000000 pybgpkit-0.4.3/bgpkit/bgpkit_broker.py
+-rw-r--r--   0 mingwei    (501) staff       (20)       34 2022-04-27 15:54:49.000000 pybgpkit-0.4.3/bgpkit/bgpkit_parser.py
+-rw-r--r--   0 mingwei    (501) staff       (20)     2012 2022-04-05 22:19:49.000000 pybgpkit-0.4.3/bgpkit/bgpkit_roas.py
+-rw-r--r--   0 mingwei    (501) staff       (20)     1589 2023-04-17 21:35:29.000000 pybgpkit-0.4.3/bgpkit/test_integration.py
+drwxr-xr-x   0 mingwei    (501) staff       (20)        0 2023-04-17 21:35:39.971498 pybgpkit-0.4.3/pybgpkit.egg-info/
+-rw-r--r--   0 mingwei    (501) staff       (20)     7643 2023-04-17 21:35:39.000000 pybgpkit-0.4.3/pybgpkit.egg-info/PKG-INFO
+-rw-r--r--   0 mingwei    (501) staff       (20)      316 2023-04-17 21:35:39.000000 pybgpkit-0.4.3/pybgpkit.egg-info/SOURCES.txt
+-rw-r--r--   0 mingwei    (501) staff       (20)        1 2023-04-17 21:35:39.000000 pybgpkit-0.4.3/pybgpkit.egg-info/dependency_links.txt
+-rw-r--r--   0 mingwei    (501) staff       (20)       49 2023-04-17 21:35:39.000000 pybgpkit-0.4.3/pybgpkit.egg-info/requires.txt
+-rw-r--r--   0 mingwei    (501) staff       (20)        7 2023-04-17 21:35:39.000000 pybgpkit-0.4.3/pybgpkit.egg-info/top_level.txt
+-rw-r--r--   0 mingwei    (501) staff       (20)      103 2022-02-01 17:35:12.000000 pybgpkit-0.4.3/pyproject.toml
+-rw-r--r--   0 mingwei    (501) staff       (20)       38 2023-04-17 21:35:39.971817 pybgpkit-0.4.3/setup.cfg
+-rw-r--r--   0 mingwei    (501) staff       (20)      709 2023-04-17 21:35:29.000000 pybgpkit-0.4.3/setup.py
```

### Comparing `pybgpkit-0.4.2/LICENSE` & `pybgpkit-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pybgpkit-0.4.2/PKG-INFO` & `pybgpkit-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybgpkit
-Version: 0.4.2
+Version: 0.4.3
 Summary: BGPKIT tools Python bindings
 Home-page: https://github.com/bgpkit/pybgpkit
 Author: Mingwei Zhang
 Author-email: mingwei@bgpkit.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pybgpkit-0.4.2/README.md` & `pybgpkit-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `pybgpkit-0.4.2/bgpkit/bgpkit_broker.py` & `pybgpkit-0.4.3/bgpkit/bgpkit_broker.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from dataclasses import dataclass
 
 import requests as requests
+import urllib3
 
 
 def check_type(value: any, ty: type) -> bool:
     try:
         ty(value)
         return True
     except ValueError:
@@ -20,17 +21,21 @@
     url: str
     rough_size: int
     exact_size: int
 
 
 class Broker:
 
-    def __init__(self, api_url: str = "https://api.broker.bgpkit.com/v2", page_size: int = 100):
+    def __init__(self, api_url: str = "https://api.broker.bgpkit.com/v2", page_size: int = 100, verify=True):
         self.base_url = api_url.strip()
         self.page_size = int(page_size)
+        self.verify = verify
+        if not verify:
+            # if a user disable SSL verification on-purpose, do not warn the user
+            urllib3.disable_warnings()
 
     def query(self,
               ts_start: str = None,
               ts_end: str = None,
               collector_id: str = None,
               project: str = None,
               data_type: str = None,
@@ -54,24 +59,24 @@
 
         api_url = f"{self.base_url}/search?" + "&".join(params)
         page = 1
 
         data_items = []
         if print_url:
             print(api_url)
-        res = requests.get(api_url).json()
+        res = requests.get(api_url, verify=self.verify).json()
         while res:
             if res["count"] > 0:
                 data_items.extend([BrokerItem(**i) for i in res["data"]])
 
                 if res["count"] < res["page_size"]:
                     break
 
                 page += 1
                 query_url = f"{api_url}&page={page}"
                 if print_url:
                     print(query_url)
-                res = requests.get(query_url).json()
+                res = requests.get(query_url, verify=self.verify).json()
             else:
                 break
 
         return data_items
```

### Comparing `pybgpkit-0.4.2/bgpkit/bgpkit_roas.py` & `pybgpkit-0.4.3/bgpkit/bgpkit_roas.py`

 * *Files identical despite different names*

### Comparing `pybgpkit-0.4.2/bgpkit/test_integration.py` & `pybgpkit-0.4.3/bgpkit/test_integration.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,22 @@
         broker = bgpkit.Broker()
         items = broker.query(ts_start="1643760000", ts_end="2022-02-02T00:20:00", collector_id="rrc00")
         for item in items:
             print(json.dumps(item.__dict__))
         print(len(items))
         assert len(items) == 7
 
+    def test_broker_no_verify(self):
+        broker = bgpkit.Broker(verify=False)
+        items = broker.query(ts_start="1643760000", ts_end="2022-02-02T00:20:00", collector_id="rrc00")
+        for item in items:
+            print(json.dumps(item.__dict__))
+        print(len(items))
+        assert len(items) == 7
+
     def test_roas(self):
         roas = bgpkit.Roas()
         data = roas.query(debug=True, asn=3333, date="2018-01-01")
         for entry in data:
             print(entry)
         assert len(data) == 10
```

### Comparing `pybgpkit-0.4.2/pybgpkit.egg-info/PKG-INFO` & `pybgpkit-0.4.3/pybgpkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybgpkit
-Version: 0.4.2
+Version: 0.4.3
 Summary: BGPKIT tools Python bindings
 Home-page: https://github.com/bgpkit/pybgpkit
 Author: Mingwei Zhang
 Author-email: mingwei@bgpkit.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pybgpkit-0.4.2/setup.py` & `pybgpkit-0.4.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name='pybgpkit',
-    version='0.4.2',
+    version='0.4.3',
     description='BGPKIT tools Python bindings',
     url='https://github.com/bgpkit/pybgpkit',
     author='Mingwei Zhang',
     author_email='mingwei@bgpkit.com',
     packages=setuptools.find_packages(),
     include_package_data=True,
     long_description=long_description,
```

