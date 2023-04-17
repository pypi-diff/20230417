# Comparing `tmp/gig-nuuuwan-3.0.8.tar.gz` & `tmp/gig-nuuuwan-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gig-nuuuwan-3.0.8.tar", last modified: Thu Feb  2 03:24:10 2023, max compression
+gzip compressed data, was "gig-nuuuwan-3.0.9.tar", last modified: Mon Apr 17 10:49:28 2023, max compression
```

## Comparing `gig-nuuuwan-3.0.8.tar` & `gig-nuuuwan-3.0.9.tar`

### file list

```diff
@@ -1,27 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 03:24:10.068930 gig-nuuuwan-3.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-02-02 03:23:11.000000 gig-nuuuwan-3.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-02-02 03:24:10.068930 gig-nuuuwan-3.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-02-02 03:23:11.000000 gig-nuuuwan-3.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-02 03:24:10.068930 gig-nuuuwan-3.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-02-02 03:23:11.000000 gig-nuuuwan-3.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 03:24:10.064930 gig-nuuuwan-3.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 03:24:10.064930 gig-nuuuwan-3.0.8/src/gig/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-02-02 03:23:11.000000 gig-nuuuwan-3.0.8/src/gig/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 03:24:10.068930 gig-nuuuwan-3.0.8/src/gig/core/
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-02-02 03:23:11.000000 gig-nuuuwan-3.0.8/src/gig/core/Ent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-02-02 03:23:11.000000 gig-nuuuwan-3.0.8/src/gig/core/EntBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-02-02 03:23:11.000000 gig-nuuuwan-3.0.8/src/gig/core/EntGIGMixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-02-02 03:23:11.000000 gig-nuuuwan-3.0.8/src/gig/core/EntGeoMixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-02-02 03:23:11.000000 gig-nuuuwan-3.0.8/src/gig/core/EntJSONMixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-02-02 03:23:11.000000 gig-nuuuwan-3.0.8/src/gig/core/EntLoadMixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-02-02 03:23:11.000000 gig-nuuuwan-3.0.8/src/gig/core/EntType.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-02-02 03:23:11.000000 gig-nuuuwan-3.0.8/src/gig/core/GIGTable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-02-02 03:23:11.000000 gig-nuuuwan-3.0.8/src/gig/core/GIGTableRow.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-02 03:23:11.000000 gig-nuuuwan-3.0.8/src/gig/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-02-02 03:23:11.000000 gig-nuuuwan-3.0.8/src/gig/core/_common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 03:24:10.068930 gig-nuuuwan-3.0.8/src/gig_nuuuwan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-02-02 03:24:10.000000 gig-nuuuwan-3.0.8/src/gig_nuuuwan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-02-02 03:24:10.000000 gig-nuuuwan-3.0.8/src/gig_nuuuwan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-02 03:24:10.000000 gig-nuuuwan-3.0.8/src/gig_nuuuwan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-02-02 03:24:10.000000 gig-nuuuwan-3.0.8/src/gig_nuuuwan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-02 03:24:10.000000 gig-nuuuwan-3.0.8/src/gig_nuuuwan.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:49:28.442692 gig-nuuuwan-3.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-17 10:48:24.000000 gig-nuuuwan-3.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-17 10:49:28.442692 gig-nuuuwan-3.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-17 10:48:24.000000 gig-nuuuwan-3.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 10:49:28.442692 gig-nuuuwan-3.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-17 10:48:24.000000 gig-nuuuwan-3.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:49:28.438691 gig-nuuuwan-3.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:49:28.438691 gig-nuuuwan-3.0.9/src/gig/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-17 10:48:24.000000 gig-nuuuwan-3.0.9/src/gig/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:49:28.442692 gig-nuuuwan-3.0.9/src/gig/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-17 10:48:24.000000 gig-nuuuwan-3.0.9/src/gig/core/Ent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-17 10:48:24.000000 gig-nuuuwan-3.0.9/src/gig/core/EntBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-17 10:48:24.000000 gig-nuuuwan-3.0.9/src/gig/core/EntGIGMixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-17 10:48:24.000000 gig-nuuuwan-3.0.9/src/gig/core/EntGeoMixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-17 10:48:24.000000 gig-nuuuwan-3.0.9/src/gig/core/EntJSONMixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-04-17 10:48:24.000000 gig-nuuuwan-3.0.9/src/gig/core/EntLoadMixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-17 10:48:24.000000 gig-nuuuwan-3.0.9/src/gig/core/EntType.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-17 10:48:24.000000 gig-nuuuwan-3.0.9/src/gig/core/GIGTable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-17 10:48:24.000000 gig-nuuuwan-3.0.9/src/gig/core/GIGTableRow.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 10:48:24.000000 gig-nuuuwan-3.0.9/src/gig/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-17 10:48:24.000000 gig-nuuuwan-3.0.9/src/gig/core/_common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:49:28.442692 gig-nuuuwan-3.0.9/src/gig_nuuuwan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-17 10:49:28.000000 gig-nuuuwan-3.0.9/src/gig_nuuuwan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-17 10:49:28.000000 gig-nuuuwan-3.0.9/src/gig_nuuuwan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 10:49:28.000000 gig-nuuuwan-3.0.9/src/gig_nuuuwan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-17 10:49:28.000000 gig-nuuuwan-3.0.9/src/gig_nuuuwan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-17 10:49:28.000000 gig-nuuuwan-3.0.9/src/gig_nuuuwan.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:49:28.442692 gig-nuuuwan-3.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-04-17 10:48:24.000000 gig-nuuuwan-3.0.9/tests/test_ent_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-04-17 10:48:24.000000 gig-nuuuwan-3.0.9/tests/test_ent_geo_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-17 10:48:24.000000 gig-nuuuwan-3.0.9/tests/test_ent_gig_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-17 10:48:24.000000 gig-nuuuwan-3.0.9/tests/test_ent_json_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-04-17 10:48:24.000000 gig-nuuuwan-3.0.9/tests/test_ent_load_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-17 10:48:24.000000 gig-nuuuwan-3.0.9/tests/test_ent_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-04-17 10:48:24.000000 gig-nuuuwan-3.0.9/tests/test_gig_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-04-17 10:48:24.000000 gig-nuuuwan-3.0.9/tests/test_gig_table_row.py
```

### Comparing `gig-nuuuwan-3.0.8/LICENSE` & `gig-nuuuwan-3.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gig-nuuuwan-3.0.8/README.md` & `gig-nuuuwan-3.0.9/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -4,15 +4,18 @@
 
 ```
 pip install gig-nuuuwan
 ```
 
 ## Release History
 
-### 3.0.8 (CURRENT RELEASE)
+### 3.0.9   (CURRENT RELEASE)
+* Fixed windows unittests
+
+### 3.0.8
 * Fixed missing dependencies BUG 
 * Replaced fuzzywuzzy with RapidFuzz for string matching
 
 ### 3.0.7 
 * refactoring (removed deprecated utils.cache)
 
 ### 3.0.6
```

### Comparing `gig-nuuuwan-3.0.8/setup.py` & `gig-nuuuwan-3.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Setup."""
 
 import setuptools
 
 DIST_NAME = "gig"
-VERSION = "3.0.8"
+VERSION = "3.0.9"
 setuptools.setup(
     name="%s-nuuuwan" % DIST_NAME,
     version=VERSION,
     author="Nuwan I. Senaratna",
     author_email="nuuuwan@gmail.com",
     description="Generalized information graph.",
     long_description="",
@@ -19,15 +19,15 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
-    python_requires=">=3.8",
+    python_requires=">=3.10",
     install_requires=[
         'geopandas',
         'RapidFuzz',
         'shapely',
         'utils-nuuuwan',
     ],
     test_suite="nose.collector",
```

### Comparing `gig-nuuuwan-3.0.8/src/gig/core/EntBase.py` & `gig-nuuuwan-3.0.9/src/gig/core/EntBase.py`

 * *Files identical despite different names*

### Comparing `gig-nuuuwan-3.0.8/src/gig/core/EntGeoMixin.py` & `gig-nuuuwan-3.0.9/src/gig/core/EntGeoMixin.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 import os
+import tempfile
 
 import geopandas as gpd
 from shapely.geometry import MultiPolygon, Polygon
 from utils import WWW, JSONFile
 
 from gig.core._common import URL_BASE
 from gig.core.EntType import EntType
 
 
 class EntGeoMixin:
     @property
     def raw_geo_file(self):
-        raw_geo_path = os.path.join('/tmp', f'ent.{self.id}.raw_geo.json')
+        raw_geo_path = os.path.join(
+            tempfile.gettempdir(), f'ent.{self.id}.raw_geo.json'
+        )
+
         return JSONFile(raw_geo_path)
 
     @property
     def url_remote_geo_data_path(self):
         id = self.id
         ent_type = EntType.from_id(id)
-        return os.path.join(
-            URL_BASE,
-            f'geo/{ent_type.name}/{id}.json',
-        )
+        return f'{URL_BASE}/geo/{ent_type.name}/{id}.json'
 
     def get_raw_geo(self):
         raw_geo_file = self.raw_geo_file
         if raw_geo_file.exists:
             raw_geo = raw_geo_file.read()
         else:
             raw_geo = WWW(self.url_remote_geo_data_path).readJSON()
```

### Comparing `gig-nuuuwan-3.0.8/src/gig/core/EntLoadMixin.py` & `gig-nuuuwan-3.0.9/src/gig/core/EntLoadMixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,14 @@
         cls,
         name_fuzzy: str,
         filter_ent_type: EntType = None,
         filter_parent_id: str = None,
         limit: int = 5,
         min_fuzz_ratio: int = 80,
     ) -> list:
-
         entity_type_list = (
             [filter_ent_type] if filter_ent_type else EntType.list()
         )
 
         ent_and_ratio_list = []
         for entity_type in entity_type_list:
             for ent in cls.list_from_type(entity_type):
```

### Comparing `gig-nuuuwan-3.0.8/src/gig/core/EntType.py` & `gig-nuuuwan-3.0.9/src/gig/core/EntType.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import os
 from dataclasses import dataclass
 from functools import cached_property
 
 from utils import WWW, FiledVariable
 
 from gig.core._common import URL_BASE
 
@@ -33,18 +32,15 @@
             EntType.PD,
             EntType.LG,
             EntType.MOH,
         ]
 
     @property
     def url_remote_data_path(self):
-        return os.path.join(
-            URL_BASE,
-            f'ents/{self.name}.tsv',
-        )
+        return f'{URL_BASE}/ents/{self.name}.tsv'
 
     @cached_property
     def remote_data_list(self) -> list:
         def inner():
             d_list = WWW(self.url_remote_data_path).readTSV()
             non_null_d_list = [d for d in d_list if d]
             return non_null_d_list
```

### Comparing `gig-nuuuwan-3.0.8/src/gig/core/GIGTable.py` & `gig-nuuuwan-3.0.9/src/gig/core/GIGTable.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import os
 from dataclasses import dataclass
 from functools import cached_property
 
 from utils import WWW, FiledVariable
 
 from gig.core._common import URL_BASE
 from gig.core.GIGTableRow import GIGTableRow
@@ -24,18 +23,15 @@
                 self.ent_type_group,
                 self.time_group,
             ]
         )
 
     @property
     def url_remote_data_path(self):
-        return os.path.join(
-            URL_BASE,
-            f'gig2/{self.table_id}.tsv',
-        )
+        return f'{URL_BASE}/gig2/{self.table_id}.tsv'
 
     @cached_property
     def remote_data_list(self) -> list:
         def inner():
             d_list = WWW(self.url_remote_data_path).readTSV()
             non_null_d_list = [d for d in d_list if d]
             return non_null_d_list
```

### Comparing `gig-nuuuwan-3.0.8/src/gig/core/GIGTableRow.py` & `gig-nuuuwan-3.0.9/src/gig/core/GIGTableRow.py`

 * *Files identical despite different names*

