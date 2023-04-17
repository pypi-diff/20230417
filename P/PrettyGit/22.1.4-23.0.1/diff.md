# Comparing `tmp/prettygit-22.1.4.tar.gz` & `tmp/prettygit-23.0.1.tar.gz`

## Comparing `prettygit-22.1.4.tar` & `prettygit-23.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 prettygit-22.1.4/build.sh
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 prettygit-22.1.4/changelog.md
--rwxr-xr-x   0        0        0      112 2020-02-02 00:00:00.000000 prettygit-22.1.4/start.sh
--rw-r--r--   0        0        0   151771 2020-02-02 00:00:00.000000 prettygit-22.1.4/img/filled.png
--rw-r--r--   0        0        0     5606 2020-02-02 00:00:00.000000 prettygit-22.1.4/img/filled.svg
--rw-r--r--   0        0        0    57741 2020-02-02 00:00:00.000000 prettygit-22.1.4/img/transparent.png
--rwxr-xr-x   0        0        0     6099 2020-02-02 00:00:00.000000 prettygit-22.1.4/img/transparent.svg
--rwxr-xr-x   0        0        0     1196 2020-02-02 00:00:00.000000 prettygit-22.1.4/launcher/prettygit.bat
--rwxr-xr-x   0        0        0      890 2020-02-02 00:00:00.000000 prettygit-22.1.4/launcher/prettygit.sh
--rwxr-xr-x   0        0        0     2573 2020-02-02 00:00:00.000000 prettygit-22.1.4/launcher/prettygit_win.py
--rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 prettygit-22.1.4/prettygit/__init__.py
--rwxr-xr-x   0        0        0      202 2020-02-02 00:00:00.000000 prettygit-22.1.4/prettygit/__main__.py
--rwxr-xr-x   0        0        0    15203 2020-02-02 00:00:00.000000 prettygit-22.1.4/prettygit/main.py
--rwxr-xr-x   0        0        0     4271 2020-02-02 00:00:00.000000 prettygit-22.1.4/prettygit/setup.py
--rw-r--r--   0        0        0    10405 2020-02-02 00:00:00.000000 prettygit-22.1.4/prettygit/icons/icon.ico
--rwxr-xr-x   0        0        0     3242 2020-02-02 00:00:00.000000 prettygit-22.1.4/prettygit/icons/icon.svg
--rwxr-xr-x   0        0        0       22 2020-02-02 00:00:00.000000 prettygit-22.1.4/.gitignore
--rwxr-xr-x   0        0        0      746 2020-02-02 00:00:00.000000 prettygit-22.1.4/pyproject.toml
--rwxr-xr-x   0        0        0     1691 2020-02-02 00:00:00.000000 prettygit-22.1.4/readme.md
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 prettygit-22.1.4/PKG-INFO
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 prettygit-23.0.1/build.sh
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 prettygit-23.0.1/changelog.md
+-rwxr-xr-x   0        0        0      112 2020-02-02 00:00:00.000000 prettygit-23.0.1/start.sh
+-rw-r--r--   0        0        0   151771 2020-02-02 00:00:00.000000 prettygit-23.0.1/img/filled.png
+-rw-r--r--   0        0        0     5606 2020-02-02 00:00:00.000000 prettygit-23.0.1/img/filled.svg
+-rw-r--r--   0        0        0    57741 2020-02-02 00:00:00.000000 prettygit-23.0.1/img/transparent.png
+-rwxr-xr-x   0        0        0     6099 2020-02-02 00:00:00.000000 prettygit-23.0.1/img/transparent.svg
+-rwxr-xr-x   0        0        0     1196 2020-02-02 00:00:00.000000 prettygit-23.0.1/launcher/prettygit.bat
+-rwxr-xr-x   0        0        0      890 2020-02-02 00:00:00.000000 prettygit-23.0.1/launcher/prettygit.sh
+-rwxr-xr-x   0        0        0     2573 2020-02-02 00:00:00.000000 prettygit-23.0.1/launcher/prettygit_win.py
+-rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 prettygit-23.0.1/prettygit/__init__.py
+-rwxr-xr-x   0        0        0      202 2020-02-02 00:00:00.000000 prettygit-23.0.1/prettygit/__main__.py
+-rwxr-xr-x   0        0        0    15198 2020-02-02 00:00:00.000000 prettygit-23.0.1/prettygit/main.py
+-rwxr-xr-x   0        0        0     4271 2020-02-02 00:00:00.000000 prettygit-23.0.1/prettygit/setup.py
+-rw-r--r--   0        0        0    10405 2020-02-02 00:00:00.000000 prettygit-23.0.1/prettygit/icons/icon.ico
+-rwxr-xr-x   0        0        0     3242 2020-02-02 00:00:00.000000 prettygit-23.0.1/prettygit/icons/icon.svg
+-rwxr-xr-x   0        0        0       22 2020-02-02 00:00:00.000000 prettygit-23.0.1/.gitignore
+-rwxr-xr-x   0        0        0      786 2020-02-02 00:00:00.000000 prettygit-23.0.1/pyproject.toml
+-rwxr-xr-x   0        0        0     1691 2020-02-02 00:00:00.000000 prettygit-23.0.1/readme.md
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 prettygit-23.0.1/PKG-INFO
```

### Comparing `prettygit-22.1.4/img/filled.png` & `prettygit-23.0.1/img/filled.png`

 * *Files identical despite different names*

### Comparing `prettygit-22.1.4/img/filled.svg` & `prettygit-23.0.1/img/filled.svg`

 * *Files identical despite different names*

### Comparing `prettygit-22.1.4/img/transparent.png` & `prettygit-23.0.1/img/transparent.png`

 * *Files identical despite different names*

### Comparing `prettygit-22.1.4/img/transparent.svg` & `prettygit-23.0.1/img/transparent.svg`

 * *Files identical despite different names*

### Comparing `prettygit-22.1.4/launcher/prettygit.bat` & `prettygit-23.0.1/launcher/prettygit.bat`

 * *Files identical despite different names*

### Comparing `prettygit-22.1.4/launcher/prettygit.sh` & `prettygit-23.0.1/launcher/prettygit.sh`

 * *Files identical despite different names*

### Comparing `prettygit-22.1.4/launcher/prettygit_win.py` & `prettygit-23.0.1/launcher/prettygit_win.py`

 * *Files identical despite different names*

### Comparing `prettygit-22.1.4/prettygit/main.py` & `prettygit-23.0.1/prettygit/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     f'[bold][deep_sky_blue1]prettygit [white]{app_version}'
 )
 proj_path = os.getcwd()
 config_path = Path(
     f'{proj_path}/.git/prettygit.yml'
 )
 config = Data(
-    file_path=config_path
+    path=config_path
 )
 temp_data = Data()
 run_st = subprocess.getstatusoutput
 options_list = [
     {
         'args': (
             '-h',
```

### Comparing `prettygit-22.1.4/prettygit/setup.py` & `prettygit-23.0.1/prettygit/setup.py`

 * *Files identical despite different names*

### Comparing `prettygit-22.1.4/prettygit/icons/icon.ico` & `prettygit-23.0.1/prettygit/icons/icon.ico`

 * *Files identical despite different names*

### Comparing `prettygit-22.1.4/prettygit/icons/icon.svg` & `prettygit-23.0.1/prettygit/icons/icon.svg`

 * *Files identical despite different names*

### Comparing `prettygit-22.1.4/pyproject.toml` & `prettygit-23.0.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 dependencies = [
-  "easyselect",
-  "betterdata",
+  "gmanka_yml==23.0.0",
+  "easyselect==23.0.0",
+  "betterdata==23.0.0",
   "hatchling",
   "twine",
   "rich",
 ]
 name = "PrettyGit"
-version = "22.1.4"
+version = "23.0.1"
 authors = [
   { name="gmanka", email="gmankab@gmail.com" },
 ]
 description = "very simple and user friendly interface for git"
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `prettygit-22.1.4/readme.md` & `prettygit-23.0.1/readme.md`

 * *Files identical despite different names*

### Comparing `prettygit-22.1.4/PKG-INFO` & `prettygit-23.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: PrettyGit
-Version: 22.1.4
+Version: 23.0.1
 Summary: very simple and user friendly interface for git
 Project-URL: Homepage, https://github.com/gmankab/PrettyGit
 Project-URL: Bug Tracker, https://github.com/gmankab/PrettyGit/issues
 Project-URL: Documentation, https://github.com/gmankab/PrettyGit
 Author-email: gmanka <gmankab@gmail.com>
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
-Requires-Dist: betterdata
-Requires-Dist: easyselect
+Requires-Dist: betterdata==23.0.0
+Requires-Dist: easyselect==23.0.0
+Requires-Dist: gmanka-yml==23.0.0
 Requires-Dist: hatchling
 Requires-Dist: rich
 Requires-Dist: twine
 Description-Content-Type: text/markdown
 
 # prettygit by gmanka
```

