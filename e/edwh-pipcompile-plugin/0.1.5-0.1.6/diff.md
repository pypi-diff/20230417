# Comparing `tmp/edwh_pipcompile_plugin-0.1.5.tar.gz` & `tmp/edwh_pipcompile_plugin-0.1.6.tar.gz`

## Comparing `edwh_pipcompile_plugin-0.1.5.tar` & `edwh_pipcompile_plugin-0.1.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.5/CHANGELOG.md
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.5/requirements-dev.in
--rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.5/requirements-dev.txt
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.5/src/edwh_pipcompile_plugin/__about__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.5/src/edwh_pipcompile_plugin/__init__.py
--rw-r--r--   0        0        0    10904 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.5/src/edwh_pipcompile_plugin/pipcompile_plugin.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.5/tests/__init__.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.5/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.5/LICENSE.txt
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.5/README.md
--rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.6/CHANGELOG.md
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.6/requirements-dev.in
+-rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.6/requirements-dev.txt
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.6/src/edwh_pipcompile_plugin/__about__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.6/src/edwh_pipcompile_plugin/__init__.py
+-rw-r--r--   0        0        0    10904 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.6/src/edwh_pipcompile_plugin/pipcompile_plugin.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.6/tests/__init__.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.6/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.6/LICENSE.txt
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.6/README.md
+-rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.6/PKG-INFO
```

### Comparing `edwh_pipcompile_plugin-0.1.5/CHANGELOG.md` & `edwh_pipcompile_plugin-0.1.6/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.1.6 (2023-04-17)
+### Fix
+* **semver:** Semantic-release types should be a comma-separated string, not an array ([`4dd0394`](https://github.com/educationwarehouse/edwh-pipcompile-plugin/commit/4dd039434decb2ed8e2b1feff6a061f5bc49b4e3))
+
 ## v0.1.5 (2023-04-17)
 
 
 ## v0.1.4 (2023-04-17)
 ### Fix
 * **project:** Remove theoretical support for Python versions below 3.10 since that has never worked ([`13f55b0`](https://github.com/educationwarehouse/edwh-pipcompile-plugin/commit/13f55b00cdc4f69c773c9771509e069dce2b8109))
```

### Comparing `edwh_pipcompile_plugin-0.1.5/requirements-dev.txt` & `edwh_pipcompile_plugin-0.1.6/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `edwh_pipcompile_plugin-0.1.5/src/edwh_pipcompile_plugin/pipcompile_plugin.py` & `edwh_pipcompile_plugin-0.1.6/src/edwh_pipcompile_plugin/pipcompile_plugin.py`

 * *Files identical despite different names*

### Comparing `edwh_pipcompile_plugin-0.1.5/LICENSE.txt` & `edwh_pipcompile_plugin-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh_pipcompile_plugin-0.1.5/README.md` & `edwh_pipcompile_plugin-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `edwh_pipcompile_plugin-0.1.5/pyproject.toml` & `edwh_pipcompile_plugin-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edwh_pipcompile_plugin-0.1.5/PKG-INFO` & `edwh_pipcompile_plugin-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edwh-pipcompile-plugin
-Version: 0.1.5
+Version: 0.1.6
 Summary: Plugin that integrates `pip-tools` with `edwh`
 Project-URL: Documentation, https://github.com/educationwarehouse/edwh-pipcompile-plugin#readme
 Project-URL: Issues, https://github.com/educationwarehouse/edwh-pipcompile-plugin/issues
 Project-URL: Source, https://github.com/educationwarehouse/edwh-pipcompile-plugin
 Author-email: Robin van der Noord <robin.vdn@educationwarehouse.nl>, Remco Boerma <remco.b@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
```

