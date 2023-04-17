# Comparing `tmp/yakui-0.1.0.tar.gz` & `tmp/yakui-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yakui-0.1.0.tar", max compression
+gzip compressed data, was "yakui-0.1.1.tar", max compression
```

## Comparing `yakui-0.1.0.tar` & `yakui-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11357 2023-04-16 18:13:18.837379 yakui-0.1.0/LICENSE
--rw-r--r--   0        0        0       35 2023-04-16 18:16:52.060289 yakui-0.1.0/README.md
--rw-r--r--   0        0        0     1506 2023-04-16 18:38:40.546743 yakui-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      770 2023-04-17 07:35:15.497084 yakui-0.1.0/src/yakui/__init__.py
--rw-r--r--   0        0        0      788 2023-04-17 07:46:03.329705 yakui-0.1.0/src/yakui/_callers.py
--rw-r--r--   0        0        0      625 2023-04-17 07:35:21.752925 yakui-0.1.0/src/yakui/_constants.py
--rw-r--r--   0        0        0     1096 2023-04-17 07:59:39.856898 yakui-0.1.0/src/yakui/_levels.py
--rw-r--r--   0        0        0     5658 2023-04-17 08:00:25.619148 yakui-0.1.0/src/yakui/_loggers.py
--rw-r--r--   0        0        0     1039 2023-04-17 07:37:02.450177 yakui-0.1.0/src/yakui/_timestamps.py
--rw-r--r--   0        0        0      923 2023-04-17 07:56:07.173109 yakui-0.1.0/src/yakui/ansi256/_beautify.py
--rw-r--r--   0        0        0     2616 2023-04-17 08:09:24.178822 yakui-0.1.0/src/yakui/ansi256/_colors.py
--rw-r--r--   0        0        0      671 2023-04-17 07:35:45.944297 yakui-0.1.0/src/yakui/ansi256/_constants.py
--rw-r--r--   0        0        0     1826 2023-04-17 08:08:57.255830 yakui-0.1.0/src/yakui/ansi256/_effects.py
--rw-r--r--   0        0        0      780 2023-04-17 07:35:32.724643 yakui-0.1.0/src/yakui/ansi256/_typehintings.py
--rw-r--r--   0        0        0     1540 2023-04-17 07:36:37.434890 yakui-0.1.0/src/yakui/ansi256/themes/_default.py
--rw-r--r--   0        0        0     2368 2023-04-17 08:09:33.870460 yakui-0.1.0/src/yakui/ansi256/themes/_theme.py
--rw-r--r--   0        0        0      419 1970-01-01 00:00:00.000000 yakui-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-16 18:13:18.837379 yakui-0.1.1/LICENSE
+-rw-r--r--   0        0        0      391 2023-04-17 08:17:46.993291 yakui-0.1.1/README.md
+-rw-r--r--   0        0        0     1506 2023-04-17 08:19:10.671413 yakui-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      770 2023-04-17 07:35:15.497084 yakui-0.1.1/src/yakui/__init__.py
+-rw-r--r--   0        0        0      788 2023-04-17 07:46:03.329705 yakui-0.1.1/src/yakui/_callers.py
+-rw-r--r--   0        0        0      625 2023-04-17 07:35:21.752925 yakui-0.1.1/src/yakui/_constants.py
+-rw-r--r--   0        0        0     1096 2023-04-17 07:59:39.856898 yakui-0.1.1/src/yakui/_levels.py
+-rw-r--r--   0        0        0     5660 2023-04-17 08:17:12.942436 yakui-0.1.1/src/yakui/_loggers.py
+-rw-r--r--   0        0        0     1039 2023-04-17 07:37:02.450177 yakui-0.1.1/src/yakui/_timestamps.py
+-rw-r--r--   0        0        0      923 2023-04-17 07:56:07.173109 yakui-0.1.1/src/yakui/ansi256/_beautify.py
+-rw-r--r--   0        0        0     2616 2023-04-17 08:09:24.178822 yakui-0.1.1/src/yakui/ansi256/_colors.py
+-rw-r--r--   0        0        0      671 2023-04-17 07:35:45.944297 yakui-0.1.1/src/yakui/ansi256/_constants.py
+-rw-r--r--   0        0        0     1826 2023-04-17 08:08:57.255830 yakui-0.1.1/src/yakui/ansi256/_effects.py
+-rw-r--r--   0        0        0      780 2023-04-17 07:35:32.724643 yakui-0.1.1/src/yakui/ansi256/_typehintings.py
+-rw-r--r--   0        0        0     1540 2023-04-17 07:36:37.434890 yakui-0.1.1/src/yakui/ansi256/themes/_default.py
+-rw-r--r--   0        0        0     2368 2023-04-17 08:09:33.870460 yakui-0.1.1/src/yakui/ansi256/themes/_theme.py
+-rw-r--r--   0        0        0      826 1970-01-01 00:00:00.000000 yakui-0.1.1/PKG-INFO
```

### Comparing `yakui-0.1.0/LICENSE` & `yakui-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yakui-0.1.0/pyproject.toml` & `yakui-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yakui"
-version = "0.1.0"
+version = "0.1.1"
 description = "Advanced Logging in Python"
 authors = ["mmlvgx <mmlvgx@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "yakui", from = "src"}]
 
 [tool.ruff]
@@ -51,13 +51,13 @@
 target-version = "py310"
 
 [tool.ruff.mccabe]
 # Unlike Flake8, default to a complexity level of 10.
 max-complexity = 10
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.10"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `yakui-0.1.0/src/yakui/__init__.py` & `yakui-0.1.1/src/yakui/__init__.py`

 * *Files identical despite different names*

### Comparing `yakui-0.1.0/src/yakui/_callers.py` & `yakui-0.1.1/src/yakui/_callers.py`

 * *Files identical despite different names*

### Comparing `yakui-0.1.0/src/yakui/_constants.py` & `yakui-0.1.1/src/yakui/_constants.py`

 * *Files identical despite different names*

### Comparing `yakui-0.1.0/src/yakui/_levels.py` & `yakui-0.1.1/src/yakui/_levels.py`

 * *Files identical despite different names*

### Comparing `yakui-0.1.0/src/yakui/_loggers.py` & `yakui-0.1.1/src/yakui/_loggers.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
             Levels.INFO,
             Levels.WARN,
             Levels.DEBUG,
             Levels.ERROR,
             Levels.FATAL
         ]
         # fmt: on
-        self.__levels = {level.value: level.name for level in levels}
+        self.__levels = {level._value: level._name for level in levels}
 
     @property
     def name(self) -> str:
         """Name of the logger"""
         return self.__name
 
     @name.setter
```

### Comparing `yakui-0.1.0/src/yakui/_timestamps.py` & `yakui-0.1.1/src/yakui/_timestamps.py`

 * *Files identical despite different names*

### Comparing `yakui-0.1.0/src/yakui/ansi256/_beautify.py` & `yakui-0.1.1/src/yakui/ansi256/_beautify.py`

 * *Files identical despite different names*

### Comparing `yakui-0.1.0/src/yakui/ansi256/_colors.py` & `yakui-0.1.1/src/yakui/ansi256/_colors.py`

 * *Files identical despite different names*

### Comparing `yakui-0.1.0/src/yakui/ansi256/_constants.py` & `yakui-0.1.1/src/yakui/ansi256/_constants.py`

 * *Files identical despite different names*

### Comparing `yakui-0.1.0/src/yakui/ansi256/_effects.py` & `yakui-0.1.1/src/yakui/ansi256/_effects.py`

 * *Files identical despite different names*

### Comparing `yakui-0.1.0/src/yakui/ansi256/_typehintings.py` & `yakui-0.1.1/src/yakui/ansi256/_typehintings.py`

 * *Files identical despite different names*

### Comparing `yakui-0.1.0/src/yakui/ansi256/themes/_default.py` & `yakui-0.1.1/src/yakui/ansi256/themes/_default.py`

 * *Files identical despite different names*

### Comparing `yakui-0.1.0/src/yakui/ansi256/themes/_theme.py` & `yakui-0.1.1/src/yakui/ansi256/themes/_theme.py`

 * *Files identical despite different names*

