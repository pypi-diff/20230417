# Comparing `tmp/function_tool-0.0.1.tar.gz` & `tmp/function_tool-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "function_tool-0.0.1.tar", last modified: Mon Apr 17 06:43:09 2023, max compression
+gzip compressed data, was "function_tool-0.0.2.tar", last modified: Mon Apr 17 06:54:07 2023, max compression
```

## Comparing `function_tool-0.0.1.tar` & `function_tool-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxr-xr-x   0 fhss       (501) staff       (20)        0 2023-04-17 06:43:09.595325 function_tool-0.0.1/
--rw-r--r--   0 fhss       (501) staff       (20)     1086 2023-04-17 06:09:13.000000 function_tool-0.0.1/LICENSE
--rw-r--r--   0 fhss       (501) staff       (20)     1220 2023-04-17 06:43:09.595000 function_tool-0.0.1/PKG-INFO
--rw-r--r--   0 fhss       (501) staff       (20)      271 2023-04-17 06:12:41.000000 function_tool-0.0.1/README.md
-drwxr-xr-x   0 fhss       (501) staff       (20)        0 2023-04-17 06:43:09.593578 function_tool-0.0.1/function_tool.egg-info/
--rw-r--r--   0 fhss       (501) staff       (20)     1220 2023-04-17 06:43:09.000000 function_tool-0.0.1/function_tool.egg-info/PKG-INFO
--rw-r--r--   0 fhss       (501) staff       (20)      279 2023-04-17 06:43:09.000000 function_tool-0.0.1/function_tool.egg-info/SOURCES.txt
--rw-r--r--   0 fhss       (501) staff       (20)        1 2023-04-17 06:43:09.000000 function_tool-0.0.1/function_tool.egg-info/dependency_links.txt
--rw-r--r--   0 fhss       (501) staff       (20)       12 2023-04-17 06:43:09.000000 function_tool-0.0.1/function_tool.egg-info/requires.txt
--rw-r--r--   0 fhss       (501) staff       (20)       22 2023-04-17 06:43:09.000000 function_tool-0.0.1/function_tool.egg-info/top_level.txt
-drwxr-xr-x   0 fhss       (501) staff       (20)        0 2023-04-17 06:43:09.594383 function_tool-0.0.1/function_tool_derrick/
--rw-r--r--   0 fhss       (501) staff       (20)     1721 2023-04-17 05:58:22.000000 function_tool-0.0.1/function_tool_derrick/UsualTool.py
--rw-r--r--   0 fhss       (501) staff       (20)      151 2023-04-17 04:54:21.000000 function_tool-0.0.1/function_tool_derrick/__init__.py
--rw-r--r--   0 fhss       (501) staff       (20)       38 2023-04-17 06:43:09.595451 function_tool-0.0.1/setup.cfg
--rw-r--r--   0 fhss       (501) staff       (20)     1366 2023-04-17 06:42:11.000000 function_tool-0.0.1/setup.py
+drwxr-xr-x   0 fhss       (501) staff       (20)        0 2023-04-17 06:54:07.416174 function_tool-0.0.2/
+-rw-r--r--   0 fhss       (501) staff       (20)     1086 2023-04-17 06:09:13.000000 function_tool-0.0.2/LICENSE
+-rw-r--r--   0 fhss       (501) staff       (20)     1220 2023-04-17 06:54:07.415857 function_tool-0.0.2/PKG-INFO
+-rw-r--r--   0 fhss       (501) staff       (20)      271 2023-04-17 06:12:41.000000 function_tool-0.0.2/README.md
+drwxr-xr-x   0 fhss       (501) staff       (20)        0 2023-04-17 06:54:07.414581 function_tool-0.0.2/function_tool.egg-info/
+-rw-r--r--   0 fhss       (501) staff       (20)     1220 2023-04-17 06:54:07.000000 function_tool-0.0.2/function_tool.egg-info/PKG-INFO
+-rw-r--r--   0 fhss       (501) staff       (20)      243 2023-04-17 06:54:07.000000 function_tool-0.0.2/function_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 fhss       (501) staff       (20)        1 2023-04-17 06:54:07.000000 function_tool-0.0.2/function_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 fhss       (501) staff       (20)       22 2023-04-17 06:54:07.000000 function_tool-0.0.2/function_tool.egg-info/top_level.txt
+drwxr-xr-x   0 fhss       (501) staff       (20)        0 2023-04-17 06:54:07.415330 function_tool-0.0.2/function_tool_derrick/
+-rw-r--r--   0 fhss       (501) staff       (20)     1721 2023-04-17 05:58:22.000000 function_tool-0.0.2/function_tool_derrick/UsualTool.py
+-rw-r--r--   0 fhss       (501) staff       (20)      151 2023-04-17 04:54:21.000000 function_tool-0.0.2/function_tool_derrick/__init__.py
+-rw-r--r--   0 fhss       (501) staff       (20)       38 2023-04-17 06:54:07.416324 function_tool-0.0.2/setup.cfg
+-rw-r--r--   0 fhss       (501) staff       (20)     1341 2023-04-17 06:53:38.000000 function_tool-0.0.2/setup.py
```

### Comparing `function_tool-0.0.1/LICENSE` & `function_tool-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `function_tool-0.0.1/PKG-INFO` & `function_tool-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: function_tool
-Version: 0.0.1
+Version: 0.0.2
 Summary: some usual tool with class
 Home-page: https://gitee.com/DerrickChiu/function_tool.git
 Author: DerrickChiu
 Author-email: chiull@foxmail.com
 License: MIT
 Description: ### function_tool工具包
         本工具包对一些常用的功能进行了Python封装，目前主要包含以下功能：
```

### Comparing `function_tool-0.0.1/function_tool.egg-info/PKG-INFO` & `function_tool-0.0.2/function_tool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: function-tool
-Version: 0.0.1
+Version: 0.0.2
 Summary: some usual tool with class
 Home-page: https://gitee.com/DerrickChiu/function_tool.git
 Author: DerrickChiu
 Author-email: chiull@foxmail.com
 License: MIT
 Description: ### function_tool工具包
         本工具包对一些常用的功能进行了Python封装，目前主要包含以下功能：
```

### Comparing `function_tool-0.0.1/function_tool_derrick/UsualTool.py` & `function_tool-0.0.2/function_tool_derrick/UsualTool.py`

 * *Files identical despite different names*

### Comparing `function_tool-0.0.1/setup.py` & `function_tool-0.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,25 +8,25 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="function_tool",
-    version='0.0.1',
+    version='0.0.2',
     author="DerrickChiu",
     author_email="chiull@foxmail.com",
     description="some usual tool with class",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://gitee.com/DerrickChiu/function_tool.git",
     packages=find_packages(),
     install_requires=[
-            "Python>=3.6"
+
         ],
     classifiers=[
         "Topic :: Scientific/Engineering",
         'Topic :: Scientific/Engineering :: GIS',
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
```

