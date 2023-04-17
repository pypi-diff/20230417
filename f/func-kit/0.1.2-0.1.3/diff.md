# Comparing `tmp/func_kit-0.1.2.tar.gz` & `tmp/func_kit-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "func_kit-0.1.2.tar", max compression
+gzip compressed data, was "func_kit-0.1.3.tar", max compression
```

## Comparing `func_kit-0.1.2.tar` & `func_kit-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0     1067 2023-04-15 12:00:29.180320 func_kit-0.1.2/LICENSE.txt
--rw-r--r--   0        0        0      106 2023-04-15 12:10:01.485691 func_kit-0.1.2/README.md
--rw-r--r--   0        0        0       75 2023-04-15 11:23:57.226908 func_kit-0.1.2/func_kit/__init__.py
--rw-r--r--   0        0        0     2848 2023-04-15 12:43:39.221285 func_kit-0.1.2/func_kit/cache.py
--rw-r--r--   0        0        0     2535 2023-04-15 14:15:46.583166 func_kit-0.1.2/func_kit/log.py
--rw-r--r--   0        0        0      441 2023-04-15 14:15:46.583166 func_kit-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      586 1970-01-01 00:00:00.000000 func_kit-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-17 09:28:53.186709 func_kit-0.1.3/LICENSE.txt
+-rw-r--r--   0        0        0      106 2023-04-17 09:28:53.186709 func_kit-0.1.3/README.md
+-rw-r--r--   0        0        0       75 2023-04-17 09:28:53.186709 func_kit-0.1.3/func_kit/__init__.py
+-rw-r--r--   0        0        0     2848 2023-04-17 09:28:53.186709 func_kit-0.1.3/func_kit/cache.py
+-rw-r--r--   0        0        0      721 2023-04-17 09:28:53.186709 func_kit-0.1.3/func_kit/cron.py
+-rw-r--r--   0        0        0     2801 2023-04-17 09:28:53.186709 func_kit-0.1.3/func_kit/log.py
+-rw-r--r--   0        0        0      462 2023-04-17 09:28:53.186709 func_kit-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      731 1970-01-01 00:00:00.000000 func_kit-0.1.3/setup.py
+-rw-r--r--   0        0        0      628 1970-01-01 00:00:00.000000 func_kit-0.1.3/PKG-INFO
```

### Comparing `func_kit-0.1.2/LICENSE.txt` & `func_kit-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `func_kit-0.1.2/func_kit/cache.py` & `func_kit-0.1.3/func_kit/cache.py`

 * *Files identical despite different names*

### Comparing `func_kit-0.1.2/func_kit/log.py` & `func_kit-0.1.3/func_kit/log.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+import inspect
 import logging
 import time
 from functools import wraps
+from typing import Callable
 
 logging.basicConfig(
     format="%(asctime)s - %(name)s - %(levelname)s - %(message)s", level=logging.INFO
 )
 
 
 def log_decorator(logger=None, log_args=False, log_return=False, log_time=False):
@@ -24,44 +26,51 @@
         >>> add_up(1, 2)
         [add_up] called with args: (1, 2), kwargs: {}
         [add_up] returned 3
         [add_up] took 1.0000 seconds to execute
 
     """
 
-    def decorator(func):
+    def decorator(func: Callable):
         @wraps(func)
         def wrapper(*args, **kwargs):
             if logger is None:
                 # Create logger from the function module.
                 logger_obj = logging.getLogger(func.__module__)
             else:
                 logger_obj = logger
             start_time = time.monotonic()
             try:
+                full_path = (
+                    inspect.getmodule(func.__module__).__name__ + "." + func.__name__
+                )
+            except AttributeError:
+                full_path = func.__name__
+
+            try:
                 # Call the function and get the result.
                 # If the function raises an exception, log it and re-raise.
                 result = func(*args, **kwargs)
             except Exception as exception:
-                logger_obj.error("[%s]: %s", func.__name__, exception)
+                logger_obj.error("[%s]: %s", full_path, exception)
                 raise exception
             end_time = time.monotonic()
             if log_args:
                 # Log the function arguments.
                 logger_obj.info(
-                    "[%s] called with args: %s, kwargs: %s", func.__name__, args, kwargs
+                    "[%s] called with args: %s, kwargs: %s", full_path, args, kwargs
                 )
             if log_return:
                 #  Log the function return value.
-                logger_obj.info("[%s] returned %s", func.__name__, result)
+                logger_obj.info("[%s] returned %s", full_path, result)
             if log_time:
                 # Log the function execution time.
                 logger_obj.info(
                     "[%s] took %.4f seconds to execute",
-                    func.__name__,
+                    full_path,
                     end_time - start_time,
                 )
             return result
 
         return wrapper
 
     return decorator
```

### Comparing `func_kit-0.1.2/PKG-INFO` & `func_kit-0.1.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: func-kit
-Version: 0.1.2
+Version: 0.1.3
 Summary: A set of useful function kits.
 License: MIT
 Author: ranguiquan
 Author-email: ranguiquan@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: croniter (>=1.3.14,<2.0.0)
 Description-Content-Type: text/markdown
 
 <!-- ABOUT THE PROJECT -->
 ## About The Project
 
 This is a package consists of some useful function kits.
```

