# Comparing `tmp/simple_parquet_viewer-0.9.0.tar.gz` & `tmp/simple_parquet_viewer-0.9.1.tar.gz`

## Comparing `simple_parquet_viewer-0.9.0.tar` & `simple_parquet_viewer-0.9.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.0/requirements-dev.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.0/src/simple_parquet_viewer/__init__.py
--rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.0/src/simple_parquet_viewer/main.py
--rw-r--r--   0        0        0   165496 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.0/src/simple_parquet_viewer/res/imgs/app_icon.ico
--rw-r--r--   0        0        0    11584 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.0/src/simple_parquet_viewer/res/imgs/app_icon.svg
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.0/src/simple_parquet_viewer/res/imgs/apply.png
--rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.0/src/simple_parquet_viewer/res/imgs/apply.svg
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.0/src/simple_parquet_viewer/res/imgs/clear.png
--rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.0/src/simple_parquet_viewer/res/imgs/clear.svg
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.0/src/simple_parquet_viewer/res/imgs/filter.png
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.0/src/simple_parquet_viewer/res/imgs/filter.svg
--rw-r--r--   0        0        0     6540 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.0/src/simple_parquet_viewer/res/imgs/info.png
--rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.0/src/simple_parquet_viewer/res/imgs/info.svg
--rw-r--r--   0        0        0     8006 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.0/src/simple_parquet_viewer/res/imgs/info_qt.png
--rw-r--r--   0        0        0     3260 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.0/src/simple_parquet_viewer/res/imgs/info_qt.svg
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.0/src/simple_parquet_viewer/res/imgs/open.png
--rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.0/src/simple_parquet_viewer/res/imgs/open.svg
--rw-r--r--   0        0        0     4209 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.0/src/simple_parquet_viewer/res/imgs/save_csv.png
--rw-r--r--   0        0        0     7681 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.0/src/simple_parquet_viewer/res/imgs/save_csv.svg
--rw-r--r--   0        0        0     4332 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.0/src/simple_parquet_viewer/res/imgs/save_json.png
--rw-r--r--   0        0        0     8352 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.0/src/simple_parquet_viewer/res/imgs/save_json.svg
--rw-r--r--   0        0        0     4770 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.0/src/simple_parquet_viewer/res/imgs/save_parquet.png
--rw-r--r--   0        0        0    12461 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.0/src/simple_parquet_viewer/res/imgs/save_parquet.svg
--rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.0/src/simple_parquet_viewer/res/stylesheet/dark.css
--rw-r--r--   0        0        0     5468 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.0/src/simple_parquet_viewer/res/translations/pt.qm
--rw-r--r--   0        0        0     8541 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.0/src/simple_parquet_viewer/res/translations/pt.ts
--rw-r--r--   0        0        0    13602 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.0/src/simple_parquet_viewer/widgets/mainwindow.py
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.0/.gitignore
--rw-r--r--   0        0        0    35821 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.0/LICENCE.txt
--rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.0/README.md
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     4652 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.1/requirements-dev.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.1/src/simple_parquet_viewer/__init__.py
+-rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.1/src/simple_parquet_viewer/main.py
+-rw-r--r--   0        0        0   165496 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.1/src/simple_parquet_viewer/res/imgs/app_icon.ico
+-rw-r--r--   0        0        0    11584 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.1/src/simple_parquet_viewer/res/imgs/app_icon.svg
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.1/src/simple_parquet_viewer/res/imgs/apply.png
+-rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.1/src/simple_parquet_viewer/res/imgs/apply.svg
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.1/src/simple_parquet_viewer/res/imgs/clear.png
+-rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.1/src/simple_parquet_viewer/res/imgs/clear.svg
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.1/src/simple_parquet_viewer/res/imgs/filter.png
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.1/src/simple_parquet_viewer/res/imgs/filter.svg
+-rw-r--r--   0        0        0     6540 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.1/src/simple_parquet_viewer/res/imgs/info.png
+-rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.1/src/simple_parquet_viewer/res/imgs/info.svg
+-rw-r--r--   0        0        0     8006 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.1/src/simple_parquet_viewer/res/imgs/info_qt.png
+-rw-r--r--   0        0        0     3260 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.1/src/simple_parquet_viewer/res/imgs/info_qt.svg
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.1/src/simple_parquet_viewer/res/imgs/open.png
+-rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.1/src/simple_parquet_viewer/res/imgs/open.svg
+-rw-r--r--   0        0        0     4209 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.1/src/simple_parquet_viewer/res/imgs/save_csv.png
+-rw-r--r--   0        0        0     7681 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.1/src/simple_parquet_viewer/res/imgs/save_csv.svg
+-rw-r--r--   0        0        0     4332 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.1/src/simple_parquet_viewer/res/imgs/save_json.png
+-rw-r--r--   0        0        0     8352 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.1/src/simple_parquet_viewer/res/imgs/save_json.svg
+-rw-r--r--   0        0        0     4770 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.1/src/simple_parquet_viewer/res/imgs/save_parquet.png
+-rw-r--r--   0        0        0    12461 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.1/src/simple_parquet_viewer/res/imgs/save_parquet.svg
+-rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.1/src/simple_parquet_viewer/res/stylesheet/dark.css
+-rw-r--r--   0        0        0     5468 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.1/src/simple_parquet_viewer/res/translations/pt.qm
+-rw-r--r--   0        0        0     8541 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.1/src/simple_parquet_viewer/res/translations/pt.ts
+-rw-r--r--   0        0        0    13602 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.1/src/simple_parquet_viewer/widgets/mainwindow.py
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.1/.gitignore
+-rw-r--r--   0        0        0    35821 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.1/LICENCE.txt
+-rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.1/README.md
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 simple_parquet_viewer-0.9.1/PKG-INFO
```

### Comparing `simple_parquet_viewer-0.9.0/requirements-dev.txt` & `simple_parquet_viewer-0.9.1/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `simple_parquet_viewer-0.9.0/src/simple_parquet_viewer/main.py` & `simple_parquet_viewer-0.9.1/src/simple_parquet_viewer/main.py`

 * *Files identical despite different names*

### Comparing `simple_parquet_viewer-0.9.0/src/simple_parquet_viewer/res/imgs/app_icon.ico` & `simple_parquet_viewer-0.9.1/src/simple_parquet_viewer/res/imgs/app_icon.ico`

 * *Files identical despite different names*

### Comparing `simple_parquet_viewer-0.9.0/src/simple_parquet_viewer/res/imgs/app_icon.svg` & `simple_parquet_viewer-0.9.1/src/simple_parquet_viewer/res/imgs/app_icon.svg`

 * *Files identical despite different names*

### Comparing `simple_parquet_viewer-0.9.0/src/simple_parquet_viewer/res/imgs/apply.png` & `simple_parquet_viewer-0.9.1/src/simple_parquet_viewer/res/imgs/apply.png`

 * *Files identical despite different names*

### Comparing `simple_parquet_viewer-0.9.0/src/simple_parquet_viewer/res/imgs/apply.svg` & `simple_parquet_viewer-0.9.1/src/simple_parquet_viewer/res/imgs/apply.svg`

 * *Files identical despite different names*

### Comparing `simple_parquet_viewer-0.9.0/src/simple_parquet_viewer/res/imgs/clear.svg` & `simple_parquet_viewer-0.9.1/src/simple_parquet_viewer/res/imgs/clear.svg`

 * *Files identical despite different names*

### Comparing `simple_parquet_viewer-0.9.0/src/simple_parquet_viewer/res/imgs/filter.png` & `simple_parquet_viewer-0.9.1/src/simple_parquet_viewer/res/imgs/filter.png`

 * *Files identical despite different names*

### Comparing `simple_parquet_viewer-0.9.0/src/simple_parquet_viewer/res/imgs/filter.svg` & `simple_parquet_viewer-0.9.1/src/simple_parquet_viewer/res/imgs/filter.svg`

 * *Files identical despite different names*

### Comparing `simple_parquet_viewer-0.9.0/src/simple_parquet_viewer/res/imgs/info.png` & `simple_parquet_viewer-0.9.1/src/simple_parquet_viewer/res/imgs/info.png`

 * *Files identical despite different names*

### Comparing `simple_parquet_viewer-0.9.0/src/simple_parquet_viewer/res/imgs/info.svg` & `simple_parquet_viewer-0.9.1/src/simple_parquet_viewer/res/imgs/info.svg`

 * *Files identical despite different names*

### Comparing `simple_parquet_viewer-0.9.0/src/simple_parquet_viewer/res/imgs/info_qt.png` & `simple_parquet_viewer-0.9.1/src/simple_parquet_viewer/res/imgs/info_qt.png`

 * *Files identical despite different names*

### Comparing `simple_parquet_viewer-0.9.0/src/simple_parquet_viewer/res/imgs/info_qt.svg` & `simple_parquet_viewer-0.9.1/src/simple_parquet_viewer/res/imgs/info_qt.svg`

 * *Files identical despite different names*

### Comparing `simple_parquet_viewer-0.9.0/src/simple_parquet_viewer/res/imgs/open.png` & `simple_parquet_viewer-0.9.1/src/simple_parquet_viewer/res/imgs/open.png`

 * *Files identical despite different names*

### Comparing `simple_parquet_viewer-0.9.0/src/simple_parquet_viewer/res/imgs/open.svg` & `simple_parquet_viewer-0.9.1/src/simple_parquet_viewer/res/imgs/open.svg`

 * *Files identical despite different names*

### Comparing `simple_parquet_viewer-0.9.0/src/simple_parquet_viewer/res/imgs/save_csv.png` & `simple_parquet_viewer-0.9.1/src/simple_parquet_viewer/res/imgs/save_csv.png`

 * *Files identical despite different names*

### Comparing `simple_parquet_viewer-0.9.0/src/simple_parquet_viewer/res/imgs/save_csv.svg` & `simple_parquet_viewer-0.9.1/src/simple_parquet_viewer/res/imgs/save_csv.svg`

 * *Files identical despite different names*

### Comparing `simple_parquet_viewer-0.9.0/src/simple_parquet_viewer/res/imgs/save_json.png` & `simple_parquet_viewer-0.9.1/src/simple_parquet_viewer/res/imgs/save_json.png`

 * *Files identical despite different names*

### Comparing `simple_parquet_viewer-0.9.0/src/simple_parquet_viewer/res/imgs/save_json.svg` & `simple_parquet_viewer-0.9.1/src/simple_parquet_viewer/res/imgs/save_json.svg`

 * *Files identical despite different names*

### Comparing `simple_parquet_viewer-0.9.0/src/simple_parquet_viewer/res/imgs/save_parquet.png` & `simple_parquet_viewer-0.9.1/src/simple_parquet_viewer/res/imgs/save_parquet.png`

 * *Files identical despite different names*

### Comparing `simple_parquet_viewer-0.9.0/src/simple_parquet_viewer/res/imgs/save_parquet.svg` & `simple_parquet_viewer-0.9.1/src/simple_parquet_viewer/res/imgs/save_parquet.svg`

 * *Files identical despite different names*

### Comparing `simple_parquet_viewer-0.9.0/src/simple_parquet_viewer/res/stylesheet/dark.css` & `simple_parquet_viewer-0.9.1/src/simple_parquet_viewer/res/stylesheet/dark.css`

 * *Files identical despite different names*

### Comparing `simple_parquet_viewer-0.9.0/src/simple_parquet_viewer/res/translations/pt.qm` & `simple_parquet_viewer-0.9.1/src/simple_parquet_viewer/res/translations/pt.qm`

 * *Files identical despite different names*

### Comparing `simple_parquet_viewer-0.9.0/src/simple_parquet_viewer/res/translations/pt.ts` & `simple_parquet_viewer-0.9.1/src/simple_parquet_viewer/res/translations/pt.ts`

 * *Files identical despite different names*

### Comparing `simple_parquet_viewer-0.9.0/src/simple_parquet_viewer/widgets/mainwindow.py` & `simple_parquet_viewer-0.9.1/src/simple_parquet_viewer/widgets/mainwindow.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 )
 from PyQt6.QtWidgets import (
     QMainWindow, QTableView, QWidget, QApplication, QToolBar,
     QVBoxLayout, QToolButton, QStatusBar, QVBoxLayout, QLabel,
     QProgressBar, QFileDialog, QMessageBox, QHBoxLayout, QLineEdit
 )
 
-APP_VERSION = (0, 9, 0)
+APP_VERSION = (0, 9, 1)
 
 def imgPath(fileName: str) -> str:
     return os.path.join(os.environ["SPV_SD_"], "res", "imgs", fileName)
 
 class ExportType(Enum):
     CSV = 1
     JSON = 2
```

### Comparing `simple_parquet_viewer-0.9.0/.gitignore` & `simple_parquet_viewer-0.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `simple_parquet_viewer-0.9.0/LICENCE.txt` & `simple_parquet_viewer-0.9.1/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `simple_parquet_viewer-0.9.0/README.md` & `simple_parquet_viewer-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `simple_parquet_viewer-0.9.0/pyproject.toml` & `simple_parquet_viewer-0.9.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "simple-parquet-viewer"
-version = "0.9.0"
+version = "0.9.1"
 authors = [
   { name="Mauro Mascarenhas de Araújo", email="mauromascarenhas@users.noreply.github.com" },
 ]
 description = "A simple (and lightweight) visualization tool for Parquet files."
 license = "GPL-3.0-or-later"
 readme = "README.md"
 requires-python = ">=3.7"
@@ -19,18 +19,18 @@
 ]
 keywords = [
     "Parquet",
     "GUI",
     "Viewer"
 ]
 dependencies = [
-    "numpy~=1.24.2",
-    "pandas~=2.0.0",
+    "numpy>=1.24",
+    "pandas>=2.0",
     "pyarrow",
-    "PyQt6~=6.5.0"
+    "PyQt6~=6.5"
 ]
 
 [project.optional-dependencies]
 windows = [
     "pywin32>=306"
 ]
```

### Comparing `simple_parquet_viewer-0.9.0/PKG-INFO` & `simple_parquet_viewer-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: simple-parquet-viewer
-Version: 0.9.0
+Version: 0.9.1
 Summary: A simple (and lightweight) visualization tool for Parquet files.
 Project-URL: Homepage, https://github.com/mauromascarenhas/simple-parquet-viewer
 Project-URL: Bug Tracker, https://github.com/mauromascarenhas/simple-parquet-viewer/issues
 Author-email: Mauro Mascarenhas de Araújo <mauromascarenhas@users.noreply.github.com>
 License-Expression: GPL-3.0-or-later
 License-File: LICENCE.txt
 Keywords: GUI,Parquet,Viewer
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
-Requires-Dist: numpy~=1.24.2
-Requires-Dist: pandas~=2.0.0
+Requires-Dist: numpy>=1.24
+Requires-Dist: pandas>=2.0
 Requires-Dist: pyarrow
-Requires-Dist: pyqt6~=6.5.0
+Requires-Dist: pyqt6~=6.5
 Provides-Extra: windows
 Requires-Dist: pywin32>=306; extra == 'windows'
 Description-Content-Type: text/markdown
 
 # Simple Parquet Viewer
 
 A simple (and lightweight) visualization tool for Parquet files.
```

