# Comparing `tmp/edwh_bundler_plugin-0.1.3.tar.gz` & `tmp/edwh_bundler_plugin-0.1.4.tar.gz`

## Comparing `edwh_bundler_plugin-0.1.3.tar` & `edwh_bundler_plugin-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.3/CHANGELOG.md
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.3/requirements-dev.in
--rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.3/requirements-dev.txt
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.3/src/edwh_bundler_plugin/__about__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.3/src/edwh_bundler_plugin/__init__.py
--rw-r--r--   0        0        0    19514 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.3/src/edwh_bundler_plugin/bundler_plugin.py
--rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.3/src/edwh_bundler_plugin/css.py
--rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.3/src/edwh_bundler_plugin/js.py
--rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.3/src/edwh_bundler_plugin/shared.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.3/tests/__init__.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.3/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.3/LICENSE.txt
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.3/README.md
--rw-r--r--   0        0        0     3894 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.4/CHANGELOG.md
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.4/requirements-dev.in
+-rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.4/requirements-dev.txt
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.4/src/edwh_bundler_plugin/__about__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.4/src/edwh_bundler_plugin/__init__.py
+-rw-r--r--   0        0        0    19514 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.4/src/edwh_bundler_plugin/bundler_plugin.py
+-rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.4/src/edwh_bundler_plugin/css.py
+-rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.4/src/edwh_bundler_plugin/js.py
+-rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.4/src/edwh_bundler_plugin/shared.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.4/LICENSE.txt
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.4/README.md
+-rw-r--r--   0        0        0     3745 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.4/PKG-INFO
```

### Comparing `edwh_bundler_plugin-0.1.3/CHANGELOG.md` & `edwh_bundler_plugin-0.1.4/CHANGELOG.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.1.4 (2023-04-17)
+### Fix
+* **project:** Remove theoretical support for Python versions below 3.10 since that has never worked ([`daa3e39`](https://github.com/educationwarehouse/edwh-bundler-plugin/commit/daa3e39abe7627a09c93ccfeb42e164612c14b6c))
+
 ## v0.1.3 (2023-04-17)
 ### Fix
 * **publish:** .db file moved to tmp ([`11613ca`](https://github.com/educationwarehouse/edwh-bundler-plugin/commit/11613caab17da02526358c5291a3f737c6d4b859))
 
 ## v0.1.2 (2023-04-11)
 ### Documentation
 * **changelog:** Manual fix changelog for missing version ([`68a71ed`](https://github.com/educationwarehouse/edwh-bundler-plugin/commit/68a71ed76ae53d758f45aca70fa2a61bbbff5a9d))
```

### Comparing `edwh_bundler_plugin-0.1.3/requirements-dev.txt` & `edwh_bundler_plugin-0.1.4/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `edwh_bundler_plugin-0.1.3/src/edwh_bundler_plugin/bundler_plugin.py` & `edwh_bundler_plugin-0.1.4/src/edwh_bundler_plugin/bundler_plugin.py`

 * *Files identical despite different names*

### Comparing `edwh_bundler_plugin-0.1.3/src/edwh_bundler_plugin/css.py` & `edwh_bundler_plugin-0.1.4/src/edwh_bundler_plugin/css.py`

 * *Files identical despite different names*

### Comparing `edwh_bundler_plugin-0.1.3/src/edwh_bundler_plugin/js.py` & `edwh_bundler_plugin-0.1.4/src/edwh_bundler_plugin/js.py`

 * *Files identical despite different names*

### Comparing `edwh_bundler_plugin-0.1.3/src/edwh_bundler_plugin/shared.py` & `edwh_bundler_plugin-0.1.4/src/edwh_bundler_plugin/shared.py`

 * *Files identical despite different names*

### Comparing `edwh_bundler_plugin-0.1.3/LICENSE.txt` & `edwh_bundler_plugin-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh_bundler_plugin-0.1.3/README.md` & `edwh_bundler_plugin-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `edwh_bundler_plugin-0.1.3/pyproject.toml` & `edwh_bundler_plugin-0.1.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -3,27 +3,24 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "edwh-bundler-plugin"
 dynamic = ["version"]
 description = 'Python-only static file (js, css) bundler for `edwh`'
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
 dependencies = ['invoke', 'python-dotenv', 'pysass', 'rjsmin', 'httpx', 'pyyaml']
 
@@ -61,15 +58,15 @@
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

### Comparing `edwh_bundler_plugin-0.1.3/PKG-INFO` & `edwh_bundler_plugin-0.1.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 Metadata-Version: 2.1
 Name: edwh-bundler-plugin
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python-only static file (js, css) bundler for `edwh`
 Project-URL: Documentation, https://github.com/educationwarehouse/edwh-bundler-plugin#readme
 Project-URL: Issues, https://github.com/educationwarehouse/edwh-bundler-plugin/issues
 Project-URL: Source, https://github.com/educationwarehouse/edwh-bundler-plugin
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
 Requires-Dist: httpx
 Requires-Dist: invoke
 Requires-Dist: pysass
 Requires-Dist: python-dotenv
 Requires-Dist: pyyaml
 Requires-Dist: rjsmin
 Description-Content-Type: text/markdown
```

