# Comparing `tmp/lctutil-0.4.0.tar.gz` & `tmp/lctutil-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lctutil-0.4.0.tar", last modified: Sun Apr 16 12:33:25 2023, max compression
+gzip compressed data, was "lctutil-0.5.0.tar", last modified: Mon Apr 17 06:02:10 2023, max compression
```

## Comparing `lctutil-0.4.0.tar` & `lctutil-0.5.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 12:33:25.558132 lctutil-0.4.0/
--rw-rw-rw-   0        0        0      328 2023-04-16 12:33:25.558132 lctutil-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0      387 2023-04-16 12:32:34.000000 lctutil-0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-16 12:33:25.553131 lctutil-0.4.0/lctutil/
--rw-rw-rw-   0        0        0        0 2023-04-16 06:06:37.000000 lctutil-0.4.0/lctutil/__init__.py
--rw-rw-rw-   0        0        0     3321 2023-04-16 07:45:57.000000 lctutil-0.4.0/lctutil/ac_matcher.py
--rw-rw-rw-   0        0        0     5766 2023-04-15 13:05:08.000000 lctutil-0.4.0/lctutil/extract_base_info.py
--rw-rw-rw-   0        0        0     1502 2023-04-16 09:10:14.000000 lctutil-0.4.0/lctutil/openai.py
--rw-rw-rw-   0        0        0     1147 2023-04-15 06:04:07.000000 lctutil-0.4.0/lctutil/stock_infos.py
-drwxrwxrwx   0        0        0        0 2023-04-16 12:33:25.557132 lctutil-0.4.0/lctutil.egg-info/
--rw-rw-rw-   0        0        0      328 2023-04-16 12:33:25.000000 lctutil-0.4.0/lctutil.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2023-04-16 12:33:25.000000 lctutil-0.4.0/lctutil.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 12:33:25.000000 lctutil-0.4.0/lctutil.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-04-16 12:33:25.000000 lctutil-0.4.0/lctutil.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-16 12:33:25.000000 lctutil-0.4.0/lctutil.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 12:33:25.559132 lctutil-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0      592 2023-04-16 12:32:53.000000 lctutil-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 06:02:10.372366 lctutil-0.5.0/
+-rw-rw-rw-   0        0        0      328 2023-04-17 06:02:10.371365 lctutil-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0      387 2023-04-16 12:32:34.000000 lctutil-0.5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 06:02:10.366364 lctutil-0.5.0/lctutil/
+-rw-rw-rw-   0        0        0        0 2023-04-16 06:06:37.000000 lctutil-0.5.0/lctutil/__init__.py
+-rw-rw-rw-   0        0        0     3321 2023-04-16 07:45:57.000000 lctutil-0.5.0/lctutil/ac_matcher.py
+-rw-rw-rw-   0        0        0     5766 2023-04-15 13:05:08.000000 lctutil-0.5.0/lctutil/extract_base_info.py
+-rw-rw-rw-   0        0        0     1526 2023-04-17 06:01:22.000000 lctutil-0.5.0/lctutil/openai.py
+-rw-rw-rw-   0        0        0     1147 2023-04-15 06:04:07.000000 lctutil-0.5.0/lctutil/stock_infos.py
+drwxrwxrwx   0        0        0        0 2023-04-17 06:02:10.370365 lctutil-0.5.0/lctutil.egg-info/
+-rw-rw-rw-   0        0        0      328 2023-04-17 06:02:10.000000 lctutil-0.5.0/lctutil.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2023-04-17 06:02:10.000000 lctutil-0.5.0/lctutil.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 06:02:10.000000 lctutil-0.5.0/lctutil.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-04-17 06:02:10.000000 lctutil-0.5.0/lctutil.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-17 06:02:10.000000 lctutil-0.5.0/lctutil.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 06:02:10.372366 lctutil-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      592 2023-04-17 06:01:22.000000 lctutil-0.5.0/setup.py
```

### Comparing `lctutil-0.4.0/lctutil/ac_matcher.py` & `lctutil-0.5.0/lctutil/ac_matcher.py`

 * *Files identical despite different names*

### Comparing `lctutil-0.4.0/lctutil/extract_base_info.py` & `lctutil-0.5.0/lctutil/extract_base_info.py`

 * *Files identical despite different names*

### Comparing `lctutil-0.4.0/lctutil/openai.py` & `lctutil-0.5.0/lctutil/openai.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 apikeys = _apikeystr.split(";")
 api_k_index = 0
 openai.api_key = apikeys[api_k_index]
 api_k_num = len(apikeys)
 
 def set_api_key_inturn():
     if api_k_num < 2: return
+    global api_k_index
     api_k_index = api_k_index % api_k_num
     openai.api_key = apikeys[api_k_index] 
     api_k_index = api_k_index + 1
 
 
 @retry(wait=wait_random_exponential(min=9, max=20), stop=stop_after_attempt(3))
 def get_embeddings(texts: List[str]) -> List[List[float]]:
```

### Comparing `lctutil-0.4.0/lctutil/stock_infos.py` & `lctutil-0.5.0/lctutil/stock_infos.py`

 * *Files identical despite different names*

### Comparing `lctutil-0.4.0/setup.py` & `lctutil-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='lctutil',
-    version='0.4.0',
+    version='0.5.0',
     packages=find_packages(),
     install_requires=[
         "pyahocorasick",
         "openai",
         "tenacity"
     ],
     py_modules=["lctutil"],
```

