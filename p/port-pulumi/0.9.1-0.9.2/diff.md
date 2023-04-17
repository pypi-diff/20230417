# Comparing `tmp/port_pulumi-0.9.1.tar.gz` & `tmp/port_pulumi-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "port_pulumi-0.9.1.tar", last modified: Sun Apr 16 11:13:59 2023, max compression
+gzip compressed data, was "port_pulumi-0.9.2.tar", last modified: Mon Apr 17 09:23:31 2023, max compression
```

## Comparing `port_pulumi-0.9.1.tar` & `port_pulumi-0.9.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:13:59.378078 port_pulumi-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-16 11:13:59.378078 port_pulumi-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-16 11:13:59.000000 port_pulumi-0.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:13:59.378078 port_pulumi-0.9.1/port_pulumi/
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-16 11:13:59.000000 port_pulumi-0.9.1/port_pulumi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25197 2023-04-16 11:13:59.000000 port_pulumi-0.9.1/port_pulumi/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-04-16 11:13:59.000000 port_pulumi-0.9.1/port_pulumi/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    20405 2023-04-16 11:13:59.000000 port_pulumi-0.9.1/port_pulumi/action.py
--rw-r--r--   0 runner    (1001) docker     (123)    31433 2023-04-16 11:13:59.000000 port_pulumi-0.9.1/port_pulumi/blueprint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:13:59.378078 port_pulumi-0.9.1/port_pulumi/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-16 11:13:59.000000 port_pulumi-0.9.1/port_pulumi/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-16 11:13:59.000000 port_pulumi-0.9.1/port_pulumi/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    22419 2023-04-16 11:13:59.000000 port_pulumi-0.9.1/port_pulumi/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    17723 2023-04-16 11:13:59.000000 port_pulumi-0.9.1/port_pulumi/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-04-16 11:13:59.000000 port_pulumi-0.9.1/port_pulumi/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-16 11:13:59.000000 port_pulumi-0.9.1/port_pulumi/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 11:13:59.000000 port_pulumi-0.9.1/port_pulumi/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:13:59.378078 port_pulumi-0.9.1/port_pulumi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-16 11:13:59.000000 port_pulumi-0.9.1/port_pulumi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-16 11:13:59.000000 port_pulumi-0.9.1/port_pulumi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 11:13:59.000000 port_pulumi-0.9.1/port_pulumi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 11:13:59.000000 port_pulumi-0.9.1/port_pulumi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-16 11:13:59.000000 port_pulumi-0.9.1/port_pulumi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-16 11:13:59.000000 port_pulumi-0.9.1/port_pulumi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 11:13:59.378078 port_pulumi-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-16 11:13:59.000000 port_pulumi-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:23:31.967380 port_pulumi-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-17 09:23:31.967380 port_pulumi-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-17 09:23:31.000000 port_pulumi-0.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:23:31.963379 port_pulumi-0.9.2/port_pulumi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-17 09:23:31.000000 port_pulumi-0.9.2/port_pulumi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25197 2023-04-17 09:23:31.000000 port_pulumi-0.9.2/port_pulumi/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-04-17 09:23:31.000000 port_pulumi-0.9.2/port_pulumi/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20405 2023-04-17 09:23:31.000000 port_pulumi-0.9.2/port_pulumi/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31433 2023-04-17 09:23:31.000000 port_pulumi-0.9.2/port_pulumi/blueprint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:23:31.967380 port_pulumi-0.9.2/port_pulumi/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-17 09:23:31.000000 port_pulumi-0.9.2/port_pulumi/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-17 09:23:31.000000 port_pulumi-0.9.2/port_pulumi/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22419 2023-04-17 09:23:31.000000 port_pulumi-0.9.2/port_pulumi/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17723 2023-04-17 09:23:31.000000 port_pulumi-0.9.2/port_pulumi/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-04-17 09:23:31.000000 port_pulumi-0.9.2/port_pulumi/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-17 09:23:31.000000 port_pulumi-0.9.2/port_pulumi/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 09:23:31.000000 port_pulumi-0.9.2/port_pulumi/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:23:31.967380 port_pulumi-0.9.2/port_pulumi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-17 09:23:31.000000 port_pulumi-0.9.2/port_pulumi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-17 09:23:31.000000 port_pulumi-0.9.2/port_pulumi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 09:23:31.000000 port_pulumi-0.9.2/port_pulumi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 09:23:31.000000 port_pulumi-0.9.2/port_pulumi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-17 09:23:31.000000 port_pulumi-0.9.2/port_pulumi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-17 09:23:31.000000 port_pulumi-0.9.2/port_pulumi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 09:23:31.967380 port_pulumi-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-17 09:23:31.000000 port_pulumi-0.9.2/setup.py
```

### Comparing `port_pulumi-0.9.1/PKG-INFO` & `port_pulumi-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: port_pulumi
-Version: 0.9.1
+Version: 0.9.2
 Summary: A Pulumi package for creating and managing Port resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/port-labs/pulumi
 Keywords: pulumi port category/utility
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `port_pulumi-0.9.1/README.md` & `port_pulumi-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `port_pulumi-0.9.1/port_pulumi/__init__.py` & `port_pulumi-0.9.2/port_pulumi/__init__.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-0.9.1/port_pulumi/_inputs.py` & `port_pulumi-0.9.2/port_pulumi/_inputs.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-0.9.1/port_pulumi/_utilities.py` & `port_pulumi-0.9.2/port_pulumi/_utilities.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-0.9.1/port_pulumi/action.py` & `port_pulumi-0.9.2/port_pulumi/action.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-0.9.1/port_pulumi/blueprint.py` & `port_pulumi-0.9.2/port_pulumi/blueprint.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-0.9.1/port_pulumi/config/vars.py` & `port_pulumi-0.9.2/port_pulumi/config/vars.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-0.9.1/port_pulumi/entity.py` & `port_pulumi-0.9.2/port_pulumi/entity.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-0.9.1/port_pulumi/outputs.py` & `port_pulumi-0.9.2/port_pulumi/outputs.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-0.9.1/port_pulumi/provider.py` & `port_pulumi-0.9.2/port_pulumi/provider.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-0.9.1/port_pulumi.egg-info/PKG-INFO` & `port_pulumi-0.9.2/port_pulumi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: port-pulumi
-Version: 0.9.1
+Version: 0.9.2
 Summary: A Pulumi package for creating and managing Port resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/port-labs/pulumi
 Keywords: pulumi port category/utility
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `port_pulumi-0.9.1/port_pulumi.egg-info/SOURCES.txt` & `port_pulumi-0.9.2/port_pulumi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `port_pulumi-0.9.1/setup.py` & `port_pulumi-0.9.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.9.1"
-PLUGIN_VERSION = "0.9.1"
+VERSION = "0.9.2"
+PLUGIN_VERSION = "0.9.2"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'port', PLUGIN_VERSION, '--server', 'github://api.github.com/port-labs/pulumi'])
         except OSError as error:
```

