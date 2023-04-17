# Comparing `tmp/pytest-frappe-0.0.5.tar.gz` & `tmp/pytest-frappe-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-frappe-0.0.5.tar", last modified: Mon Apr 17 02:59:57 2023, max compression
+gzip compressed data, was "pytest-frappe-0.0.6.tar", last modified: Mon Apr 17 03:29:37 2023, max compression
```

## Comparing `pytest-frappe-0.0.5.tar` & `pytest-frappe-0.0.6.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1819 2023-04-14 11:50:24.300726 pytest-frappe-0.0.5/.gitignore
--rw-r--r--   0        0        0     1066 2023-04-14 11:37:30.475170 pytest-frappe-0.0.5/LICENSE
--rw-r--r--   0        0        0      356 2023-04-14 12:07:20.818247 pytest-frappe-0.0.5/Makefile
--rw-r--r--   0        0        0       69 2023-04-14 11:37:30.475170 pytest-frappe-0.0.5/README.md
--rw-r--r--   0        0        0     1541 2023-04-17 00:22:58.251748 pytest-frappe-0.0.5/pyproject.toml
--rw-r--r--   0        0        0       86 2023-04-17 02:59:38.446751 pytest-frappe-0.0.5/pytest_frappe/__init__.py
--rw-r--r--   0        0        0      963 2023-04-17 02:59:00.031437 pytest-frappe-0.0.5/pytest_frappe/fixtures.py
--rw-r--r--   0        0        0      194 2023-04-17 02:58:59.615444 pytest-frappe-0.0.5/pytest_frappe/plugin.py
--rw-r--r--   0        0        0      279 2023-04-14 12:07:08.826506 pytest-frappe-0.0.5/setup.cfg
--rw-r--r--   0        0        0     1118 1970-01-01 00:00:00.000000 pytest-frappe-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1819 2023-04-14 11:50:24.300726 pytest-frappe-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1066 2023-04-14 11:37:30.475170 pytest-frappe-0.0.6/LICENSE
+-rw-r--r--   0        0        0      356 2023-04-14 12:07:20.818247 pytest-frappe-0.0.6/Makefile
+-rw-r--r--   0        0        0       69 2023-04-14 11:37:30.475170 pytest-frappe-0.0.6/README.md
+-rw-r--r--   0        0        0     1541 2023-04-17 00:22:58.251748 pytest-frappe-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0       86 2023-04-17 03:27:40.278207 pytest-frappe-0.0.6/pytest_frappe/__init__.py
+-rw-r--r--   0        0        0     1159 2023-04-17 03:26:52.621198 pytest-frappe-0.0.6/pytest_frappe/fixtures.py
+-rw-r--r--   0        0        0      279 2023-04-14 12:07:08.826506 pytest-frappe-0.0.6/setup.cfg
+-rw-r--r--   0        0        0     1118 1970-01-01 00:00:00.000000 pytest-frappe-0.0.6/PKG-INFO
```

### Comparing `pytest-frappe-0.0.5/.gitignore` & `pytest-frappe-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest-frappe-0.0.5/LICENSE` & `pytest-frappe-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-frappe-0.0.5/pyproject.toml` & `pytest-frappe-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytest-frappe-0.0.5/PKG-INFO` & `pytest-frappe-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-frappe
-Version: 0.0.5
+Version: 0.0.6
 Summary: Pytest Frappe Plugin - A set of pytest fixtures to test Frappe applications
 Author-email: 0xsirsaif <sirsaif99@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

