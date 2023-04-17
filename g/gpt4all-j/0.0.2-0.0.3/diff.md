# Comparing `tmp/gpt4all-j-0.0.2.tar.gz` & `tmp/gpt4all-j-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt4all-j-0.0.2.tar", last modified: Mon Apr 17 19:47:29 2023, max compression
+gzip compressed data, was "gpt4all-j-0.0.3.tar", last modified: Mon Apr 17 20:19:53 2023, max compression
```

## Comparing `gpt4all-j-0.0.2.tar` & `gpt4all-j-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,20 @@
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-04-17 19:47:29.092445 gpt4all-j-0.0.2/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2102 2023-04-17 19:47:29.092445 gpt4all-j-0.0.2/PKG-INFO
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1095 2023-04-17 19:11:04.000000 gpt4all-j-0.0.2/README.md
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-04-17 19:47:29.092445 gpt4all-j-0.0.2/gpt4all_j.egg-info/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2102 2023-04-17 19:47:28.000000 gpt4all-j-0.0.2/gpt4all_j.egg-info/PKG-INFO
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      237 2023-04-17 19:47:29.000000 gpt4all-j-0.0.2/gpt4all_j.egg-info/SOURCES.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-04-17 19:47:28.000000 gpt4all-j-0.0.2/gpt4all_j.egg-info/dependency_links.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-04-17 19:47:28.000000 gpt4all-j-0.0.2/gpt4all_j.egg-info/not-zip-safe
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        9 2023-04-17 19:47:28.000000 gpt4all-j-0.0.2/gpt4all_j.egg-info/top_level.txt
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-04-17 19:47:29.092445 gpt4all-j-0.0.2/gpt4allj/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       55 2023-04-17 19:06:48.000000 gpt4all-j-0.0.2/gpt4allj/__init__.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1372 2023-04-17 19:15:23.000000 gpt4all-j-0.0.2/gpt4allj/lib.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1338 2023-04-17 19:12:58.000000 gpt4all-j-0.0.2/gpt4allj/model.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       38 2023-04-17 19:47:29.092445 gpt4all-j-0.0.2/setup.cfg
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      888 2023-04-17 19:47:19.000000 gpt4all-j-0.0.2/setup.py
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-04-17 20:19:53.132448 gpt4all-j-0.0.3/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2102 2023-04-17 20:19:53.132448 gpt4all-j-0.0.3/PKG-INFO
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1095 2023-04-17 19:11:04.000000 gpt4all-j-0.0.3/README.md
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-04-17 20:19:53.132448 gpt4all-j-0.0.3/gpt4all_j.egg-info/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2102 2023-04-17 20:19:53.000000 gpt4all-j-0.0.3/gpt4all_j.egg-info/PKG-INFO
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      329 2023-04-17 20:19:53.000000 gpt4all-j-0.0.3/gpt4all_j.egg-info/SOURCES.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-04-17 20:19:53.000000 gpt4all-j-0.0.3/gpt4all_j.egg-info/dependency_links.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-04-17 20:19:53.000000 gpt4all-j-0.0.3/gpt4all_j.egg-info/not-zip-safe
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        9 2023-04-17 20:19:53.000000 gpt4all-j-0.0.3/gpt4all_j.egg-info/top_level.txt
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-04-17 20:19:53.132448 gpt4all-j-0.0.3/gpt4allj/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       55 2023-04-17 19:06:48.000000 gpt4all-j-0.0.3/gpt4allj/__init__.py
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-04-17 20:19:53.132448 gpt4all-j-0.0.3/gpt4allj/lib/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)   304128 2023-04-17 17:56:24.000000 gpt4all-j-0.0.3/gpt4allj/lib/ggml.dll
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)   896000 2023-04-17 17:56:27.000000 gpt4all-j-0.0.3/gpt4allj/lib/gptj.dll
+-rwxr-xr-x   0 ravindra  (1000) ravindra  (1000)   169848 2023-04-17 17:54:20.000000 gpt4all-j-0.0.3/gpt4allj/lib/libggml.so
+-rwxr-xr-x   0 ravindra  (1000) ravindra  (1000)   268536 2023-04-17 17:53:22.000000 gpt4all-j-0.0.3/gpt4allj/lib/libgptj.so
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1372 2023-04-17 19:15:23.000000 gpt4all-j-0.0.3/gpt4allj/lib.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1338 2023-04-17 19:12:58.000000 gpt4all-j-0.0.3/gpt4allj/model.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       38 2023-04-17 20:19:53.132448 gpt4all-j-0.0.3/setup.cfg
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      894 2023-04-17 20:18:39.000000 gpt4all-j-0.0.3/setup.py
```

### Comparing `gpt4all-j-0.0.2/PKG-INFO` & `gpt4all-j-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt4all-j
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python bindings for the C++ port of GPT4All-J model.
 Home-page: UNKNOWN
 License: MIT
 Description: [GPT4All-J](https://github.com/marella/gpt4all-j)
         
         Python bindings for the [C++ port][gptj.cpp] of GPT4All-J model.
```

### Comparing `gpt4all-j-0.0.2/README.md` & `gpt4all-j-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `gpt4all-j-0.0.2/gpt4all_j.egg-info/PKG-INFO` & `gpt4all-j-0.0.3/gpt4all_j.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt4all-j
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python bindings for the C++ port of GPT4All-J model.
 Home-page: UNKNOWN
 License: MIT
 Description: [GPT4All-J](https://github.com/marella/gpt4all-j)
         
         Python bindings for the [C++ port][gptj.cpp] of GPT4All-J model.
```

### Comparing `gpt4all-j-0.0.2/gpt4allj/lib.py` & `gpt4all-j-0.0.3/gpt4allj/lib.py`

 * *Files identical despite different names*

### Comparing `gpt4all-j-0.0.2/gpt4allj/model.py` & `gpt4all-j-0.0.3/gpt4allj/model.py`

 * *Files identical despite different names*

### Comparing `gpt4all-j-0.0.2/setup.py` & `gpt4all-j-0.0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 with open('README.md') as f:
     long_description = f.read()
 
 name = 'gpt4all-j'
 
 setup(
     name=name,
-    version='0.0.2',
+    version='0.0.3',
     description='Python bindings for the C++ port of GPT4All-J model.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='MIT',
     packages=find_packages(),
-    package_data={name: ['**/*.so', '**/*.dll']},
+    package_data={'gpt4allj': ['**/*.so', '**/*.dll']},
     install_requires=[],
     zip_safe=False,
     classifiers=[
         'Development Status :: 1 - Planning',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
```

