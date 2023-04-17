# Comparing `tmp/python_contest_template-0.0.2.tar.gz` & `tmp/python_contest_template-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_contest_template-0.0.2.tar", last modified: Mon Apr 17 07:25:04 2023, max compression
+gzip compressed data, was "python_contest_template-0.0.3.tar", last modified: Mon Apr 17 07:45:11 2023, max compression
```

## Comparing `python_contest_template-0.0.2.tar` & `python_contest_template-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2023-04-17 07:25:04.484866 python_contest_template-0.0.2/
--rw-rw-r--   0 zty       (1000) zty       (1000)    11357 2023-04-10 07:05:07.000000 python_contest_template-0.0.2/LICENSE
--rw-rw-r--   0 zty       (1000) zty       (1000)      669 2023-04-17 07:25:04.484866 python_contest_template-0.0.2/PKG-INFO
--rw-rw-r--   0 zty       (1000) zty       (1000)      108 2023-04-10 06:51:34.000000 python_contest_template-0.0.2/README.md
--rw-rw-r--   0 zty       (1000) zty       (1000)      634 2023-04-17 07:24:45.000000 python_contest_template-0.0.2/pyproject.toml
--rw-rw-r--   0 zty       (1000) zty       (1000)       38 2023-04-17 07:25:04.484866 python_contest_template-0.0.2/setup.cfg
-drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2023-04-17 07:25:04.480866 python_contest_template-0.0.2/src/
-drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2023-04-17 07:25:04.480866 python_contest_template-0.0.2/src/python_contest_template/
--rw-rw-r--   0 zty       (1000) zty       (1000)        0 2023-04-10 06:53:27.000000 python_contest_template-0.0.2/src/python_contest_template/__init__.py
--rw-rw-r--   0 zty       (1000) zty       (1000)     1141 2022-10-30 07:19:15.000000 python_contest_template-0.0.2/src/python_contest_template/binary_tree.py
-drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2023-04-17 07:25:04.484866 python_contest_template-0.0.2/src/python_contest_template/graph/
--rw-rw-r--   0 zty       (1000) zty       (1000)        0 2023-04-17 07:05:43.000000 python_contest_template-0.0.2/src/python_contest_template/graph/__init__.py
--rw-rw-r--   0 zty       (1000) zty       (1000)     2911 2023-04-17 06:59:40.000000 python_contest_template-0.0.2/src/python_contest_template/graph/smallest_routes.py
--rw-rw-r--   0 zty       (1000) zty       (1000)      587 2022-10-13 06:09:27.000000 python_contest_template-0.0.2/src/python_contest_template/single_linked_list.py
-drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2023-04-17 07:25:04.480866 python_contest_template-0.0.2/src/python_contest_template.egg-info/
--rw-rw-r--   0 zty       (1000) zty       (1000)      669 2023-04-17 07:25:04.000000 python_contest_template-0.0.2/src/python_contest_template.egg-info/PKG-INFO
--rw-rw-r--   0 zty       (1000) zty       (1000)      498 2023-04-17 07:25:04.000000 python_contest_template-0.0.2/src/python_contest_template.egg-info/SOURCES.txt
--rw-rw-r--   0 zty       (1000) zty       (1000)        1 2023-04-17 07:25:04.000000 python_contest_template-0.0.2/src/python_contest_template.egg-info/dependency_links.txt
--rw-rw-r--   0 zty       (1000) zty       (1000)       24 2023-04-17 07:25:04.000000 python_contest_template-0.0.2/src/python_contest_template.egg-info/top_level.txt
-drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2023-04-17 07:25:04.484866 python_contest_template-0.0.2/tests/
--rw-rw-r--   0 zty       (1000) zty       (1000)      301 2023-04-17 07:20:24.000000 python_contest_template-0.0.2/tests/test_smallest_routes.py
+drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2023-04-17 07:45:11.123470 python_contest_template-0.0.3/
+-rw-rw-r--   0 zty       (1000) zty       (1000)    11357 2023-04-10 07:05:07.000000 python_contest_template-0.0.3/LICENSE
+-rw-rw-r--   0 zty       (1000) zty       (1000)      669 2023-04-17 07:45:11.123470 python_contest_template-0.0.3/PKG-INFO
+-rw-rw-r--   0 zty       (1000) zty       (1000)      108 2023-04-10 06:51:34.000000 python_contest_template-0.0.3/README.md
+-rw-rw-r--   0 zty       (1000) zty       (1000)      634 2023-04-17 07:42:12.000000 python_contest_template-0.0.3/pyproject.toml
+-rw-rw-r--   0 zty       (1000) zty       (1000)       38 2023-04-17 07:45:11.123470 python_contest_template-0.0.3/setup.cfg
+drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2023-04-17 07:45:11.119470 python_contest_template-0.0.3/src/
+drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2023-04-17 07:45:11.123470 python_contest_template-0.0.3/src/graph/
+-rw-rw-r--   0 zty       (1000) zty       (1000)        0 2023-04-17 07:05:43.000000 python_contest_template-0.0.3/src/graph/__init__.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)     2911 2023-04-17 07:32:26.000000 python_contest_template-0.0.3/src/graph/smallest_routes.py
+drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2023-04-17 07:45:11.123470 python_contest_template-0.0.3/src/python_contest_template/
+-rw-rw-r--   0 zty       (1000) zty       (1000)        0 2023-04-10 06:53:27.000000 python_contest_template-0.0.3/src/python_contest_template/__init__.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)     1141 2022-10-30 07:19:15.000000 python_contest_template-0.0.3/src/python_contest_template/binary_tree.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)      587 2022-10-13 06:09:27.000000 python_contest_template-0.0.3/src/python_contest_template/single_linked_list.py
+drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2023-04-17 07:45:11.123470 python_contest_template-0.0.3/src/python_contest_template.egg-info/
+-rw-rw-r--   0 zty       (1000) zty       (1000)      669 2023-04-17 07:45:11.000000 python_contest_template-0.0.3/src/python_contest_template.egg-info/PKG-INFO
+-rw-rw-r--   0 zty       (1000) zty       (1000)      450 2023-04-17 07:45:11.000000 python_contest_template-0.0.3/src/python_contest_template.egg-info/SOURCES.txt
+-rw-rw-r--   0 zty       (1000) zty       (1000)        1 2023-04-17 07:45:11.000000 python_contest_template-0.0.3/src/python_contest_template.egg-info/dependency_links.txt
+-rw-rw-r--   0 zty       (1000) zty       (1000)       30 2023-04-17 07:45:11.000000 python_contest_template-0.0.3/src/python_contest_template.egg-info/top_level.txt
+drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2023-04-17 07:45:11.123470 python_contest_template-0.0.3/tests/
+-rw-rw-r--   0 zty       (1000) zty       (1000)      296 2023-04-17 07:42:05.000000 python_contest_template-0.0.3/tests/test_smallest_routes.py
```

### Comparing `python_contest_template-0.0.2/LICENSE` & `python_contest_template-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python_contest_template-0.0.2/PKG-INFO` & `python_contest_template-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python_contest_template
-Version: 0.0.2
+Version: 0.0.3
 Summary: python template for contest
 Author-email: Grapymage <zhangty21@mails.jlu.edu.cn>
 Project-URL: Homepage, https://github.com/zhangtingyu11/python_contest_template
 Project-URL: Bug Tracker, https://github.com/zhangtingyu11/python_contest_template/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `python_contest_template-0.0.2/pyproject.toml` & `python_contest_template-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "python_contest_template"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Grapymage", email="zhangty21@mails.jlu.edu.cn" },
 ]
 description = "python template for contest"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `python_contest_template-0.0.2/src/python_contest_template/binary_tree.py` & `python_contest_template-0.0.3/src/python_contest_template/binary_tree.py`

 * *Files identical despite different names*

### Comparing `python_contest_template-0.0.2/src/python_contest_template/graph/smallest_routes.py` & `python_contest_template-0.0.3/src/graph/smallest_routes.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     n = len(g)
     dis = [inf] * n
     dis[start] = 0
     vis = [False]*n #* 标记已经被更新成最短路的点
     for i in range(n):
         x = -1
         for j in range(n):
-            if(not vis[i] and (x<0 or dis[i] < dis[x])):   #* 如果没有被标记过且当前的最短路, 那么就用x来更新其他点
+            if(not vis[i] and (x<0 or dis[j] < dis[x])):   #* 如果没有被标记过且当前的最短路, 那么就用x来更新其他点
                 x = j
         vis[x] = True
         for y, w in g[x]:
             if(dis[y] > dis[x] + w):
                 dis[y] = dis[x] + w
     return dis
```

### Comparing `python_contest_template-0.0.2/src/python_contest_template/single_linked_list.py` & `python_contest_template-0.0.3/src/python_contest_template/single_linked_list.py`

 * *Files identical despite different names*

### Comparing `python_contest_template-0.0.2/src/python_contest_template.egg-info/PKG-INFO` & `python_contest_template-0.0.3/src/python_contest_template.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-contest-template
-Version: 0.0.2
+Version: 0.0.3
 Summary: python template for contest
 Author-email: Grapymage <zhangty21@mails.jlu.edu.cn>
 Project-URL: Homepage, https://github.com/zhangtingyu11/python_contest_template
 Project-URL: Bug Tracker, https://github.com/zhangtingyu11/python_contest_template/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

