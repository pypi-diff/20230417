# Comparing `tmp/pytest-frappe-0.0.7.tar.gz` & `tmp/pytest-frappe-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-frappe-0.0.7.tar", last modified: Mon Apr 17 14:18:23 2023, max compression
+gzip compressed data, was "pytest-frappe-0.0.8.tar", last modified: Mon Apr 17 14:20:32 2023, max compression
```

## Comparing `pytest-frappe-0.0.7.tar` & `pytest-frappe-0.0.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1819 2023-04-14 11:50:24.300726 pytest-frappe-0.0.7/.gitignore
--rw-r--r--   0        0        0     1066 2023-04-14 11:37:30.475170 pytest-frappe-0.0.7/LICENSE
--rw-r--r--   0        0        0      356 2023-04-14 12:07:20.818247 pytest-frappe-0.0.7/Makefile
--rw-r--r--   0        0        0       69 2023-04-14 11:37:30.475170 pytest-frappe-0.0.7/README.md
--rw-r--r--   0        0        0     1606 2023-04-17 14:14:17.766917 pytest-frappe-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      119 2023-04-17 14:17:24.489198 pytest-frappe-0.0.7/pytest_frappe/__init__.py
--rw-r--r--   0        0        0      963 2023-04-17 14:15:25.070473 pytest-frappe-0.0.7/pytest_frappe/fixtures.py
--rw-r--r--   0        0        0      194 2023-04-17 14:16:22.166615 pytest-frappe-0.0.7/pytest_frappe/plugin.py
--rw-r--r--   0        0        0      279 2023-04-14 12:07:08.826506 pytest-frappe-0.0.7/setup.cfg
--rw-r--r--   0        0        0     1118 1970-01-01 00:00:00.000000 pytest-frappe-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1819 2023-04-14 11:50:24.300726 pytest-frappe-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1066 2023-04-14 11:37:30.475170 pytest-frappe-0.0.8/LICENSE
+-rw-r--r--   0        0        0      356 2023-04-14 12:07:20.818247 pytest-frappe-0.0.8/Makefile
+-rw-r--r--   0        0        0       69 2023-04-14 11:37:30.475170 pytest-frappe-0.0.8/README.md
+-rw-r--r--   0        0        0     1613 2023-04-17 14:19:41.748819 pytest-frappe-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      119 2023-04-17 14:19:52.273556 pytest-frappe-0.0.8/pytest_frappe/__init__.py
+-rw-r--r--   0        0        0      963 2023-04-17 14:15:25.070473 pytest-frappe-0.0.8/pytest_frappe/fixtures.py
+-rw-r--r--   0        0        0      194 2023-04-17 14:16:22.166615 pytest-frappe-0.0.8/pytest_frappe/plugin.py
+-rw-r--r--   0        0        0      279 2023-04-14 12:07:08.826506 pytest-frappe-0.0.8/setup.cfg
+-rw-r--r--   0        0        0     1118 1970-01-01 00:00:00.000000 pytest-frappe-0.0.8/PKG-INFO
```

### Comparing `pytest-frappe-0.0.7/.gitignore` & `pytest-frappe-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest-frappe-0.0.7/LICENSE` & `pytest-frappe-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-frappe-0.0.7/pyproject.toml` & `pytest-frappe-0.0.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -54,8 +54,8 @@
     "flit",
 ]
 
 [project.urls]
 Documentation = "https://github.com/0xsirsaif/pytest-frappe"
 
 [project.entry-points.pytest11]
-pytest_frappe = "pytest_frappe"
+pytest_frappe = "pytest_frappe.plugin"
```

### Comparing `pytest-frappe-0.0.7/pytest_frappe/fixtures.py` & `pytest-frappe-0.0.8/pytest_frappe/fixtures.py`

 * *Files identical despite different names*

### Comparing `pytest-frappe-0.0.7/PKG-INFO` & `pytest-frappe-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-frappe
-Version: 0.0.7
+Version: 0.0.8
 Summary: Pytest Frappe Plugin - A set of pytest fixtures to test Frappe applications
 Author-email: 0xsirsaif <sirsaif99@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

