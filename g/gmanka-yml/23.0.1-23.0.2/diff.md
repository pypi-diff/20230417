# Comparing `tmp/gmanka_yml-23.0.1.tar.gz` & `tmp/gmanka_yml-23.0.2.tar.gz`

## Comparing `gmanka_yml-23.0.1.tar` & `gmanka_yml-23.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 gmanka_yml-23.0.1/changelog.md
--rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 gmanka_yml-23.0.1/start.sh
--rwxr-xr-x   0        0        0     1551 2020-02-02 00:00:00.000000 gmanka_yml-23.0.1/gmanka_yml/__init__.py
--rwxr-xr-x   0        0        0       24 2020-02-02 00:00:00.000000 gmanka_yml-23.0.1/.gitignore
--rwxr-xr-x   0        0        0      658 2020-02-02 00:00:00.000000 gmanka_yml-23.0.1/pyproject.toml
--rwxr-xr-x   0        0        0     1291 2020-02-02 00:00:00.000000 gmanka_yml-23.0.1/readme.md
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 gmanka_yml-23.0.1/PKG-INFO
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 gmanka_yml-23.0.2/changelog.md
+-rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 gmanka_yml-23.0.2/start.sh
+-rwxr-xr-x   0        0        0     1981 2020-02-02 00:00:00.000000 gmanka_yml-23.0.2/gmanka_yml/__init__.py
+-rwxr-xr-x   0        0        0       24 2020-02-02 00:00:00.000000 gmanka_yml-23.0.2/.gitignore
+-rwxr-xr-x   0        0        0      658 2020-02-02 00:00:00.000000 gmanka_yml-23.0.2/pyproject.toml
+-rwxr-xr-x   0        0        0     1493 2020-02-02 00:00:00.000000 gmanka_yml-23.0.2/readme.md
+-rw-r--r--   0        0        0     2067 2020-02-02 00:00:00.000000 gmanka_yml-23.0.2/PKG-INFO
```

### Comparing `gmanka_yml-23.0.1/pyproject.toml` & `gmanka_yml-23.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [project]
 dependencies = [
   "pyyaml",
 ]
 name = "gmanka_yml"
-version = "23.0.1"
+version = "23.0.2"
 authors = [
   { name="gmanka", email="gmankab@gmail.com" },
 ]
 description = "some useful shortcuts for pyyaml"
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `gmanka_yml-23.0.1/readme.md` & `gmanka_yml-23.0.2/readme.md`

 * *Files 16% similar despite different names*

```diff
@@ -95,7 +95,22 @@
 
 ```py
 yml.read_str(1) # raises TypeError
 
 yml.read_str(1, default = None) # returns None
 ```
 
+## expected_type
+
+```py
+yml.read_str(
+    data = '{}',
+    expected_type = list,
+) # raises TypeError
+
+yml.read_str(
+    data = '{}',
+    default = None,
+    expected_type = list,
+) # returns None
+```
+
```

### Comparing `gmanka_yml-23.0.1/PKG-INFO` & `gmanka_yml-23.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmanka_yml
-Version: 23.0.1
+Version: 23.0.2
 Summary: some useful shortcuts for pyyaml
 Project-URL: Homepage, https://github.com/gmankab/yml
 Project-URL: Documentation, https://github.com/gmankab/yml
 Project-URL: Bug Tracker, https://github.com/gmankab/yml/issues
 Author-email: gmanka <gmankab@gmail.com>
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -110,7 +110,22 @@
 
 ```py
 yml.read_str(1) # raises TypeError
 
 yml.read_str(1, default = None) # returns None
 ```
 
+## expected_type
+
+```py
+yml.read_str(
+    data = '{}',
+    expected_type = list,
+) # raises TypeError
+
+yml.read_str(
+    data = '{}',
+    default = None,
+    expected_type = list,
+) # returns None
+```
+
```

