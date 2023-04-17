# Comparing `tmp/accurating-0.3.tar.gz` & `tmp/accurating-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accurating-0.3.tar", max compression
+gzip compressed data, was "accurating-0.3.1.tar", max compression
```

## Comparing `accurating-0.3.tar` & `accurating-0.3.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1068 2023-04-16 18:25:22.173292 accurating-0.3/LICENSE
--rw-r--r--   0        0        0      126 2023-04-16 18:26:44.687984 accurating-0.3/README.md
--rw-r--r--   0        0        0       77 2023-04-16 19:43:19.355111 accurating-0.3/accurating/__init__.py
--rw-r--r--   0        0        0     4613 2023-04-16 20:02:11.985128 accurating-0.3/accurating/model.py
--rw-r--r--   0        0        0        0 2023-04-16 18:25:22.173292 accurating-0.3/accurating/tests/__init__.py
--rw-r--r--   0        0        0     3313 2023-04-16 20:07:51.802000 accurating-0.3/accurating/tests/model_test.py
--rw-r--r--   0        0        0      460 2023-04-16 20:16:28.967228 accurating-0.3/pyproject.toml
--rw-r--r--   0        0        0      577 1970-01-01 00:00:00.000000 accurating-0.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-16 18:25:22.173292 accurating-0.3.1/LICENSE
+-rw-r--r--   0        0        0     5888 2023-04-16 20:21:22.236412 accurating-0.3.1/README.md
+-rw-r--r--   0        0        0       77 2023-04-16 19:43:19.355111 accurating-0.3.1/accurating/__init__.py
+-rw-r--r--   0        0        0     4613 2023-04-16 20:02:11.985128 accurating-0.3.1/accurating/model.py
+-rw-r--r--   0        0        0        0 2023-04-16 18:25:22.173292 accurating-0.3.1/accurating/tests/__init__.py
+-rw-r--r--   0        0        0     3313 2023-04-16 20:07:51.802000 accurating-0.3.1/accurating/tests/model_test.py
+-rw-r--r--   0        0        0      462 2023-04-16 20:20:40.120259 accurating-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     6341 1970-01-01 00:00:00.000000 accurating-0.3.1/PKG-INFO
```

### Comparing `accurating-0.3/LICENSE` & `accurating-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `accurating-0.3/accurating/model.py` & `accurating-0.3.1/accurating/model.py`

 * *Files identical despite different names*

### Comparing `accurating-0.3/accurating/tests/model_test.py` & `accurating-0.3.1/accurating/tests/model_test.py`

 * *Files identical despite different names*

