# Comparing `tmp/log_decor-2.0.4.tar.gz` & `tmp/log_decor-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "log_decor-2.0.4.tar", max compression
+gzip compressed data, was "log_decor-2.0.5.tar", max compression
```

## Comparing `log_decor-2.0.4.tar` & `log_decor-2.0.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1073 2023-04-05 15:23:21.185474 log_decor-2.0.4/LICENSE
--rw-r--r--   0        0        0      600 2023-04-05 15:23:21.185474 log_decor-2.0.4/README.rst
--rw-r--r--   0        0        0      191 2023-04-05 15:23:21.185474 log_decor-2.0.4/log_decor/__init__.py
--rw-r--r--   0        0        0      853 2023-04-05 15:23:21.185474 log_decor-2.0.4/log_decor/add.py
--rw-r--r--   0        0        0     2775 2023-04-05 15:23:21.185474 log_decor-2.0.4/log_decor/func.py
--rw-r--r--   0        0        0     2514 2023-04-05 15:23:21.185474 log_decor-2.0.4/log_decor/info.py
--rw-r--r--   0        0        0     1690 2023-04-05 15:23:21.185474 log_decor-2.0.4/log_decor/msg.py
--rw-r--r--   0        0        0      690 2023-04-05 15:23:38.109309 log_decor-2.0.4/pyproject.toml
--rw-r--r--   0        0        0     1227 1970-01-01 00:00:00.000000 log_decor-2.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-17 18:37:17.844987 log_decor-2.0.5/LICENSE
+-rw-r--r--   0        0        0      600 2023-04-17 18:37:17.844987 log_decor-2.0.5/README.rst
+-rw-r--r--   0        0        0      191 2023-04-17 18:37:17.844987 log_decor-2.0.5/log_decor/__init__.py
+-rw-r--r--   0        0        0      853 2023-04-17 18:37:17.844987 log_decor-2.0.5/log_decor/add.py
+-rw-r--r--   0        0        0     2775 2023-04-17 18:37:17.844987 log_decor-2.0.5/log_decor/func.py
+-rw-r--r--   0        0        0     2514 2023-04-17 18:37:17.844987 log_decor-2.0.5/log_decor/info.py
+-rw-r--r--   0        0        0     1690 2023-04-17 18:37:17.844987 log_decor-2.0.5/log_decor/msg.py
+-rw-r--r--   0        0        0      690 2023-04-17 18:37:36.445207 log_decor-2.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1227 1970-01-01 00:00:00.000000 log_decor-2.0.5/PKG-INFO
```

### Comparing `log_decor-2.0.4/LICENSE` & `log_decor-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `log_decor-2.0.4/README.rst` & `log_decor-2.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `log_decor-2.0.4/log_decor/add.py` & `log_decor-2.0.5/log_decor/add.py`

 * *Files identical despite different names*

### Comparing `log_decor-2.0.4/log_decor/func.py` & `log_decor-2.0.5/log_decor/func.py`

 * *Files identical despite different names*

### Comparing `log_decor-2.0.4/log_decor/info.py` & `log_decor-2.0.5/log_decor/info.py`

 * *Files identical despite different names*

### Comparing `log_decor-2.0.4/log_decor/msg.py` & `log_decor-2.0.5/log_decor/msg.py`

 * *Files identical despite different names*

### Comparing `log_decor-2.0.4/pyproject.toml` & `log_decor-2.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "log_decor"
-version = "2.0.4"
+version = "2.0.5"
 description = "Logging decorators for functions and methods."
 authors = ["Bernardo Paulsen <paulsen.bernardo@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 packages = [{ include = "log_decor" }]
 keywords = ["logging", "decorator", "OOP"]
```

### Comparing `log_decor-2.0.4/PKG-INFO` & `log_decor-2.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: log-decor
-Version: 2.0.4
+Version: 2.0.5
 Summary: Logging decorators for functions and methods.
 License: MIT
 Keywords: logging,decorator,OOP
 Author: Bernardo Paulsen
 Author-email: paulsen.bernardo@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

