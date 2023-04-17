# Comparing `tmp/UserReadWriteMemory-1.2.tar.gz` & `tmp/UserReadWriteMemory-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UserReadWriteMemory-1.2.tar", last modified: Mon Apr 17 04:16:52 2023, max compression
+gzip compressed data, was "UserReadWriteMemory-1.2.1.tar", last modified: Mon Apr 17 21:37:02 2023, max compression
```

## Comparing `UserReadWriteMemory-1.2.tar` & `UserReadWriteMemory-1.2.1.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 04:16:52.006382 UserReadWriteMemory-1.2/
--rw-rw-rw-   0        0        0     1093 2023-04-17 04:13:40.000000 UserReadWriteMemory-1.2/LICENSE
--rw-rw-rw-   0        0        0      984 2023-04-17 04:16:52.005382 UserReadWriteMemory-1.2/PKG-INFO
--rw-rw-rw-   0        0        0     4562 2023-04-17 04:12:56.000000 UserReadWriteMemory-1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 04:16:51.992366 UserReadWriteMemory-1.2/UserReadWriteMemory/
--rw-rw-rw-   0        0        0    12836 2023-04-17 04:16:29.000000 UserReadWriteMemory-1.2/UserReadWriteMemory/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 04:16:52.002382 UserReadWriteMemory-1.2/UserReadWriteMemory.egg-info/
--rw-rw-rw-   0        0        0      984 2023-04-17 04:16:51.000000 UserReadWriteMemory-1.2/UserReadWriteMemory.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2023-04-17 04:16:51.000000 UserReadWriteMemory-1.2/UserReadWriteMemory.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 04:16:51.000000 UserReadWriteMemory-1.2/UserReadWriteMemory.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-04-17 04:16:51.000000 UserReadWriteMemory-1.2/UserReadWriteMemory.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 04:16:52.006382 UserReadWriteMemory-1.2/setup.cfg
--rw-rw-rw-   0        0        0     1182 2023-04-17 04:16:29.000000 UserReadWriteMemory-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 21:37:02.816462 UserReadWriteMemory-1.2.1/
+-rw-rw-rw-   0        0        0     6811 2023-04-17 21:37:02.815461 UserReadWriteMemory-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5893 2023-04-17 21:34:43.000000 UserReadWriteMemory-1.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 21:37:02.801427 UserReadWriteMemory-1.2.1/UserReadWriteMemory/
+-rw-rw-rw-   0        0        0    12976 2023-04-17 21:24:48.000000 UserReadWriteMemory-1.2.1/UserReadWriteMemory/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 21:37:02.813461 UserReadWriteMemory-1.2.1/UserReadWriteMemory.egg-info/
+-rw-rw-rw-   0        0        0     6811 2023-04-17 21:37:02.000000 UserReadWriteMemory-1.2.1/UserReadWriteMemory.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2023-04-17 21:37:02.000000 UserReadWriteMemory-1.2.1/UserReadWriteMemory.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 21:37:02.000000 UserReadWriteMemory-1.2.1/UserReadWriteMemory.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-04-17 21:37:02.000000 UserReadWriteMemory-1.2.1/UserReadWriteMemory.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 21:37:02.816462 UserReadWriteMemory-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1145 2023-04-17 21:36:18.000000 UserReadWriteMemory-1.2.1/setup.py
```

### Comparing `UserReadWriteMemory-1.2/UserReadWriteMemory/__init__.py` & `UserReadWriteMemory-1.2.1/UserReadWriteMemory/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Source: https://github.com/User00092/UserReadWriteMemory
 from typing import Any, List
 import ctypes.wintypes
 import os.path
 import ctypes
 
-__VERSION__ = 1.2
+__VERSION__ = '1.2.1'
 
 # Process Permissions
 PROCESS_QUERY_INFORMATION = 0x0400
 PROCESS_VM_OPERATION = 0x0008
 PROCESS_VM_READ = 0x0010
 PROCESS_VM_WRITE = 0x0020
 PROCESS_ALL_ACCESS = 0x1f0fff
@@ -75,14 +75,22 @@
 		"""
 		Get the last error code.
 
 		:return: The last error code.
 		"""
 		return ctypes.windll.kernel32.GetLastError()
 
+	def get_handle(self) -> int:
+		"""
+		Get the handle of the process.
+
+		:return: The process handle
+		"""
+		return self.handle
+
 	def get_pointer(self, lp_base_address: hex, offsets: List[hex] = ()) -> int:
 		"""
 		Get the pointer of a given address.
 
 		:param lp_base_address: The address from where you want to get the pointer.
 		:param offsets: a list of offets.
```

### Comparing `UserReadWriteMemory-1.2/setup.py` & `UserReadWriteMemory-1.2.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from setuptools import setup
+import codecs
+import os
 
-VERSION = '1.2'
+here = os.path.abspath(os.path.dirname(__file__))
+
+with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
+    LONG_DESCRIPTION = "\n" + fh.read()
+
+VERSION = '1.2.1'
 DESCRIPTION = 'Reading and writing to the memory of any process.'
-LONG_DESCRIPTION = """
-The UserReadWriteMemory module is specifically designed to enable the process of reading from and writing to the memory
-of any given process. View documentation here: https://github.com/User00092/UserReadWriteMemory
-"""
 
 # Setting up
 setup(
 	name="UserReadWriteMemory",
-	url="https://github.com/User00092/UserReadWriteMemory",
+	url="https://github.com/User00092/UserReadWriteMemory/tree/1.2.1",
 	version=VERSION,
 	license='MIT',
 	author="User0092",
 	author_email="unknownuser0092@protonmail.com",
 	description=DESCRIPTION,
 	long_description_content_type="text/markdown",
 	long_description=LONG_DESCRIPTION,
@@ -26,9 +29,9 @@
 		'Development Status :: 5 - Production/Stable',
 		'Topic :: Utilities',
 		'Operating System :: MacOS :: MacOS X',
 		'Operating System :: Microsoft :: Windows',
 		'Operating System :: POSIX :: Linux',
 		'Programming Language :: Python',
 		'Intended Audience :: Developers'
-	],
+	]
 )
```

