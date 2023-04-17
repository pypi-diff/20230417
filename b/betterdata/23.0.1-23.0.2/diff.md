# Comparing `tmp/betterdata-23.0.1.tar.gz` & `tmp/betterdata-23.0.2.tar.gz`

## Comparing `betterdata-23.0.1.tar` & `betterdata-23.0.2.tar`

### file list

```diff
@@ -1,12 +1,10 @@
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 betterdata-23.0.1/build.sh
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 betterdata-23.0.1/changelog.md
--rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 betterdata-23.0.1/start.sh
--rwxr-xr-x   0        0        0     4409 2020-02-02 00:00:00.000000 betterdata-23.0.1/betterdata/__init__.py
--rw-r--r--   0        0        0   153907 2020-02-02 00:00:00.000000 betterdata-23.0.1/img/filled.png
--rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 betterdata-23.0.1/img/filled.svg
--rw-r--r--   0        0        0    59577 2020-02-02 00:00:00.000000 betterdata-23.0.1/img/transparent.png
--rwxr-xr-x   0        0        0     3969 2020-02-02 00:00:00.000000 betterdata-23.0.1/img/transparent.svg
--rwxr-xr-x   0        0        0       32 2020-02-02 00:00:00.000000 betterdata-23.0.1/.gitignore
--rwxr-xr-x   0        0        0      720 2020-02-02 00:00:00.000000 betterdata-23.0.1/pyproject.toml
--rwxr-xr-x   0        0        0     3760 2020-02-02 00:00:00.000000 betterdata-23.0.1/readme.md
--rw-r--r--   0        0        0     4416 2020-02-02 00:00:00.000000 betterdata-23.0.1/PKG-INFO
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 betterdata-23.0.2/changelog.md
+-rwxr-xr-x   0        0        0     4409 2020-02-02 00:00:00.000000 betterdata-23.0.2/betterdata/__init__.py
+-rw-r--r--   0        0        0   153907 2020-02-02 00:00:00.000000 betterdata-23.0.2/img/filled.png
+-rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 betterdata-23.0.2/img/filled.svg
+-rw-r--r--   0        0        0    59577 2020-02-02 00:00:00.000000 betterdata-23.0.2/img/transparent.png
+-rwxr-xr-x   0        0        0     3969 2020-02-02 00:00:00.000000 betterdata-23.0.2/img/transparent.svg
+-rwxr-xr-x   0        0        0       32 2020-02-02 00:00:00.000000 betterdata-23.0.2/.gitignore
+-rwxr-xr-x   0        0        0      720 2020-02-02 00:00:00.000000 betterdata-23.0.2/pyproject.toml
+-rwxr-xr-x   0        0        0     3760 2020-02-02 00:00:00.000000 betterdata-23.0.2/readme.md
+-rw-r--r--   0        0        0     4416 2020-02-02 00:00:00.000000 betterdata-23.0.2/PKG-INFO
```

### Comparing `betterdata-23.0.1/betterdata/__init__.py` & `betterdata-23.0.2/betterdata/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,15 @@
         self,
         path = None,
     ):
         self.set_data(
             path = path,
         )
         self.set_data(
-            data = yml.read_file(
+            data = yml.from_file(
                 path = self.path
             )
         )
 
     def to_file(
         self,
         path = None
```

### Comparing `betterdata-23.0.1/img/filled.png` & `betterdata-23.0.2/img/filled.png`

 * *Files identical despite different names*

### Comparing `betterdata-23.0.1/img/filled.svg` & `betterdata-23.0.2/img/filled.svg`

 * *Files identical despite different names*

### Comparing `betterdata-23.0.1/img/transparent.png` & `betterdata-23.0.2/img/transparent.png`

 * *Files identical despite different names*

### Comparing `betterdata-23.0.1/img/transparent.svg` & `betterdata-23.0.2/img/transparent.svg`

 * *Files identical despite different names*

### Comparing `betterdata-23.0.1/pyproject.toml` & `betterdata-23.0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 dependencies = [
   "rich",
   "easyselect==23.0.0",
-  "gmanka_yml==23.0.0",
+  "gmanka_yml==23.0.4",
 ]
 name = "betterdata"
-version = "23.0.1"
+version = "23.0.2"
 authors = [
   { name="gmanka", email="gmankab@gmail.com" },
 ]
 description = "a lib for working with data"
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `betterdata-23.0.1/readme.md` & `betterdata-23.0.2/readme.md`

 * *Files identical despite different names*

### Comparing `betterdata-23.0.1/PKG-INFO` & `betterdata-23.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: betterdata
-Version: 23.0.1
+Version: 23.0.2
 Summary: a lib for working with data
 Project-URL: Homepage, https://github.com/gmankab/betterdata
 Project-URL: Documentation, https://github.com/gmankab/betterdata
 Project-URL: Bug Tracker, https://github.com/gmankab/betterdata/issues
 Author-email: gmanka <gmankab@gmail.com>
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: easyselect==23.0.0
-Requires-Dist: gmanka-yml==23.0.0
+Requires-Dist: gmanka-yml==23.0.4
 Requires-Dist: rich
 Description-Content-Type: text/markdown
 
 # betterdata by gmanka
 
 <img src="https://github.com/gmankab/betterdata/raw/main/img/transparent.png">
```

