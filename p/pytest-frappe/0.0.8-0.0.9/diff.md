# Comparing `tmp/pytest-frappe-0.0.8.tar.gz` & `tmp/pytest-frappe-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-frappe-0.0.8.tar", last modified: Mon Apr 17 14:20:32 2023, max compression
+gzip compressed data, was "pytest-frappe-0.0.9.tar", last modified: Mon Apr 17 14:36:22 2023, max compression
```

## Comparing `pytest-frappe-0.0.8.tar` & `pytest-frappe-0.0.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1819 2023-04-14 11:50:24.300726 pytest-frappe-0.0.8/.gitignore
--rw-r--r--   0        0        0     1066 2023-04-14 11:37:30.475170 pytest-frappe-0.0.8/LICENSE
--rw-r--r--   0        0        0      356 2023-04-14 12:07:20.818247 pytest-frappe-0.0.8/Makefile
--rw-r--r--   0        0        0       69 2023-04-14 11:37:30.475170 pytest-frappe-0.0.8/README.md
--rw-r--r--   0        0        0     1613 2023-04-17 14:19:41.748819 pytest-frappe-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      119 2023-04-17 14:19:52.273556 pytest-frappe-0.0.8/pytest_frappe/__init__.py
--rw-r--r--   0        0        0      963 2023-04-17 14:15:25.070473 pytest-frappe-0.0.8/pytest_frappe/fixtures.py
--rw-r--r--   0        0        0      194 2023-04-17 14:16:22.166615 pytest-frappe-0.0.8/pytest_frappe/plugin.py
--rw-r--r--   0        0        0      279 2023-04-14 12:07:08.826506 pytest-frappe-0.0.8/setup.cfg
--rw-r--r--   0        0        0     1118 1970-01-01 00:00:00.000000 pytest-frappe-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1819 2023-04-14 11:50:24.300726 pytest-frappe-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1066 2023-04-14 11:37:30.475170 pytest-frappe-0.0.9/LICENSE
+-rw-r--r--   0        0        0      356 2023-04-14 12:07:20.818247 pytest-frappe-0.0.9/Makefile
+-rw-r--r--   0        0        0       69 2023-04-14 11:37:30.475170 pytest-frappe-0.0.9/README.md
+-rw-r--r--   0        0        0     1411 2023-04-17 14:28:42.325679 pytest-frappe-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      119 2023-04-17 14:35:35.089311 pytest-frappe-0.0.9/pytest_frappe/__init__.py
+-rw-r--r--   0        0        0      963 2023-04-17 14:15:25.070473 pytest-frappe-0.0.9/pytest_frappe/fixtures.py
+-rw-r--r--   0        0        0      259 2023-04-17 14:35:34.965334 pytest-frappe-0.0.9/pytest_frappe/plugin.py
+-rw-r--r--   0        0        0      279 2023-04-14 12:07:08.826506 pytest-frappe-0.0.9/setup.cfg
+-rw-r--r--   0        0        0      896 1970-01-01 00:00:00.000000 pytest-frappe-0.0.9/PKG-INFO
```

### Comparing `pytest-frappe-0.0.8/.gitignore` & `pytest-frappe-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest-frappe-0.0.8/LICENSE` & `pytest-frappe-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-frappe-0.0.8/pyproject.toml` & `pytest-frappe-0.0.9/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -28,20 +28,16 @@
 # This clearly delineates which metadata is purposefully unspecified and expected to stay unspecified
 # compared to being provided via tooling later on.
 dynamic = ["version"]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
+    "Framework :: Pytest",
     "Programming Language :: Python :: 3 :: Only",
-    "Topic :: Internet :: WWW/HTTP :: Session",
 ]
 requires-python = ">=3.9"
 dependencies = [
     "pytest>=7.0.0",
 ]
 
 [project.optional-dependencies]
```

### Comparing `pytest-frappe-0.0.8/pytest_frappe/fixtures.py` & `pytest-frappe-0.0.9/pytest_frappe/fixtures.py`

 * *Files identical despite different names*

### Comparing `pytest-frappe-0.0.8/PKG-INFO` & `pytest-frappe-0.0.9/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 Metadata-Version: 2.1
 Name: pytest-frappe
-Version: 0.0.8
+Version: 0.0.9
 Summary: Pytest Frappe Plugin - A set of pytest fixtures to test Frappe applications
 Author-email: 0xsirsaif <sirsaif99@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Framework :: Pytest
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Topic :: Internet :: WWW/HTTP :: Session
 Requires-Dist: pytest>=7.0.0
 Requires-Dist: flake8 ; extra == "dev"
 Requires-Dist: pytest ; extra == "dev"
 Requires-Dist: isort ; extra == "dev"
 Requires-Dist: black ; extra == "dev"
 Requires-Dist: mypy ; extra == "dev"
 Requires-Dist: flit ; extra == "dev"
```

