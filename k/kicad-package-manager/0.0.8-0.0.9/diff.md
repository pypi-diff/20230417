# Comparing `tmp/kicad_package_manager-0.0.8.tar.gz` & `tmp/kicad_package_manager-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kicad_package_manager-0.0.8.tar", last modified: Sun Apr 16 02:49:46 2023, max compression
+gzip compressed data, was "kicad_package_manager-0.0.9.tar", last modified: Sun Apr 16 03:09:34 2023, max compression
```

## Comparing `kicad_package_manager-0.0.8.tar` & `kicad_package_manager-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-16 02:49:46.728020 kicad_package_manager-0.0.8/
--rwxrwxrwx   0 root         (0) root         (0)     3543 2023-04-16 02:49:46.720894 kicad_package_manager-0.0.8/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     2060 2023-04-16 01:54:19.000000 kicad_package_manager-0.0.8/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-16 02:49:46.430459 kicad_package_manager-0.0.8/kicad_package_manager/
--rwxrwxrwx   0 root         (0) root         (0)       14 2023-04-16 02:15:17.000000 kicad_package_manager-0.0.8/kicad_package_manager/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      614 2023-04-16 02:15:17.000000 kicad_package_manager-0.0.8/kicad_package_manager/config.py
--rwxrwxrwx   0 root         (0) root         (0)      479 2023-04-16 02:15:17.000000 kicad_package_manager-0.0.8/kicad_package_manager/init.py
--rwxrwxrwx   0 root         (0) root         (0)     1815 2023-04-16 02:18:30.000000 kicad_package_manager-0.0.8/kicad_package_manager/install.py
--rwxrwxrwx   0 root         (0) root         (0)     1105 2023-04-16 02:17:53.000000 kicad_package_manager-0.0.8/kicad_package_manager/kicad_project_tables.py
--rwxrwxrwx   0 root         (0) root         (0)      842 2023-04-16 02:45:56.000000 kicad_package_manager-0.0.8/kicad_package_manager/kpm.py
--rwxrwxrwx   0 root         (0) root         (0)      358 2023-04-16 02:49:10.000000 kicad_package_manager-0.0.8/kicad_package_manager/listt.py
--rwxrwxrwx   0 root         (0) root         (0)      777 2023-04-16 02:48:10.000000 kicad_package_manager-0.0.8/kicad_package_manager/registry.py
--rwxrwxrwx   0 root         (0) root         (0)      437 2023-04-16 02:46:21.000000 kicad_package_manager-0.0.8/kicad_package_manager/search.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-16 02:49:46.677664 kicad_package_manager-0.0.8/kicad_package_manager.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     3543 2023-04-16 02:49:45.000000 kicad_package_manager-0.0.8/kicad_package_manager.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      591 2023-04-16 02:49:45.000000 kicad_package_manager-0.0.8/kicad_package_manager.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-16 02:49:45.000000 kicad_package_manager-0.0.8/kicad_package_manager.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       56 2023-04-16 02:49:45.000000 kicad_package_manager-0.0.8/kicad_package_manager.egg-info/entry_points.txt
--rwxrwxrwx   0 root         (0) root         (0)       18 2023-04-16 02:49:45.000000 kicad_package_manager-0.0.8/kicad_package_manager.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       22 2023-04-16 02:49:45.000000 kicad_package_manager-0.0.8/kicad_package_manager.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-16 02:49:46.730759 kicad_package_manager-0.0.8/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     3832 2023-04-16 02:49:26.000000 kicad_package_manager-0.0.8/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-16 03:09:34.428656 kicad_package_manager-0.0.9/
+-rwxrwxrwx   0 root         (0) root         (0)     3543 2023-04-16 03:09:34.426653 kicad_package_manager-0.0.9/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     2060 2023-04-16 01:54:19.000000 kicad_package_manager-0.0.9/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-16 03:09:34.310486 kicad_package_manager-0.0.9/kicad_package_manager/
+-rwxrwxrwx   0 root         (0) root         (0)       14 2023-04-16 02:15:17.000000 kicad_package_manager-0.0.9/kicad_package_manager/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      614 2023-04-16 02:15:17.000000 kicad_package_manager-0.0.9/kicad_package_manager/config.py
+-rwxrwxrwx   0 root         (0) root         (0)      479 2023-04-16 02:15:17.000000 kicad_package_manager-0.0.9/kicad_package_manager/init.py
+-rwxrwxrwx   0 root         (0) root         (0)     1815 2023-04-16 02:18:30.000000 kicad_package_manager-0.0.9/kicad_package_manager/install.py
+-rwxrwxrwx   0 root         (0) root         (0)     1026 2023-04-16 03:08:39.000000 kicad_package_manager-0.0.9/kicad_package_manager/kicad_project_tables.py
+-rwxrwxrwx   0 root         (0) root         (0)      842 2023-04-16 02:45:56.000000 kicad_package_manager-0.0.9/kicad_package_manager/kpm.py
+-rwxrwxrwx   0 root         (0) root         (0)      358 2023-04-16 02:49:10.000000 kicad_package_manager-0.0.9/kicad_package_manager/listt.py
+-rwxrwxrwx   0 root         (0) root         (0)      777 2023-04-16 02:48:10.000000 kicad_package_manager-0.0.9/kicad_package_manager/registry.py
+-rwxrwxrwx   0 root         (0) root         (0)      437 2023-04-16 02:46:21.000000 kicad_package_manager-0.0.9/kicad_package_manager/search.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-16 03:09:34.408223 kicad_package_manager-0.0.9/kicad_package_manager.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     3543 2023-04-16 03:09:33.000000 kicad_package_manager-0.0.9/kicad_package_manager.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      591 2023-04-16 03:09:34.000000 kicad_package_manager-0.0.9/kicad_package_manager.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-16 03:09:33.000000 kicad_package_manager-0.0.9/kicad_package_manager.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       56 2023-04-16 03:09:33.000000 kicad_package_manager-0.0.9/kicad_package_manager.egg-info/entry_points.txt
+-rwxrwxrwx   0 root         (0) root         (0)       18 2023-04-16 03:09:33.000000 kicad_package_manager-0.0.9/kicad_package_manager.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       22 2023-04-16 03:09:33.000000 kicad_package_manager-0.0.9/kicad_package_manager.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-16 03:09:34.429654 kicad_package_manager-0.0.9/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     3832 2023-04-16 03:09:31.000000 kicad_package_manager-0.0.9/setup.py
```

### Comparing `kicad_package_manager-0.0.8/PKG-INFO` & `kicad_package_manager-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kicad_package_manager
-Version: 0.0.8
+Version: 0.0.9
 Summary: A package manager for KiCad projects
 Home-page: https://github.com/danroblewis/kicad-package-manager
 Author: Daniel Lewis
 Author-email: daniel.robert.lewis@gmail.com
 License: MIT
 Description: 
         # KiCad Package Manager
```

### Comparing `kicad_package_manager-0.0.8/README.md` & `kicad_package_manager-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `kicad_package_manager-0.0.8/kicad_package_manager/config.py` & `kicad_package_manager-0.0.9/kicad_package_manager/config.py`

 * *Files identical despite different names*

### Comparing `kicad_package_manager-0.0.8/kicad_package_manager/install.py` & `kicad_package_manager-0.0.9/kicad_package_manager/install.py`

 * *Files identical despite different names*

### Comparing `kicad_package_manager-0.0.8/kicad_package_manager/kicad_project_tables.py` & `kicad_package_manager-0.0.9/kicad_package_manager/kicad_project_tables.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import sexpdata
 from sexpdata import Symbol
+import ntpath
 import os
-import re
 
 
 def write_sym_lib_table(files):
 	print("writing sym")
 	s = [ Symbol('sym_lib_table'), [ Symbol('version'), 7 ] ]
 	for path in files:
-		print(path)
-		name = re.match(".*[\\/]([^\\/]+\.kicad_sym).*", path).group(1)[:-10]
-		print(name)
+		fname = ntpath.basename(path)
+		name = fname.replace(".kicad_sym", "")
 		s.append([
 			Symbol('lib'),
 			[ Symbol('name'), name ],
 			[ Symbol('type'), 'KiCad' ],
 			[ Symbol('uri'), os.path.join('${KIPRJMOD}', path) ],
 			[ Symbol('options'), '' ],
 			[ Symbol('descr'), '' ],
@@ -23,18 +22,16 @@
 		sexpdata.dump(s, f)
 
 
 def write_fp_lib_table(files):
 	print("writing foot")
 	s = [ Symbol('fp_lib_table'), [ Symbol('version'), 7 ] ]
 	for path in files:
-		print(path)
-		name = re.match(".*[\\/]([^\\/]+\.pretty).*", path).group(1)[:-7]
-		name.replace(".pretty", "")
-		print(name)
+		fname = ntpath.basename(path)
+		name = fname.replace(".pretty", "")
 		s.append([
 			Symbol('lib'),
 			[ Symbol('name'), name ],
 			[ Symbol('type'), 'KiCad' ],
 			[ Symbol('uri'), os.path.join('${KIPRJMOD}', path) ],
 			[ Symbol('options'), '' ],
 			[ Symbol('descr'), '' ],
```

### Comparing `kicad_package_manager-0.0.8/kicad_package_manager/kpm.py` & `kicad_package_manager-0.0.9/kicad_package_manager/kpm.py`

 * *Files identical despite different names*

### Comparing `kicad_package_manager-0.0.8/kicad_package_manager/registry.py` & `kicad_package_manager-0.0.9/kicad_package_manager/registry.py`

 * *Files identical despite different names*

### Comparing `kicad_package_manager-0.0.8/kicad_package_manager.egg-info/PKG-INFO` & `kicad_package_manager-0.0.9/kicad_package_manager.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kicad-package-manager
-Version: 0.0.8
+Version: 0.0.9
 Summary: A package manager for KiCad projects
 Home-page: https://github.com/danroblewis/kicad-package-manager
 Author: Daniel Lewis
 Author-email: daniel.robert.lewis@gmail.com
 License: MIT
 Description: 
         # KiCad Package Manager
```

### Comparing `kicad_package_manager-0.0.8/kicad_package_manager.egg-info/SOURCES.txt` & `kicad_package_manager-0.0.9/kicad_package_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kicad_package_manager-0.0.8/setup.py` & `kicad_package_manager-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'kicad_package_manager'
 DESCRIPTION = 'A package manager for KiCad projects'
 URL = 'https://github.com/danroblewis/kicad-package-manager'
 EMAIL = 'daniel.robert.lewis@gmail.com'
 AUTHOR = 'Daniel Lewis'
 REQUIRES_PYTHON = '>=3.7.0'
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'requests',
     'sexpdata'
 ]
```

