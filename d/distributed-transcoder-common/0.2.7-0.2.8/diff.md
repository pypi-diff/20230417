# Comparing `tmp/distributed-transcoder-common-0.2.7.tar.gz` & `tmp/distributed-transcoder-common-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "distributed-transcoder-common-0.2.7.tar", max compression
+gzip compressed data, was "distributed-transcoder-common-0.2.8.tar", max compression
```

## Comparing `distributed-transcoder-common-0.2.7.tar` & `distributed-transcoder-common-0.2.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       86 2023-04-04 05:32:08.748355 distributed-transcoder-common-0.2.7/distributed_transcoder_common/__init__.py
--rw-r--r--   0        0        0      496 2023-04-16 23:02:16.825649 distributed-transcoder-common-0.2.7/distributed_transcoder_common/message_types.py
--rw-r--r--   0        0        0     1939 2023-04-16 22:17:26.016806 distributed-transcoder-common-0.2.7/distributed_transcoder_common/models.py
--rw-r--r--   0        0        0      390 2023-04-16 23:02:40.005332 distributed-transcoder-common-0.2.7/pyproject.toml
--rw-r--r--   0        0        0      695 2023-04-16 23:02:42.654451 distributed-transcoder-common-0.2.7/setup.py
--rw-r--r--   0        0        0      422 2023-04-16 23:02:42.654643 distributed-transcoder-common-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0       86 2023-04-04 05:32:08.748355 distributed-transcoder-common-0.2.8/distributed_transcoder_common/__init__.py
+-rw-r--r--   0        0        0      561 2023-04-17 00:20:24.807686 distributed-transcoder-common-0.2.8/distributed_transcoder_common/message_types.py
+-rw-r--r--   0        0        0     1939 2023-04-16 22:17:26.016806 distributed-transcoder-common-0.2.8/distributed_transcoder_common/models.py
+-rw-r--r--   0        0        0      390 2023-04-17 00:20:34.627575 distributed-transcoder-common-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0      695 2023-04-17 00:20:37.053000 distributed-transcoder-common-0.2.8/setup.py
+-rw-r--r--   0        0        0      422 2023-04-17 00:20:37.053211 distributed-transcoder-common-0.2.8/PKG-INFO
```

### Comparing `distributed-transcoder-common-0.2.7/distributed_transcoder_common/models.py` & `distributed-transcoder-common-0.2.8/distributed_transcoder_common/models.py`

 * *Files identical despite different names*

### Comparing `distributed-transcoder-common-0.2.7/setup.py` & `distributed-transcoder-common-0.2.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['tortoise-orm>=0.19.3,<0.20.0']
 
 setup_kwargs = {
     'name': 'distributed-transcoder-common',
-    'version': '0.2.7',
+    'version': '0.2.8',
     'description': 'A common library for for the distributed transcoder project',
     'long_description': None,
     'author': 'Eric Volpert',
     'author_email': 'ericvolp12@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

