# Comparing `tmp/UserReadWriteMemory-1.tar.gz` & `tmp/UserReadWriteMemory-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UserReadWriteMemory-1.tar", last modified: Mon Apr 17 00:25:00 2023, max compression
+gzip compressed data, was "UserReadWriteMemory-1.1.tar", last modified: Mon Apr 17 01:16:12 2023, max compression
```

## Comparing `UserReadWriteMemory-1.tar` & `UserReadWriteMemory-1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 00:25:00.234748 UserReadWriteMemory-1/
--rw-rw-rw-   0        0        0      905 2023-04-17 00:25:00.234748 UserReadWriteMemory-1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-17 00:25:00.220712 UserReadWriteMemory-1/UserReadWriteMemory/
--rw-rw-rw-   0        0        0    12817 2023-04-17 00:08:07.000000 UserReadWriteMemory-1/UserReadWriteMemory/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 00:25:00.231235 UserReadWriteMemory-1/UserReadWriteMemory.egg-info/
--rw-rw-rw-   0        0        0      905 2023-04-17 00:25:00.000000 UserReadWriteMemory-1/UserReadWriteMemory.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2023-04-17 00:25:00.000000 UserReadWriteMemory-1/UserReadWriteMemory.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 00:25:00.000000 UserReadWriteMemory-1/UserReadWriteMemory.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-04-17 00:25:00.000000 UserReadWriteMemory-1/UserReadWriteMemory.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 00:25:00.235747 UserReadWriteMemory-1/setup.cfg
--rw-rw-rw-   0        0        0     1101 2023-04-17 00:18:01.000000 UserReadWriteMemory-1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 01:16:12.266618 UserReadWriteMemory-1.1/
+-rw-rw-rw-   0        0        0      886 2023-04-17 01:16:12.265110 UserReadWriteMemory-1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-17 01:16:12.251573 UserReadWriteMemory-1.1/UserReadWriteMemory/
+-rw-rw-rw-   0        0        0    12836 2023-04-17 01:04:40.000000 UserReadWriteMemory-1.1/UserReadWriteMemory/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 01:16:12.262598 UserReadWriteMemory-1.1/UserReadWriteMemory.egg-info/
+-rw-rw-rw-   0        0        0      886 2023-04-17 01:16:12.000000 UserReadWriteMemory-1.1/UserReadWriteMemory.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2023-04-17 01:16:12.000000 UserReadWriteMemory-1.1/UserReadWriteMemory.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 01:16:12.000000 UserReadWriteMemory-1.1/UserReadWriteMemory.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-04-17 01:16:12.000000 UserReadWriteMemory-1.1/UserReadWriteMemory.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 01:16:12.266618 UserReadWriteMemory-1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1107 2023-04-17 01:06:09.000000 UserReadWriteMemory-1.1/setup.py
```

### Comparing `UserReadWriteMemory-1/UserReadWriteMemory/__init__.py` & `UserReadWriteMemory-1.1/UserReadWriteMemory/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Source: https://github.com/User00092/UserReadWriteMemory
-
 from typing import Any, List
+import ctypes.wintypes
 import os.path
 import ctypes
-import ctypes.wintypes
+
+__VERSION__ = 1.1
 
 # Process Permissions
 PROCESS_QUERY_INFORMATION = 0x0400
 PROCESS_VM_OPERATION = 0x0008
 PROCESS_VM_READ = 0x0010
 PROCESS_VM_WRITE = 0x0020
 PROCESS_ALL_ACCESS = 0x1f0fff
```

### Comparing `UserReadWriteMemory-1/setup.py` & `UserReadWriteMemory-1.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 from setuptools import setup
 
-VERSION = '1'
+VERSION = '1.1'
 DESCRIPTION = 'Reading and writing to the memory of any process.'
-LONG_DESCRIPTION = '''The ReadWriteMemory Class is made on Python for reading and writing to the memory of any process.
-                   This Class does not depend on any extra modules and only uses standard Python libraries like ctypes.
-                   '''
+LONG_DESCRIPTION = """
+The UserReadWriteMemory module is specifically designed to enable the process of reading from and writing to the memory of any given process.
+"""
 
 # Setting up
 setup(
 	name="UserReadWriteMemory",
+	url="https://github.com/User00092/UserReadWriteMemory",
 	version=VERSION,
+	license='MIT',
 	author="User0092",
 	author_email="unknownuser0092@protonmail.com",
 	description=DESCRIPTION,
 	long_description_content_type="text/markdown",
 	long_description=LONG_DESCRIPTION,
 	packages=['UserReadWriteMemory'],
 	keywords=['Read Memory', 'Write Memory', 'Process memory', 'Hacking', 'UserReadWriteMemory'],
 	python_requires='>=3.4.0',
+	install_requires=[],
 	classifiers=[
 		'Development Status :: 5 - Production/Stable',
 		'Topic :: Utilities',
 		'Operating System :: MacOS :: MacOS X',
 		'Operating System :: Microsoft :: Windows',
 		'Operating System :: POSIX :: Linux',
 		'Programming Language :: Python',
```

