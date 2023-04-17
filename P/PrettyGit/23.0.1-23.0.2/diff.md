# Comparing `tmp/prettygit-23.0.1.tar.gz` & `tmp/prettygit-23.0.2.tar.gz`

## Comparing `prettygit-23.0.1.tar` & `prettygit-23.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 prettygit-23.0.1/build.sh
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 prettygit-23.0.1/changelog.md
--rwxr-xr-x   0        0        0      112 2020-02-02 00:00:00.000000 prettygit-23.0.1/start.sh
--rw-r--r--   0        0        0   151771 2020-02-02 00:00:00.000000 prettygit-23.0.1/img/filled.png
--rw-r--r--   0        0        0     5606 2020-02-02 00:00:00.000000 prettygit-23.0.1/img/filled.svg
--rw-r--r--   0        0        0    57741 2020-02-02 00:00:00.000000 prettygit-23.0.1/img/transparent.png
--rwxr-xr-x   0        0        0     6099 2020-02-02 00:00:00.000000 prettygit-23.0.1/img/transparent.svg
--rwxr-xr-x   0        0        0     1196 2020-02-02 00:00:00.000000 prettygit-23.0.1/launcher/prettygit.bat
--rwxr-xr-x   0        0        0      890 2020-02-02 00:00:00.000000 prettygit-23.0.1/launcher/prettygit.sh
--rwxr-xr-x   0        0        0     2573 2020-02-02 00:00:00.000000 prettygit-23.0.1/launcher/prettygit_win.py
--rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 prettygit-23.0.1/prettygit/__init__.py
--rwxr-xr-x   0        0        0      202 2020-02-02 00:00:00.000000 prettygit-23.0.1/prettygit/__main__.py
--rwxr-xr-x   0        0        0    15198 2020-02-02 00:00:00.000000 prettygit-23.0.1/prettygit/main.py
--rwxr-xr-x   0        0        0     4271 2020-02-02 00:00:00.000000 prettygit-23.0.1/prettygit/setup.py
--rw-r--r--   0        0        0    10405 2020-02-02 00:00:00.000000 prettygit-23.0.1/prettygit/icons/icon.ico
--rwxr-xr-x   0        0        0     3242 2020-02-02 00:00:00.000000 prettygit-23.0.1/prettygit/icons/icon.svg
--rwxr-xr-x   0        0        0       22 2020-02-02 00:00:00.000000 prettygit-23.0.1/.gitignore
--rwxr-xr-x   0        0        0      786 2020-02-02 00:00:00.000000 prettygit-23.0.1/pyproject.toml
--rwxr-xr-x   0        0        0     1691 2020-02-02 00:00:00.000000 prettygit-23.0.1/readme.md
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 prettygit-23.0.1/PKG-INFO
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 prettygit-23.0.2/build.sh
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 prettygit-23.0.2/changelog.md
+-rwxr-xr-x   0        0        0      112 2020-02-02 00:00:00.000000 prettygit-23.0.2/start.sh
+-rw-r--r--   0        0        0   151771 2020-02-02 00:00:00.000000 prettygit-23.0.2/img/filled.png
+-rw-r--r--   0        0        0     5606 2020-02-02 00:00:00.000000 prettygit-23.0.2/img/filled.svg
+-rw-r--r--   0        0        0    57741 2020-02-02 00:00:00.000000 prettygit-23.0.2/img/transparent.png
+-rwxr-xr-x   0        0        0     6099 2020-02-02 00:00:00.000000 prettygit-23.0.2/img/transparent.svg
+-rwxr-xr-x   0        0        0     1196 2020-02-02 00:00:00.000000 prettygit-23.0.2/launcher/prettygit.bat
+-rwxr-xr-x   0        0        0      890 2020-02-02 00:00:00.000000 prettygit-23.0.2/launcher/prettygit.sh
+-rwxr-xr-x   0        0        0     2573 2020-02-02 00:00:00.000000 prettygit-23.0.2/launcher/prettygit_win.py
+-rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 prettygit-23.0.2/prettygit/__init__.py
+-rwxr-xr-x   0        0        0      202 2020-02-02 00:00:00.000000 prettygit-23.0.2/prettygit/__main__.py
+-rwxr-xr-x   0        0        0    15198 2020-02-02 00:00:00.000000 prettygit-23.0.2/prettygit/main.py
+-rwxr-xr-x   0        0        0     4271 2020-02-02 00:00:00.000000 prettygit-23.0.2/prettygit/setup.py
+-rw-r--r--   0        0        0    10405 2020-02-02 00:00:00.000000 prettygit-23.0.2/prettygit/icons/icon.ico
+-rwxr-xr-x   0        0        0     3242 2020-02-02 00:00:00.000000 prettygit-23.0.2/prettygit/icons/icon.svg
+-rwxr-xr-x   0        0        0       22 2020-02-02 00:00:00.000000 prettygit-23.0.2/.gitignore
+-rwxr-xr-x   0        0        0      786 2020-02-02 00:00:00.000000 prettygit-23.0.2/pyproject.toml
+-rwxr-xr-x   0        0        0     1691 2020-02-02 00:00:00.000000 prettygit-23.0.2/readme.md
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 prettygit-23.0.2/PKG-INFO
```

### Comparing `prettygit-23.0.1/img/filled.png` & `prettygit-23.0.2/img/filled.png`

 * *Files identical despite different names*

### Comparing `prettygit-23.0.1/img/filled.svg` & `prettygit-23.0.2/img/filled.svg`

 * *Files identical despite different names*

### Comparing `prettygit-23.0.1/img/transparent.png` & `prettygit-23.0.2/img/transparent.png`

 * *Files identical despite different names*

### Comparing `prettygit-23.0.1/img/transparent.svg` & `prettygit-23.0.2/img/transparent.svg`

 * *Files identical despite different names*

### Comparing `prettygit-23.0.1/launcher/prettygit.bat` & `prettygit-23.0.2/launcher/prettygit.bat`

 * *Files identical despite different names*

### Comparing `prettygit-23.0.1/launcher/prettygit.sh` & `prettygit-23.0.2/launcher/prettygit.sh`

 * *Files identical despite different names*

### Comparing `prettygit-23.0.1/launcher/prettygit_win.py` & `prettygit-23.0.2/launcher/prettygit_win.py`

 * *Files identical despite different names*

### Comparing `prettygit-23.0.1/prettygit/main.py` & `prettygit-23.0.2/prettygit/main.py`

 * *Files identical despite different names*

### Comparing `prettygit-23.0.1/prettygit/setup.py` & `prettygit-23.0.2/prettygit/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import shutil as sh
 import subprocess as sp
 import platform
 import rich
 import sys
 import os
 
-app_version = '22.1.4'
+app_version = '23.0.2'
 app_name = 'prettygit'
 proj_path = Path(__file__).parent.resolve()
 modules_path = Path(__file__).parent.parent.resolve()
 c = rich.console.Console()
 print = c.print
 win_py_file = Path(f'{modules_path}/{app_name}_win.py')
 portable = win_py_file.exists()
```

### Comparing `prettygit-23.0.1/prettygit/icons/icon.ico` & `prettygit-23.0.2/prettygit/icons/icon.ico`

 * *Files identical despite different names*

### Comparing `prettygit-23.0.1/prettygit/icons/icon.svg` & `prettygit-23.0.2/prettygit/icons/icon.svg`

 * *Files identical despite different names*

### Comparing `prettygit-23.0.1/pyproject.toml` & `prettygit-23.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 dependencies = [
   "gmanka_yml==23.0.0",
   "easyselect==23.0.0",
-  "betterdata==23.0.0",
+  "betterdata==23.0.1",
   "hatchling",
   "twine",
   "rich",
 ]
 name = "PrettyGit"
-version = "23.0.1"
+version = "23.0.2"
 authors = [
   { name="gmanka", email="gmankab@gmail.com" },
 ]
 description = "very simple and user friendly interface for git"
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `prettygit-23.0.1/readme.md` & `prettygit-23.0.2/readme.md`

 * *Files identical despite different names*

### Comparing `prettygit-23.0.1/PKG-INFO` & `prettygit-23.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: PrettyGit
-Version: 23.0.1
+Version: 23.0.2
 Summary: very simple and user friendly interface for git
 Project-URL: Homepage, https://github.com/gmankab/PrettyGit
 Project-URL: Bug Tracker, https://github.com/gmankab/PrettyGit/issues
 Project-URL: Documentation, https://github.com/gmankab/PrettyGit
 Author-email: gmanka <gmankab@gmail.com>
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
-Requires-Dist: betterdata==23.0.0
+Requires-Dist: betterdata==23.0.1
 Requires-Dist: easyselect==23.0.0
 Requires-Dist: gmanka-yml==23.0.0
 Requires-Dist: hatchling
 Requires-Dist: rich
 Requires-Dist: twine
 Description-Content-Type: text/markdown
```

