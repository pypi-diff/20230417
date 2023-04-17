# Comparing `tmp/ttkDesigner-0.30.0a7.tar.gz` & `tmp/ttkDesigner-0.30.0a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ttkDesigner-0.30.0a7.tar", last modified: Mon Apr 17 18:19:52 2023, max compression
+gzip compressed data, was "ttkDesigner-0.30.0a8.tar", last modified: Mon Apr 17 18:26:30 2023, max compression
```

## Comparing `ttkDesigner-0.30.0a7.tar` & `ttkDesigner-0.30.0a8.tar`

### file list

```diff
@@ -1,28 +1,39 @@
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2023-04-17 18:19:52.710204 ttkDesigner-0.30.0a7/
--rw-rw-r--   0 one       (1000) one       (1000)     1118 2023-04-17 18:19:49.000000 ttkDesigner-0.30.0a7/LICENSE
--rw-rw-r--   0 one       (1000) one       (1000)     1832 2023-04-17 18:19:52.706204 ttkDesigner-0.30.0a7/PKG-INFO
--rw-rw-r--   0 one       (1000) one       (1000)     1047 2023-04-17 18:19:49.000000 ttkDesigner-0.30.0a7/README.md
--rw-rw-r--   0 one       (1000) one       (1000)       38 2023-04-17 18:19:52.710204 ttkDesigner-0.30.0a7/setup.cfg
--rw-rw-r--   0 one       (1000) one       (1000)     1335 2023-04-17 18:19:49.000000 ttkDesigner-0.30.0a7/setup.py
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2023-04-17 18:19:52.706204 ttkDesigner-0.30.0a7/ttkDesigner/
--rwxrwxr-x   0 one       (1000) one       (1000)     1215 2023-04-14 17:07:05.000000 ttkDesigner-0.30.0a7/ttkDesigner/__init__.py
--rw-rw-r--   0 one       (1000) one       (1000)     1218 2023-04-14 17:07:05.000000 ttkDesigner-0.30.0a7/ttkDesigner/__main__.py
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2023-04-17 18:19:52.706204 ttkDesigner-0.30.0a7/ttkDesigner/app/
--rw-rw-r--   0 one       (1000) one       (1000)     1540 2023-04-14 17:07:05.000000 ttkDesigner-0.30.0a7/ttkDesigner/app/__init__.py
--rw-rw-r--   0 one       (1000) one       (1000)     3313 2023-04-17 16:52:51.000000 ttkDesigner-0.30.0a7/ttkDesigner/app/about.py
--rw-rw-r--   0 one       (1000) one       (1000)     1351 2023-04-17 18:19:49.000000 ttkDesigner-0.30.0a7/ttkDesigner/app/cfg.py
--rw-rw-r--   0 one       (1000) one       (1000)    14349 2023-04-17 13:42:54.000000 ttkDesigner-0.30.0a7/ttkDesigner/app/designer.py
--rw-rw-r--   0 one       (1000) one       (1000)     1538 2023-04-14 17:07:05.000000 ttkDesigner-0.30.0a7/ttkDesigner/app/main.py
--rw-rw-r--   0 one       (1000) one       (1000)    12474 2023-04-15 00:27:24.000000 ttkDesigner-0.30.0a7/ttkDesigner/app/propertyeditor.py
--rw-rw-r--   0 one       (1000) one       (1000)     2985 2023-04-14 17:07:05.000000 ttkDesigner-0.30.0a7/ttkDesigner/app/quickexport.py
--rw-rw-r--   0 one       (1000) one       (1000)     9448 2023-04-15 00:31:37.000000 ttkDesigner-0.30.0a7/ttkDesigner/app/signalsloteditor.py
--rw-rw-r--   0 one       (1000) one       (1000)     6623 2023-04-14 17:07:05.000000 ttkDesigner-0.30.0a7/ttkDesigner/app/treeinspector.py
--rw-rw-r--   0 one       (1000) one       (1000)     7053 2023-04-17 14:07:48.000000 ttkDesigner-0.30.0a7/ttkDesigner/app/widgetbox.py
--rw-rw-r--   0 one       (1000) one       (1000)     5205 2023-04-14 17:07:05.000000 ttkDesigner-0.30.0a7/ttkDesigner/app/windoweditor.py
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2023-04-17 18:19:52.706204 ttkDesigner-0.30.0a7/ttkDesigner.egg-info/
--rw-rw-r--   0 one       (1000) one       (1000)     1832 2023-04-17 18:19:52.000000 ttkDesigner-0.30.0a7/ttkDesigner.egg-info/PKG-INFO
--rw-rw-r--   0 one       (1000) one       (1000)      609 2023-04-17 18:19:52.000000 ttkDesigner-0.30.0a7/ttkDesigner.egg-info/SOURCES.txt
--rw-rw-r--   0 one       (1000) one       (1000)        1 2023-04-17 18:19:52.000000 ttkDesigner-0.30.0a7/ttkDesigner.egg-info/dependency_links.txt
--rw-rw-r--   0 one       (1000) one       (1000)       49 2023-04-17 18:19:52.000000 ttkDesigner-0.30.0a7/ttkDesigner.egg-info/entry_points.txt
--rw-rw-r--   0 one       (1000) one       (1000)       36 2023-04-17 18:19:52.000000 ttkDesigner-0.30.0a7/ttkDesigner.egg-info/requires.txt
--rw-rw-r--   0 one       (1000) one       (1000)       12 2023-04-17 18:19:52.000000 ttkDesigner-0.30.0a7/ttkDesigner.egg-info/top_level.txt
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2023-04-17 18:26:30.465949 ttkDesigner-0.30.0a8/
+-rw-rw-r--   0 one       (1000) one       (1000)     1118 2023-04-17 18:26:27.000000 ttkDesigner-0.30.0a8/LICENSE
+-rw-rw-r--   0 one       (1000) one       (1000)     1832 2023-04-17 18:26:30.465949 ttkDesigner-0.30.0a8/PKG-INFO
+-rw-rw-r--   0 one       (1000) one       (1000)     1047 2023-04-17 18:26:27.000000 ttkDesigner-0.30.0a8/README.md
+-rw-rw-r--   0 one       (1000) one       (1000)       38 2023-04-17 18:26:30.465949 ttkDesigner-0.30.0a8/setup.cfg
+-rw-rw-r--   0 one       (1000) one       (1000)     1363 2023-04-17 18:26:27.000000 ttkDesigner-0.30.0a8/setup.py
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2023-04-17 18:26:30.461949 ttkDesigner-0.30.0a8/ttkDesigner/
+-rwxrwxr-x   0 one       (1000) one       (1000)     1215 2023-04-14 17:07:05.000000 ttkDesigner-0.30.0a8/ttkDesigner/__init__.py
+-rw-rw-r--   0 one       (1000) one       (1000)     1218 2023-04-14 17:07:05.000000 ttkDesigner-0.30.0a8/ttkDesigner/__main__.py
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2023-04-17 18:26:30.465949 ttkDesigner-0.30.0a8/ttkDesigner/app/
+-rw-rw-r--   0 one       (1000) one       (1000)     1540 2023-04-14 17:07:05.000000 ttkDesigner-0.30.0a8/ttkDesigner/app/__init__.py
+-rw-rw-r--   0 one       (1000) one       (1000)     3313 2023-04-17 16:52:51.000000 ttkDesigner-0.30.0a8/ttkDesigner/app/about.py
+-rw-rw-r--   0 one       (1000) one       (1000)     1351 2023-04-17 18:26:27.000000 ttkDesigner-0.30.0a8/ttkDesigner/app/cfg.py
+-rw-rw-r--   0 one       (1000) one       (1000)    14349 2023-04-17 13:42:54.000000 ttkDesigner-0.30.0a8/ttkDesigner/app/designer.py
+-rw-rw-r--   0 one       (1000) one       (1000)     1538 2023-04-14 17:07:05.000000 ttkDesigner-0.30.0a8/ttkDesigner/app/main.py
+-rw-rw-r--   0 one       (1000) one       (1000)    12474 2023-04-15 00:27:24.000000 ttkDesigner-0.30.0a8/ttkDesigner/app/propertyeditor.py
+-rw-rw-r--   0 one       (1000) one       (1000)     2985 2023-04-14 17:07:05.000000 ttkDesigner-0.30.0a8/ttkDesigner/app/quickexport.py
+-rw-rw-r--   0 one       (1000) one       (1000)     9448 2023-04-15 00:31:37.000000 ttkDesigner-0.30.0a8/ttkDesigner/app/signalsloteditor.py
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2023-04-17 18:26:30.465949 ttkDesigner-0.30.0a8/ttkDesigner/app/superobj/
+-rw-rw-r--   0 one       (1000) one       (1000)     1544 2023-04-14 17:07:05.000000 ttkDesigner-0.30.0a8/ttkDesigner/app/superobj/__init__.py
+-rw-rw-r--   0 one       (1000) one       (1000)     4308 2023-04-14 17:07:05.000000 ttkDesigner-0.30.0a8/ttkDesigner/app/superobj/supercontrol.py
+-rw-rw-r--   0 one       (1000) one       (1000)     8555 2023-04-14 17:07:05.000000 ttkDesigner-0.30.0a8/ttkDesigner/app/superobj/superlayout.py
+-rw-rw-r--   0 one       (1000) one       (1000)    12712 2023-04-14 17:07:05.000000 ttkDesigner-0.30.0a8/ttkDesigner/app/superobj/superlayoutgrid.py
+-rw-rw-r--   0 one       (1000) one       (1000)     1481 2023-04-14 17:07:05.000000 ttkDesigner-0.30.0a8/ttkDesigner/app/superobj/superlayouthbox.py
+-rw-rw-r--   0 one       (1000) one       (1000)     1479 2023-04-14 17:07:05.000000 ttkDesigner-0.30.0a8/ttkDesigner/app/superobj/superlayoutvbox.py
+-rw-rw-r--   0 one       (1000) one       (1000)     4004 2023-04-14 17:07:05.000000 ttkDesigner-0.30.0a8/ttkDesigner/app/superobj/superobj.py
+-rw-rw-r--   0 one       (1000) one       (1000)    10603 2023-04-16 15:59:33.000000 ttkDesigner-0.30.0a8/ttkDesigner/app/superobj/superwidget.py
+-rw-rw-r--   0 one       (1000) one       (1000)     1679 2023-04-14 17:07:05.000000 ttkDesigner-0.30.0a8/ttkDesigner/app/superobj/superwidgetradiobutton.py
+-rw-rw-r--   0 one       (1000) one       (1000)     1793 2023-04-14 17:07:05.000000 ttkDesigner-0.30.0a8/ttkDesigner/app/superobj/superwidgettextedit.py
+-rw-rw-r--   0 one       (1000) one       (1000)     6623 2023-04-14 17:07:05.000000 ttkDesigner-0.30.0a8/ttkDesigner/app/treeinspector.py
+-rw-rw-r--   0 one       (1000) one       (1000)     7053 2023-04-17 14:07:48.000000 ttkDesigner-0.30.0a8/ttkDesigner/app/widgetbox.py
+-rw-rw-r--   0 one       (1000) one       (1000)     5205 2023-04-14 17:07:05.000000 ttkDesigner-0.30.0a8/ttkDesigner/app/windoweditor.py
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2023-04-17 18:26:30.461949 ttkDesigner-0.30.0a8/ttkDesigner.egg-info/
+-rw-rw-r--   0 one       (1000) one       (1000)     1832 2023-04-17 18:26:30.000000 ttkDesigner-0.30.0a8/ttkDesigner.egg-info/PKG-INFO
+-rw-rw-r--   0 one       (1000) one       (1000)     1035 2023-04-17 18:26:30.000000 ttkDesigner-0.30.0a8/ttkDesigner.egg-info/SOURCES.txt
+-rw-rw-r--   0 one       (1000) one       (1000)        1 2023-04-17 18:26:30.000000 ttkDesigner-0.30.0a8/ttkDesigner.egg-info/dependency_links.txt
+-rw-rw-r--   0 one       (1000) one       (1000)       49 2023-04-17 18:26:30.000000 ttkDesigner-0.30.0a8/ttkDesigner.egg-info/entry_points.txt
+-rw-rw-r--   0 one       (1000) one       (1000)       36 2023-04-17 18:26:30.000000 ttkDesigner-0.30.0a8/ttkDesigner.egg-info/requires.txt
+-rw-rw-r--   0 one       (1000) one       (1000)       12 2023-04-17 18:26:30.000000 ttkDesigner-0.30.0a8/ttkDesigner.egg-info/top_level.txt
```

### Comparing `ttkDesigner-0.30.0a7/LICENSE` & `ttkDesigner-0.30.0a8/LICENSE`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.30.0a7/PKG-INFO` & `ttkDesigner-0.30.0a8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ttkDesigner
-Version: 0.30.0a7
+Version: 0.30.0a8
 Summary: ttkDesigner is a terminal user interface designer for pyTermTk applications
 Home-page: https://github.com/ceccopierangiolieugenio/pyTermTk
 Author: Eugenio Parodi
 Author-email: ceccopierangiolieugenio@googlemail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ttkDesigner-0.30.0a7/README.md` & `ttkDesigner-0.30.0a8/README.md`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.30.0a7/setup.py` & `ttkDesigner-0.30.0a8/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-version = "0.30.0-a7"
+version = "0.30.0-a8"
 name = "ttkDesigner"
 
 print(f"Version: {version}")
 print(f"Name: {name}")
 
 setup(
     name=name,
@@ -25,15 +25,15 @@
         "Development Status :: 3 - Alpha",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "Topic :: Terminals",
         "Topic :: Software Development :: User Interfaces"],
     include_package_data=False,
-    packages=['ttkDesigner','ttkDesigner.app'],
+    packages=['ttkDesigner','ttkDesigner.app', 'ttkDesigner.app.superobj'],
     python_requires=">=3.8",
     install_requires=[
         'pyTermTk>=0.30.0a5',
         'pyperclip',
         'Pillow'],
     entry_points={
         'console_scripts': [
```

### Comparing `ttkDesigner-0.30.0a7/ttkDesigner/__init__.py` & `ttkDesigner-0.30.0a8/ttkDesigner/__init__.py`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.30.0a7/ttkDesigner/__main__.py` & `ttkDesigner-0.30.0a8/ttkDesigner/__main__.py`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.30.0a7/ttkDesigner/app/__init__.py` & `ttkDesigner-0.30.0a8/ttkDesigner/app/__init__.py`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.30.0a7/ttkDesigner/app/about.py` & `ttkDesigner-0.30.0a8/ttkDesigner/app/about.py`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.30.0a7/ttkDesigner/app/cfg.py` & `ttkDesigner-0.30.0a8/ttkDesigner/app/cfg.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,14 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import os
 # import yaml
 
 class TTkDesignerCfg:
-    version="0.30.0-a7"
+    version="0.30.0-a8"
     name="ttkDesigner"
     cfgVersion = '1.0'
     pathCfg="."
     options={}
     maxsearches=200
```

### Comparing `ttkDesigner-0.30.0a7/ttkDesigner/app/designer.py` & `ttkDesigner-0.30.0a8/ttkDesigner/app/designer.py`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.30.0a7/ttkDesigner/app/main.py` & `ttkDesigner-0.30.0a8/ttkDesigner/app/main.py`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.30.0a7/ttkDesigner/app/propertyeditor.py` & `ttkDesigner-0.30.0a8/ttkDesigner/app/propertyeditor.py`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.30.0a7/ttkDesigner/app/quickexport.py` & `ttkDesigner-0.30.0a8/ttkDesigner/app/quickexport.py`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.30.0a7/ttkDesigner/app/signalsloteditor.py` & `ttkDesigner-0.30.0a8/ttkDesigner/app/signalsloteditor.py`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.30.0a7/ttkDesigner/app/treeinspector.py` & `ttkDesigner-0.30.0a8/ttkDesigner/app/treeinspector.py`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.30.0a7/ttkDesigner/app/widgetbox.py` & `ttkDesigner-0.30.0a8/ttkDesigner/app/widgetbox.py`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.30.0a7/ttkDesigner/app/windoweditor.py` & `ttkDesigner-0.30.0a8/ttkDesigner/app/windoweditor.py`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.30.0a7/ttkDesigner.egg-info/PKG-INFO` & `ttkDesigner-0.30.0a8/ttkDesigner.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ttkDesigner
-Version: 0.30.0a7
+Version: 0.30.0a8
 Summary: ttkDesigner is a terminal user interface designer for pyTermTk applications
 Home-page: https://github.com/ceccopierangiolieugenio/pyTermTk
 Author: Eugenio Parodi
 Author-email: ceccopierangiolieugenio@googlemail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

