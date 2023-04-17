# Comparing `tmp/easyselect-22.1.0.tar.gz` & `tmp/easyselect-23.0.0.tar.gz`

## Comparing `easyselect-22.1.0.tar` & `easyselect-23.0.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 easyselect-22.1.0/build.sh
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 easyselect-22.1.0/changelog
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 easyselect-22.1.0/start.sh
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 easyselect-22.1.0/test.py
--rwxr-xr-x   0        0        0     5647 2020-02-02 00:00:00.000000 easyselect-22.1.0/easyselect/__init__.py
--rw-r--r--   0        0        0   170648 2020-02-02 00:00:00.000000 easyselect-22.1.0/img/filled.png
--rw-r--r--   0        0        0     3508 2020-02-02 00:00:00.000000 easyselect-22.1.0/img/filled.svg
--rw-r--r--   0        0        0    64875 2020-02-02 00:00:00.000000 easyselect-22.1.0/img/transparent.png
--rwxr-xr-x   0        0        0     3110 2020-02-02 00:00:00.000000 easyselect-22.1.0/img/transparent.svg
--rwxr-xr-x   0        0        0       26 2020-02-02 00:00:00.000000 easyselect-22.1.0/.gitignore
--rwxr-xr-x   0        0        0      762 2020-02-02 00:00:00.000000 easyselect-22.1.0/pyproject.toml
--rwxr-xr-x   0        0        0     1964 2020-02-02 00:00:00.000000 easyselect-22.1.0/readme.md
--rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 easyselect-22.1.0/PKG-INFO
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 easyselect-23.0.0/build.sh
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 easyselect-23.0.0/changelog.md
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 easyselect-23.0.0/start.sh
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 easyselect-23.0.0/test.py
+-rwxr-xr-x   0        0        0     5647 2020-02-02 00:00:00.000000 easyselect-23.0.0/easyselect/__init__.py
+-rw-r--r--   0        0        0   170648 2020-02-02 00:00:00.000000 easyselect-23.0.0/img/filled.png
+-rw-r--r--   0        0        0     3508 2020-02-02 00:00:00.000000 easyselect-23.0.0/img/filled.svg
+-rw-r--r--   0        0        0    64875 2020-02-02 00:00:00.000000 easyselect-23.0.0/img/transparent.png
+-rwxr-xr-x   0        0        0     3110 2020-02-02 00:00:00.000000 easyselect-23.0.0/img/transparent.svg
+-rwxr-xr-x   0        0        0       26 2020-02-02 00:00:00.000000 easyselect-23.0.0/.gitignore
+-rwxr-xr-x   0        0        0      762 2020-02-02 00:00:00.000000 easyselect-23.0.0/pyproject.toml
+-rwxr-xr-x   0        0        0     2115 2020-02-02 00:00:00.000000 easyselect-23.0.0/readme.md
+-rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 easyselect-23.0.0/PKG-INFO
```

### Comparing `easyselect-22.1.0/easyselect/__init__.py` & `easyselect-23.0.0/easyselect/__init__.py`

 * *Files identical despite different names*

### Comparing `easyselect-22.1.0/img/filled.png` & `easyselect-23.0.0/img/filled.png`

 * *Files identical despite different names*

### Comparing `easyselect-22.1.0/img/filled.svg` & `easyselect-23.0.0/img/filled.svg`

 * *Files identical despite different names*

### Comparing `easyselect-22.1.0/img/transparent.png` & `easyselect-23.0.0/img/transparent.png`

 * *Files identical despite different names*

### Comparing `easyselect-22.1.0/img/transparent.svg` & `easyselect-23.0.0/img/transparent.svg`

 * *Files identical despite different names*

### Comparing `easyselect-22.1.0/pyproject.toml` & `easyselect-23.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 dependencies = [
   "rich",
   "windows-curses ; platform_system==\"Windows\"",
 ]
 name = "easyselect"
-version = "22.1.0"
+version = "23.0.0"
 authors = [
   { name="gmanka", email="gmankab@gmail.com" },
 ]
 description = "simple and pretty tool for selecting items by keyboard in terminal"
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `easyselect-22.1.0/readme.md` & `easyselect-23.0.0/readme.md`

 * *Files 16% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 - [installation](#installation)
 - [usage](#usage)
 - [print text while choosing](#print-text-while-choosing)
 - [rich styles support](#rich-styles-support)
 - [long items list support](#long-items-list-support)
 - [page size](#page-size)
 - [supported buttons](#supported-buttons)
+- [changelog](#changelog)
 - [license](#license)
 
 ### installation[^](#navigation)
 
 ```sh
 pip install easyselect
 ```
@@ -94,10 +95,15 @@
 user will able to use these buttons
 
 - up, down, left, right
 - w, a, s, d, j, k
 - home, end
 - page up, page down
 
+### changelog[^](#navigation)
+
+you can read changelog [here](https://github.com/gmankab/easyselect/blob/main/changelog.md)
+
+
 ### license[^](#navigation)
 
 [gnu gpl 3](https://gnu.org/licenses/gpl-3.0.en.html)
```

### Comparing `easyselect-22.1.0/PKG-INFO` & `easyselect-23.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyselect
-Version: 22.1.0
+Version: 23.0.0
 Summary: simple and pretty tool for selecting items by keyboard in terminal
 Project-URL: Homepage, https://github.com/gmankab/easyselect
 Project-URL: Bug Tracker, https://github.com/gmankab/easyselect/issues
 Project-URL: Documentation, https://github.com/gmankab/easyselect
 Author-email: gmanka <gmankab@gmail.com>
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -25,14 +25,15 @@
 - [installation](#installation)
 - [usage](#usage)
 - [print text while choosing](#print-text-while-choosing)
 - [rich styles support](#rich-styles-support)
 - [long items list support](#long-items-list-support)
 - [page size](#page-size)
 - [supported buttons](#supported-buttons)
+- [changelog](#changelog)
 - [license](#license)
 
 ### installation[^](#navigation)
 
 ```sh
 pip install easyselect
 ```
@@ -110,10 +111,15 @@
 user will able to use these buttons
 
 - up, down, left, right
 - w, a, s, d, j, k
 - home, end
 - page up, page down
 
+### changelog[^](#navigation)
+
+you can read changelog [here](https://github.com/gmankab/easyselect/blob/main/changelog.md)
+
+
 ### license[^](#navigation)
 
 [gnu gpl 3](https://gnu.org/licenses/gpl-3.0.en.html)
```

