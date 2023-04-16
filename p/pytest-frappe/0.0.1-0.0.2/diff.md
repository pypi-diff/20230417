# Comparing `tmp/pytest-frappe-0.0.1.tar.gz` & `tmp/pytest-frappe-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-frappe-0.0.1.tar", last modified: Fri Apr 14 13:19:12 2023, max compression
+gzip compressed data, was "pytest-frappe-0.0.2.tar", last modified: Sun Apr 16 23:52:51 2023, max compression
```

## Comparing `pytest-frappe-0.0.1.tar` & `pytest-frappe-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1819 2023-04-14 11:50:24.300726 pytest-frappe-0.0.1/.gitignore
--rw-r--r--   0        0        0     1066 2023-04-14 11:37:30.475170 pytest-frappe-0.0.1/LICENSE
--rw-r--r--   0        0        0      356 2023-04-14 12:07:20.818247 pytest-frappe-0.0.1/Makefile
--rw-r--r--   0        0        0       69 2023-04-14 11:37:30.475170 pytest-frappe-0.0.1/README.md
--rw-r--r--   0        0        0     1562 2023-04-14 12:10:26.797503 pytest-frappe-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       23 2023-04-14 12:13:17.962811 pytest-frappe-0.0.1/pytest_frappe/__init__.py
--rw-r--r--   0        0        0      920 2023-04-14 12:13:18.390859 pytest-frappe-0.0.1/pytest_frappe/fixtures.py
--rw-r--r--   0        0        0      279 2023-04-14 12:07:08.826506 pytest-frappe-0.0.1/setup.cfg
--rw-r--r--   0        0        0     1147 1970-01-01 00:00:00.000000 pytest-frappe-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1819 2023-04-14 11:50:24.300726 pytest-frappe-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1066 2023-04-14 11:37:30.475170 pytest-frappe-0.0.2/LICENSE
+-rw-r--r--   0        0        0      356 2023-04-14 12:07:20.818247 pytest-frappe-0.0.2/Makefile
+-rw-r--r--   0        0        0       69 2023-04-14 11:37:30.475170 pytest-frappe-0.0.2/README.md
+-rw-r--r--   0        0        0     1541 2023-04-16 23:45:11.707380 pytest-frappe-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       23 2023-04-16 23:50:29.116474 pytest-frappe-0.0.2/pytest_frappe/__init__.py
+-rw-r--r--   0        0        0      920 2023-04-14 12:13:18.390859 pytest-frappe-0.0.2/pytest_frappe/fixtures.py
+-rw-r--r--   0        0        0      279 2023-04-14 12:07:08.826506 pytest-frappe-0.0.2/setup.cfg
+-rw-r--r--   0        0        0     1118 1970-01-01 00:00:00.000000 pytest-frappe-0.0.2/PKG-INFO
```

### Comparing `pytest-frappe-0.0.1/.gitignore` & `pytest-frappe-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest-frappe-0.0.1/LICENSE` & `pytest-frappe-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-frappe-0.0.1/pyproject.toml` & `pytest-frappe-0.0.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,14 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Internet :: WWW/HTTP :: Session",
 ]
 requires-python = ">=3.9"
 dependencies = [
     "pytest>=7.0.0",
-    "frappe>=0.0.1",
 ]
 
 [project.optional-dependencies]
 dev = [
     "flake8",
     "pytest",
     "isort",
```

### Comparing `pytest-frappe-0.0.1/pytest_frappe/fixtures.py` & `pytest-frappe-0.0.2/pytest_frappe/fixtures.py`

 * *Files identical despite different names*

### Comparing `pytest-frappe-0.0.1/PKG-INFO` & `pytest-frappe-0.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: pytest-frappe
-Version: 0.0.1
+Version: 0.0.2
 Summary: Pytest Frappe Plugin - A set of pytest fixtures to test Frappe applications
 Author-email: 0xsirsaif <sirsaif99@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Internet :: WWW/HTTP :: Session
 Requires-Dist: pytest>=7.0.0
-Requires-Dist: frappe>=0.0.1
 Requires-Dist: flake8 ; extra == "dev"
 Requires-Dist: pytest ; extra == "dev"
 Requires-Dist: isort ; extra == "dev"
 Requires-Dist: black ; extra == "dev"
 Requires-Dist: mypy ; extra == "dev"
 Requires-Dist: flit ; extra == "dev"
 Project-URL: Documentation, https://github.com/0xsirsaif/pytest-frappe
```

