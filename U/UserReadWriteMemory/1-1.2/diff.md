# Comparing `tmp/UserReadWriteMemory-1.tar.gz` & `tmp/UserReadWriteMemory-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UserReadWriteMemory-1.tar", last modified: Mon Apr 17 00:25:00 2023, max compression
+gzip compressed data, was "UserReadWriteMemory-1.2.tar", last modified: Mon Apr 17 04:16:52 2023, max compression
```

## Comparing `UserReadWriteMemory-1.tar` & `UserReadWriteMemory-1.2.tar`

### file list

```diff
@@ -1,11 +1,13 @@
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
+drwxrwxrwx   0        0        0        0 2023-04-17 04:16:52.006382 UserReadWriteMemory-1.2/
+-rw-rw-rw-   0        0        0     1093 2023-04-17 04:13:40.000000 UserReadWriteMemory-1.2/LICENSE
+-rw-rw-rw-   0        0        0      984 2023-04-17 04:16:52.005382 UserReadWriteMemory-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4562 2023-04-17 04:12:56.000000 UserReadWriteMemory-1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 04:16:51.992366 UserReadWriteMemory-1.2/UserReadWriteMemory/
+-rw-rw-rw-   0        0        0    12836 2023-04-17 04:16:29.000000 UserReadWriteMemory-1.2/UserReadWriteMemory/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 04:16:52.002382 UserReadWriteMemory-1.2/UserReadWriteMemory.egg-info/
+-rw-rw-rw-   0        0        0      984 2023-04-17 04:16:51.000000 UserReadWriteMemory-1.2/UserReadWriteMemory.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-04-17 04:16:51.000000 UserReadWriteMemory-1.2/UserReadWriteMemory.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 04:16:51.000000 UserReadWriteMemory-1.2/UserReadWriteMemory.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-04-17 04:16:51.000000 UserReadWriteMemory-1.2/UserReadWriteMemory.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 04:16:52.006382 UserReadWriteMemory-1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1182 2023-04-17 04:16:29.000000 UserReadWriteMemory-1.2/setup.py
```

### Comparing `UserReadWriteMemory-1/UserReadWriteMemory/__init__.py` & `UserReadWriteMemory-1.2/UserReadWriteMemory/__init__.py`

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
+__VERSION__ = 1.2
 
 # Process Permissions
 PROCESS_QUERY_INFORMATION = 0x0400
 PROCESS_VM_OPERATION = 0x0008
 PROCESS_VM_READ = 0x0010
 PROCESS_VM_WRITE = 0x0020
 PROCESS_ALL_ACCESS = 0x1f0fff
@@ -280,15 +281,15 @@
 	"""
 
 	def __init__(self):
 		self.process = Process()
 
 	def get_process_by_name(self, process_name: str) -> "Process":
 		"""
-		:description: Get the process by the process executabe\'s name and return a Process object.
+		:description: Get the process by the process executable's name and return a Process object.
 
 		:param process_name: The name of the executable file for the specified process for example, my_program.exe.
 
 		:return: A Process object containing the information from the requested Process.
 		"""
 		if not process_name.endswith('.exe'):
 			self.process.name = process_name + '.exe'
```

### Comparing `UserReadWriteMemory-1/setup.py` & `UserReadWriteMemory-1.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 from setuptools import setup
 
-VERSION = '1'
+VERSION = '1.2'
 DESCRIPTION = 'Reading and writing to the memory of any process.'
-LONG_DESCRIPTION = '''The ReadWriteMemory Class is made on Python for reading and writing to the memory of any process.
-                   This Class does not depend on any extra modules and only uses standard Python libraries like ctypes.
-                   '''
+LONG_DESCRIPTION = """
+The UserReadWriteMemory module is specifically designed to enable the process of reading from and writing to the memory
+of any given process. View documentation here: https://github.com/User00092/UserReadWriteMemory
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

