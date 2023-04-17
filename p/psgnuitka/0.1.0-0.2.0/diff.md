# Comparing `tmp/psgnuitka-0.1.0.tar.gz` & `tmp/psgnuitka-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psgnuitka-0.1.0.tar", max compression
+gzip compressed data, was "psgnuitka-0.2.0.tar", max compression
```

## Comparing `psgnuitka-0.1.0.tar` & `psgnuitka-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1086 2023-04-12 00:26:22.121472 psgnuitka-0.1.0/LICENSE
--rw-r--r--   0        0        0    13921 2023-04-12 00:49:18.623909 psgnuitka-0.1.0/psgnuitka.py
--rw-r--r--   0        0        0      838 2023-04-12 01:28:59.527136 psgnuitka-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1622 2023-04-12 00:48:22.955769 psgnuitka-0.1.0/README.md
--rw-r--r--   0        0        0     2342 1970-01-01 00:00:00.000000 psgnuitka-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-04-12 00:26:22.121472 psgnuitka-0.2.0/LICENSE
+-rw-r--r--   0        0        0    16453 2023-04-17 02:13:13.643372 psgnuitka-0.2.0/psgnuitka.py
+-rw-r--r--   0        0        0      837 2023-04-17 01:54:36.809754 psgnuitka-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1622 2023-04-12 12:13:22.154596 psgnuitka-0.2.0/README.md
+-rw-r--r--   0        0        0     2342 1970-01-01 00:00:00.000000 psgnuitka-0.2.0/PKG-INFO
```

### Comparing `psgnuitka-0.1.0/LICENSE` & `psgnuitka-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `psgnuitka-0.1.0/pyproject.toml` & `psgnuitka-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "psgnuitka"
-version = "0.1.0"
+version = "0.2.0"
 description = "A graphical tool to facilitate the generation of Python executables using Nuitka"
 authors = ["boulderh <boulderh@163.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/BoulderH/psgnuitka"
 repository = "https://github.com/BoulderH/psgnuitka"
 keywords = ["nuitka","PySimpleGUI","psgnuitka"]
@@ -23,14 +23,14 @@
 url = "https://pypi.tuna.tsinghua.edu.cn/simple/"
 default = true
 secondary = false
 
 
 [tool.poetry.group.dev.dependencies]
 autopep8 = "^2.0.2"
-nuitka = "^1.5.5"
+nuitka = "1.4.*"
 zstandard = "^0.20.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `psgnuitka-0.1.0/README.md` & `psgnuitka-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `psgnuitka-0.1.0/PKG-INFO` & `psgnuitka-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psgnuitka
-Version: 0.1.0
+Version: 0.2.0
 Summary: A graphical tool to facilitate the generation of Python executables using Nuitka
 Home-page: https://github.com/BoulderH/psgnuitka
 License: MIT
 Keywords: nuitka,PySimpleGUI,psgnuitka
 Author: boulderh
 Author-email: boulderh@163.com
 Requires-Python: >=3.8,<4.0
```

