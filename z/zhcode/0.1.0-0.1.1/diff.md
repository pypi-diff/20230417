# Comparing `tmp/zhcode-0.1.0.tar.gz` & `tmp/zhcode-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhcode-0.1.0.tar", last modified: Sun Apr 16 21:53:29 2023, max compression
+gzip compressed data, was "zhcode-0.1.1.tar", last modified: Sun Apr 16 22:22:31 2023, max compression
```

## Comparing `zhcode-0.1.0.tar` & `zhcode-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 lnjng      (501) staff       (20)        0 2023-04-16 21:53:29.714396 zhcode-0.1.0/
--rw-r--r--   0 lnjng      (501) staff       (20)     1066 2023-04-16 21:51:24.000000 zhcode-0.1.0/LICENSE
--rw-r--r--   0 lnjng      (501) staff       (20)      129 2023-04-16 21:53:29.714002 zhcode-0.1.0/PKG-INFO
--rw-r--r--   0 lnjng      (501) staff       (20)     1157 2023-04-16 21:51:24.000000 zhcode-0.1.0/README.md
--rw-r--r--   0 lnjng      (501) staff       (20)       38 2023-04-16 21:53:29.714490 zhcode-0.1.0/setup.cfg
--rw-r--r--   0 lnjng      (501) staff       (20)      204 2023-04-16 21:52:51.000000 zhcode-0.1.0/setup.py
-drwxr-xr-x   0 lnjng      (501) staff       (20)        0 2023-04-16 21:53:29.712449 zhcode-0.1.0/zhcode/
--rw-r--r--   0 lnjng      (501) staff       (20)       13 2023-04-16 21:51:24.000000 zhcode-0.1.0/zhcode/__init__.py
--rw-r--r--   0 lnjng      (501) staff       (20)      896 2023-04-16 21:51:24.000000 zhcode-0.1.0/zhcode/helper.py
--rw-r--r--   0 lnjng      (501) staff       (20)     1503 2023-04-16 21:51:24.000000 zhcode-0.1.0/zhcode/main.py
-drwxr-xr-x   0 lnjng      (501) staff       (20)        0 2023-04-16 21:53:29.713644 zhcode-0.1.0/zhcode.egg-info/
--rw-r--r--   0 lnjng      (501) staff       (20)      129 2023-04-16 21:53:29.000000 zhcode-0.1.0/zhcode.egg-info/PKG-INFO
--rw-r--r--   0 lnjng      (501) staff       (20)      197 2023-04-16 21:53:29.000000 zhcode-0.1.0/zhcode.egg-info/SOURCES.txt
--rw-r--r--   0 lnjng      (501) staff       (20)        1 2023-04-16 21:53:29.000000 zhcode-0.1.0/zhcode.egg-info/dependency_links.txt
--rw-r--r--   0 lnjng      (501) staff       (20)        7 2023-04-16 21:53:29.000000 zhcode-0.1.0/zhcode.egg-info/top_level.txt
+drwxr-xr-x   0 lnjng      (501) staff       (20)        0 2023-04-16 22:22:31.313219 zhcode-0.1.1/
+-rw-r--r--   0 lnjng      (501) staff       (20)     1066 2023-04-16 21:51:24.000000 zhcode-0.1.1/LICENSE
+-rw-r--r--   0 lnjng      (501) staff       (20)      129 2023-04-16 22:22:31.312817 zhcode-0.1.1/PKG-INFO
+-rw-r--r--   0 lnjng      (501) staff       (20)     1127 2023-04-16 22:16:34.000000 zhcode-0.1.1/README.md
+-rw-r--r--   0 lnjng      (501) staff       (20)       38 2023-04-16 22:22:31.313315 zhcode-0.1.1/setup.cfg
+-rw-r--r--   0 lnjng      (501) staff       (20)      204 2023-04-16 22:21:52.000000 zhcode-0.1.1/setup.py
+drwxr-xr-x   0 lnjng      (501) staff       (20)        0 2023-04-16 22:22:31.311237 zhcode-0.1.1/zhcode/
+-rw-r--r--   0 lnjng      (501) staff       (20)       19 2023-04-16 22:21:09.000000 zhcode-0.1.1/zhcode/__init__.py
+-rw-r--r--   0 lnjng      (501) staff       (20)      896 2023-04-16 21:51:24.000000 zhcode-0.1.1/zhcode/helper.py
+-rw-r--r--   0 lnjng      (501) staff       (20)     1503 2023-04-16 21:51:24.000000 zhcode-0.1.1/zhcode/main.py
+drwxr-xr-x   0 lnjng      (501) staff       (20)        0 2023-04-16 22:22:31.312473 zhcode-0.1.1/zhcode.egg-info/
+-rw-r--r--   0 lnjng      (501) staff       (20)      129 2023-04-16 22:22:31.000000 zhcode-0.1.1/zhcode.egg-info/PKG-INFO
+-rw-r--r--   0 lnjng      (501) staff       (20)      197 2023-04-16 22:22:31.000000 zhcode-0.1.1/zhcode.egg-info/SOURCES.txt
+-rw-r--r--   0 lnjng      (501) staff       (20)        1 2023-04-16 22:22:31.000000 zhcode-0.1.1/zhcode.egg-info/dependency_links.txt
+-rw-r--r--   0 lnjng      (501) staff       (20)        7 2023-04-16 22:22:31.000000 zhcode-0.1.1/zhcode.egg-info/top_level.txt
```

### Comparing `zhcode-0.1.0/LICENSE` & `zhcode-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zhcode-0.1.0/README.md` & `zhcode-0.1.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # zhcode
-`zhcode` is a Python library designed to facilitate coding in Chinese. It's main purpose is to advance certain programming languages by transforming them into esoteric forms through the Chinese language.
+`zhcode` is a Python library designed to facilitate coding in Chinese. It's main purpose is to create **esoteric forms of programming languages using the Chinese language**.
 
 You can install `zhcode` by running `pip3 install zhcode` in your environment.
 
 ## Python
 Currently, basic Python 3 functions are supported. The project is still in the process of translating library keywords, names, and functions into Chinese equivalents. In general, the syntax for coding in 
 中文Python is the same as that of normal Python, simply with variables switched. However, several syntactic additions have been made: the dot delimeter `.` in standard Python has been changed to `·`, and 
 variables should be enclosed with `「」` to facilitate easier differentiation.
```

### Comparing `zhcode-0.1.0/zhcode/helper.py` & `zhcode-0.1.1/zhcode/helper.py`

 * *Files identical despite different names*

### Comparing `zhcode-0.1.0/zhcode/main.py` & `zhcode-0.1.1/zhcode/main.py`

 * *Files identical despite different names*

