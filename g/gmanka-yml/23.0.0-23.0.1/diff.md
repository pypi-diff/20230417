# Comparing `tmp/gmanka_yml-23.0.0.tar.gz` & `tmp/gmanka_yml-23.0.1.tar.gz`

## Comparing `gmanka_yml-23.0.0.tar` & `gmanka_yml-23.0.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 gmanka_yml-23.0.0/changelog.md
--rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 gmanka_yml-23.0.0/start.sh
--rwxr-xr-x   0        0        0     1101 2020-02-02 00:00:00.000000 gmanka_yml-23.0.0/gmanka_yml/__init__.py
--rwxr-xr-x   0        0        0       24 2020-02-02 00:00:00.000000 gmanka_yml-23.0.0/.gitignore
--rwxr-xr-x   0        0        0      658 2020-02-02 00:00:00.000000 gmanka_yml-23.0.0/pyproject.toml
--rwxr-xr-x   0        0        0     1189 2020-02-02 00:00:00.000000 gmanka_yml-23.0.0/readme.md
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 gmanka_yml-23.0.0/PKG-INFO
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 gmanka_yml-23.0.1/changelog.md
+-rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 gmanka_yml-23.0.1/start.sh
+-rwxr-xr-x   0        0        0     1551 2020-02-02 00:00:00.000000 gmanka_yml-23.0.1/gmanka_yml/__init__.py
+-rwxr-xr-x   0        0        0       24 2020-02-02 00:00:00.000000 gmanka_yml-23.0.1/.gitignore
+-rwxr-xr-x   0        0        0      658 2020-02-02 00:00:00.000000 gmanka_yml-23.0.1/pyproject.toml
+-rwxr-xr-x   0        0        0     1291 2020-02-02 00:00:00.000000 gmanka_yml-23.0.1/readme.md
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 gmanka_yml-23.0.1/PKG-INFO
```

### Comparing `gmanka_yml-23.0.0/gmanka_yml/__init__.py` & `gmanka_yml-23.0.1/gmanka_yml/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from io import TextIOWrapper
 from pathlib import Path
 import yaml
 
 
-version = '23.0.0'
+version = '23.0.1'
+_sential = object()
 
 
 def to_str(
     data,
 ) -> str:
     try:
         return yaml.dump(
@@ -19,53 +20,67 @@
         return yaml.dump(
             data,
             allow_unicode = True,
             Dumper = yaml.Dumper,
         )
 
 
-
 def to_file(
     data,
     path: str | Path,
 ) -> None:
     Path(path).parent.mkdir(
         exist_ok = True,
         parents = True,
     )
     with open(
-        path,
-        'w'
+        file = path,
+        mode = 'w',
+        encoding = 'utf-8',
     ) as file:
         file.write(
             to_str(
                 data,
             )
         )
 
 
 def read_str(
     data: str | TextIOWrapper,
+    default = _sential,
 ):
     try:
         return yaml.load(
             data,
             Loader = yaml.CLoader,
         )
     except AttributeError:
         return yaml.load(
             data,
             Loader = yaml.Loader,
         )
+    except Exception as error:
+        if default == _sential:
+            raise error
+        else:
+            return default
 
 
 def read_file(
-    path: str | Path
+    path: str | Path,
+    default = _sential,
 ):
-    with open(
-        path,
-        'r',
-    ) as file:
-        return read_str(
-            file
-        )
+    try:
+        with open(
+            file = path,
+            mode = 'r',
+            encoding = 'utf-8',
+        ) as file:
+            return read_str(
+                file
+            )
+    except Exception as error:
+        if default == _sential:
+            raise error
+        else:
+            return default
```

### Comparing `gmanka_yml-23.0.0/pyproject.toml` & `gmanka_yml-23.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [project]
 dependencies = [
   "pyyaml",
 ]
 name = "gmanka_yml"
-version = "23.0.0"
+version = "23.0.1"
 authors = [
   { name="gmanka", email="gmankab@gmail.com" },
 ]
 description = "some useful shortcuts for pyyaml"
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `gmanka_yml-23.0.0/readme.md` & `gmanka_yml-23.0.1/readme.md`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 ## to_file[^](#functions)
 
 same as [to_str](#to_str), but writes data to file instead of returning
 
 ```py
 yml.to_file(
     data = my_dict,
-    file_path = 'file.yml',
+    path = 'file.yml',
 )
 ```
 
 ## read_str[^](#functions)
 
 ```py
 import gmanka_yml as yml
@@ -84,9 +84,18 @@
 ```
 
 ## read_file[^](#functions)
 
 same as [read_str](#read_str), but reads data from file
 
 ```py
-print(yml.read_file('file.yml'))
+yml.read_file('file.yml')
 ```
+
+## default values
+
+```py
+yml.read_str(1) # raises TypeError
+
+yml.read_str(1, default = None) # returns None
+```
+
```

### Comparing `gmanka_yml-23.0.0/PKG-INFO` & `gmanka_yml-23.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmanka_yml
-Version: 23.0.0
+Version: 23.0.1
 Summary: some useful shortcuts for pyyaml
 Project-URL: Homepage, https://github.com/gmankab/yml
 Project-URL: Documentation, https://github.com/gmankab/yml
 Project-URL: Bug Tracker, https://github.com/gmankab/yml/issues
 Author-email: gmanka <gmankab@gmail.com>
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -62,15 +62,15 @@
 ## to_file[^](#functions)
 
 same as [to_str](#to_str), but writes data to file instead of returning
 
 ```py
 yml.to_file(
     data = my_dict,
-    file_path = 'file.yml',
+    path = 'file.yml',
 )
 ```
 
 ## read_str[^](#functions)
 
 ```py
 import gmanka_yml as yml
@@ -99,9 +99,18 @@
 ```
 
 ## read_file[^](#functions)
 
 same as [read_str](#read_str), but reads data from file
 
 ```py
-print(yml.read_file('file.yml'))
+yml.read_file('file.yml')
 ```
+
+## default values
+
+```py
+yml.read_str(1) # raises TypeError
+
+yml.read_str(1, default = None) # returns None
+```
+
```

