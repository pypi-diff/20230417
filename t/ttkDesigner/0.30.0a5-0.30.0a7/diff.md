# Comparing `tmp/ttkDesigner-0.30.0a5.tar.gz` & `tmp/ttkDesigner-0.30.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ttkDesigner-0.30.0a5.tar", last modified: Mon Apr 17 17:02:45 2023, max compression
+gzip compressed data, was "ttkDesigner-0.30.0a7.tar", last modified: Mon Apr 17 18:19:52 2023, max compression
```

## Comparing `ttkDesigner-0.30.0a5.tar` & `ttkDesigner-0.30.0a7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2023-04-17 17:02:45.963054 ttkDesigner-0.30.0a5/
--rw-rw-r--   0 one       (1000) one       (1000)     1118 2023-04-17 17:02:40.000000 ttkDesigner-0.30.0a5/LICENSE
--rw-rw-r--   0 one       (1000) one       (1000)     1830 2023-04-17 17:02:45.963054 ttkDesigner-0.30.0a5/PKG-INFO
--rw-rw-r--   0 one       (1000) one       (1000)     1047 2023-04-17 17:02:40.000000 ttkDesigner-0.30.0a5/README.md
--rw-rw-r--   0 one       (1000) one       (1000)       38 2023-04-17 17:02:45.963054 ttkDesigner-0.30.0a5/setup.cfg
--rw-rw-r--   0 one       (1000) one       (1000)     1330 2023-04-17 17:02:40.000000 ttkDesigner-0.30.0a5/setup.py
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2023-04-17 17:02:45.959054 ttkDesigner-0.30.0a5/ttkDesigner/
--rwxrwxr-x   0 one       (1000) one       (1000)     1215 2023-04-14 17:07:05.000000 ttkDesigner-0.30.0a5/ttkDesigner/__init__.py
--rw-rw-r--   0 one       (1000) one       (1000)     1218 2023-04-14 17:07:05.000000 ttkDesigner-0.30.0a5/ttkDesigner/__main__.py
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2023-04-17 17:02:45.963054 ttkDesigner-0.30.0a5/ttkDesigner/app/
--rw-rw-r--   0 one       (1000) one       (1000)     1540 2023-04-14 17:07:05.000000 ttkDesigner-0.30.0a5/ttkDesigner/app/__init__.py
--rw-rw-r--   0 one       (1000) one       (1000)     3313 2023-04-17 16:52:51.000000 ttkDesigner-0.30.0a5/ttkDesigner/app/about.py
--rw-rw-r--   0 one       (1000) one       (1000)     1351 2023-04-17 17:02:40.000000 ttkDesigner-0.30.0a5/ttkDesigner/app/cfg.py
--rw-rw-r--   0 one       (1000) one       (1000)    14349 2023-04-17 13:42:54.000000 ttkDesigner-0.30.0a5/ttkDesigner/app/designer.py
--rw-rw-r--   0 one       (1000) one       (1000)     1538 2023-04-14 17:07:05.000000 ttkDesigner-0.30.0a5/ttkDesigner/app/main.py
--rw-rw-r--   0 one       (1000) one       (1000)    12474 2023-04-15 00:27:24.000000 ttkDesigner-0.30.0a5/ttkDesigner/app/propertyeditor.py
--rw-rw-r--   0 one       (1000) one       (1000)     2985 2023-04-14 17:07:05.000000 ttkDesigner-0.30.0a5/ttkDesigner/app/quickexport.py
--rw-rw-r--   0 one       (1000) one       (1000)     9448 2023-04-15 00:31:37.000000 ttkDesigner-0.30.0a5/ttkDesigner/app/signalsloteditor.py
--rw-rw-r--   0 one       (1000) one       (1000)     6623 2023-04-14 17:07:05.000000 ttkDesigner-0.30.0a5/ttkDesigner/app/treeinspector.py
--rw-rw-r--   0 one       (1000) one       (1000)     7053 2023-04-17 14:07:48.000000 ttkDesigner-0.30.0a5/ttkDesigner/app/widgetbox.py
--rw-rw-r--   0 one       (1000) one       (1000)     5205 2023-04-14 17:07:05.000000 ttkDesigner-0.30.0a5/ttkDesigner/app/windoweditor.py
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2023-04-17 17:02:45.959054 ttkDesigner-0.30.0a5/ttkDesigner.egg-info/
--rw-rw-r--   0 one       (1000) one       (1000)     1830 2023-04-17 17:02:45.000000 ttkDesigner-0.30.0a5/ttkDesigner.egg-info/PKG-INFO
--rw-rw-r--   0 one       (1000) one       (1000)      609 2023-04-17 17:02:45.000000 ttkDesigner-0.30.0a5/ttkDesigner.egg-info/SOURCES.txt
--rw-rw-r--   0 one       (1000) one       (1000)        1 2023-04-17 17:02:45.000000 ttkDesigner-0.30.0a5/ttkDesigner.egg-info/dependency_links.txt
--rw-rw-r--   0 one       (1000) one       (1000)       49 2023-04-17 17:02:45.000000 ttkDesigner-0.30.0a5/ttkDesigner.egg-info/entry_points.txt
--rw-rw-r--   0 one       (1000) one       (1000)       33 2023-04-17 17:02:45.000000 ttkDesigner-0.30.0a5/ttkDesigner.egg-info/requires.txt
--rw-rw-r--   0 one       (1000) one       (1000)       12 2023-04-17 17:02:45.000000 ttkDesigner-0.30.0a5/ttkDesigner.egg-info/top_level.txt
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2023-04-17 18:19:52.710204 ttkDesigner-0.30.0a7/
+-rw-rw-r--   0 one       (1000) one       (1000)     1118 2023-04-17 18:19:49.000000 ttkDesigner-0.30.0a7/LICENSE
+-rw-rw-r--   0 one       (1000) one       (1000)     1832 2023-04-17 18:19:52.706204 ttkDesigner-0.30.0a7/PKG-INFO
+-rw-rw-r--   0 one       (1000) one       (1000)     1047 2023-04-17 18:19:49.000000 ttkDesigner-0.30.0a7/README.md
+-rw-rw-r--   0 one       (1000) one       (1000)       38 2023-04-17 18:19:52.710204 ttkDesigner-0.30.0a7/setup.cfg
+-rw-rw-r--   0 one       (1000) one       (1000)     1335 2023-04-17 18:19:49.000000 ttkDesigner-0.30.0a7/setup.py
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2023-04-17 18:19:52.706204 ttkDesigner-0.30.0a7/ttkDesigner/
+-rwxrwxr-x   0 one       (1000) one       (1000)     1215 2023-04-14 17:07:05.000000 ttkDesigner-0.30.0a7/ttkDesigner/__init__.py
+-rw-rw-r--   0 one       (1000) one       (1000)     1218 2023-04-14 17:07:05.000000 ttkDesigner-0.30.0a7/ttkDesigner/__main__.py
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2023-04-17 18:19:52.706204 ttkDesigner-0.30.0a7/ttkDesigner/app/
+-rw-rw-r--   0 one       (1000) one       (1000)     1540 2023-04-14 17:07:05.000000 ttkDesigner-0.30.0a7/ttkDesigner/app/__init__.py
+-rw-rw-r--   0 one       (1000) one       (1000)     3313 2023-04-17 16:52:51.000000 ttkDesigner-0.30.0a7/ttkDesigner/app/about.py
+-rw-rw-r--   0 one       (1000) one       (1000)     1351 2023-04-17 18:19:49.000000 ttkDesigner-0.30.0a7/ttkDesigner/app/cfg.py
+-rw-rw-r--   0 one       (1000) one       (1000)    14349 2023-04-17 13:42:54.000000 ttkDesigner-0.30.0a7/ttkDesigner/app/designer.py
+-rw-rw-r--   0 one       (1000) one       (1000)     1538 2023-04-14 17:07:05.000000 ttkDesigner-0.30.0a7/ttkDesigner/app/main.py
+-rw-rw-r--   0 one       (1000) one       (1000)    12474 2023-04-15 00:27:24.000000 ttkDesigner-0.30.0a7/ttkDesigner/app/propertyeditor.py
+-rw-rw-r--   0 one       (1000) one       (1000)     2985 2023-04-14 17:07:05.000000 ttkDesigner-0.30.0a7/ttkDesigner/app/quickexport.py
+-rw-rw-r--   0 one       (1000) one       (1000)     9448 2023-04-15 00:31:37.000000 ttkDesigner-0.30.0a7/ttkDesigner/app/signalsloteditor.py
+-rw-rw-r--   0 one       (1000) one       (1000)     6623 2023-04-14 17:07:05.000000 ttkDesigner-0.30.0a7/ttkDesigner/app/treeinspector.py
+-rw-rw-r--   0 one       (1000) one       (1000)     7053 2023-04-17 14:07:48.000000 ttkDesigner-0.30.0a7/ttkDesigner/app/widgetbox.py
+-rw-rw-r--   0 one       (1000) one       (1000)     5205 2023-04-14 17:07:05.000000 ttkDesigner-0.30.0a7/ttkDesigner/app/windoweditor.py
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2023-04-17 18:19:52.706204 ttkDesigner-0.30.0a7/ttkDesigner.egg-info/
+-rw-rw-r--   0 one       (1000) one       (1000)     1832 2023-04-17 18:19:52.000000 ttkDesigner-0.30.0a7/ttkDesigner.egg-info/PKG-INFO
+-rw-rw-r--   0 one       (1000) one       (1000)      609 2023-04-17 18:19:52.000000 ttkDesigner-0.30.0a7/ttkDesigner.egg-info/SOURCES.txt
+-rw-rw-r--   0 one       (1000) one       (1000)        1 2023-04-17 18:19:52.000000 ttkDesigner-0.30.0a7/ttkDesigner.egg-info/dependency_links.txt
+-rw-rw-r--   0 one       (1000) one       (1000)       49 2023-04-17 18:19:52.000000 ttkDesigner-0.30.0a7/ttkDesigner.egg-info/entry_points.txt
+-rw-rw-r--   0 one       (1000) one       (1000)       36 2023-04-17 18:19:52.000000 ttkDesigner-0.30.0a7/ttkDesigner.egg-info/requires.txt
+-rw-rw-r--   0 one       (1000) one       (1000)       12 2023-04-17 18:19:52.000000 ttkDesigner-0.30.0a7/ttkDesigner.egg-info/top_level.txt
```

### Comparing `ttkDesigner-0.30.0a5/LICENSE` & `ttkDesigner-0.30.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.30.0a5/PKG-INFO` & `ttkDesigner-0.30.0a7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: ttkDesigner
-Version: 0.30.0a5
+Version: 0.30.0a7
 Summary: ttkDesigner is a terminal user interface designer for pyTermTk applications
-Home-page: https://github.com/ceccopierangiolieugenio/ttkode
+Home-page: https://github.com/ceccopierangiolieugenio/pyTermTk
 Author: Eugenio Parodi
 Author-email: ceccopierangiolieugenio@googlemail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `ttkDesigner-0.30.0a5/README.md` & `ttkDesigner-0.30.0a7/README.md`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.30.0a5/setup.py` & `ttkDesigner-0.30.0a7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-version = "0.30.0-a5"
+version = "0.30.0-a7"
 name = "ttkDesigner"
 
 print(f"Version: {version}")
 print(f"Name: {name}")
 
 setup(
     name=name,
     version=version,
     author='Eugenio Parodi',
     author_email='ceccopierangiolieugenio@googlemail.com',
     description='ttkDesigner is a terminal user interface designer for pyTermTk applications',
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/ceccopierangiolieugenio/ttkode",
+    url="https://github.com/ceccopierangiolieugenio/pyTermTk",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Development Status :: 3 - Alpha",
         "Environment :: Console",
         "Intended Audience :: Developers",
@@ -30,14 +30,14 @@
         "Topic :: Software Development :: User Interfaces"],
     include_package_data=False,
     packages=['ttkDesigner','ttkDesigner.app'],
     python_requires=">=3.8",
     install_requires=[
         'pyTermTk>=0.30.0a5',
         'pyperclip',
-        'PIL'],
+        'Pillow'],
     entry_points={
         'console_scripts': [
             'ttkDesigner = ttkDesigner:main',
         ],
     },
 )
```

### Comparing `ttkDesigner-0.30.0a5/ttkDesigner/__init__.py` & `ttkDesigner-0.30.0a7/ttkDesigner/__init__.py`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.30.0a5/ttkDesigner/__main__.py` & `ttkDesigner-0.30.0a7/ttkDesigner/__main__.py`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.30.0a5/ttkDesigner/app/__init__.py` & `ttkDesigner-0.30.0a7/ttkDesigner/app/__init__.py`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.30.0a5/ttkDesigner/app/about.py` & `ttkDesigner-0.30.0a7/ttkDesigner/app/about.py`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.30.0a5/ttkDesigner/app/cfg.py` & `ttkDesigner-0.30.0a7/ttkDesigner/app/cfg.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,14 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import os
 # import yaml
 
 class TTkDesignerCfg:
-    version="0.30.0-a5"
+    version="0.30.0-a7"
     name="ttkDesigner"
     cfgVersion = '1.0'
     pathCfg="."
     options={}
     maxsearches=200
```

### Comparing `ttkDesigner-0.30.0a5/ttkDesigner/app/designer.py` & `ttkDesigner-0.30.0a7/ttkDesigner/app/designer.py`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.30.0a5/ttkDesigner/app/main.py` & `ttkDesigner-0.30.0a7/ttkDesigner/app/main.py`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.30.0a5/ttkDesigner/app/propertyeditor.py` & `ttkDesigner-0.30.0a7/ttkDesigner/app/propertyeditor.py`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.30.0a5/ttkDesigner/app/quickexport.py` & `ttkDesigner-0.30.0a7/ttkDesigner/app/quickexport.py`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.30.0a5/ttkDesigner/app/signalsloteditor.py` & `ttkDesigner-0.30.0a7/ttkDesigner/app/signalsloteditor.py`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.30.0a5/ttkDesigner/app/treeinspector.py` & `ttkDesigner-0.30.0a7/ttkDesigner/app/treeinspector.py`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.30.0a5/ttkDesigner/app/widgetbox.py` & `ttkDesigner-0.30.0a7/ttkDesigner/app/widgetbox.py`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.30.0a5/ttkDesigner/app/windoweditor.py` & `ttkDesigner-0.30.0a7/ttkDesigner/app/windoweditor.py`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.30.0a5/ttkDesigner.egg-info/PKG-INFO` & `ttkDesigner-0.30.0a7/ttkDesigner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: ttkDesigner
-Version: 0.30.0a5
+Version: 0.30.0a7
 Summary: ttkDesigner is a terminal user interface designer for pyTermTk applications
-Home-page: https://github.com/ceccopierangiolieugenio/ttkode
+Home-page: https://github.com/ceccopierangiolieugenio/pyTermTk
 Author: Eugenio Parodi
 Author-email: ceccopierangiolieugenio@googlemail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `ttkDesigner-0.30.0a5/ttkDesigner.egg-info/SOURCES.txt` & `ttkDesigner-0.30.0a7/ttkDesigner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

