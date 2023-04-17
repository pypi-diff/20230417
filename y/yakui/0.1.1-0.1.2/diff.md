# Comparing `tmp/yakui-0.1.1.tar.gz` & `tmp/yakui-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yakui-0.1.1.tar", max compression
+gzip compressed data, was "yakui-0.1.2.tar", max compression
```

## Comparing `yakui-0.1.1.tar` & `yakui-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11357 2023-04-16 18:13:18.837379 yakui-0.1.1/LICENSE
--rw-r--r--   0        0        0      391 2023-04-17 08:17:46.993291 yakui-0.1.1/README.md
--rw-r--r--   0        0        0     1506 2023-04-17 08:19:10.671413 yakui-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      770 2023-04-17 07:35:15.497084 yakui-0.1.1/src/yakui/__init__.py
--rw-r--r--   0        0        0      788 2023-04-17 07:46:03.329705 yakui-0.1.1/src/yakui/_callers.py
--rw-r--r--   0        0        0      625 2023-04-17 07:35:21.752925 yakui-0.1.1/src/yakui/_constants.py
--rw-r--r--   0        0        0     1096 2023-04-17 07:59:39.856898 yakui-0.1.1/src/yakui/_levels.py
--rw-r--r--   0        0        0     5660 2023-04-17 08:17:12.942436 yakui-0.1.1/src/yakui/_loggers.py
--rw-r--r--   0        0        0     1039 2023-04-17 07:37:02.450177 yakui-0.1.1/src/yakui/_timestamps.py
--rw-r--r--   0        0        0      923 2023-04-17 07:56:07.173109 yakui-0.1.1/src/yakui/ansi256/_beautify.py
--rw-r--r--   0        0        0     2616 2023-04-17 08:09:24.178822 yakui-0.1.1/src/yakui/ansi256/_colors.py
--rw-r--r--   0        0        0      671 2023-04-17 07:35:45.944297 yakui-0.1.1/src/yakui/ansi256/_constants.py
--rw-r--r--   0        0        0     1826 2023-04-17 08:08:57.255830 yakui-0.1.1/src/yakui/ansi256/_effects.py
--rw-r--r--   0        0        0      780 2023-04-17 07:35:32.724643 yakui-0.1.1/src/yakui/ansi256/_typehintings.py
--rw-r--r--   0        0        0     1540 2023-04-17 07:36:37.434890 yakui-0.1.1/src/yakui/ansi256/themes/_default.py
--rw-r--r--   0        0        0     2368 2023-04-17 08:09:33.870460 yakui-0.1.1/src/yakui/ansi256/themes/_theme.py
--rw-r--r--   0        0        0      826 1970-01-01 00:00:00.000000 yakui-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-16 18:13:18.837379 yakui-0.1.2/LICENSE
+-rw-r--r--   0        0        0      391 2023-04-17 08:17:46.993291 yakui-0.1.2/README.md
+-rw-r--r--   0        0        0     1506 2023-04-17 08:24:17.017511 yakui-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      770 2023-04-17 07:35:15.497084 yakui-0.1.2/src/yakui/__init__.py
+-rw-r--r--   0        0        0      788 2023-04-17 07:46:03.329705 yakui-0.1.2/src/yakui/_callers.py
+-rw-r--r--   0        0        0      625 2023-04-17 07:35:21.752925 yakui-0.1.2/src/yakui/_constants.py
+-rw-r--r--   0        0        0     1096 2023-04-17 07:59:39.856898 yakui-0.1.2/src/yakui/_levels.py
+-rw-r--r--   0        0        0     5667 2023-04-17 08:22:10.144999 yakui-0.1.2/src/yakui/_loggers.py
+-rw-r--r--   0        0        0     1039 2023-04-17 07:37:02.450177 yakui-0.1.2/src/yakui/_timestamps.py
+-rw-r--r--   0        0        0      923 2023-04-17 07:56:07.173109 yakui-0.1.2/src/yakui/ansi256/_beautify.py
+-rw-r--r--   0        0        0     2616 2023-04-17 08:09:24.178822 yakui-0.1.2/src/yakui/ansi256/_colors.py
+-rw-r--r--   0        0        0      671 2023-04-17 07:35:45.944297 yakui-0.1.2/src/yakui/ansi256/_constants.py
+-rw-r--r--   0        0        0     1826 2023-04-17 08:08:57.255830 yakui-0.1.2/src/yakui/ansi256/_effects.py
+-rw-r--r--   0        0        0      780 2023-04-17 07:35:32.724643 yakui-0.1.2/src/yakui/ansi256/_typehintings.py
+-rw-r--r--   0        0        0     1540 2023-04-17 07:36:37.434890 yakui-0.1.2/src/yakui/ansi256/themes/_default.py
+-rw-r--r--   0        0        0     2368 2023-04-17 08:09:33.870460 yakui-0.1.2/src/yakui/ansi256/themes/_theme.py
+-rw-r--r--   0        0        0      826 1970-01-01 00:00:00.000000 yakui-0.1.2/PKG-INFO
```

### Comparing `yakui-0.1.1/LICENSE` & `yakui-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yakui-0.1.1/pyproject.toml` & `yakui-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yakui"
-version = "0.1.1"
+version = "0.1.2"
 description = "Advanced Logging in Python"
 authors = ["mmlvgx <mmlvgx@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "yakui", from = "src"}]
 
 [tool.ruff]
```

### Comparing `yakui-0.1.1/src/yakui/__init__.py` & `yakui-0.1.2/src/yakui/__init__.py`

 * *Files identical despite different names*

### Comparing `yakui-0.1.1/src/yakui/_callers.py` & `yakui-0.1.2/src/yakui/_callers.py`

 * *Files identical despite different names*

### Comparing `yakui-0.1.1/src/yakui/_constants.py` & `yakui-0.1.2/src/yakui/_constants.py`

 * *Files identical despite different names*

### Comparing `yakui-0.1.1/src/yakui/_levels.py` & `yakui-0.1.2/src/yakui/_levels.py`

 * *Files identical despite different names*

### Comparing `yakui-0.1.1/src/yakui/_loggers.py` & `yakui-0.1.2/src/yakui/_loggers.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,16 +110,16 @@
 
         Parameters:
             `level` (Level): Level of logging
             `message` (str): A message to log
         """
         logger_name = self.__name
 
-        level_name = level.name
-        level_value = level.value
+        level_name = level._name
+        level_value = level._value
         level_text = level_name.upper()
 
         assert level_value in self.__levels
 
         _timestamp = timestamp()
         _caller = caller()
 
@@ -143,15 +143,15 @@
         (
             f"{logger_name}{W * self.__indent}"
             f"[{_timestamp} {level_text}]{W * self.__indent}"
             f"({caller_parent_name}/{caller_name}){W * self.__indent}{message}\n"
         )
         # fmt: on
         if self.__filename is not None:
-            with open(self.__filename) as stream:
+            with open(self.__filename, "w") as stream:
                 stream.write(log)
 
         stdout.write(log)
 
     def info(self, message: str) -> None:
         """
         Confirmation that things are working as expected
```

### Comparing `yakui-0.1.1/src/yakui/_timestamps.py` & `yakui-0.1.2/src/yakui/_timestamps.py`

 * *Files identical despite different names*

### Comparing `yakui-0.1.1/src/yakui/ansi256/_beautify.py` & `yakui-0.1.2/src/yakui/ansi256/_beautify.py`

 * *Files identical despite different names*

### Comparing `yakui-0.1.1/src/yakui/ansi256/_colors.py` & `yakui-0.1.2/src/yakui/ansi256/_colors.py`

 * *Files identical despite different names*

### Comparing `yakui-0.1.1/src/yakui/ansi256/_constants.py` & `yakui-0.1.2/src/yakui/ansi256/_constants.py`

 * *Files identical despite different names*

### Comparing `yakui-0.1.1/src/yakui/ansi256/_effects.py` & `yakui-0.1.2/src/yakui/ansi256/_effects.py`

 * *Files identical despite different names*

### Comparing `yakui-0.1.1/src/yakui/ansi256/_typehintings.py` & `yakui-0.1.2/src/yakui/ansi256/_typehintings.py`

 * *Files identical despite different names*

### Comparing `yakui-0.1.1/src/yakui/ansi256/themes/_default.py` & `yakui-0.1.2/src/yakui/ansi256/themes/_default.py`

 * *Files identical despite different names*

### Comparing `yakui-0.1.1/src/yakui/ansi256/themes/_theme.py` & `yakui-0.1.2/src/yakui/ansi256/themes/_theme.py`

 * *Files identical despite different names*

### Comparing `yakui-0.1.1/PKG-INFO` & `yakui-0.1.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yakui
-Version: 0.1.1
+Version: 0.1.2
 Summary: Advanced Logging in Python
 License: Apache-2.0
 Author: mmlvgx
 Author-email: mmlvgx@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

