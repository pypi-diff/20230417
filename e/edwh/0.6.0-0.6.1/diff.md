# Comparing `tmp/edwh-0.6.0.tar.gz` & `tmp/edwh-0.6.1.tar.gz`

## Comparing `edwh-0.6.0.tar` & `edwh-0.6.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     3401 2020-02-02 00:00:00.000000 edwh-0.6.0/CHANGELOG.md
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 edwh-0.6.0/config.toml
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 edwh-0.6.0/requirements-dev.txt
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh-0.6.0/src/edwh/__about__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh-0.6.0/src/edwh/__init__.py
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 edwh-0.6.0/src/edwh/cli.py
--rw-r--r--   0        0        0    21484 2020-02-02 00:00:00.000000 edwh-0.6.0/src/edwh/tasks.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh-0.6.0/tests/__init__.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 edwh-0.6.0/.gitignore
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 edwh-0.6.0/LICENSE.txt
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 edwh-0.6.0/README.md
--rw-r--r--   0        0        0     4303 2020-02-02 00:00:00.000000 edwh-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     4046 2020-02-02 00:00:00.000000 edwh-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     3426 2020-02-02 00:00:00.000000 edwh-0.6.1/CHANGELOG.md
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 edwh-0.6.1/config.toml
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 edwh-0.6.1/requirements-dev.txt
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh-0.6.1/src/edwh/__about__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh-0.6.1/src/edwh/__init__.py
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 edwh-0.6.1/src/edwh/cli.py
+-rw-r--r--   0        0        0    21484 2020-02-02 00:00:00.000000 edwh-0.6.1/src/edwh/tasks.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh-0.6.1/tests/__init__.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 edwh-0.6.1/.gitignore
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 edwh-0.6.1/LICENSE.txt
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 edwh-0.6.1/README.md
+-rw-r--r--   0        0        0     4404 2020-02-02 00:00:00.000000 edwh-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 edwh-0.6.1/PKG-INFO
```

### Comparing `edwh-0.6.0/CHANGELOG.md` & `edwh-0.6.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.6.1 (2023-04-17)
+
+
 ## v0.6.0 (2023-04-17)
 ### Feature
 * **core:** Replaced invoke with fabric for possibly more plugin functionality ([`85838ea`](https://github.com/educationwarehouse/edwh/commit/85838ea3b4cd2a50dc6e8a90e3955d9d82778b0f))
 
 ### Fix
 * **project:** Remove theoretical support for Python versions below 3.10 since that has never worked ([`2f567e2`](https://github.com/educationwarehouse/edwh/commit/2f567e2404a3c10019b9bc8efd39c2ed4248bca3))
 * **dependencies:** Importilb is only a package for python 2, not needed as dependency for py 3 ([`f5e0745`](https://github.com/educationwarehouse/edwh/commit/f5e0745f143d09cd6a9cfc4b5884d8f11faa2e35))
```

### Comparing `edwh-0.6.0/src/edwh/cli.py` & `edwh-0.6.1/src/edwh/cli.py`

 * *Files identical despite different names*

### Comparing `edwh-0.6.0/src/edwh/tasks.py` & `edwh-0.6.1/src/edwh/tasks.py`

 * *Files identical despite different names*

### Comparing `edwh-0.6.0/LICENSE.txt` & `edwh-0.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh-0.6.0/README.md` & `edwh-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `edwh-0.6.0/pyproject.toml` & `edwh-0.6.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -47,15 +47,20 @@
   'tomlkit'
 ]
 plugins = [
   'edwh-multipass-plugin',
   'edwh-demo-tasks-plugin',
   'edwh-restic-plugin',
   'edwh-pipcompile-plugin',
-  'edwh-bundler-plugin'
+  'edwh-bundler-plugin',
+  'edwh-server-provisioning-plugin',
+]
+
+server-provisioning = [
+  "edwh-server-provisioning-plugin"
 ]
 
 restic = [
   'edwh-restic-plugin',
 ]
 
 multipass = [
```

### Comparing `edwh-0.6.0/PKG-INFO` & `edwh-0.6.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edwh
-Version: 0.6.0
+Version: 0.6.1
 Summary: Education Warehouse maintenance tools
 Project-URL: Documentation, https://github.com/educationwarehouse/edwh#readme
 Project-URL: Issues, https://github.com/educationwarehouse/edwh/issues
 Project-URL: Source, https://github.com/educationwarehouse/edwh
 Author-email: Remco Boerma <remco.b@educationwarehouse.nl>, Robin van der Noord <robin.vdn@educationwarehouse.nl>, Romy Schöller <romy.s@educationwarehouse.nl>, Sven Keimpema <sven.k@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -43,16 +43,19 @@
 Requires-Dist: edwh-pipcompile-plugin; extra == 'pip-compile'
 Provides-Extra: plugins
 Requires-Dist: edwh-bundler-plugin; extra == 'plugins'
 Requires-Dist: edwh-demo-tasks-plugin; extra == 'plugins'
 Requires-Dist: edwh-multipass-plugin; extra == 'plugins'
 Requires-Dist: edwh-pipcompile-plugin; extra == 'plugins'
 Requires-Dist: edwh-restic-plugin; extra == 'plugins'
+Requires-Dist: edwh-server-provisioning-plugin; extra == 'plugins'
 Provides-Extra: restic
 Requires-Dist: edwh-restic-plugin; extra == 'restic'
+Provides-Extra: server-provisioning
+Requires-Dist: edwh-server-provisioning-plugin; extra == 'server-provisioning'
 Description-Content-Type: text/markdown
 
 # edwh
 
 [![PyPI - Version](https://img.shields.io/pypi/v/edwh.svg)](https://pypi.org/project/edwh)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/edwh.svg)](https://pypi.org/project/edwh)
```

