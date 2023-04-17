# Comparing `tmp/licant-1.9.4.tar.gz` & `tmp/licant-1.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "licant-1.9.4.tar", last modified: Fri May 13 14:20:36 2022, max compression
+gzip compressed data, was "licant-1.9.5.tar", last modified: Tue Jun 21 18:08:12 2022, max compression
```

## Comparing `licant-1.9.4.tar` & `licant-1.9.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-13 14:20:36.835058 licant-1.9.4/
--rw-r--r--   0 root         (0) root         (0)     2349 2022-05-13 14:20:36.835058 licant-1.9.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1694 2022-05-13 14:19:11.000000 licant-1.9.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-13 14:20:36.825058 licant-1.9.4/configurator/
--rwxr-xr-x   0 root         (0) root         (0)     1813 2022-05-13 14:19:11.000000 licant-1.9.4/configurator/licant-libs
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-13 14:20:36.835058 licant-1.9.4/licant/
--rw-r--r--   0 root         (0) root         (0)     2229 2022-05-13 14:19:11.000000 licant-1.9.4/licant/__init__.py
--rw-r--r--   0 root         (0) root         (0)      550 2022-05-13 14:19:11.000000 licant-1.9.4/licant/cache.py
--rw-r--r--   0 root         (0) root         (0)     3501 2022-05-13 14:19:11.000000 licant-1.9.4/licant/cli.py
--rw-r--r--   0 root         (0) root         (0)    13280 2022-05-13 14:19:11.000000 licant-1.9.4/licant/core.py
--rw-r--r--   0 root         (0) root         (0)     8382 2022-05-13 14:19:11.000000 licant-1.9.4/licant/cxx_make.py
--rw-r--r--   0 root         (0) root         (0)    18967 2022-05-13 14:19:11.000000 licant-1.9.4/licant/cxx_modules.py
--rw-r--r--   0 root         (0) root         (0)     3525 2022-05-13 14:19:11.000000 licant-1.9.4/licant/install.py
--rw-r--r--   0 root         (0) root         (0)     1383 2022-05-13 14:19:11.000000 licant-1.9.4/licant/java_make.py
--rw-r--r--   0 root         (0) root         (0)     3051 2022-05-13 14:19:11.000000 licant-1.9.4/licant/libs.py
--rw-r--r--   0 root         (0) root         (0)     5411 2022-05-13 14:19:11.000000 licant-1.9.4/licant/make.py
--rw-r--r--   0 root         (0) root         (0)     5633 2022-05-13 14:19:11.000000 licant-1.9.4/licant/modules.py
--rw-r--r--   0 root         (0) root         (0)      983 2022-05-13 14:19:11.000000 licant-1.9.4/licant/scripter.py
--rw-r--r--   0 root         (0) root         (0)     5559 2022-05-13 14:19:11.000000 licant-1.9.4/licant/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-13 14:20:36.835058 licant-1.9.4/licant.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2349 2022-05-13 14:20:36.000000 licant-1.9.4/licant.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      388 2022-05-13 14:20:36.000000 licant-1.9.4/licant.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-13 14:20:36.000000 licant-1.9.4/licant.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        7 2022-05-13 14:20:36.000000 licant-1.9.4/licant.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-05-13 14:20:36.835058 licant-1.9.4/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)      734 2022-05-13 14:19:11.000000 licant-1.9.4/setup.py
+drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2022-06-21 18:08:12.057888 licant-1.9.5/
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     1970 2022-06-21 18:08:12.057888 licant-1.9.5/PKG-INFO
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     1694 2022-06-21 18:06:43.000000 licant-1.9.5/README.md
+drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2022-06-21 18:08:12.057888 licant-1.9.5/configurator/
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)     1813 2022-06-21 18:06:43.000000 licant-1.9.5/configurator/licant-libs
+drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2022-06-21 18:08:12.057888 licant-1.9.5/licant/
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     2229 2022-06-21 18:07:39.000000 licant-1.9.5/licant/__init__.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)      550 2022-06-21 18:06:43.000000 licant-1.9.5/licant/cache.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     3501 2022-06-21 18:06:57.000000 licant-1.9.5/licant/cli.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)    13280 2022-06-21 18:06:43.000000 licant-1.9.5/licant/core.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     8382 2022-06-21 18:06:43.000000 licant-1.9.5/licant/cxx_make.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)    18967 2022-06-21 18:06:43.000000 licant-1.9.5/licant/cxx_modules.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     3525 2022-06-21 18:06:43.000000 licant-1.9.5/licant/install.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     1383 2022-06-21 18:06:43.000000 licant-1.9.5/licant/java_make.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     3051 2022-06-21 18:06:43.000000 licant-1.9.5/licant/libs.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     5411 2022-06-21 18:06:43.000000 licant-1.9.5/licant/make.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     5633 2022-06-21 18:06:43.000000 licant-1.9.5/licant/modules.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)      983 2022-06-21 18:06:43.000000 licant-1.9.5/licant/scripter.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     5559 2022-06-21 18:06:43.000000 licant-1.9.5/licant/util.py
+drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2022-06-21 18:08:12.057888 licant-1.9.5/licant.egg-info/
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     1970 2022-06-21 18:08:12.000000 licant-1.9.5/licant.egg-info/PKG-INFO
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)      388 2022-06-21 18:08:12.000000 licant-1.9.5/licant.egg-info/SOURCES.txt
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)        1 2022-06-21 18:08:12.000000 licant-1.9.5/licant.egg-info/dependency_links.txt
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)        7 2022-06-21 18:08:12.000000 licant-1.9.5/licant.egg-info/top_level.txt
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)       38 2022-06-21 18:08:12.057888 licant-1.9.5/setup.cfg
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      734 2022-06-21 18:06:43.000000 licant-1.9.5/setup.py
```

### Comparing `licant-1.9.4/PKG-INFO` & `licant-1.9.5/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,58 +1,60 @@
 Metadata-Version: 2.1
 Name: licant
-Version: 1.9.4
+Version: 1.9.5
 Summary: licant make system
 Home-page: https://github.com/mirmik/licant
 Author: Sorokin Nikolay
 Author-email: mirmikns@yandex.ru
 License: MIT
-Description: # Licant
-        
-        Licant is designed to build small modular projects with a complex dependency tree.
-        
-        What is it?
-        -----------
-        Initially Likant was written as a system for assembling code for projects on microcontrollers.
-        
-        The core of the Lycant system is a make-like assembly tree solver written in python.
-        
-        But, the main feature of Licant in the system of modules.
-        The Likant paradigm consists in the description of a project by a set of modules that link to each other. Connecting the module automatically tightens the connection of dependent modules.
-        
-        Modules can have several implementations, which allows flexible configuration of the project. (For example, you can change the initialization code of the microcontroller or the implementation of the input-output system simply by replacing the implementation of the corresponding module).
-        
-        One of the goals of the project is to work with submodules located in remote directories. The library subsystem allows a project to refer to modules located in remote directories, which allows several projects to use the same code.
-        
-        Installing
-        ----------
-        
-        ```sh
-        python3 -m pip install licant
-        ```
-        
-        HelloWorld
-        ----------
-        ```python
-        #!/usr/bin/env python
-        
-        import licant.make as lmake
-        import licant
-        
-        lmake.source("a.txt")
-        lmake.copy(tgt = "build/b.txt", src = "a.txt")
-        lmake.copy(tgt = "build/c.txt", src = "build/b.txt")
-        
-        print("licant targets list:" + str(licant.core.core.targets))
-        
-        licant.ex(default = "build/c.txt")
-        ```
-        
-        Example projects
-        ----------------
-        [https://github.com/mirmik/nos](https://github.com/mirmik/nos)  
-        [https://github.com/mirmik/igris](https://github.com/mirmik/igris)  
-        [https://github.com/mirmik/genos](https://github.com/mirmik/genos)  
-        
 Keywords: testing,make
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
+
+# Licant
+
+Licant is designed to build small modular projects with a complex dependency tree.
+
+What is it?
+-----------
+Initially Likant was written as a system for assembling code for projects on microcontrollers.
+
+The core of the Lycant system is a make-like assembly tree solver written in python.
+
+But, the main feature of Licant in the system of modules.
+The Likant paradigm consists in the description of a project by a set of modules that link to each other. Connecting the module automatically tightens the connection of dependent modules.
+
+Modules can have several implementations, which allows flexible configuration of the project. (For example, you can change the initialization code of the microcontroller or the implementation of the input-output system simply by replacing the implementation of the corresponding module).
+
+One of the goals of the project is to work with submodules located in remote directories. The library subsystem allows a project to refer to modules located in remote directories, which allows several projects to use the same code.
+
+Installing
+----------
+
+```sh
+python3 -m pip install licant
+```
+
+HelloWorld
+----------
+```python
+#!/usr/bin/env python
+
+import licant.make as lmake
+import licant
+
+lmake.source("a.txt")
+lmake.copy(tgt = "build/b.txt", src = "a.txt")
+lmake.copy(tgt = "build/c.txt", src = "build/b.txt")
+
+print("licant targets list:" + str(licant.core.core.targets))
+
+licant.ex(default = "build/c.txt")
+```
+
+Example projects
+----------------
+[https://github.com/mirmik/nos](https://github.com/mirmik/nos)  
+[https://github.com/mirmik/igris](https://github.com/mirmik/igris)  
+[https://github.com/mirmik/genos](https://github.com/mirmik/genos)  
+
+
```

### Comparing `licant-1.9.4/README.md` & `licant-1.9.5/README.md`

 * *Files identical despite different names*

### Comparing `licant-1.9.4/configurator/licant-libs` & `licant-1.9.5/configurator/licant-libs`

 * *Files identical despite different names*

### Comparing `licant-1.9.4/licant/__init__.py` & `licant-1.9.5/licant/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from licant.util import error
 
 from licant.cxx_make import gcc_toolchain, clang_toolchain, host_toolchain
 
 import licant.scripter
 from licant.libs import include
 
-__version__ = "1.9.4"
+__version__ = "1.9.5"
 
 
 def directory():
     return licant.scripter.scriptq.curdir()
 
 
 def subtree(tgt):
```

### Comparing `licant-1.9.4/licant/cache.py` & `licant-1.9.5/licant/cache.py`

 * *Files identical despite different names*

### Comparing `licant-1.9.4/licant/cli.py` & `licant-1.9.5/licant/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     "-t",
     "--trace",
     action="store_true",
     default=False,
     help="print trace information",
 )
 parser.add_argument(
-    "-j", "--threads", default='j', help="amount of threads for executor"
+    "-j", "--threads", default='1', help="amount of threads for executor"
 )
 parser.add_argument(
     "-q",
     "--quite",
     action="store_true",
     default=False,
     help="don`t print shell operations",
```

### Comparing `licant-1.9.4/licant/core.py` & `licant-1.9.5/licant/core.py`

 * *Files identical despite different names*

### Comparing `licant-1.9.4/licant/cxx_make.py` & `licant-1.9.5/licant/cxx_make.py`

 * *Files identical despite different names*

### Comparing `licant-1.9.4/licant/cxx_modules.py` & `licant-1.9.5/licant/cxx_modules.py`

 * *Files identical despite different names*

### Comparing `licant-1.9.4/licant/install.py` & `licant-1.9.5/licant/install.py`

 * *Files identical despite different names*

### Comparing `licant-1.9.4/licant/java_make.py` & `licant-1.9.5/licant/java_make.py`

 * *Files identical despite different names*

### Comparing `licant-1.9.4/licant/libs.py` & `licant-1.9.5/licant/libs.py`

 * *Files identical despite different names*

### Comparing `licant-1.9.4/licant/make.py` & `licant-1.9.5/licant/make.py`

 * *Files identical despite different names*

### Comparing `licant-1.9.4/licant/modules.py` & `licant-1.9.5/licant/modules.py`

 * *Files identical despite different names*

### Comparing `licant-1.9.4/licant/scripter.py` & `licant-1.9.5/licant/scripter.py`

 * *Files identical despite different names*

### Comparing `licant-1.9.4/licant/util.py` & `licant-1.9.5/licant/util.py`

 * *Files identical despite different names*

### Comparing `licant-1.9.4/licant.egg-info/PKG-INFO` & `licant-1.9.5/licant.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,58 +1,60 @@
 Metadata-Version: 2.1
 Name: licant
-Version: 1.9.4
+Version: 1.9.5
 Summary: licant make system
 Home-page: https://github.com/mirmik/licant
 Author: Sorokin Nikolay
 Author-email: mirmikns@yandex.ru
 License: MIT
-Description: # Licant
-        
-        Licant is designed to build small modular projects with a complex dependency tree.
-        
-        What is it?
-        -----------
-        Initially Likant was written as a system for assembling code for projects on microcontrollers.
-        
-        The core of the Lycant system is a make-like assembly tree solver written in python.
-        
-        But, the main feature of Licant in the system of modules.
-        The Likant paradigm consists in the description of a project by a set of modules that link to each other. Connecting the module automatically tightens the connection of dependent modules.
-        
-        Modules can have several implementations, which allows flexible configuration of the project. (For example, you can change the initialization code of the microcontroller or the implementation of the input-output system simply by replacing the implementation of the corresponding module).
-        
-        One of the goals of the project is to work with submodules located in remote directories. The library subsystem allows a project to refer to modules located in remote directories, which allows several projects to use the same code.
-        
-        Installing
-        ----------
-        
-        ```sh
-        python3 -m pip install licant
-        ```
-        
-        HelloWorld
-        ----------
-        ```python
-        #!/usr/bin/env python
-        
-        import licant.make as lmake
-        import licant
-        
-        lmake.source("a.txt")
-        lmake.copy(tgt = "build/b.txt", src = "a.txt")
-        lmake.copy(tgt = "build/c.txt", src = "build/b.txt")
-        
-        print("licant targets list:" + str(licant.core.core.targets))
-        
-        licant.ex(default = "build/c.txt")
-        ```
-        
-        Example projects
-        ----------------
-        [https://github.com/mirmik/nos](https://github.com/mirmik/nos)  
-        [https://github.com/mirmik/igris](https://github.com/mirmik/igris)  
-        [https://github.com/mirmik/genos](https://github.com/mirmik/genos)  
-        
 Keywords: testing,make
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
+
+# Licant
+
+Licant is designed to build small modular projects with a complex dependency tree.
+
+What is it?
+-----------
+Initially Likant was written as a system for assembling code for projects on microcontrollers.
+
+The core of the Lycant system is a make-like assembly tree solver written in python.
+
+But, the main feature of Licant in the system of modules.
+The Likant paradigm consists in the description of a project by a set of modules that link to each other. Connecting the module automatically tightens the connection of dependent modules.
+
+Modules can have several implementations, which allows flexible configuration of the project. (For example, you can change the initialization code of the microcontroller or the implementation of the input-output system simply by replacing the implementation of the corresponding module).
+
+One of the goals of the project is to work with submodules located in remote directories. The library subsystem allows a project to refer to modules located in remote directories, which allows several projects to use the same code.
+
+Installing
+----------
+
+```sh
+python3 -m pip install licant
+```
+
+HelloWorld
+----------
+```python
+#!/usr/bin/env python
+
+import licant.make as lmake
+import licant
+
+lmake.source("a.txt")
+lmake.copy(tgt = "build/b.txt", src = "a.txt")
+lmake.copy(tgt = "build/c.txt", src = "build/b.txt")
+
+print("licant targets list:" + str(licant.core.core.targets))
+
+licant.ex(default = "build/c.txt")
+```
+
+Example projects
+----------------
+[https://github.com/mirmik/nos](https://github.com/mirmik/nos)  
+[https://github.com/mirmik/igris](https://github.com/mirmik/igris)  
+[https://github.com/mirmik/genos](https://github.com/mirmik/genos)  
+
+
```

### Comparing `licant-1.9.4/setup.py` & `licant-1.9.5/setup.py`

 * *Files identical despite different names*

