# Comparing `tmp/hyperdb-python-0.1.0.tar.gz` & `tmp/hyperdb-python-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperdb-python-0.1.0.tar", last modified: Sun Apr 16 07:50:49 2023, max compression
+gzip compressed data, was "hyperdb-python-0.1.1.tar", last modified: Sun Apr 16 07:56:37 2023, max compression
```

## Comparing `hyperdb-python-0.1.0.tar` & `hyperdb-python-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 jdagdelen   (501) staff       (20)        0 2023-04-16 07:50:49.056416 hyperdb-python-0.1.0/
--rw-r--r--   0 jdagdelen   (501) staff       (20)     1070 2023-04-16 06:27:54.000000 hyperdb-python-0.1.0/LICENSE
--rw-r--r--   0 jdagdelen   (501) staff       (20)     1573 2023-04-16 07:50:49.056246 hyperdb-python-0.1.0/PKG-INFO
--rw-r--r--   0 jdagdelen   (501) staff       (20)      918 2023-04-16 07:50:45.000000 hyperdb-python-0.1.0/README.md
-drwxr-xr-x   0 jdagdelen   (501) staff       (20)        0 2023-04-16 07:50:49.055324 hyperdb-python-0.1.0/hyperdb/
--rw-r--r--   0 jdagdelen   (501) staff       (20)        0 2023-04-16 06:29:28.000000 hyperdb-python-0.1.0/hyperdb/__init__.py
--rw-r--r--   0 jdagdelen   (501) staff       (20)      381 2023-04-16 07:39:19.000000 hyperdb-python-0.1.0/hyperdb/galaxy_brain_math_shit.py
--rw-r--r--   0 jdagdelen   (501) staff       (20)     2660 2023-04-16 07:40:13.000000 hyperdb-python-0.1.0/hyperdb/hyperdb.py
-drwxr-xr-x   0 jdagdelen   (501) staff       (20)        0 2023-04-16 07:50:49.056047 hyperdb-python-0.1.0/hyperdb_python.egg-info/
--rw-r--r--   0 jdagdelen   (501) staff       (20)     1573 2023-04-16 07:50:49.000000 hyperdb-python-0.1.0/hyperdb_python.egg-info/PKG-INFO
--rw-r--r--   0 jdagdelen   (501) staff       (20)      288 2023-04-16 07:50:49.000000 hyperdb-python-0.1.0/hyperdb_python.egg-info/SOURCES.txt
--rw-r--r--   0 jdagdelen   (501) staff       (20)        1 2023-04-16 07:50:49.000000 hyperdb-python-0.1.0/hyperdb_python.egg-info/dependency_links.txt
--rw-r--r--   0 jdagdelen   (501) staff       (20)       13 2023-04-16 07:50:49.000000 hyperdb-python-0.1.0/hyperdb_python.egg-info/requires.txt
--rw-r--r--   0 jdagdelen   (501) staff       (20)        8 2023-04-16 07:50:49.000000 hyperdb-python-0.1.0/hyperdb_python.egg-info/top_level.txt
--rw-r--r--   0 jdagdelen   (501) staff       (20)       38 2023-04-16 07:50:49.056467 hyperdb-python-0.1.0/setup.cfg
--rw-r--r--   0 jdagdelen   (501) staff       (20)      935 2023-04-16 07:50:09.000000 hyperdb-python-0.1.0/setup.py
+drwxr-xr-x   0 jdagdelen   (501) staff       (20)        0 2023-04-16 07:56:37.666257 hyperdb-python-0.1.1/
+-rw-r--r--   0 jdagdelen   (501) staff       (20)     1070 2023-04-16 06:27:54.000000 hyperdb-python-0.1.1/LICENSE
+-rw-r--r--   0 jdagdelen   (501) staff       (20)     1573 2023-04-16 07:56:37.666089 hyperdb-python-0.1.1/PKG-INFO
+-rw-r--r--   0 jdagdelen   (501) staff       (20)      918 2023-04-16 07:50:45.000000 hyperdb-python-0.1.1/README.md
+drwxr-xr-x   0 jdagdelen   (501) staff       (20)        0 2023-04-16 07:56:37.665156 hyperdb-python-0.1.1/hyperdb/
+-rw-r--r--   0 jdagdelen   (501) staff       (20)       22 2023-04-16 07:55:26.000000 hyperdb-python-0.1.1/hyperdb/__init__.py
+-rw-r--r--   0 jdagdelen   (501) staff       (20)      381 2023-04-16 07:39:19.000000 hyperdb-python-0.1.1/hyperdb/galaxy_brain_math_shit.py
+-rw-r--r--   0 jdagdelen   (501) staff       (20)     2667 2023-04-16 07:55:04.000000 hyperdb-python-0.1.1/hyperdb/hyperdb.py
+drwxr-xr-x   0 jdagdelen   (501) staff       (20)        0 2023-04-16 07:56:37.665886 hyperdb-python-0.1.1/hyperdb_python.egg-info/
+-rw-r--r--   0 jdagdelen   (501) staff       (20)     1573 2023-04-16 07:56:37.000000 hyperdb-python-0.1.1/hyperdb_python.egg-info/PKG-INFO
+-rw-r--r--   0 jdagdelen   (501) staff       (20)      288 2023-04-16 07:56:37.000000 hyperdb-python-0.1.1/hyperdb_python.egg-info/SOURCES.txt
+-rw-r--r--   0 jdagdelen   (501) staff       (20)        1 2023-04-16 07:56:37.000000 hyperdb-python-0.1.1/hyperdb_python.egg-info/dependency_links.txt
+-rw-r--r--   0 jdagdelen   (501) staff       (20)       13 2023-04-16 07:56:37.000000 hyperdb-python-0.1.1/hyperdb_python.egg-info/requires.txt
+-rw-r--r--   0 jdagdelen   (501) staff       (20)        8 2023-04-16 07:56:37.000000 hyperdb-python-0.1.1/hyperdb_python.egg-info/top_level.txt
+-rw-r--r--   0 jdagdelen   (501) staff       (20)       38 2023-04-16 07:56:37.666306 hyperdb-python-0.1.1/setup.cfg
+-rw-r--r--   0 jdagdelen   (501) staff       (20)      935 2023-04-16 07:56:08.000000 hyperdb-python-0.1.1/setup.py
```

### Comparing `hyperdb-python-0.1.0/LICENSE` & `hyperdb-python-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperdb-python-0.1.0/PKG-INFO` & `hyperdb-python-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperdb-python
-Version: 0.1.0
+Version: 0.1.1
 Summary: A hyper-fast local vector database for use with LLM Agents.
 Home-page: https://github.com/jdagdelen/hyperdb
 Author: John Dagdelen
 Author-email: jjdagdelen@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hyperdb-python-0.1.0/README.md` & `hyperdb-python-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `hyperdb-python-0.1.0/hyperdb/hyperdb.py` & `hyperdb-python-0.1.1/hyperdb/hyperdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import json
 import numpy as np
 import openai
-from galaxy_brain_math_shit import cosine_similarity
-
+from hyperdb.galaxy_brain_math_shit import cosine_similarity
 
 def get_embedding(documents, key=None, model="text-embedding-ada-002"):
     """Default embedding function that uses OpenAI Embeddings."""
     if isinstance(documents, list):
         if isinstance(documents[0], dict):
             if "." in key:
                 key_chain = key.split(".")
```

### Comparing `hyperdb-python-0.1.0/hyperdb_python.egg-info/PKG-INFO` & `hyperdb-python-0.1.1/hyperdb_python.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperdb-python
-Version: 0.1.0
+Version: 0.1.1
 Summary: A hyper-fast local vector database for use with LLM Agents.
 Home-page: https://github.com/jdagdelen/hyperdb
 Author: John Dagdelen
 Author-email: jjdagdelen@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hyperdb-python-0.1.0/setup.py` & `hyperdb-python-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="hyperdb-python",
-    version="0.1.0",
+    version="0.1.1",
     author="John Dagdelen",
     author_email="jjdagdelen@gmail.com",
     description="A hyper-fast local vector database for use with LLM Agents.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jdagdelen/hyperdb",
     packages=find_packages(),
```

