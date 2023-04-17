# Comparing `tmp/gmanka_yml-22.0.5.tar.gz` & `tmp/gmanka_yml-23.0.0.tar.gz`

## Comparing `gmanka_yml-22.0.5.tar` & `gmanka_yml-23.0.0.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 gmanka_yml-22.0.5/changelog.md
--rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 gmanka_yml-22.0.5/file.yml
--rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 gmanka_yml-22.0.5/start.sh
--rwxr-xr-x   0        0        0     1097 2020-02-02 00:00:00.000000 gmanka_yml-22.0.5/gmanka_yml/__init__.py
--rwxr-xr-x   0        0        0       24 2020-02-02 00:00:00.000000 gmanka_yml-22.0.5/.gitignore
--rwxr-xr-x   0        0        0      658 2020-02-02 00:00:00.000000 gmanka_yml-22.0.5/pyproject.toml
--rwxr-xr-x   0        0        0     1189 2020-02-02 00:00:00.000000 gmanka_yml-22.0.5/readme.md
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 gmanka_yml-22.0.5/PKG-INFO
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 gmanka_yml-23.0.0/changelog.md
+-rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 gmanka_yml-23.0.0/start.sh
+-rwxr-xr-x   0        0        0     1101 2020-02-02 00:00:00.000000 gmanka_yml-23.0.0/gmanka_yml/__init__.py
+-rwxr-xr-x   0        0        0       24 2020-02-02 00:00:00.000000 gmanka_yml-23.0.0/.gitignore
+-rwxr-xr-x   0        0        0      658 2020-02-02 00:00:00.000000 gmanka_yml-23.0.0/pyproject.toml
+-rwxr-xr-x   0        0        0     1189 2020-02-02 00:00:00.000000 gmanka_yml-23.0.0/readme.md
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 gmanka_yml-23.0.0/PKG-INFO
```

### Comparing `gmanka_yml-22.0.5/gmanka_yml/__init__.py` & `gmanka_yml-23.0.0/gmanka_yml/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+from io import TextIOWrapper
 from pathlib import Path
 import yaml
 
 
-version = '22.0.1'
+version = '23.0.0'
 
 
 def to_str(
-    data: any,
+    data,
 ) -> str:
     try:
         return yaml.dump(
             data,
             allow_unicode = True,
             Dumper = yaml.CDumper,
         )
@@ -20,50 +21,51 @@
             allow_unicode = True,
             Dumper = yaml.Dumper,
         )
 
 
 
 def to_file(
-    data: any,
-    file_path: str | Path,
+    data,
+    path: str | Path,
 ) -> None:
-    Path(file_path).parent.mkdir(
+    Path(path).parent.mkdir(
         exist_ok = True,
         parents = True,
     )
     with open(
-        file_path,
+        path,
         'w'
     ) as file:
         file.write(
             to_str(
                 data,
             )
         )
 
 
 def read_str(
-    data: str,
-) -> any:
+    data: str | TextIOWrapper,
+):
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
 
 
 def read_file(
-    file_path: str | Path
+    path: str | Path
 ):
     with open(
-        file_path,
+        path,
         'r',
     ) as file:
         return read_str(
             file
         )
+
```

### Comparing `gmanka_yml-22.0.5/pyproject.toml` & `gmanka_yml-23.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [project]
 dependencies = [
   "pyyaml",
 ]
 name = "gmanka_yml"
-version = "22.0.5"
+version = "23.0.0"
 authors = [
   { name="gmanka", email="gmankab@gmail.com" },
 ]
 description = "some useful shortcuts for pyyaml"
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `gmanka_yml-22.0.5/readme.md` & `gmanka_yml-23.0.0/readme.md`

 * *Files identical despite different names*

### Comparing `gmanka_yml-22.0.5/PKG-INFO` & `gmanka_yml-23.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmanka_yml
-Version: 22.0.5
+Version: 23.0.0
 Summary: some useful shortcuts for pyyaml
 Project-URL: Homepage, https://github.com/gmankab/yml
 Project-URL: Documentation, https://github.com/gmankab/yml
 Project-URL: Bug Tracker, https://github.com/gmankab/yml/issues
 Author-email: gmanka <gmankab@gmail.com>
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

