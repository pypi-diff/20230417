# Comparing `tmp/evidence_ext-0.5.1.tar.gz` & `tmp/evidence_ext-0.5.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evidence_ext-0.5.1.tar", max compression
+gzip compressed data, was "evidence_ext-0.5.2a1.tar", max compression
```

## Comparing `evidence_ext-0.5.1.tar` & `evidence_ext-0.5.2a1.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1623 2023-02-21 19:02:52.222861 evidence_ext-0.5.1/README.md
--rw-r--r--   0        0        0       34 2023-02-21 19:02:52.222861 evidence_ext-0.5.1/evidence_ext/__init__.py
--rw-r--r--   0        0        0     5240 2023-02-21 19:02:52.222861 evidence_ext-0.5.1/evidence_ext/config.py
--rw-r--r--   0        0        0     4337 2023-02-21 19:02:52.222861 evidence_ext-0.5.1/evidence_ext/extension.py
--rw-r--r--   0        0        0     3949 2023-02-21 19:02:52.222861 evidence_ext-0.5.1/evidence_ext/main.py
--rw-r--r--   0        0        0     1442 2023-02-21 19:03:24.881454 evidence_ext-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     2528 1970-01-01 00:00:00.000000 evidence_ext-0.5.1/setup.py
--rw-r--r--   0        0        0     2404 1970-01-01 00:00:00.000000 evidence_ext-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1623 2023-04-17 21:09:01.311210 evidence_ext-0.5.2a1/README.md
+-rw-r--r--   0        0        0       34 2023-04-17 21:09:01.311210 evidence_ext-0.5.2a1/evidence_ext/__init__.py
+-rw-r--r--   0        0        0     5240 2023-04-17 21:09:01.311210 evidence_ext-0.5.2a1/evidence_ext/config.py
+-rw-r--r--   0        0        0     4337 2023-04-17 21:09:01.311210 evidence_ext-0.5.2a1/evidence_ext/extension.py
+-rw-r--r--   0        0        0     3949 2023-04-17 21:09:01.311210 evidence_ext-0.5.2a1/evidence_ext/main.py
+-rw-r--r--   0        0        0     1446 2023-04-17 21:09:24.167569 evidence_ext-0.5.2a1/pyproject.toml
+-rw-r--r--   0        0        0     2406 1970-01-01 00:00:00.000000 evidence_ext-0.5.2a1/PKG-INFO
```

### Comparing `evidence_ext-0.5.1/README.md` & `evidence_ext-0.5.2a1/README.md`

 * *Files identical despite different names*

### Comparing `evidence_ext-0.5.1/evidence_ext/config.py` & `evidence_ext-0.5.2a1/evidence_ext/config.py`

 * *Files identical despite different names*

### Comparing `evidence_ext-0.5.1/evidence_ext/extension.py` & `evidence_ext-0.5.2a1/evidence_ext/extension.py`

 * *Files identical despite different names*

### Comparing `evidence_ext-0.5.1/evidence_ext/main.py` & `evidence_ext-0.5.2a1/evidence_ext/main.py`

 * *Files identical despite different names*

### Comparing `evidence_ext-0.5.1/pyproject.toml` & `evidence_ext-0.5.2a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "evidence-ext"
-version = "0.5.1"
+version = "0.5.2-a.1"
 description = "`evidence-ext` is a Meltano utility extension."
 authors = ["Ken Payne"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [
     { include = "evidence_ext" },
     # uncomment this if you want to include static assets
```

### Comparing `evidence_ext-0.5.1/PKG-INFO` & `evidence_ext-0.5.2a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evidence-ext
-Version: 0.5.1
+Version: 0.5.2a1
 Summary: `evidence-ext` is a Meltano utility extension.
 License: Apache 2.0
 Author: Ken Payne
 Requires-Python: >=3.7,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

