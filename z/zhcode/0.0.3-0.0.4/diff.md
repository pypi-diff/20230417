# Comparing `tmp/zhcode-0.0.3.tar.gz` & `tmp/zhcode-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhcode-0.0.3.tar", last modified: Mon Apr 17 01:05:27 2023, max compression
+gzip compressed data, was "zhcode-0.0.4.tar", last modified: Mon Apr 17 16:29:42 2023, max compression
```

## Comparing `zhcode-0.0.3.tar` & `zhcode-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 lnjng      (501) staff       (20)        0 2023-04-17 01:05:27.231299 zhcode-0.0.3/
--rw-r--r--   0 lnjng      (501) staff       (20)     1066 2023-04-16 21:51:24.000000 zhcode-0.0.3/LICENSE
--rw-r--r--   0 lnjng      (501) staff       (20)     1353 2023-04-17 01:05:27.230907 zhcode-0.0.3/PKG-INFO
--rw-r--r--   0 lnjng      (501) staff       (20)     1127 2023-04-16 22:16:34.000000 zhcode-0.0.3/README.md
--rw-r--r--   0 lnjng      (501) staff       (20)       38 2023-04-17 01:05:27.231397 zhcode-0.0.3/setup.cfg
--rw-r--r--   0 lnjng      (501) staff       (20)      484 2023-04-17 01:05:21.000000 zhcode-0.0.3/setup.py
-drwxr-xr-x   0 lnjng      (501) staff       (20)        0 2023-04-17 01:05:27.228134 zhcode-0.0.3/zhcode/
--rw-r--r--   0 lnjng      (501) staff       (20)       50 2023-04-16 23:38:02.000000 zhcode-0.0.3/zhcode/__init__.py
--rw-r--r--   0 lnjng      (501) staff       (20)      896 2023-04-16 21:51:24.000000 zhcode-0.0.3/zhcode/helper.py
--rw-r--r--   0 lnjng      (501) staff       (20)     1524 2023-04-16 23:39:23.000000 zhcode-0.0.3/zhcode/main.py
-drwxr-xr-x   0 lnjng      (501) staff       (20)        0 2023-04-17 01:05:27.230560 zhcode-0.0.3/zhcode/python/
--rw-r--r--   0 lnjng      (501) staff       (20)       24 2023-04-16 23:30:59.000000 zhcode-0.0.3/zhcode/python/__init__.py
--rw-r--r--   0 lnjng      (501) staff       (20)      896 2023-04-16 21:51:24.000000 zhcode-0.0.3/zhcode/python/helper.py
--rw-r--r--   0 lnjng      (501) staff       (20)     3333 2023-04-17 01:02:19.000000 zhcode-0.0.3/zhcode/python/stdlib.py
--rw-r--r--   0 lnjng      (501) staff       (20)     8409 2023-04-16 23:31:32.000000 zhcode-0.0.3/zhcode/python/translate.py
-drwxr-xr-x   0 lnjng      (501) staff       (20)        0 2023-04-17 01:05:27.229357 zhcode-0.0.3/zhcode.egg-info/
--rw-r--r--   0 lnjng      (501) staff       (20)     1353 2023-04-17 01:05:27.000000 zhcode-0.0.3/zhcode.egg-info/PKG-INFO
--rw-r--r--   0 lnjng      (501) staff       (20)      298 2023-04-17 01:05:27.000000 zhcode-0.0.3/zhcode.egg-info/SOURCES.txt
--rw-r--r--   0 lnjng      (501) staff       (20)        1 2023-04-17 01:05:27.000000 zhcode-0.0.3/zhcode.egg-info/dependency_links.txt
--rw-r--r--   0 lnjng      (501) staff       (20)        7 2023-04-17 01:05:27.000000 zhcode-0.0.3/zhcode.egg-info/top_level.txt
+drwxr-xr-x   0 lnjng      (501) staff       (20)        0 2023-04-17 16:29:42.147960 zhcode-0.0.4/
+-rw-r--r--   0 lnjng      (501) staff       (20)     1066 2023-04-16 21:51:24.000000 zhcode-0.0.4/LICENSE
+-rw-r--r--   0 lnjng      (501) staff       (20)     1353 2023-04-17 16:29:42.147389 zhcode-0.0.4/PKG-INFO
+-rw-r--r--   0 lnjng      (501) staff       (20)     1127 2023-04-16 22:16:34.000000 zhcode-0.0.4/README.md
+-rw-r--r--   0 lnjng      (501) staff       (20)       38 2023-04-17 16:29:42.148076 zhcode-0.0.4/setup.cfg
+-rw-r--r--   0 lnjng      (501) staff       (20)      484 2023-04-17 16:29:25.000000 zhcode-0.0.4/setup.py
+drwxr-xr-x   0 lnjng      (501) staff       (20)        0 2023-04-17 16:29:42.144067 zhcode-0.0.4/zhcode/
+-rw-r--r--   0 lnjng      (501) staff       (20)       50 2023-04-16 23:38:02.000000 zhcode-0.0.4/zhcode/__init__.py
+-rw-r--r--   0 lnjng      (501) staff       (20)      896 2023-04-16 21:51:24.000000 zhcode-0.0.4/zhcode/helper.py
+-rw-r--r--   0 lnjng      (501) staff       (20)     1524 2023-04-16 23:39:23.000000 zhcode-0.0.4/zhcode/main.py
+drwxr-xr-x   0 lnjng      (501) staff       (20)        0 2023-04-17 16:29:42.146922 zhcode-0.0.4/zhcode/python/
+-rw-r--r--   0 lnjng      (501) staff       (20)       24 2023-04-16 23:30:59.000000 zhcode-0.0.4/zhcode/python/__init__.py
+-rw-r--r--   0 lnjng      (501) staff       (20)      896 2023-04-16 21:51:24.000000 zhcode-0.0.4/zhcode/python/helper.py
+-rw-r--r--   0 lnjng      (501) staff       (20)     3334 2023-04-17 16:23:19.000000 zhcode-0.0.4/zhcode/python/stdlib.py
+-rw-r--r--   0 lnjng      (501) staff       (20)     8543 2023-04-17 15:29:14.000000 zhcode-0.0.4/zhcode/python/translate.py
+drwxr-xr-x   0 lnjng      (501) staff       (20)        0 2023-04-17 16:29:42.145447 zhcode-0.0.4/zhcode.egg-info/
+-rw-r--r--   0 lnjng      (501) staff       (20)     1353 2023-04-17 16:29:42.000000 zhcode-0.0.4/zhcode.egg-info/PKG-INFO
+-rw-r--r--   0 lnjng      (501) staff       (20)      298 2023-04-17 16:29:42.000000 zhcode-0.0.4/zhcode.egg-info/SOURCES.txt
+-rw-r--r--   0 lnjng      (501) staff       (20)        1 2023-04-17 16:29:42.000000 zhcode-0.0.4/zhcode.egg-info/dependency_links.txt
+-rw-r--r--   0 lnjng      (501) staff       (20)        7 2023-04-17 16:29:42.000000 zhcode-0.0.4/zhcode.egg-info/top_level.txt
```

### Comparing `zhcode-0.0.3/LICENSE` & `zhcode-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `zhcode-0.0.3/PKG-INFO` & `zhcode-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhcode
-Version: 0.0.3
+Version: 0.0.4
 Summary: Programming languages in Chinese.
 Home-page: https://github.com/Injng/zhcode
 Author: lnjng
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `zhcode-0.0.3/README.md` & `zhcode-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `zhcode-0.0.3/zhcode/helper.py` & `zhcode-0.0.4/zhcode/helper.py`

 * *Files identical despite different names*

### Comparing `zhcode-0.0.3/zhcode/main.py` & `zhcode-0.0.4/zhcode/main.py`

 * *Files identical despite different names*

### Comparing `zhcode-0.0.3/zhcode/python/helper.py` & `zhcode-0.0.4/zhcode/python/helper.py`

 * *Files identical despite different names*

### Comparing `zhcode-0.0.3/zhcode/python/stdlib.py` & `zhcode-0.0.4/zhcode/python/stdlib.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         "除" : "except",
         "终" : "finally",
         "从" : "from",
         "是" : "is",
         "姆" : "lambda",
         "外" : "nonlocal",
         "非" : "not",
-        "产" : "yield
+        "产" : "yield"
         }
 
 # names and functions/methods not to exceed four characters
 names = {
         "数学" : "math",
         "系统" : "sys"
```

### Comparing `zhcode-0.0.3/zhcode/python/translate.py` & `zhcode-0.0.4/zhcode/python/translate.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,16 @@
                         py.write('"')
                         sstate = 2
                     elif sstate == 2:  # State to end the ignoring period
                         py.write('"')
                         sstate = 0
                     else:
                         try:
-                            if x[i + 1] == "—" and x[i + 2] == "—" and x[i + 4] == "—" and x[i + 5] == "—":  # Check for __main__
+                            # Check for __main__
+                            if x[i + 1] == "—" and x[i + 2] == "—" and x[i + 4] == "—" and x[i + 5] == "—": 
                                 if x[i + 3] == "主":
                                     py.write('"__main__"')
                                     state = -6
                                 else:
                                     py.write('"')
                                     state = 4
                             else:
@@ -156,14 +157,17 @@
                 elif x[i] == "】":
                     py.write("]")
                 # Check for carats
                 elif x[i] == "《":
                     py.write("<")
                 elif x[i] == "》":
                     py.write(">")
+                # Check for tildes
+                elif x[i] == "～":
+                    py.write('~') 
                 # Check for period punctuation
                 elif x[i] == "。":
                     if bstate == 1:
                         py.write("}")
                         bstate = 0
                     else:
                         py.write("{")
```

### Comparing `zhcode-0.0.3/zhcode.egg-info/PKG-INFO` & `zhcode-0.0.4/zhcode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhcode
-Version: 0.0.3
+Version: 0.0.4
 Summary: Programming languages in Chinese.
 Home-page: https://github.com/Injng/zhcode
 Author: lnjng
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

