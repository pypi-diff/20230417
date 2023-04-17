# Comparing `tmp/pytest-frappe-0.0.3.tar.gz` & `tmp/pytest-frappe-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-frappe-0.0.3.tar", last modified: Mon Apr 17 00:02:12 2023, max compression
+gzip compressed data, was "pytest-frappe-0.0.4.tar", last modified: Mon Apr 17 01:07:11 2023, max compression
```

## Comparing `pytest-frappe-0.0.3.tar` & `pytest-frappe-0.0.4.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1819 2023-04-14 11:50:24.300726 pytest-frappe-0.0.3/.gitignore
--rw-r--r--   0        0        0     1066 2023-04-14 11:37:30.475170 pytest-frappe-0.0.3/LICENSE
--rw-r--r--   0        0        0      356 2023-04-14 12:07:20.818247 pytest-frappe-0.0.3/Makefile
--rw-r--r--   0        0        0       69 2023-04-14 11:37:30.475170 pytest-frappe-0.0.3/README.md
--rw-r--r--   0        0        0     1541 2023-04-16 23:45:11.707380 pytest-frappe-0.0.3/pyproject.toml
--rw-r--r--   0        0        0       86 2023-04-17 00:01:54.972073 pytest-frappe-0.0.3/pytest_frappe/__init__.py
--rw-r--r--   0        0        0      920 2023-04-14 12:13:18.390859 pytest-frappe-0.0.3/pytest_frappe/fixtures.py
--rw-r--r--   0        0        0      279 2023-04-14 12:07:08.826506 pytest-frappe-0.0.3/setup.cfg
--rw-r--r--   0        0        0     1118 1970-01-01 00:00:00.000000 pytest-frappe-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1819 2023-04-14 11:50:24.300726 pytest-frappe-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1066 2023-04-14 11:37:30.475170 pytest-frappe-0.0.4/LICENSE
+-rw-r--r--   0        0        0      356 2023-04-14 12:07:20.818247 pytest-frappe-0.0.4/Makefile
+-rw-r--r--   0        0        0       69 2023-04-14 11:37:30.475170 pytest-frappe-0.0.4/README.md
+-rw-r--r--   0        0        0     1541 2023-04-17 00:22:58.251748 pytest-frappe-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0       86 2023-04-17 01:04:40.309974 pytest-frappe-0.0.4/pytest_frappe/__init__.py
+-rw-r--r--   0        0        0      949 2023-04-17 01:04:39.909970 pytest-frappe-0.0.4/pytest_frappe/fixtures.py
+-rw-r--r--   0        0        0      149 2023-04-17 01:01:23.184320 pytest-frappe-0.0.4/pytest_frappe/plugin.py
+-rw-r--r--   0        0        0      279 2023-04-14 12:07:08.826506 pytest-frappe-0.0.4/setup.cfg
+-rw-r--r--   0        0        0     1118 1970-01-01 00:00:00.000000 pytest-frappe-0.0.4/PKG-INFO
```

### Comparing `pytest-frappe-0.0.3/.gitignore` & `pytest-frappe-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest-frappe-0.0.3/LICENSE` & `pytest-frappe-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-frappe-0.0.3/pyproject.toml` & `pytest-frappe-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytest-frappe-0.0.3/pytest_frappe/fixtures.py` & `pytest-frappe-0.0.4/pytest_frappe/fixtures.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import pathlib
 import frappe
 import pytest
 
 
-def get_site_configs():
+def get_site_configs(sites_path_as_str):
     """Returns the sites path and the current site"""
-    sites_path = pathlib.Path(__file__).parent.parent.parent.parent.parent / "sites"
+    sites_path = pathlib.Path(sites_path_as_str)
     current_site = sites_path / "currentsite.txt"
     with open(current_site, "r") as f:
         current_site = f.readline().strip()
     return str(sites_path), current_site
 
 
 @pytest.fixture(scope='session')
-def db_instance():
+def db_instance(request):
     """Returns a database instance."""
-    sites_path, current_site = get_site_configs()
+    sites_path, current_site = get_site_configs(request.config.getoption("--sites-path"))
+
     frappe.init(site=current_site, sites_path=sites_path)
     frappe.connect()
 
     # TODO: should we mock the commit method?
     # mock_commit = MagicMock()
     # frappe.db.commit = mock_commit
```

### Comparing `pytest-frappe-0.0.3/PKG-INFO` & `pytest-frappe-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-frappe
-Version: 0.0.3
+Version: 0.0.4
 Summary: Pytest Frappe Plugin - A set of pytest fixtures to test Frappe applications
 Author-email: 0xsirsaif <sirsaif99@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

