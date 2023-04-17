# Comparing `tmp/gspm-0.1.8.tar.gz` & `tmp/gspm-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\gspm-0.1.8.tar", last modified: Sun Jan 27 05:38:37 2019, max compression
+gzip compressed data, was "dist\gspm-0.1.9.tar", last modified: Mon Apr 15 04:51:11 2019, max compression
```

## Comparing `gspm-0.1.8.tar` & `gspm-0.1.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2019-01-27 05:38:37.000000 gspm-0.1.8/
--rw-rw-rw-   0        0        0      146 2018-10-08 16:28:56.000000 gspm-0.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0     1758 2019-01-27 05:38:37.000000 gspm-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      669 2018-12-22 23:34:01.000000 gspm-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2019-01-27 05:38:37.000000 gspm-0.1.8/gspm/
--rw-rw-rw-   0        0        0      405 2019-01-27 05:36:27.000000 gspm-0.1.8/gspm/__init__.py
--rw-rw-rw-   0        0        0       76 2018-10-17 05:11:40.000000 gspm-0.1.8/gspm/__main__.py
-drwxrwxrwx   0        0        0        0 2019-01-27 05:38:37.000000 gspm-0.1.8/gspm/commands/
--rw-rw-rw-   0        0        0        0 2018-11-11 17:29:33.000000 gspm-0.1.8/gspm/commands/__init__.py
--rw-rw-rw-   0        0        0        0 2018-10-16 00:20:42.000000 gspm-0.1.8/gspm/commands/clean.py
--rw-rw-rw-   0        0        0      596 2018-10-27 04:30:08.000000 gspm-0.1.8/gspm/commands/edit.py
--rw-rw-rw-   0        0        0     2969 2018-10-26 11:57:34.000000 gspm-0.1.8/gspm/commands/install.py
--rw-rw-rw-   0        0        0     5521 2018-12-22 18:26:00.000000 gspm-0.1.8/gspm/commands/new.py
--rw-rw-rw-   0        0        0      580 2018-12-22 21:20:27.000000 gspm-0.1.8/gspm/commands/run.py
--rw-rw-rw-   0        0        0     1247 2018-12-27 22:07:31.000000 gspm-0.1.8/gspm/commands/update.py
--rw-rw-rw-   0        0        0       69 2018-10-08 22:18:18.000000 gspm-0.1.8/gspm/config.py
--rw-rw-rw-   0        0        0     1944 2018-12-23 00:17:55.000000 gspm-0.1.8/gspm/gspm.py
--rw-rw-rw-   0        0        0     1641 2018-12-27 18:25:02.000000 gspm-0.1.8/gspm/parser.py
--rw-rw-rw-   0        0        0     3357 2018-12-29 21:29:05.000000 gspm-0.1.8/gspm/project.py
-drwxrwxrwx   0        0        0        0 2019-01-27 05:38:37.000000 gspm-0.1.8/gspm/utils/
--rw-rw-rw-   0        0        0        0 2018-10-09 04:18:56.000000 gspm-0.1.8/gspm/utils/__init__.py
--rw-rw-rw-   0        0        0     3274 2018-12-27 23:36:08.000000 gspm-0.1.8/gspm/utils/asset_utils.py
--rw-rw-rw-   0        0        0      322 2018-10-16 03:34:54.000000 gspm-0.1.8/gspm/utils/git_utils.py
--rw-rw-rw-   0        0        0     8309 2018-12-23 01:13:42.000000 gspm-0.1.8/gspm/utils/godot_utils.py
--rw-rw-rw-   0        0        0     1593 2018-12-22 23:16:54.000000 gspm-0.1.8/gspm/utils/path_utils.py
--rw-rw-rw-   0        0        0      365 2018-11-11 15:53:34.000000 gspm-0.1.8/gspm/utils/process_utils.py
-drwxrwxrwx   0        0        0        0 2019-01-27 05:38:37.000000 gspm-0.1.8/gspm.egg-info/
--rw-rw-rw-   0        0        0     1758 2019-01-27 05:38:36.000000 gspm-0.1.8/gspm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      647 2019-01-27 05:38:36.000000 gspm-0.1.8/gspm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2019-01-27 05:38:36.000000 gspm-0.1.8/gspm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2019-01-27 05:38:36.000000 gspm-0.1.8/gspm.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       39 2019-01-27 05:38:36.000000 gspm-0.1.8/gspm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2019-01-27 05:38:36.000000 gspm-0.1.8/gspm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2018-10-08 22:15:13.000000 gspm-0.1.8/gspm.egg-info/zip-safe
--rw-rw-rw-   0        0        0       64 2018-10-28 03:58:18.000000 gspm-0.1.8/requirements.txt
--rw-rw-rw-   0        0        0       42 2019-01-27 05:38:37.000000 gspm-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1677 2018-12-21 20:14:26.000000 gspm-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2019-04-15 04:51:11.000000 gspm-0.1.9/
+-rw-rw-rw-   0        0        0      146 2019-04-15 04:29:58.000000 gspm-0.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     1758 2019-04-15 04:51:11.000000 gspm-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      669 2019-04-15 04:29:58.000000 gspm-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2019-04-15 04:51:11.000000 gspm-0.1.9/gspm/
+-rw-rw-rw-   0        0        0      405 2019-04-15 04:29:58.000000 gspm-0.1.9/gspm/__init__.py
+-rw-rw-rw-   0        0        0       76 2019-04-15 04:29:58.000000 gspm-0.1.9/gspm/__main__.py
+drwxrwxrwx   0        0        0        0 2019-04-15 04:51:11.000000 gspm-0.1.9/gspm/commands/
+-rw-rw-rw-   0        0        0        0 2019-04-15 04:29:58.000000 gspm-0.1.9/gspm/commands/__init__.py
+-rw-rw-rw-   0        0        0        0 2019-04-15 04:29:58.000000 gspm-0.1.9/gspm/commands/clean.py
+-rw-rw-rw-   0        0        0      596 2019-04-15 04:29:58.000000 gspm-0.1.9/gspm/commands/edit.py
+-rw-rw-rw-   0        0        0     2969 2019-04-15 04:29:58.000000 gspm-0.1.9/gspm/commands/install.py
+-rw-rw-rw-   0        0        0     5521 2019-04-15 04:29:58.000000 gspm-0.1.9/gspm/commands/new.py
+-rw-rw-rw-   0        0        0      580 2019-04-15 04:35:45.000000 gspm-0.1.9/gspm/commands/run.py
+-rw-rw-rw-   0        0        0     1247 2019-04-15 04:29:58.000000 gspm-0.1.9/gspm/commands/update.py
+-rw-rw-rw-   0        0        0       69 2019-04-15 04:29:58.000000 gspm-0.1.9/gspm/config.py
+-rw-rw-rw-   0        0        0     1946 2019-04-15 04:35:54.000000 gspm-0.1.9/gspm/gspm.py
+-rw-rw-rw-   0        0        0     1641 2019-04-15 04:29:58.000000 gspm-0.1.9/gspm/parser.py
+-rw-rw-rw-   0        0        0     3357 2019-04-15 04:29:58.000000 gspm-0.1.9/gspm/project.py
+drwxrwxrwx   0        0        0        0 2019-04-15 04:51:11.000000 gspm-0.1.9/gspm/utils/
+-rw-rw-rw-   0        0        0        0 2019-04-15 04:29:58.000000 gspm-0.1.9/gspm/utils/__init__.py
+-rw-rw-rw-   0        0        0     3274 2019-04-15 04:29:58.000000 gspm-0.1.9/gspm/utils/asset_utils.py
+-rw-rw-rw-   0        0        0      322 2019-04-15 04:29:58.000000 gspm-0.1.9/gspm/utils/git_utils.py
+-rw-rw-rw-   0        0        0     8310 2019-04-15 04:45:25.000000 gspm-0.1.9/gspm/utils/godot_utils.py
+-rw-rw-rw-   0        0        0     1593 2019-04-15 04:29:58.000000 gspm-0.1.9/gspm/utils/path_utils.py
+-rw-rw-rw-   0        0        0      365 2019-04-15 04:29:58.000000 gspm-0.1.9/gspm/utils/process_utils.py
+drwxrwxrwx   0        0        0        0 2019-04-15 04:51:11.000000 gspm-0.1.9/gspm.egg-info/
+-rw-rw-rw-   0        0        0     1758 2019-04-15 04:51:09.000000 gspm-0.1.9/gspm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      647 2019-04-15 04:51:09.000000 gspm-0.1.9/gspm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2019-04-15 04:51:09.000000 gspm-0.1.9/gspm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2019-04-15 04:51:09.000000 gspm-0.1.9/gspm.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       39 2019-04-15 04:51:09.000000 gspm-0.1.9/gspm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2019-04-15 04:51:09.000000 gspm-0.1.9/gspm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2019-04-15 04:30:18.000000 gspm-0.1.9/gspm.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       64 2019-04-15 04:29:58.000000 gspm-0.1.9/requirements.txt
+-rw-rw-rw-   0        0        0       42 2019-04-15 04:51:11.000000 gspm-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1677 2019-04-15 04:29:58.000000 gspm-0.1.9/setup.py
```

### Comparing `gspm-0.1.8/PKG-INFO` & `gspm-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gspm
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Command Line Utility to Assist in Managing your GODOT projects.
 Home-page: https://gitlab.com/godot-stuff/gs-project-manager.git
 Author: Paul Hocker
 Author-email: paul@spocker.net
 License: MIT
 Description: A tool to assist you in managing the assets used in your Godot projects.
```

### Comparing `gspm-0.1.8/README.md` & `gspm-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `gspm-0.1.8/gspm/commands/edit.py` & `gspm-0.1.9/gspm/commands/edit.py`

 * *Files identical despite different names*

### Comparing `gspm-0.1.8/gspm/commands/install.py` & `gspm-0.1.9/gspm/commands/install.py`

 * *Files identical despite different names*

### Comparing `gspm-0.1.8/gspm/commands/new.py` & `gspm-0.1.9/gspm/commands/new.py`

 * *Files identical despite different names*

### Comparing `gspm-0.1.8/gspm/commands/run.py` & `gspm-0.1.9/gspm/commands/run.py`

 * *Files identical despite different names*

### Comparing `gspm-0.1.8/gspm/commands/update.py` & `gspm-0.1.9/gspm/commands/update.py`

 * *Files identical despite different names*

### Comparing `gspm-0.1.8/gspm/gspm.py` & `gspm-0.1.9/gspm/gspm.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 import gspm.parser as parser
 import gspm.project as project
 import gspm.utils.path_utils as path_utils
 
 
 def _get_logging_level():
-    return logging.DEBUG
+    return logging.WARNING
 
 
 def init():
     '''
     Initialize the Environment
 
     Used to setup the Logging Environment and
```

### Comparing `gspm-0.1.8/gspm/parser.py` & `gspm-0.1.9/gspm/parser.py`

 * *Files identical despite different names*

### Comparing `gspm-0.1.8/gspm/project.py` & `gspm-0.1.9/gspm/project.py`

 * *Files identical despite different names*

### Comparing `gspm-0.1.8/gspm/utils/asset_utils.py` & `gspm-0.1.9/gspm/utils/asset_utils.py`

 * *Files identical despite different names*

### Comparing `gspm-0.1.8/gspm/utils/godot_utils.py` & `gspm-0.1.9/gspm/utils/godot_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -112,15 +112,15 @@
 
 def _build_windows_uri(project):
 
     logging.debug("[godot_utils] _build_windows_uri")
 
     stable = 'stable'
 
-    if Version('{0}'.format(project.config.godot.version)) < Version('3.1'):
+    if Version('{0}'.format(project.config.godot.version)) < Version('3.2'):
         host = host_url.format(project.config.godot.version)
     else:
         host = host_url.format("{0}".format(project.config.godot.version) + "/alpha1")
         stable = 'alpha1'
 
     if Version('{0}'.format(project.config.godot.version)) < Version("2.1"):
         template = "{2}Godot_v{0}_{3}_win{1}.exe.zip"
@@ -133,15 +133,15 @@
 
 def _build_darwin_uri(project):
 
     logging.debug("[godot_utils] _build_darwin_uri")
 
     stable = 'stable'
 
-    if Version('{0}'.format(project.config.godot.version)) < Version('3.1'):
+    if Version('{0}'.format(project.config.godot.version)) < Version('3.2'):
         host = host_url.format(project.config.godot.version)
     else:
         host = host_url.format("{0}".format(project.config.godot.version) + "/alpha1")
         stable = 'alpha1'
 
     if Version('{0}'.format(project.config.godot.version)) < Version("2.1"):
         template = "{2}Godot_v{0}_{3}_osx.fat.zip"
@@ -154,15 +154,15 @@
 
 def _build_linux_uri(project):
 
     logging.debug("[godot_utils] _build_linux_uri")
 
     stable = 'stable'
 
-    if Version('{0}'.format(project.config.godot.version)) < Version('3.1'):
+    if Version('{0}'.format(project.config.godot.version)) < Version('3.2'):
         host = host_url.format(project.config.godot.version)
     else:
         host = host_url.format("{0}".format(project.config.godot.version) + "/alpha1")
         stable = 'alpha1'
 
     if Version('{0}'.format(project.config.godot.version)) < Version("2.1"):
         template = "{2}Godot_v{0}_{3}_x11.{1}.zip"
@@ -210,15 +210,15 @@
     proj_path = os.path.abspath(project.project_path)
 
     if project.config.godot.location:
         cmd = "{0} --path {1}".format(os.path.abspath(project.config.godot.location), proj_path)
     else:
         godot_path = os.path.abspath("{0}/godot-{1}/".format(project.repository_home, project.config.godot.version))
         cmd = "arch -{3} {0}/{1} --path {2}".format(godot_path, _get_godot_runtime(project), proj_path, project.config.godot.arch)
-        logger.debug(cmd)
+        logging.debug(cmd)
 
     return cmd
 
 
 #   return the platform we are running on
 def _get_platform():
     return platform.system().lower()
@@ -241,26 +241,26 @@
         raise Exception("Platform [{0}] Not Supported".format(plat))
 
     return runtime
 
 
 def _get_windows_runtime(project):
     logging.debug('[godot_utils] _get_windows_runtime')
-    if Version('{0}'.format(project.config.godot.version)) < Version('3.1'):
+    if Version('{0}'.format(project.config.godot.version)) < Version('3.2'):
         stable = 'stable'
     else:
         stable = 'alpha1'
 
     runtime = "Godot_v{0}-{2}_win{1}.exe".format(project.config.godot.version, project.config.godot.arch, stable)
     return runtime
 
 
 def _get_linux_runtime(project):
     logging.debug('[godot_utils] _get_linux_runtime')
-    if Version('{0}'.format(project.config.godot.version)) < Version('3.1'):
+    if Version('{0}'.format(project.config.godot.version)) < Version('3.2'):
         stable = 'stable'
     else:
         stable = 'alpha1'
 
     runtime = "Godot_v{0}-{2}_x11.{1}".format(project.config.godot.version, project.config.godot.arch, stable)
     return runtime
```

### Comparing `gspm-0.1.8/gspm/utils/path_utils.py` & `gspm-0.1.9/gspm/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `gspm-0.1.8/gspm.egg-info/PKG-INFO` & `gspm-0.1.9/gspm.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gspm
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Command Line Utility to Assist in Managing your GODOT projects.
 Home-page: https://gitlab.com/godot-stuff/gs-project-manager.git
 Author: Paul Hocker
 Author-email: paul@spocker.net
 License: MIT
 Description: A tool to assist you in managing the assets used in your Godot projects.
```

### Comparing `gspm-0.1.8/gspm.egg-info/SOURCES.txt` & `gspm-0.1.9/gspm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gspm-0.1.8/setup.py` & `gspm-0.1.9/setup.py`

 * *Files identical despite different names*

