# Comparing `tmp/simp_le-client-0.8.1.tar.gz` & `tmp/simp_le-client-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/simp_le-client-0.8.1.tar", last modified: Mon Jun 11 17:08:22 2018, max compression
+gzip compressed data, was "dist/simp_le-client-0.9.0.tar", last modified: Mon Jun 11 17:12:44 2018, max compression
```

## Comparing `simp_le-client-0.8.1.tar` & `simp_le-client-0.9.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 isd       (1000) users      (984)        0 2018-06-11 17:08:22.000000 simp_le-client-0.8.1/
-drwxr-xr-x   0 isd       (1000) users      (984)        0 2018-06-11 17:08:22.000000 simp_le-client-0.8.1/docker/
-drwxr-xr-x   0 isd       (1000) users      (984)        0 2018-06-11 17:08:22.000000 simp_le-client-0.8.1/docker/hooks/
--rwxr-xr-x   0 isd       (1000) users      (984)      495 2018-01-10 12:46:56.000000 simp_le-client-0.8.1/docker/hooks/build
--rwxr-xr-x   0 isd       (1000) users      (984)      329 2018-01-10 12:46:56.000000 simp_le-client-0.8.1/docker/hooks/post_push
--rwxr-xr-x   0 isd       (1000) users      (984)      101 2018-01-10 12:46:56.000000 simp_le-client-0.8.1/docker/hooks/push
--rw-r--r--   0 isd       (1000) users      (984)      763 2018-01-10 12:46:56.000000 simp_le-client-0.8.1/docker/Dockerfile
--rw-r--r--   0 isd       (1000) users      (984)     2599 2018-01-10 12:46:56.000000 simp_le-client-0.8.1/docker/README.md
--rwxr-xr-x   0 isd       (1000) users      (984)      389 2018-01-10 12:46:56.000000 simp_le-client-0.8.1/docker/entrypoint.sh
-drwxr-xr-x   0 isd       (1000) users      (984)        0 2018-06-11 17:08:22.000000 simp_le-client-0.8.1/examples/
--rwxr-xr-x   0 isd       (1000) users      (984)      453 2018-01-10 12:46:56.000000 simp_le-client-0.8.1/examples/external.sh
-drwxr-xr-x   0 isd       (1000) users      (984)        0 2018-06-11 17:08:22.000000 simp_le-client-0.8.1/pyi/
--rw-r--r--   0 isd       (1000) users      (984)       14 2018-01-10 12:46:56.000000 simp_le-client-0.8.1/pyi/.gitignore
--rw-r--r--   0 isd       (1000) users      (984)       58 2018-01-10 12:46:56.000000 simp_le-client-0.8.1/pyi/Makefile
--rw-r--r--   0 isd       (1000) users      (984)      169 2018-01-10 12:46:56.000000 simp_le-client-0.8.1/pyi/README.md
--rw-r--r--   0 isd       (1000) users      (984)      917 2018-01-10 12:46:56.000000 simp_le-client-0.8.1/pyi/entrypoints.py
--rw-r--r--   0 isd       (1000) users      (984)       17 2018-01-10 12:46:56.000000 simp_le-client-0.8.1/pyi/requirements.txt
--rw-r--r--   0 isd       (1000) users      (984)     1876 2018-01-10 12:46:56.000000 simp_le-client-0.8.1/pyi/rthook-entrypoints.py
--rw-r--r--   0 isd       (1000) users      (984)     1150 2018-01-10 12:46:56.000000 simp_le-client-0.8.1/pyi/simp_le.spec
-drwxr-xr-x   0 isd       (1000) users      (984)        0 2018-06-11 17:08:22.000000 simp_le-client-0.8.1/simp_le_client.egg-info/
--rw-r--r--   0 isd       (1000) users      (984)     7645 2018-06-11 17:08:22.000000 simp_le-client-0.8.1/simp_le_client.egg-info/PKG-INFO
--rw-r--r--   0 isd       (1000) users      (984)      643 2018-06-11 17:08:22.000000 simp_le-client-0.8.1/simp_le_client.egg-info/SOURCES.txt
--rw-r--r--   0 isd       (1000) users      (984)        1 2018-06-11 17:08:22.000000 simp_le-client-0.8.1/simp_le_client.egg-info/dependency_links.txt
--rw-r--r--   0 isd       (1000) users      (984)       42 2018-06-11 17:08:22.000000 simp_le-client-0.8.1/simp_le_client.egg-info/entry_points.txt
--rw-r--r--   0 isd       (1000) users      (984)       94 2018-06-11 17:08:22.000000 simp_le-client-0.8.1/simp_le_client.egg-info/requires.txt
--rw-r--r--   0 isd       (1000) users      (984)        8 2018-06-11 17:08:22.000000 simp_le-client-0.8.1/simp_le_client.egg-info/top_level.txt
-drwxr-xr-x   0 isd       (1000) users      (984)        0 2018-06-11 17:08:22.000000 simp_le-client-0.8.1/tests/
--rwxr-xr-x   0 isd       (1000) users      (984)     1911 2018-01-10 12:46:56.000000 simp_le-client-0.8.1/tests/install.sh
--rwxr-xr-x   0 isd       (1000) users      (984)      726 2018-01-10 12:46:56.000000 simp_le-client-0.8.1/tests/test-suite.sh
--rw-r--r--   0 isd       (1000) users      (984)      306 2018-01-10 12:46:56.000000 simp_le-client-0.8.1/.gitignore
--rw-r--r--   0 isd       (1000) users      (984)      894 2018-03-12 19:21:19.000000 simp_le-client-0.8.1/.travis.yml
--rw-r--r--   0 isd       (1000) users      (984)      133 2018-01-10 12:46:56.000000 simp_le-client-0.8.1/CONTRIBUTING.md
--rw-r--r--   0 isd       (1000) users      (984)    35147 2018-01-10 12:46:56.000000 simp_le-client-0.8.1/LICENSE.txt
--rw-r--r--   0 isd       (1000) users      (984)       63 2018-01-10 12:46:56.000000 simp_le-client-0.8.1/MANIFEST.in
--rw-r--r--   0 isd       (1000) users      (984)     4994 2018-06-11 17:07:31.000000 simp_le-client-0.8.1/README.rst
--rwxr-xr-x   0 isd       (1000) users      (984)      835 2018-01-10 12:46:56.000000 simp_le-client-0.8.1/bootstrap.sh
--rw-r--r--   0 isd       (1000) users      (984)     2239 2018-06-11 17:05:19.000000 simp_le-client-0.8.1/setup.py
--rwxr-xr-x   0 isd       (1000) users      (984)    61251 2018-03-12 19:21:19.000000 simp_le-client-0.8.1/simp_le.py
--rwxr-xr-x   0 isd       (1000) users      (984)      504 2018-01-10 12:46:56.000000 simp_le-client-0.8.1/venv.sh
--rw-r--r--   0 isd       (1000) users      (984)     7645 2018-06-11 17:08:22.000000 simp_le-client-0.8.1/PKG-INFO
--rw-r--r--   0 isd       (1000) users      (984)       38 2018-06-11 17:08:22.000000 simp_le-client-0.8.1/setup.cfg
+drwxr-xr-x   0 isd       (1000) users      (984)        0 2018-06-11 17:12:44.000000 simp_le-client-0.9.0/
+drwxr-xr-x   0 isd       (1000) users      (984)        0 2018-06-11 17:12:44.000000 simp_le-client-0.9.0/docker/
+drwxr-xr-x   0 isd       (1000) users      (984)        0 2018-06-11 17:12:44.000000 simp_le-client-0.9.0/docker/hooks/
+-rwxr-xr-x   0 isd       (1000) users      (984)      495 2018-01-10 12:46:56.000000 simp_le-client-0.9.0/docker/hooks/build
+-rwxr-xr-x   0 isd       (1000) users      (984)      329 2018-01-10 12:46:56.000000 simp_le-client-0.9.0/docker/hooks/post_push
+-rwxr-xr-x   0 isd       (1000) users      (984)      101 2018-01-10 12:46:56.000000 simp_le-client-0.9.0/docker/hooks/push
+-rw-r--r--   0 isd       (1000) users      (984)      763 2018-01-10 12:46:56.000000 simp_le-client-0.9.0/docker/Dockerfile
+-rw-r--r--   0 isd       (1000) users      (984)     2599 2018-01-10 12:46:56.000000 simp_le-client-0.9.0/docker/README.md
+-rwxr-xr-x   0 isd       (1000) users      (984)      389 2018-01-10 12:46:56.000000 simp_le-client-0.9.0/docker/entrypoint.sh
+drwxr-xr-x   0 isd       (1000) users      (984)        0 2018-06-11 17:12:44.000000 simp_le-client-0.9.0/examples/
+-rwxr-xr-x   0 isd       (1000) users      (984)      453 2018-01-10 12:46:56.000000 simp_le-client-0.9.0/examples/external.sh
+drwxr-xr-x   0 isd       (1000) users      (984)        0 2018-06-11 17:12:44.000000 simp_le-client-0.9.0/pyi/
+-rw-r--r--   0 isd       (1000) users      (984)       14 2018-01-10 12:46:56.000000 simp_le-client-0.9.0/pyi/.gitignore
+-rw-r--r--   0 isd       (1000) users      (984)       58 2018-01-10 12:46:56.000000 simp_le-client-0.9.0/pyi/Makefile
+-rw-r--r--   0 isd       (1000) users      (984)      169 2018-01-10 12:46:56.000000 simp_le-client-0.9.0/pyi/README.md
+-rw-r--r--   0 isd       (1000) users      (984)      917 2018-01-10 12:46:56.000000 simp_le-client-0.9.0/pyi/entrypoints.py
+-rw-r--r--   0 isd       (1000) users      (984)       17 2018-01-10 12:46:56.000000 simp_le-client-0.9.0/pyi/requirements.txt
+-rw-r--r--   0 isd       (1000) users      (984)     1876 2018-01-10 12:46:56.000000 simp_le-client-0.9.0/pyi/rthook-entrypoints.py
+-rw-r--r--   0 isd       (1000) users      (984)     1150 2018-01-10 12:46:56.000000 simp_le-client-0.9.0/pyi/simp_le.spec
+drwxr-xr-x   0 isd       (1000) users      (984)        0 2018-06-11 17:12:44.000000 simp_le-client-0.9.0/simp_le_client.egg-info/
+-rw-r--r--   0 isd       (1000) users      (984)     7724 2018-06-11 17:12:44.000000 simp_le-client-0.9.0/simp_le_client.egg-info/PKG-INFO
+-rw-r--r--   0 isd       (1000) users      (984)      643 2018-06-11 17:12:44.000000 simp_le-client-0.9.0/simp_le_client.egg-info/SOURCES.txt
+-rw-r--r--   0 isd       (1000) users      (984)        1 2018-06-11 17:12:44.000000 simp_le-client-0.9.0/simp_le_client.egg-info/dependency_links.txt
+-rw-r--r--   0 isd       (1000) users      (984)       42 2018-06-11 17:12:44.000000 simp_le-client-0.9.0/simp_le_client.egg-info/entry_points.txt
+-rw-r--r--   0 isd       (1000) users      (984)       94 2018-06-11 17:12:44.000000 simp_le-client-0.9.0/simp_le_client.egg-info/requires.txt
+-rw-r--r--   0 isd       (1000) users      (984)        8 2018-06-11 17:12:44.000000 simp_le-client-0.9.0/simp_le_client.egg-info/top_level.txt
+drwxr-xr-x   0 isd       (1000) users      (984)        0 2018-06-11 17:12:44.000000 simp_le-client-0.9.0/tests/
+-rwxr-xr-x   0 isd       (1000) users      (984)     2111 2018-06-11 17:09:03.000000 simp_le-client-0.9.0/tests/install.sh
+-rwxr-xr-x   0 isd       (1000) users      (984)      726 2018-01-10 12:46:56.000000 simp_le-client-0.9.0/tests/test-suite.sh
+-rw-r--r--   0 isd       (1000) users      (984)      306 2018-01-10 12:46:56.000000 simp_le-client-0.9.0/.gitignore
+-rw-r--r--   0 isd       (1000) users      (984)      837 2018-06-11 17:09:03.000000 simp_le-client-0.9.0/.travis.yml
+-rw-r--r--   0 isd       (1000) users      (984)      133 2018-01-10 12:46:56.000000 simp_le-client-0.9.0/CONTRIBUTING.md
+-rw-r--r--   0 isd       (1000) users      (984)    35147 2018-01-10 12:46:56.000000 simp_le-client-0.9.0/LICENSE.txt
+-rw-r--r--   0 isd       (1000) users      (984)       63 2018-01-10 12:46:56.000000 simp_le-client-0.9.0/MANIFEST.in
+-rw-r--r--   0 isd       (1000) users      (984)     5033 2018-06-11 17:10:35.000000 simp_le-client-0.9.0/README.rst
+-rwxr-xr-x   0 isd       (1000) users      (984)      835 2018-01-10 12:46:56.000000 simp_le-client-0.9.0/bootstrap.sh
+-rw-r--r--   0 isd       (1000) users      (984)     2228 2018-06-11 17:10:56.000000 simp_le-client-0.9.0/setup.py
+-rwxr-xr-x   0 isd       (1000) users      (984)    61251 2018-06-11 17:09:03.000000 simp_le-client-0.9.0/simp_le.py
+-rwxr-xr-x   0 isd       (1000) users      (984)      504 2018-01-10 12:46:56.000000 simp_le-client-0.9.0/venv.sh
+-rw-r--r--   0 isd       (1000) users      (984)     7724 2018-06-11 17:12:44.000000 simp_le-client-0.9.0/PKG-INFO
+-rw-r--r--   0 isd       (1000) users      (984)       38 2018-06-11 17:12:44.000000 simp_le-client-0.9.0/setup.cfg
```

### Comparing `simp_le-client-0.8.1/docker/Dockerfile` & `simp_le-client-0.9.0/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `simp_le-client-0.8.1/docker/README.md` & `simp_le-client-0.9.0/docker/README.md`

 * *Files identical despite different names*

### Comparing `simp_le-client-0.8.1/pyi/entrypoints.py` & `simp_le-client-0.9.0/pyi/entrypoints.py`

 * *Files identical despite different names*

### Comparing `simp_le-client-0.8.1/pyi/rthook-entrypoints.py` & `simp_le-client-0.9.0/pyi/rthook-entrypoints.py`

 * *Files identical despite different names*

### Comparing `simp_le-client-0.8.1/pyi/simp_le.spec` & `simp_le-client-0.9.0/pyi/simp_le.spec`

 * *Files identical despite different names*

### Comparing `simp_le-client-0.8.1/simp_le_client.egg-info/PKG-INFO` & `simp_le-client-0.9.0/simp_le_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simp-le-client
-Version: 0.8.1
+Version: 0.9.0
 Summary: Simple Let's Encrypt Client
 Home-page: https://github.com/zenhack/simp_le
 Author: Ian Denhardt
 Author-email: ian@zenhack.net
 License: GPLv3
 Description: simp\_le
         ========
@@ -115,14 +115,19 @@
         Below is a summary of changes introduced in each release. Any user-visible
         changes *must* be recorded here. Note that the topmost entry sometimes
         represents the *next* (i.e. not yet released) version.
         
         Releases occur approximately every two months, unless there is a pressing need
         to do otherwise (e.g. security & serious bug fixes).
         
+        0.9.0
+        +++++
+        
+        * Upgrade acme to 0.24.x
+        
         0.8.1
         +++++
         
         * Add a workaround for some installation problems caused by a bug in pip.
         
         0.8.0
         +++++
```

### Comparing `simp_le-client-0.8.1/simp_le_client.egg-info/SOURCES.txt` & `simp_le-client-0.9.0/simp_le_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `simp_le-client-0.8.1/tests/test-suite.sh` & `simp_le-client-0.9.0/tests/test-suite.sh`

 * *Files identical despite different names*

### Comparing `simp_le-client-0.8.1/LICENSE.txt` & `simp_le-client-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `simp_le-client-0.8.1/README.rst` & `simp_le-client-0.9.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -107,14 +107,19 @@
 Below is a summary of changes introduced in each release. Any user-visible
 changes *must* be recorded here. Note that the topmost entry sometimes
 represents the *next* (i.e. not yet released) version.
 
 Releases occur approximately every two months, unless there is a pressing need
 to do otherwise (e.g. security & serious bug fixes).
 
+0.9.0
++++++
+
+* Upgrade acme to 0.24.x
+
 0.8.1
 +++++
 
 * Add a workaround for some installation problems caused by a bug in pip.
 
 0.8.0
 +++++
```

### Comparing `simp_le-client-0.8.1/bootstrap.sh` & `simp_le-client-0.9.0/bootstrap.sh`

 * *Files identical despite different names*

### Comparing `simp_le-client-0.8.1/setup.py` & `simp_le-client-0.9.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import codecs
 import os
-import sys
 import setuptools
 
 
 here = os.path.abspath(os.path.dirname(__file__))
 readme = codecs.open(os.path.join(here, 'README.rst'), encoding='utf-8').read()
 
 install_requires = [
@@ -16,15 +15,15 @@
     #
     # See:
     #
     # * https://github.com/zenhack/simp_le/issues/62
     # * https://github.com/pypa/pip/issues/988
     'idna<2.7',
 
-    'acme>=0.22,<0.23',
+    'acme>=0.24,<0.25',
     'cryptography',
     # formerly known as acme.jose:
     'josepy',
     'mock',
     'pyOpenSSL',
     'pytz',
 ]
```

### Comparing `simp_le-client-0.8.1/simp_le.py` & `simp_le-client-0.9.0/simp_le.py`

 * *Files 1% similar despite different names*

```diff
@@ -1653,21 +1653,20 @@
 
 
 class IntegrationTests(unittest.TestCase):
     """Integrations tests with Boulder.
 
     Prerequisites:
     - /etc/hosts:127.0.0.1 le.wtf
-    - Boulder running on localhost:4000
+    - Boulder running on 10.77.77.1:4000 (with Docker)
     - Boulder verifying http-01 on port 5002
     """
     # this is a test suite | pylint: disable=missing-docstring
 
-    SERVER = 'http://localhost:4000/directory'
-    PORT = 5002
+    SERVER = 'http://10.77.77.1:4000/directory'
 
     @classmethod
     def _run(cls, cmd):
         args = ' '.join(cmd[1:])
         logger.debug('Running simp_le with the following args: %s', args)
         return subprocess.call(cmd)
```

### Comparing `simp_le-client-0.8.1/PKG-INFO` & `simp_le-client-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simp_le-client
-Version: 0.8.1
+Version: 0.9.0
 Summary: Simple Let's Encrypt Client
 Home-page: https://github.com/zenhack/simp_le
 Author: Ian Denhardt
 Author-email: ian@zenhack.net
 License: GPLv3
 Description: simp\_le
         ========
@@ -115,14 +115,19 @@
         Below is a summary of changes introduced in each release. Any user-visible
         changes *must* be recorded here. Note that the topmost entry sometimes
         represents the *next* (i.e. not yet released) version.
         
         Releases occur approximately every two months, unless there is a pressing need
         to do otherwise (e.g. security & serious bug fixes).
         
+        0.9.0
+        +++++
+        
+        * Upgrade acme to 0.24.x
+        
         0.8.1
         +++++
         
         * Add a workaround for some installation problems caused by a bug in pip.
         
         0.8.0
         +++++
```

