# Comparing `tmp/gmanka_yml-23.0.3.tar.gz` & `tmp/gmanka_yml-23.0.4.tar.gz`

## Comparing `gmanka_yml-23.0.3.tar` & `gmanka_yml-23.0.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 gmanka_yml-23.0.3/changelog.md
--rwxr-xr-x   0        0        0     1831 2020-02-02 00:00:00.000000 gmanka_yml-23.0.3/gmanka_yml/__init__.py
--rwxr-xr-x   0        0        0       24 2020-02-02 00:00:00.000000 gmanka_yml-23.0.3/.gitignore
--rwxr-xr-x   0        0        0      658 2020-02-02 00:00:00.000000 gmanka_yml-23.0.3/pyproject.toml
--rwxr-xr-x   0        0        0     1493 2020-02-02 00:00:00.000000 gmanka_yml-23.0.3/readme.md
--rw-r--r--   0        0        0     2067 2020-02-02 00:00:00.000000 gmanka_yml-23.0.3/PKG-INFO
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 gmanka_yml-23.0.4/changelog.md
+-rwxr-xr-x   0        0        0     1831 2020-02-02 00:00:00.000000 gmanka_yml-23.0.4/gmanka_yml/__init__.py
+-rwxr-xr-x   0        0        0       24 2020-02-02 00:00:00.000000 gmanka_yml-23.0.4/.gitignore
+-rwxr-xr-x   0        0        0      658 2020-02-02 00:00:00.000000 gmanka_yml-23.0.4/pyproject.toml
+-rwxr-xr-x   0        0        0     1493 2020-02-02 00:00:00.000000 gmanka_yml-23.0.4/readme.md
+-rw-r--r--   0        0        0     2067 2020-02-02 00:00:00.000000 gmanka_yml-23.0.4/PKG-INFO
```

### Comparing `gmanka_yml-23.0.3/gmanka_yml/__init__.py` & `gmanka_yml-23.0.4/gmanka_yml/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from io import TextIOWrapper
 from pathlib import Path
 import yaml
 
 
-version = '23.0.1'
+version = '23.0.4'
 _sential = object()
 
 
 def to_str(
     data,
 ) -> str:
     try:
```

### Comparing `gmanka_yml-23.0.3/pyproject.toml` & `gmanka_yml-23.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [project]
 dependencies = [
   "pyyaml",
 ]
 name = "gmanka_yml"
-version = "23.0.3"
+version = "23.0.4"
 authors = [
   { name="gmanka", email="gmankab@gmail.com" },
 ]
 description = "some useful shortcuts for pyyaml"
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `gmanka_yml-23.0.3/readme.md` & `gmanka_yml-23.0.4/readme.md`

 * *Files identical despite different names*

### Comparing `gmanka_yml-23.0.3/PKG-INFO` & `gmanka_yml-23.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmanka_yml
-Version: 23.0.3
+Version: 23.0.4
 Summary: some useful shortcuts for pyyaml
 Project-URL: Homepage, https://github.com/gmankab/yml
 Project-URL: Documentation, https://github.com/gmankab/yml
 Project-URL: Bug Tracker, https://github.com/gmankab/yml/issues
 Author-email: gmanka <gmankab@gmail.com>
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

