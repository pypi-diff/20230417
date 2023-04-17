# Comparing `tmp/trainyolo-py-0.0.8.tar.gz` & `tmp/trainyolo-py-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trainyolo-py-0.0.8.tar", last modified: Thu Mar  9 01:01:22 2023, max compression
+gzip compressed data, was "trainyolo-py-0.0.9.tar", last modified: Mon Apr 17 13:55:08 2023, max compression
```

## Comparing `trainyolo-py-0.0.8.tar` & `trainyolo-py-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 01:01:22.963663 trainyolo-py-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-03-09 01:01:05.000000 trainyolo-py-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-03-09 01:01:22.963663 trainyolo-py-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-09 01:01:05.000000 trainyolo-py-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-09 01:01:22.963663 trainyolo-py-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-03-09 01:01:05.000000 trainyolo-py-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 01:01:22.963663 trainyolo-py-0.0.8/trainyolo/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-09 01:01:05.000000 trainyolo-py-0.0.8/trainyolo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-03-09 01:01:05.000000 trainyolo-py-0.0.8/trainyolo/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-03-09 01:01:05.000000 trainyolo-py-0.0.8/trainyolo/cli_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-03-09 01:01:05.000000 trainyolo-py-0.0.8/trainyolo/cli_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    18664 2023-03-09 01:01:05.000000 trainyolo-py-0.0.8/trainyolo/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 01:01:22.963663 trainyolo-py-0.0.8/trainyolo/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 01:01:05.000000 trainyolo-py-0.0.8/trainyolo/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-03-09 01:01:05.000000 trainyolo-py-0.0.8/trainyolo/utils/ocr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-03-09 01:01:05.000000 trainyolo-py-0.0.8/trainyolo/utils/yolov5.py
--rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-03-09 01:01:05.000000 trainyolo-py-0.0.8/trainyolo/utils/yolov8.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 01:01:22.963663 trainyolo-py-0.0.8/trainyolo_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-03-09 01:01:22.000000 trainyolo-py-0.0.8/trainyolo_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-03-09 01:01:22.000000 trainyolo-py-0.0.8/trainyolo_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 01:01:22.000000 trainyolo-py-0.0.8/trainyolo_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-09 01:01:22.000000 trainyolo-py-0.0.8/trainyolo_py.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-09 01:01:22.000000 trainyolo-py-0.0.8/trainyolo_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-09 01:01:22.000000 trainyolo-py-0.0.8/trainyolo_py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:55:08.639168 trainyolo-py-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-17 13:54:54.000000 trainyolo-py-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-17 13:55:08.639168 trainyolo-py-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-17 13:54:54.000000 trainyolo-py-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 13:55:08.639168 trainyolo-py-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-17 13:54:54.000000 trainyolo-py-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:55:08.639168 trainyolo-py-0.0.9/trainyolo/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-17 13:54:54.000000 trainyolo-py-0.0.9/trainyolo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-17 13:54:54.000000 trainyolo-py-0.0.9/trainyolo/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-04-17 13:54:54.000000 trainyolo-py-0.0.9/trainyolo/cli_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-04-17 13:54:54.000000 trainyolo-py-0.0.9/trainyolo/cli_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18664 2023-04-17 13:54:54.000000 trainyolo-py-0.0.9/trainyolo/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:55:08.639168 trainyolo-py-0.0.9/trainyolo/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 13:54:54.000000 trainyolo-py-0.0.9/trainyolo/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-17 13:54:54.000000 trainyolo-py-0.0.9/trainyolo/utils/ocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-04-17 13:54:54.000000 trainyolo-py-0.0.9/trainyolo/utils/yolov5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8226 2023-04-17 13:54:54.000000 trainyolo-py-0.0.9/trainyolo/utils/yolov8.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:55:08.639168 trainyolo-py-0.0.9/trainyolo_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-17 13:55:08.000000 trainyolo-py-0.0.9/trainyolo_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-17 13:55:08.000000 trainyolo-py-0.0.9/trainyolo_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 13:55:08.000000 trainyolo-py-0.0.9/trainyolo_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-17 13:55:08.000000 trainyolo-py-0.0.9/trainyolo_py.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-17 13:55:08.000000 trainyolo-py-0.0.9/trainyolo_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-17 13:55:08.000000 trainyolo-py-0.0.9/trainyolo_py.egg-info/top_level.txt
```

### Comparing `trainyolo-py-0.0.8/LICENSE` & `trainyolo-py-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `trainyolo-py-0.0.8/setup.py` & `trainyolo-py-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `trainyolo-py-0.0.8/trainyolo/cli.py` & `trainyolo-py-0.0.9/trainyolo/cli.py`

 * *Files identical despite different names*

### Comparing `trainyolo-py-0.0.8/trainyolo/cli_functions.py` & `trainyolo-py-0.0.9/trainyolo/cli_functions.py`

 * *Files identical despite different names*

### Comparing `trainyolo-py-0.0.8/trainyolo/cli_options.py` & `trainyolo-py-0.0.9/trainyolo/cli_options.py`

 * *Files identical despite different names*

### Comparing `trainyolo-py-0.0.8/trainyolo/client.py` & `trainyolo-py-0.0.9/trainyolo/client.py`

 * *Files identical despite different names*

### Comparing `trainyolo-py-0.0.8/trainyolo/utils/yolov5.py` & `trainyolo-py-0.0.9/trainyolo/utils/yolov5.py`

 * *Files identical despite different names*

