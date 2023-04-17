# Comparing `tmp/python_contest_template-0.0.1.tar.gz` & `tmp/python_contest_template-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_contest_template-0.0.1.tar", last modified: Mon Apr 10 07:08:24 2023, max compression
+gzip compressed data, was "python_contest_template-0.0.2.tar", last modified: Mon Apr 17 07:25:04 2023, max compression
```

## Comparing `python_contest_template-0.0.1.tar` & `python_contest_template-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,21 @@
-drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2023-04-10 07:08:24.808168 python_contest_template-0.0.1/
--rw-rw-r--   0 zty       (1000) zty       (1000)    11357 2023-04-10 07:05:07.000000 python_contest_template-0.0.1/LICENSE
--rw-rw-r--   0 zty       (1000) zty       (1000)      669 2023-04-10 07:08:24.808168 python_contest_template-0.0.1/PKG-INFO
--rw-rw-r--   0 zty       (1000) zty       (1000)      108 2023-04-10 06:51:34.000000 python_contest_template-0.0.1/README.md
--rw-rw-r--   0 zty       (1000) zty       (1000)      634 2023-04-10 07:05:57.000000 python_contest_template-0.0.1/pyproject.toml
--rw-rw-r--   0 zty       (1000) zty       (1000)       38 2023-04-10 07:08:24.808168 python_contest_template-0.0.1/setup.cfg
-drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2023-04-10 07:08:24.804168 python_contest_template-0.0.1/src/
-drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2023-04-10 07:08:24.808168 python_contest_template-0.0.1/src/python_contest_template/
--rw-rw-r--   0 zty       (1000) zty       (1000)        0 2023-04-10 06:53:27.000000 python_contest_template-0.0.1/src/python_contest_template/__init__.py
--rw-rw-r--   0 zty       (1000) zty       (1000)     1141 2022-10-30 07:19:15.000000 python_contest_template-0.0.1/src/python_contest_template/binary_tree.py
--rw-rw-r--   0 zty       (1000) zty       (1000)      587 2022-10-13 06:09:27.000000 python_contest_template-0.0.1/src/python_contest_template/single_linked_list.py
-drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2023-04-10 07:08:24.808168 python_contest_template-0.0.1/src/python_contest_template.egg-info/
--rw-rw-r--   0 zty       (1000) zty       (1000)      669 2023-04-10 07:08:24.000000 python_contest_template-0.0.1/src/python_contest_template.egg-info/PKG-INFO
--rw-rw-r--   0 zty       (1000) zty       (1000)      369 2023-04-10 07:08:24.000000 python_contest_template-0.0.1/src/python_contest_template.egg-info/SOURCES.txt
--rw-rw-r--   0 zty       (1000) zty       (1000)        1 2023-04-10 07:08:24.000000 python_contest_template-0.0.1/src/python_contest_template.egg-info/dependency_links.txt
--rw-rw-r--   0 zty       (1000) zty       (1000)       24 2023-04-10 07:08:24.000000 python_contest_template-0.0.1/src/python_contest_template.egg-info/top_level.txt
+drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2023-04-17 07:25:04.484866 python_contest_template-0.0.2/
+-rw-rw-r--   0 zty       (1000) zty       (1000)    11357 2023-04-10 07:05:07.000000 python_contest_template-0.0.2/LICENSE
+-rw-rw-r--   0 zty       (1000) zty       (1000)      669 2023-04-17 07:25:04.484866 python_contest_template-0.0.2/PKG-INFO
+-rw-rw-r--   0 zty       (1000) zty       (1000)      108 2023-04-10 06:51:34.000000 python_contest_template-0.0.2/README.md
+-rw-rw-r--   0 zty       (1000) zty       (1000)      634 2023-04-17 07:24:45.000000 python_contest_template-0.0.2/pyproject.toml
+-rw-rw-r--   0 zty       (1000) zty       (1000)       38 2023-04-17 07:25:04.484866 python_contest_template-0.0.2/setup.cfg
+drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2023-04-17 07:25:04.480866 python_contest_template-0.0.2/src/
+drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2023-04-17 07:25:04.480866 python_contest_template-0.0.2/src/python_contest_template/
+-rw-rw-r--   0 zty       (1000) zty       (1000)        0 2023-04-10 06:53:27.000000 python_contest_template-0.0.2/src/python_contest_template/__init__.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)     1141 2022-10-30 07:19:15.000000 python_contest_template-0.0.2/src/python_contest_template/binary_tree.py
+drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2023-04-17 07:25:04.484866 python_contest_template-0.0.2/src/python_contest_template/graph/
+-rw-rw-r--   0 zty       (1000) zty       (1000)        0 2023-04-17 07:05:43.000000 python_contest_template-0.0.2/src/python_contest_template/graph/__init__.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)     2911 2023-04-17 06:59:40.000000 python_contest_template-0.0.2/src/python_contest_template/graph/smallest_routes.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)      587 2022-10-13 06:09:27.000000 python_contest_template-0.0.2/src/python_contest_template/single_linked_list.py
+drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2023-04-17 07:25:04.480866 python_contest_template-0.0.2/src/python_contest_template.egg-info/
+-rw-rw-r--   0 zty       (1000) zty       (1000)      669 2023-04-17 07:25:04.000000 python_contest_template-0.0.2/src/python_contest_template.egg-info/PKG-INFO
+-rw-rw-r--   0 zty       (1000) zty       (1000)      498 2023-04-17 07:25:04.000000 python_contest_template-0.0.2/src/python_contest_template.egg-info/SOURCES.txt
+-rw-rw-r--   0 zty       (1000) zty       (1000)        1 2023-04-17 07:25:04.000000 python_contest_template-0.0.2/src/python_contest_template.egg-info/dependency_links.txt
+-rw-rw-r--   0 zty       (1000) zty       (1000)       24 2023-04-17 07:25:04.000000 python_contest_template-0.0.2/src/python_contest_template.egg-info/top_level.txt
+drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2023-04-17 07:25:04.484866 python_contest_template-0.0.2/tests/
+-rw-rw-r--   0 zty       (1000) zty       (1000)      301 2023-04-17 07:20:24.000000 python_contest_template-0.0.2/tests/test_smallest_routes.py
```

### Comparing `python_contest_template-0.0.1/LICENSE` & `python_contest_template-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python_contest_template-0.0.1/PKG-INFO` & `python_contest_template-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python_contest_template
-Version: 0.0.1
+Version: 0.0.2
 Summary: python template for contest
 Author-email: Grapymage <zhangty21@mails.jlu.edu.cn>
 Project-URL: Homepage, https://github.com/zhangtingyu11/python_contest_template
 Project-URL: Bug Tracker, https://github.com/zhangtingyu11/python_contest_template/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `python_contest_template-0.0.1/pyproject.toml` & `python_contest_template-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "python_contest_template"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Grapymage", email="zhangty21@mails.jlu.edu.cn" },
 ]
 description = "python template for contest"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `python_contest_template-0.0.1/src/python_contest_template/binary_tree.py` & `python_contest_template-0.0.2/src/python_contest_template/binary_tree.py`

 * *Files identical despite different names*

### Comparing `python_contest_template-0.0.1/src/python_contest_template/single_linked_list.py` & `python_contest_template-0.0.2/src/python_contest_template/single_linked_list.py`

 * *Files identical despite different names*

### Comparing `python_contest_template-0.0.1/src/python_contest_template.egg-info/PKG-INFO` & `python_contest_template-0.0.2/src/python_contest_template.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-contest-template
-Version: 0.0.1
+Version: 0.0.2
 Summary: python template for contest
 Author-email: Grapymage <zhangty21@mails.jlu.edu.cn>
 Project-URL: Homepage, https://github.com/zhangtingyu11/python_contest_template
 Project-URL: Bug Tracker, https://github.com/zhangtingyu11/python_contest_template/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

