# Comparing `tmp/zhcode-0.0.2.tar.gz` & `tmp/zhcode-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhcode-0.0.2.tar", last modified: Mon Apr 17 00:07:07 2023, max compression
+gzip compressed data, was "zhcode-0.0.3.tar", last modified: Mon Apr 17 01:05:27 2023, max compression
```

## Comparing `zhcode-0.0.2.tar` & `zhcode-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 lnjng      (501) staff       (20)        0 2023-04-17 00:07:07.059444 zhcode-0.0.2/
--rw-r--r--   0 lnjng      (501) staff       (20)     1066 2023-04-16 21:51:24.000000 zhcode-0.0.2/LICENSE
--rw-r--r--   0 lnjng      (501) staff       (20)     1353 2023-04-17 00:07:07.058884 zhcode-0.0.2/PKG-INFO
--rw-r--r--   0 lnjng      (501) staff       (20)     1127 2023-04-16 22:16:34.000000 zhcode-0.0.2/README.md
--rw-r--r--   0 lnjng      (501) staff       (20)       38 2023-04-17 00:07:07.059596 zhcode-0.0.2/setup.cfg
--rw-r--r--   0 lnjng      (501) staff       (20)      484 2023-04-17 00:07:03.000000 zhcode-0.0.2/setup.py
-drwxr-xr-x   0 lnjng      (501) staff       (20)        0 2023-04-17 00:07:07.056017 zhcode-0.0.2/zhcode/
--rw-r--r--   0 lnjng      (501) staff       (20)       50 2023-04-16 23:38:02.000000 zhcode-0.0.2/zhcode/__init__.py
--rw-r--r--   0 lnjng      (501) staff       (20)      896 2023-04-16 21:51:24.000000 zhcode-0.0.2/zhcode/helper.py
--rw-r--r--   0 lnjng      (501) staff       (20)     1524 2023-04-16 23:39:23.000000 zhcode-0.0.2/zhcode/main.py
-drwxr-xr-x   0 lnjng      (501) staff       (20)        0 2023-04-17 00:07:07.058513 zhcode-0.0.2/zhcode/python/
--rw-r--r--   0 lnjng      (501) staff       (20)       24 2023-04-16 23:30:59.000000 zhcode-0.0.2/zhcode/python/__init__.py
--rw-r--r--   0 lnjng      (501) staff       (20)      896 2023-04-16 21:51:24.000000 zhcode-0.0.2/zhcode/python/helper.py
--rw-r--r--   0 lnjng      (501) staff       (20)     3017 2023-04-16 21:51:24.000000 zhcode-0.0.2/zhcode/python/stdlib.py
--rw-r--r--   0 lnjng      (501) staff       (20)     8409 2023-04-16 23:31:32.000000 zhcode-0.0.2/zhcode/python/translate.py
-drwxr-xr-x   0 lnjng      (501) staff       (20)        0 2023-04-17 00:07:07.057335 zhcode-0.0.2/zhcode.egg-info/
--rw-r--r--   0 lnjng      (501) staff       (20)     1353 2023-04-17 00:07:07.000000 zhcode-0.0.2/zhcode.egg-info/PKG-INFO
--rw-r--r--   0 lnjng      (501) staff       (20)      298 2023-04-17 00:07:07.000000 zhcode-0.0.2/zhcode.egg-info/SOURCES.txt
--rw-r--r--   0 lnjng      (501) staff       (20)        1 2023-04-17 00:07:07.000000 zhcode-0.0.2/zhcode.egg-info/dependency_links.txt
--rw-r--r--   0 lnjng      (501) staff       (20)        7 2023-04-17 00:07:07.000000 zhcode-0.0.2/zhcode.egg-info/top_level.txt
+drwxr-xr-x   0 lnjng      (501) staff       (20)        0 2023-04-17 01:05:27.231299 zhcode-0.0.3/
+-rw-r--r--   0 lnjng      (501) staff       (20)     1066 2023-04-16 21:51:24.000000 zhcode-0.0.3/LICENSE
+-rw-r--r--   0 lnjng      (501) staff       (20)     1353 2023-04-17 01:05:27.230907 zhcode-0.0.3/PKG-INFO
+-rw-r--r--   0 lnjng      (501) staff       (20)     1127 2023-04-16 22:16:34.000000 zhcode-0.0.3/README.md
+-rw-r--r--   0 lnjng      (501) staff       (20)       38 2023-04-17 01:05:27.231397 zhcode-0.0.3/setup.cfg
+-rw-r--r--   0 lnjng      (501) staff       (20)      484 2023-04-17 01:05:21.000000 zhcode-0.0.3/setup.py
+drwxr-xr-x   0 lnjng      (501) staff       (20)        0 2023-04-17 01:05:27.228134 zhcode-0.0.3/zhcode/
+-rw-r--r--   0 lnjng      (501) staff       (20)       50 2023-04-16 23:38:02.000000 zhcode-0.0.3/zhcode/__init__.py
+-rw-r--r--   0 lnjng      (501) staff       (20)      896 2023-04-16 21:51:24.000000 zhcode-0.0.3/zhcode/helper.py
+-rw-r--r--   0 lnjng      (501) staff       (20)     1524 2023-04-16 23:39:23.000000 zhcode-0.0.3/zhcode/main.py
+drwxr-xr-x   0 lnjng      (501) staff       (20)        0 2023-04-17 01:05:27.230560 zhcode-0.0.3/zhcode/python/
+-rw-r--r--   0 lnjng      (501) staff       (20)       24 2023-04-16 23:30:59.000000 zhcode-0.0.3/zhcode/python/__init__.py
+-rw-r--r--   0 lnjng      (501) staff       (20)      896 2023-04-16 21:51:24.000000 zhcode-0.0.3/zhcode/python/helper.py
+-rw-r--r--   0 lnjng      (501) staff       (20)     3333 2023-04-17 01:02:19.000000 zhcode-0.0.3/zhcode/python/stdlib.py
+-rw-r--r--   0 lnjng      (501) staff       (20)     8409 2023-04-16 23:31:32.000000 zhcode-0.0.3/zhcode/python/translate.py
+drwxr-xr-x   0 lnjng      (501) staff       (20)        0 2023-04-17 01:05:27.229357 zhcode-0.0.3/zhcode.egg-info/
+-rw-r--r--   0 lnjng      (501) staff       (20)     1353 2023-04-17 01:05:27.000000 zhcode-0.0.3/zhcode.egg-info/PKG-INFO
+-rw-r--r--   0 lnjng      (501) staff       (20)      298 2023-04-17 01:05:27.000000 zhcode-0.0.3/zhcode.egg-info/SOURCES.txt
+-rw-r--r--   0 lnjng      (501) staff       (20)        1 2023-04-17 01:05:27.000000 zhcode-0.0.3/zhcode.egg-info/dependency_links.txt
+-rw-r--r--   0 lnjng      (501) staff       (20)        7 2023-04-17 01:05:27.000000 zhcode-0.0.3/zhcode.egg-info/top_level.txt
```

### Comparing `zhcode-0.0.2/LICENSE` & `zhcode-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `zhcode-0.0.2/PKG-INFO` & `zhcode-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhcode
-Version: 0.0.2
+Version: 0.0.3
 Summary: Programming languages in Chinese.
 Home-page: https://github.com/Injng/zhcode
 Author: lnjng
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `zhcode-0.0.2/README.md` & `zhcode-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `zhcode-0.0.2/zhcode/helper.py` & `zhcode-0.0.3/zhcode/helper.py`

 * *Files identical despite different names*

### Comparing `zhcode-0.0.2/zhcode/main.py` & `zhcode-0.0.3/zhcode/main.py`

 * *Files identical despite different names*

### Comparing `zhcode-0.0.2/zhcode/python/helper.py` & `zhcode-0.0.3/zhcode/python/helper.py`

 * *Files identical despite different names*

### Comparing `zhcode-0.0.2/zhcode/python/stdlib.py` & `zhcode-0.0.3/zhcode/python/stdlib.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,37 +3,47 @@
 
 # keywords not to exceed one character
 keywords = {
         "用" : "import",
         "定" : "def",
         "为" : "for",
         "在" : "in",
-        "是" : "if",
+        "如" : "if",
         "还" : "elif",
         "否" : "else",
         "回" : "return",
         "通" : "pass",
         "断" : "break",
         "或" : "or",
         "与" : "and",
-        "当" : "while",
+        "正" : "while",
         "真" : "True",
         "假" : "False",
         "提" : "raise",
         "试" : "try",
         "以" : "with",
         "配" : "match",
         "说" : "assert",
         "续" : "continue",
         "全" : "global",
         "类" : "class",
-        "自" : "self"
-
-
-
+        "自" : "self",
+        "无" : "None",
+        "当" : "as",
+        "异" : "async",
+        "等" : "await",
+        "删" : "del",
+        "除" : "except",
+        "终" : "finally",
+        "从" : "from",
+        "是" : "is",
+        "姆" : "lambda",
+        "外" : "nonlocal",
+        "非" : "not",
+        "产" : "yield
         }
 
 # names and functions/methods not to exceed four characters
 names = {
         "数学" : "math",
         "系统" : "sys"
```

### Comparing `zhcode-0.0.2/zhcode/python/translate.py` & `zhcode-0.0.3/zhcode/python/translate.py`

 * *Files identical despite different names*

### Comparing `zhcode-0.0.2/zhcode.egg-info/PKG-INFO` & `zhcode-0.0.3/zhcode.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhcode
-Version: 0.0.2
+Version: 0.0.3
 Summary: Programming languages in Chinese.
 Home-page: https://github.com/Injng/zhcode
 Author: lnjng
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

