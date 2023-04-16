# Comparing `tmp/dailalib-1.0.0.tar.gz` & `tmp/dailalib-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dailalib-1.0.0.tar", last modified: Sun Apr 16 08:23:33 2023, max compression
+gzip compressed data, was "dailalib-1.1.2.tar", last modified: Sun Apr 16 23:16:56 2023, max compression
```

## Comparing `dailalib-1.0.0.tar` & `dailalib-1.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 mahaloz   (1000) mahaloz   (1000)        0 2023-04-16 08:23:33.023352 dailalib-1.0.0/
--rw-rw-r--   0 mahaloz   (1000) mahaloz   (1000)     2709 2023-04-16 08:23:33.023352 dailalib-1.0.0/PKG-INFO
--rw-rw-r--   0 mahaloz   (1000) mahaloz   (1000)     2314 2023-01-01 17:50:29.000000 dailalib-1.0.0/README.md
-drwxrwxr-x   0 mahaloz   (1000) mahaloz   (1000)        0 2023-04-16 08:23:33.019352 dailalib-1.0.0/dailalib/
--rw-rw-r--   0 mahaloz   (1000) mahaloz   (1000)       22 2023-04-16 08:08:04.000000 dailalib-1.0.0/dailalib/__init__.py
--rw-rw-r--   0 mahaloz   (1000) mahaloz   (1000)     1055 2023-01-01 17:50:29.000000 dailalib-1.0.0/dailalib/__main__.py
--rw-rw-r--   0 mahaloz   (1000) mahaloz   (1000)     3378 2023-04-16 08:08:04.000000 dailalib-1.0.0/dailalib/controller_server.py
--rw-rw-r--   0 mahaloz   (1000) mahaloz   (1000)     3758 2023-01-01 17:50:29.000000 dailalib-1.0.0/dailalib/installer.py
-drwxrwxr-x   0 mahaloz   (1000) mahaloz   (1000)        0 2023-04-16 08:23:33.023352 dailalib-1.0.0/dailalib/interfaces/
--rw-rw-r--   0 mahaloz   (1000) mahaloz   (1000)       99 2023-04-16 08:08:04.000000 dailalib-1.0.0/dailalib/interfaces/__init__.py
--rw-rw-r--   0 mahaloz   (1000) mahaloz   (1000)      743 2023-04-16 08:08:04.000000 dailalib-1.0.0/dailalib/interfaces/generic_ai_interface.py
--rw-rw-r--   0 mahaloz   (1000) mahaloz   (1000)    11138 2023-04-16 08:08:04.000000 dailalib-1.0.0/dailalib/interfaces/openai_interface.py
--rw-rw-r--   0 mahaloz   (1000) mahaloz   (1000)     2027 2023-04-16 08:08:04.000000 dailalib-1.0.0/dailalib/utils.py
-drwxrwxr-x   0 mahaloz   (1000) mahaloz   (1000)        0 2023-04-16 08:23:33.019352 dailalib-1.0.0/dailalib.egg-info/
--rw-rw-r--   0 mahaloz   (1000) mahaloz   (1000)     2709 2023-04-16 08:23:32.000000 dailalib-1.0.0/dailalib.egg-info/PKG-INFO
--rw-rw-r--   0 mahaloz   (1000) mahaloz   (1000)      450 2023-04-16 08:23:32.000000 dailalib-1.0.0/dailalib.egg-info/SOURCES.txt
--rw-rw-r--   0 mahaloz   (1000) mahaloz   (1000)        1 2023-04-16 08:23:32.000000 dailalib-1.0.0/dailalib.egg-info/dependency_links.txt
--rw-rw-r--   0 mahaloz   (1000) mahaloz   (1000)       49 2023-04-16 08:23:32.000000 dailalib-1.0.0/dailalib.egg-info/entry_points.txt
--rw-rw-r--   0 mahaloz   (1000) mahaloz   (1000)       31 2023-04-16 08:23:32.000000 dailalib-1.0.0/dailalib.egg-info/requires.txt
--rw-rw-r--   0 mahaloz   (1000) mahaloz   (1000)        9 2023-04-16 08:23:32.000000 dailalib-1.0.0/dailalib.egg-info/top_level.txt
--rw-rw-r--   0 mahaloz   (1000) mahaloz   (1000)      726 2023-04-16 08:23:33.023352 dailalib-1.0.0/setup.cfg
--rw-rw-r--   0 mahaloz   (1000) mahaloz   (1000)     1718 2023-01-01 17:50:29.000000 dailalib-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:16:56.200838 dailalib-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-04-16 23:16:56.200838 dailalib-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-04-16 23:16:45.000000 dailalib-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:16:56.200838 dailalib-1.1.2/dailalib/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-16 23:16:45.000000 dailalib-1.1.2/dailalib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-16 23:16:45.000000 dailalib-1.1.2/dailalib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-04-16 23:16:45.000000 dailalib-1.1.2/dailalib/controller_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-04-16 23:16:45.000000 dailalib-1.1.2/dailalib/installer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:16:56.200838 dailalib-1.1.2/dailalib/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-16 23:16:45.000000 dailalib-1.1.2/dailalib/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-16 23:16:45.000000 dailalib-1.1.2/dailalib/interfaces/generic_ai_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11138 2023-04-16 23:16:45.000000 dailalib-1.1.2/dailalib/interfaces/openai_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-16 23:16:45.000000 dailalib-1.1.2/dailalib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:16:56.200838 dailalib-1.1.2/dailalib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-04-16 23:16:56.000000 dailalib-1.1.2/dailalib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-16 23:16:56.000000 dailalib-1.1.2/dailalib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 23:16:56.000000 dailalib-1.1.2/dailalib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-16 23:16:56.000000 dailalib-1.1.2/dailalib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-16 23:16:56.000000 dailalib-1.1.2/dailalib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-16 23:16:56.000000 dailalib-1.1.2/dailalib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-16 23:16:56.200838 dailalib-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-16 23:16:45.000000 dailalib-1.1.2/setup.py
```

### Comparing `dailalib-1.0.0/PKG-INFO` & `dailalib-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dailalib
-Version: 1.0.0
+Version: 1.1.2
 Summary: Decompiler Artificial Intelligence Language Assistant
 Home-page: https://github.com/mahaloz/DAILA
 License: BSD 2 Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.5
@@ -15,15 +15,15 @@
 Utilize OpenAI to improve your decompilation experience in most modern decompilers.
 
 ![](./assets/ida_daila.png)
 
 ## Installation
 Clone down this repo and pip install and use the daila installer:
 ```bash
-pip3 install -e . && daila --install 
+pip3 install -e . && dailalib --install 
 ```
 
 Depending on your decompiler, this will attempt to copy the script files into your decompiler and install
 the DAILA core to your current Python. If you are using Binja or IDA, make sure your Python is the same 
 as the one you are using in your decompiler. 
 
 If you are using Ghidra, you may be required to enable the `$USER_HOME/ghidra_scripts` as a valid
```

### Comparing `dailalib-1.0.0/README.md` & `dailalib-1.1.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Utilize OpenAI to improve your decompilation experience in most modern decompilers.
 
 ![](./assets/ida_daila.png)
 
 ## Installation
 Clone down this repo and pip install and use the daila installer:
 ```bash
-pip3 install -e . && daila --install 
+pip3 install -e . && dailalib --install 
 ```
 
 Depending on your decompiler, this will attempt to copy the script files into your decompiler and install
 the DAILA core to your current Python. If you are using Binja or IDA, make sure your Python is the same 
 as the one you are using in your decompiler. 
 
 If you are using Ghidra, you may be required to enable the `$USER_HOME/ghidra_scripts` as a valid
```

### Comparing `dailalib-1.0.0/dailalib/__main__.py` & `dailalib-1.1.2/dailalib/__main__.py`

 * *Files identical despite different names*

### Comparing `dailalib-1.0.0/dailalib/controller_server.py` & `dailalib-1.1.2/dailalib/controller_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from daila.interfaces.openai_interface import OpenAIInterface
+from dailalib.interfaces.openai_interface import OpenAIInterface
 from xmlrpc.server import SimpleXMLRPCServer, SimpleXMLRPCRequestHandler
 from functools import wraps
 
 class RequestHandler(SimpleXMLRPCRequestHandler):
     rpc_paths = ("/RPC2",)
```

### Comparing `dailalib-1.0.0/dailalib/installer.py` & `dailalib-1.1.2/dailalib/installer.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from binsync.installer import Installer
 
 
 class DAILAInstaller(Installer):
     def __init__(self):
         super().__init__(targets=("ida", "ghidra", "binja"))
         self.plugins_path = Path(
-            pkg_resources.resource_filename("daila", f"plugins")
+            pkg_resources.resource_filename("dailalib", f"plugins")
         )
 
     def display_prologue(self):
         print(textwrap.dedent("""
          ▄▄▄▄▄▄▄▄▄▄   ▄▄▄▄▄▄▄▄▄▄▄  ▄▄▄▄▄▄▄▄▄▄▄  ▄            ▄▄▄▄▄▄▄▄▄▄▄ 
         ▐░░░░░░░░░░▌ ▐░░░░░░░░░░░▌▐░░░░░░░░░░░▌▐░▌          ▐░░░░░░░░░░░▌
         ▐░█▀▀▀▀▀▀▀█░▌▐░█▀▀▀▀▀▀▀█░▌ ▀▀▀▀█░█▀▀▀▀ ▐░▌          ▐░█▀▀▀▀▀▀▀█░▌
```

### Comparing `dailalib-1.0.0/dailalib/interfaces/generic_ai_interface.py` & `dailalib-1.1.2/dailalib/interfaces/generic_ai_interface.py`

 * *Files identical despite different names*

### Comparing `dailalib-1.0.0/dailalib/interfaces/openai_interface.py` & `dailalib-1.1.2/dailalib/interfaces/openai_interface.py`

 * *Files identical despite different names*

### Comparing `dailalib-1.0.0/dailalib/utils.py` & `dailalib-1.1.2/dailalib/utils.py`

 * *Files identical despite different names*

### Comparing `dailalib-1.0.0/dailalib.egg-info/PKG-INFO` & `dailalib-1.1.2/dailalib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dailalib
-Version: 1.0.0
+Version: 1.1.2
 Summary: Decompiler Artificial Intelligence Language Assistant
 Home-page: https://github.com/mahaloz/DAILA
 License: BSD 2 Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.5
@@ -15,15 +15,15 @@
 Utilize OpenAI to improve your decompilation experience in most modern decompilers.
 
 ![](./assets/ida_daila.png)
 
 ## Installation
 Clone down this repo and pip install and use the daila installer:
 ```bash
-pip3 install -e . && daila --install 
+pip3 install -e . && dailalib --install 
 ```
 
 Depending on your decompiler, this will attempt to copy the script files into your decompiler and install
 the DAILA core to your current Python. If you are using Binja or IDA, make sure your Python is the same 
 as the one you are using in your decompiler. 
 
 If you are using Ghidra, you may be required to enable the `$USER_HOME/ghidra_scripts` as a valid
```

### Comparing `dailalib-1.0.0/setup.cfg` & `dailalib-1.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `dailalib-1.0.0/setup.py` & `dailalib-1.1.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from setuptools import setup
 from setuptools.command.develop import develop as st_develop
 
 
 def _copy_plugins():
     local_plugins = Path("plugins").absolute()
-    daila_loc = Path("daila").absolute()
+    daila_loc = Path("dailalib").absolute()
     pip_e_plugins = daila_loc.joinpath("plugins").absolute()
 
     # clean the install location of symlink or folder
     shutil.rmtree(pip_e_plugins, ignore_errors=True)
     try:
         os.unlink(pip_e_plugins)
     except:
@@ -28,15 +28,15 @@
         os.symlink(local_plugins, pip_e_plugins, target_is_directory=True)
         return
     except:
         pass
 
     # copy if symlinking is not available on target system
     try:
-        shutil.copytree("plugins", "daila/plugins")
+        shutil.copytree("plugins", "dailalib/plugins")
     except:
         pass
 
 class build(st_build):
     def run(self, *args):
         self.execute(_copy_plugins, (), msg="Copying plugins...")
         super().run(*args)
```

