# Comparing `tmp/edwh_pipcompile_plugin-0.1.3.tar.gz` & `tmp/edwh_pipcompile_plugin-0.1.4.tar.gz`

## Comparing `edwh_pipcompile_plugin-0.1.3.tar` & `edwh_pipcompile_plugin-0.1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.3/CHANGELOG.md
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.3/requirements-dev.in
--rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.3/requirements-dev.txt
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.3/src/edwh_pipcompile_plugin/__about__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.3/src/edwh_pipcompile_plugin/__init__.py
--rw-r--r--   0        0        0    10904 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.3/src/edwh_pipcompile_plugin/pipcompile_plugin.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.3/tests/__init__.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.3/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.3/LICENSE.txt
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.3/README.md
--rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.4/CHANGELOG.md
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.4/requirements-dev.in
+-rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.4/requirements-dev.txt
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.4/src/edwh_pipcompile_plugin/__about__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.4/src/edwh_pipcompile_plugin/__init__.py
+-rw-r--r--   0        0        0    10904 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.4/src/edwh_pipcompile_plugin/pipcompile_plugin.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.4/LICENSE.txt
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.4/README.md
+-rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.4/PKG-INFO
```

### Comparing `edwh_pipcompile_plugin-0.1.3/CHANGELOG.md` & `edwh_pipcompile_plugin-0.1.4/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.1.4 (2023-04-17)
+### Fix
+* **project:** Remove theoretical support for Python versions below 3.10 since that has never worked ([`13f55b0`](https://github.com/educationwarehouse/edwh-pipcompile-plugin/commit/13f55b00cdc4f69c773c9771509e069dce2b8109))
+
 ## v0.1.3 (2023-04-11)
 ### Fix
 * **pip.test:** Remove debug task ([`593dc8c`](https://github.com/educationwarehouse/edwh-pipcompile-plugin/commit/593dc8c4704dd17b519ae1bd8310938399d49b95))
 
 ## v0.1.2 (2023-04-11)
 ### Fix
 * **deps:** Remove `pip.install-pip-tools` since that is a dependency of the plugin already ([`52a0658`](https://github.com/educationwarehouse/edwh-pipcompile-plugin/commit/52a0658d89e60bbc7a6ef972fc2638105090fa91))
```

### Comparing `edwh_pipcompile_plugin-0.1.3/requirements-dev.txt` & `edwh_pipcompile_plugin-0.1.4/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `edwh_pipcompile_plugin-0.1.3/src/edwh_pipcompile_plugin/pipcompile_plugin.py` & `edwh_pipcompile_plugin-0.1.4/src/edwh_pipcompile_plugin/pipcompile_plugin.py`

 * *Files identical despite different names*

### Comparing `edwh_pipcompile_plugin-0.1.3/LICENSE.txt` & `edwh_pipcompile_plugin-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh_pipcompile_plugin-0.1.3/README.md` & `edwh_pipcompile_plugin-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `edwh_pipcompile_plugin-0.1.3/pyproject.toml` & `edwh_pipcompile_plugin-0.1.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -3,27 +3,24 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "edwh-pipcompile-plugin"
 dynamic = ["version"]
 description = 'Plugin that integrates `pip-tools` with `edwh`'
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.10"
 license = "MIT"
 keywords = []
 authors = [
   { name = "Robin van der Noord", email = "robin.vdn@educationwarehouse.nl" },
   { name = "Remco Boerma", email = "remco.b@educationwarehouse.nl" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
-  "Programming Language :: Python :: 3.7",
-  "Programming Language :: Python :: 3.8",
-  "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = ['invoke', "pip-tools"]
 
@@ -60,15 +57,15 @@
 ]
 cov = [
   "test-cov",
   "cov-report",
 ]
 
 [[tool.hatch.envs.all.matrix]]
-python = ["3.7", "3.8", "3.9", "3.10", "3.11"]
+python = ["3.10", "3.11"]
 
 [tool.hatch.envs.lint]
 detached = true
 dependencies = [
   "black>=23.1.0",
   "mypy>=1.0.0",
   "ruff>=0.0.243",
```

### Comparing `edwh_pipcompile_plugin-0.1.3/PKG-INFO` & `edwh_pipcompile_plugin-0.1.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 Metadata-Version: 2.1
 Name: edwh-pipcompile-plugin
-Version: 0.1.3
+Version: 0.1.4
 Summary: Plugin that integrates `pip-tools` with `edwh`
 Project-URL: Documentation, https://github.com/educationwarehouse/edwh-pipcompile-plugin#readme
 Project-URL: Issues, https://github.com/educationwarehouse/edwh-pipcompile-plugin/issues
 Project-URL: Source, https://github.com/educationwarehouse/edwh-pipcompile-plugin
 Author-email: Robin van der Noord <robin.vdn@educationwarehouse.nl>, Remco Boerma <remco.b@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Requires-Dist: invoke
 Requires-Dist: pip-tools
 Description-Content-Type: text/markdown
 
 # edwh-pipcompile-plugin
 
 [![PyPI - Version](https://img.shields.io/pypi/v/edwh-pipcompile-plugin.svg)](https://pypi.org/project/edwh-pipcompile-plugin)
```

