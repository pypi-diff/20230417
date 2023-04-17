# Comparing `tmp/pyntree-1.1.0.tar.gz` & `tmp/pyntree-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyntree-1.1.0.tar", last modified: Mon Apr 10 21:49:51 2023, max compression
+gzip compressed data, was "pyntree-1.1.1.tar", last modified: Mon Apr 17 13:41:42 2023, max compression
```

## Comparing `pyntree-1.1.0.tar` & `pyntree-1.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 jvadair   (1000) jvadair   (1000)        0 2023-04-10 21:49:51.862145 pyntree-1.1.0/
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)    11357 2023-03-27 17:16:15.000000 pyntree-1.1.0/LICENSE.txt
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)    15475 2023-04-10 21:49:51.862145 pyntree-1.1.0/PKG-INFO
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)     1585 2023-03-29 03:58:07.000000 pyntree-1.1.0/README.md
-drwxrwxr-x   0 jvadair   (1000) jvadair   (1000)        0 2023-04-10 21:49:51.858145 pyntree-1.1.0/pyntree/
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)     8585 2023-04-10 21:45:07.000000 pyntree-1.1.0/pyntree/__init__.py
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)     1128 2023-03-29 03:58:07.000000 pyntree-1.1.0/pyntree/encryption.py
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)      166 2023-04-10 21:40:01.000000 pyntree-1.1.0/pyntree/errors.py
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)     6259 2023-03-29 03:58:07.000000 pyntree-1.1.0/pyntree/file.py
-drwxrwxr-x   0 jvadair   (1000) jvadair   (1000)        0 2023-04-10 21:49:51.858145 pyntree-1.1.0/pyntree.egg-info/
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)    15475 2023-04-10 21:49:51.000000 pyntree-1.1.0/pyntree.egg-info/PKG-INFO
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)      298 2023-04-10 21:49:51.000000 pyntree-1.1.0/pyntree.egg-info/SOURCES.txt
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)        1 2023-04-10 21:49:51.000000 pyntree-1.1.0/pyntree.egg-info/dependency_links.txt
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)      117 2023-04-10 21:49:51.000000 pyntree-1.1.0/pyntree.egg-info/requires.txt
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)        8 2023-04-10 21:49:51.000000 pyntree-1.1.0/pyntree.egg-info/top_level.txt
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)     1298 2023-04-10 21:49:29.000000 pyntree-1.1.0/pyproject.toml
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)       23 2023-03-27 16:14:00.000000 pyntree-1.1.0/requirements.txt
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)       38 2023-04-10 21:49:51.862145 pyntree-1.1.0/setup.cfg
-drwxrwxr-x   0 jvadair   (1000) jvadair   (1000)        0 2023-04-10 21:49:51.858145 pyntree-1.1.0/tests/
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)    10991 2023-04-10 21:47:23.000000 pyntree-1.1.0/tests/tests.py
+drwxrwxr-x   0 jvadair   (1000) jvadair   (1000)        0 2023-04-17 13:41:42.639535 pyntree-1.1.1/
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)    11357 2023-03-27 17:16:15.000000 pyntree-1.1.1/LICENSE.txt
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)    15475 2023-04-17 13:41:42.639535 pyntree-1.1.1/PKG-INFO
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)     1585 2023-03-29 03:58:07.000000 pyntree-1.1.1/README.md
+drwxrwxr-x   0 jvadair   (1000) jvadair   (1000)        0 2023-04-17 13:41:42.631535 pyntree-1.1.1/pyntree/
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)     8585 2023-04-17 13:36:16.000000 pyntree-1.1.1/pyntree/__init__.py
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)     1128 2023-04-17 13:39:08.000000 pyntree-1.1.1/pyntree/encryption.py
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)      166 2023-04-10 21:40:01.000000 pyntree-1.1.1/pyntree/errors.py
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)     6259 2023-03-29 03:58:07.000000 pyntree-1.1.1/pyntree/file.py
+drwxrwxr-x   0 jvadair   (1000) jvadair   (1000)        0 2023-04-17 13:41:42.635535 pyntree-1.1.1/pyntree.egg-info/
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)    15475 2023-04-17 13:41:42.000000 pyntree-1.1.1/pyntree.egg-info/PKG-INFO
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)      298 2023-04-17 13:41:42.000000 pyntree-1.1.1/pyntree.egg-info/SOURCES.txt
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)        1 2023-04-17 13:41:42.000000 pyntree-1.1.1/pyntree.egg-info/dependency_links.txt
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)      117 2023-04-17 13:41:42.000000 pyntree-1.1.1/pyntree.egg-info/requires.txt
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)        8 2023-04-17 13:41:42.000000 pyntree-1.1.1/pyntree.egg-info/top_level.txt
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)     1298 2023-04-17 13:40:26.000000 pyntree-1.1.1/pyproject.toml
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)       23 2023-03-27 16:14:00.000000 pyntree-1.1.1/requirements.txt
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)       38 2023-04-17 13:41:42.639535 pyntree-1.1.1/setup.cfg
+drwxrwxr-x   0 jvadair   (1000) jvadair   (1000)        0 2023-04-17 13:41:42.635535 pyntree-1.1.1/tests/
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)    10991 2023-04-17 13:36:16.000000 pyntree-1.1.1/tests/tests.py
```

### Comparing `pyntree-1.1.0/LICENSE.txt` & `pyntree-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyntree-1.1.0/PKG-INFO` & `pyntree-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyntree
-Version: 1.1.0
+Version: 1.1.1
 Summary: pyntree is a python package which allows you to easily and syntactically save your data. Not only that, it also lets you save in multiple formats, and even serialize and compress data by merely changing a few characters.
 Author-email: jvadair <dev@jvadair.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `pyntree-1.1.0/README.md` & `pyntree-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pyntree-1.1.0/pyntree/__init__.py` & `pyntree-1.1.1/pyntree/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,29 +143,29 @@
         Check if the specified child Node exists
         :param items: The items to check for
         :return:
         """
         for item in items:
             return True if item in self._values else False
 
-    def where(self, **kwargs) -> list['Node']:
+    def where(self, **kwargs) -> List['Node']:
         """
         :param kwargs: Return all children with a child <kwarg> and its corresponding value
         :return: A list of Nodes matching the criteria
         """
         matches = []
         for name in self._values:
             child = self.get(name)
             for kwarg in kwargs:
                 if child.has(kwarg) and child.get(kwarg)() == kwargs[kwarg]:  # Evaluated left to right, so no error
                     matches.append(child)
 
         return matches
 
-    def containing(self, *args) -> list['Node']:
+    def containing(self, *args) -> List['Node']:
         """
         :param args: Return all children with children named <*args>
         :return: A list of Nodes matching the criteria
         """
         matches = []
         for name in self._values:
             child = self.get(name)
```

### Comparing `pyntree-1.1.0/pyntree/encryption.py` & `pyntree-1.1.1/pyntree/encryption.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 try:
     from cryptography.fernet import Fernet
     from argon2.low_level import hash_secret_raw, Type
     import base64
-    from pyntree.errors import Error
     SUPPORTED = True
 except:
     SUPPORTED = False
+    from pyntree.errors import Error
 
 
 def derive_key(password: str, salt: bytes):
     password = password.encode()
     key = hash_secret_raw(
         password,
         salt,
```

### Comparing `pyntree-1.1.0/pyntree/file.py` & `pyntree-1.1.1/pyntree/file.py`

 * *Files identical despite different names*

### Comparing `pyntree-1.1.0/pyntree.egg-info/PKG-INFO` & `pyntree-1.1.1/pyntree.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyntree
-Version: 1.1.0
+Version: 1.1.1
 Summary: pyntree is a python package which allows you to easily and syntactically save your data. Not only that, it also lets you save in multiple formats, and even serialize and compress data by merely changing a few characters.
 Author-email: jvadair <dev@jvadair.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `pyntree-1.1.0/pyproject.toml` & `pyntree-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 dynamic = ["dependencies"]
 name = "pyntree"
-version = "1.1.0"
+version = "1.1.1"
 description = "pyntree is a python package which allows you to easily and syntactically save your data. Not only that, it also lets you save in multiple formats, and even serialize and compress data by merely changing a few characters."
 readme = "README.md"
 authors = [{ name = "jvadair", email = "dev@jvadair.com" }]
 license = { file = "LICENSE.txt" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
```

### Comparing `pyntree-1.1.0/tests/tests.py` & `pyntree-1.1.1/tests/tests.py`

 * *Files identical despite different names*

