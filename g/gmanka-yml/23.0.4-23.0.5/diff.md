# Comparing `tmp/gmanka_yml-23.0.4.tar.gz` & `tmp/gmanka_yml-23.0.5.tar.gz`

## Comparing `gmanka_yml-23.0.4.tar` & `gmanka_yml-23.0.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 gmanka_yml-23.0.4/changelog.md
--rwxr-xr-x   0        0        0     1831 2020-02-02 00:00:00.000000 gmanka_yml-23.0.4/gmanka_yml/__init__.py
--rwxr-xr-x   0        0        0       24 2020-02-02 00:00:00.000000 gmanka_yml-23.0.4/.gitignore
--rwxr-xr-x   0        0        0      658 2020-02-02 00:00:00.000000 gmanka_yml-23.0.4/pyproject.toml
--rwxr-xr-x   0        0        0     1493 2020-02-02 00:00:00.000000 gmanka_yml-23.0.4/readme.md
--rw-r--r--   0        0        0     2067 2020-02-02 00:00:00.000000 gmanka_yml-23.0.4/PKG-INFO
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 gmanka_yml-23.0.5/changelog.md
+-rwxr-xr-x   0        0        0     1868 2020-02-02 00:00:00.000000 gmanka_yml-23.0.5/gmanka_yml/__init__.py
+-rwxr-xr-x   0        0        0       24 2020-02-02 00:00:00.000000 gmanka_yml-23.0.5/.gitignore
+-rwxr-xr-x   0        0        0      658 2020-02-02 00:00:00.000000 gmanka_yml-23.0.5/pyproject.toml
+-rwxr-xr-x   0        0        0     1568 2020-02-02 00:00:00.000000 gmanka_yml-23.0.5/readme.md
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 gmanka_yml-23.0.5/PKG-INFO
```

### Comparing `gmanka_yml-23.0.4/gmanka_yml/__init__.py` & `gmanka_yml-23.0.5/gmanka_yml/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from io import TextIOWrapper
 from pathlib import Path
+from typing import Any
 import yaml
 
 
 version = '23.0.4'
 _sential = object()
 
 
@@ -44,15 +45,15 @@
         )
 
 
 def from_str(
     data: str | TextIOWrapper,
     default = _sential,
     expected_type = None,
-):
+) -> Any:
     try:
         parsed = yaml.safe_load(
             stream = data,
         )
     except Exception as error:
         if default == _sential:
             raise error
@@ -73,15 +74,15 @@
         return default
 
 
 def from_file(
     path: str | Path,
     default = _sential,
     expected_type = None,
-):
+) -> Any:
     try:
         with open(
             file = path,
             mode = 'r',
         ) as file:
             return from_str( 
                 data = file,
```

### Comparing `gmanka_yml-23.0.4/pyproject.toml` & `gmanka_yml-23.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [project]
 dependencies = [
   "pyyaml",
 ]
 name = "gmanka_yml"
-version = "23.0.4"
+version = "23.0.5"
 authors = [
   { name="gmanka", email="gmankab@gmail.com" },
 ]
 description = "some useful shortcuts for pyyaml"
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `gmanka_yml-23.0.4/readme.md` & `gmanka_yml-23.0.5/readme.md`

 * *Files 7% similar despite different names*

```diff
@@ -4,20 +4,23 @@
 
 ## installation
 
 ```bash
 pip install gmanka_yml
 ```
 
-## functions
+## navigation
 
 - [to_str](#to_str)  
 - [to_file](#to_file)  
 - [from_str](#read_str)  
 - [from_file](#read_file)  
+- [default](#default)
+- [expected_type](#expected_type)
+- [changelog](changelog)
 
 ## to_str[^](#functions)
 
 converts any data to yml string and returns it
 
 ```py
 import gmanka_yml as yml
@@ -87,23 +90,23 @@
 
 same as [from_str](#read_str), but reads data from file
 
 ```py
 yml.from_file('file.yml')
 ```
 
-## default values
+## default
 
 ```py
 yml.from_str(1) # raises TypeError
 
 yml.from_str(1, default = None) # returns None
 ```
 
-## expected_type
+## expected type
 
 ```py
 yml.from_str(
     data = '{}',
     expected_type = list,
 ) # raises TypeError
```

### Comparing `gmanka_yml-23.0.4/PKG-INFO` & `gmanka_yml-23.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmanka_yml
-Version: 23.0.4
+Version: 23.0.5
 Summary: some useful shortcuts for pyyaml
 Project-URL: Homepage, https://github.com/gmankab/yml
 Project-URL: Documentation, https://github.com/gmankab/yml
 Project-URL: Bug Tracker, https://github.com/gmankab/yml/issues
 Author-email: gmanka <gmankab@gmail.com>
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -19,20 +19,23 @@
 
 ## installation
 
 ```bash
 pip install gmanka_yml
 ```
 
-## functions
+## navigation
 
 - [to_str](#to_str)  
 - [to_file](#to_file)  
 - [from_str](#read_str)  
 - [from_file](#read_file)  
+- [default](#default)
+- [expected_type](#expected_type)
+- [changelog](changelog)
 
 ## to_str[^](#functions)
 
 converts any data to yml string and returns it
 
 ```py
 import gmanka_yml as yml
@@ -102,23 +105,23 @@
 
 same as [from_str](#read_str), but reads data from file
 
 ```py
 yml.from_file('file.yml')
 ```
 
-## default values
+## default
 
 ```py
 yml.from_str(1) # raises TypeError
 
 yml.from_str(1, default = None) # returns None
 ```
 
-## expected_type
+## expected type
 
 ```py
 yml.from_str(
     data = '{}',
     expected_type = list,
 ) # raises TypeError
```

