# Comparing `tmp/hdf5view-0.0.6.tar.gz` & `tmp/hdf5view-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdf5view-0.0.6.tar", last modified: Fri Sep 30 13:22:00 2022, max compression
+gzip compressed data, was "hdf5view-0.0.7.tar", last modified: Mon Apr 17 14:15:33 2023, max compression
```

## Comparing `hdf5view-0.0.6.tar` & `hdf5view-0.0.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2022-09-30 13:22:00.091020 hdf5view-0.0.6/
--rw-rw-rw-   0        0        0     1094 2022-09-01 15:06:11.000000 hdf5view-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     7685 2022-09-30 13:22:00.088023 hdf5view-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     5342 2022-09-15 15:07:05.000000 hdf5view-0.0.6/README.md
--rw-rw-rw-   0        0        0     1590 2022-09-15 08:15:32.000000 hdf5view-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-09-30 13:22:00.092020 hdf5view-0.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-09-30 13:21:59.886138 hdf5view-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2022-09-30 13:21:59.951102 hdf5view-0.0.6/src/hdf5view/
--rw-rw-rw-   0        0        0       23 2022-09-30 13:18:09.000000 hdf5view-0.0.6/src/hdf5view/__init__.py
--rw-rw-rw-   0        0        0     2010 2022-09-30 11:46:39.000000 hdf5view-0.0.6/src/hdf5view/main.py
--rw-rw-rw-   0        0        0    14245 2022-09-30 13:05:50.000000 hdf5view-0.0.6/src/hdf5view/mainwindow.py
--rw-rw-rw-   0        0        0    16798 2022-09-07 14:51:19.000000 hdf5view-0.0.6/src/hdf5view/models.py
-drwxrwxrwx   0        0        0        0 2022-09-30 13:21:59.888137 hdf5view-0.0.6/src/hdf5view/resources/
-drwxrwxrwx   0        0        0        0 2022-09-30 13:22:00.082026 hdf5view-0.0.6/src/hdf5view/resources/images/
--rw-rw-rw-   0        0        0     4416 2022-09-01 15:06:11.000000 hdf5view-0.0.6/src/hdf5view/resources/images/dataset.svg
--rw-rw-rw-   0        0        0     3075 2022-09-01 15:06:11.000000 hdf5view-0.0.6/src/hdf5view/resources/images/folder-open.svg
--rw-rw-rw-   0        0        0     2326 2022-09-01 15:06:11.000000 hdf5view-0.0.6/src/hdf5view/resources/images/folder.svg
--rw-rw-rw-   0        0        0    14343 2022-09-01 15:35:00.000000 hdf5view-0.0.6/src/hdf5view/resources/images/hdf5view.ico
--rw-rw-rw-   0        0        0     5523 2022-09-01 15:06:11.000000 hdf5view-0.0.6/src/hdf5view/resources/images/hdf5view.svg
--rw-rw-rw-   0        0        0     2841 2022-09-01 15:35:00.000000 hdf5view-0.0.6/src/hdf5view/resources/images/image.svg
--rw-rw-rw-   0        0        0     2509 2022-09-01 15:35:00.000000 hdf5view-0.0.6/src/hdf5view/resources/images/plot.svg
--rw-rw-rw-   0        0        0    13933 2022-09-01 15:35:00.000000 hdf5view-0.0.6/src/hdf5view/views.py
-drwxrwxrwx   0        0        0        0 2022-09-30 13:22:00.021061 hdf5view-0.0.6/src/hdf5view.egg-info/
--rw-rw-rw-   0        0        0     7685 2022-09-30 13:21:59.000000 hdf5view-0.0.6/src/hdf5view.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      662 2022-09-30 13:21:59.000000 hdf5view-0.0.6/src/hdf5view.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-30 13:21:59.000000 hdf5view-0.0.6/src/hdf5view.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2022-09-30 13:21:59.000000 hdf5view-0.0.6/src/hdf5view.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       20 2022-09-30 13:21:59.000000 hdf5view-0.0.6/src/hdf5view.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-09-30 13:21:59.000000 hdf5view-0.0.6/src/hdf5view.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 14:15:33.093536 hdf5view-0.0.7/
+-rw-rw-rw-   0        0        0     1094 2022-09-01 15:06:11.000000 hdf5view-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     8177 2023-04-17 14:15:33.077911 hdf5view-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     5834 2022-12-12 13:15:02.000000 hdf5view-0.0.7/README.md
+-rw-rw-rw-   0        0        0     1590 2022-12-09 11:45:27.000000 hdf5view-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-17 14:15:33.093536 hdf5view-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-17 14:15:32.877401 hdf5view-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-04-17 14:15:32.962031 hdf5view-0.0.7/src/hdf5view/
+-rw-rw-rw-   0        0        0       23 2023-04-17 14:14:14.000000 hdf5view-0.0.7/src/hdf5view/__init__.py
+-rw-rw-rw-   0        0        0     2011 2022-12-13 08:25:45.000000 hdf5view-0.0.7/src/hdf5view/main.py
+-rw-rw-rw-   0        0        0    14417 2022-12-09 11:45:27.000000 hdf5view-0.0.7/src/hdf5view/mainwindow.py
+-rw-rw-rw-   0        0        0    19420 2022-12-12 13:01:09.000000 hdf5view-0.0.7/src/hdf5view/models.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:15:32.877401 hdf5view-0.0.7/src/hdf5view/resources/
+drwxrwxrwx   0        0        0        0 2023-04-17 14:15:33.077911 hdf5view-0.0.7/src/hdf5view/resources/images/
+-rw-rw-rw-   0        0        0     4416 2022-12-09 11:45:27.000000 hdf5view-0.0.7/src/hdf5view/resources/images/dataset.svg
+-rw-rw-rw-   0        0        0     3075 2022-12-09 11:45:27.000000 hdf5view-0.0.7/src/hdf5view/resources/images/folder-open.svg
+-rw-rw-rw-   0        0        0     2326 2022-12-09 11:45:27.000000 hdf5view-0.0.7/src/hdf5view/resources/images/folder.svg
+-rw-rw-rw-   0        0        0    14343 2022-12-09 11:45:27.000000 hdf5view-0.0.7/src/hdf5view/resources/images/hdf5view.ico
+-rw-rw-rw-   0        0        0     5523 2022-12-09 11:45:27.000000 hdf5view-0.0.7/src/hdf5view/resources/images/hdf5view.svg
+-rw-rw-rw-   0        0        0     2841 2022-12-09 11:45:27.000000 hdf5view-0.0.7/src/hdf5view/resources/images/image.svg
+-rw-rw-rw-   0        0        0     2509 2022-12-09 11:45:27.000000 hdf5view-0.0.7/src/hdf5view/resources/images/plot.svg
+-rw-rw-rw-   0        0        0    14496 2022-12-13 08:23:46.000000 hdf5view-0.0.7/src/hdf5view/views.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:15:33.015416 hdf5view-0.0.7/src/hdf5view.egg-info/
+-rw-rw-rw-   0        0        0     8177 2023-04-17 14:15:32.000000 hdf5view-0.0.7/src/hdf5view.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      662 2023-04-17 14:15:32.000000 hdf5view-0.0.7/src/hdf5view.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 14:15:32.000000 hdf5view-0.0.7/src/hdf5view.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-04-17 14:15:32.000000 hdf5view-0.0.7/src/hdf5view.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2023-04-17 14:15:32.000000 hdf5view-0.0.7/src/hdf5view.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-17 14:15:32.000000 hdf5view-0.0.7/src/hdf5view.egg-info/top_level.txt
```

### Comparing `hdf5view-0.0.6/LICENSE` & `hdf5view-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hdf5view-0.0.6/PKG-INFO` & `hdf5view-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdf5view
-Version: 0.0.6
+Version: 0.0.7
 Summary: HDF5View is a python based HDF5 file viewer built on PyQt5/PySide2/PyQt6/PySide6, QtPy, h5py and pyqtgraph.
 Author: Martin Swarbrick, Thomas G. Woodcock
 Maintainer: Thomas G. Woodcock
 License: MIT License
         
         Copyright (c) 2019 Martin Swarbrick
         
@@ -45,15 +45,15 @@
 License-File: LICENSE
 
 [![PyPI Version](https://img.shields.io/pypi/v/hdf5view.svg)](https://pypi.python.org/pypi/hdf5view/)
 [![Supported Python Versions](https://img.shields.io/pypi/pyversions/hdf5view.svg)](https://pypi.python.org/pypi/hdf5view/)
 
 # hdf5view
 
-Simple Qt/Python based viewer for HDF5 files. Displays a file tree, data tables and attributes and can render greyscale images of any nodes which have two or more dimensions. Everything is loaded dynamically, so hopefully it should be able to handle HDF5 files of any size and structure.
+Simple Qt/Python based viewer for HDF5 files. Displays a file tree, data tables and attributes and can render greyscale images of any nodes which have two or more dimensions, and rgb or rgba images of any nodes with three or more dimensions. Everything is loaded dynamically, so hopefully it should be able to handle HDF5 files of any size and structure.
 
 
 ## 1. Installing
 
 #### Qt API Bindings
 
 One of [pyqt5](https://www.riverbankcomputing.com/software/pyqt/), [pyside2](https://pyside.org), [pyqt6](https://www.riverbankcomputing.com/software/pyqt/) or [pyside6](https://pyside.org) is required in order to be able to run hdf5view. Please install one of these e.g. with pip:
@@ -172,15 +172,19 @@
 
 You can also create a desktop link to start the program for convenience. A Windows icon file hdf5view.ico is provided in the folder hdf5view/resources/images.
 
 ## 3. Usage
 
 The structure of the HDF5 file can be navigated using the tree view on the left hand side. The central panel displays a table of the data at the node selected. If the node has more than two dimensions, a 2D slice of the data is displayed in the table. On the right hand side you can see and modify the slice shown; and see details of the node and any associated attributes.
 
-To display a greyscale image of the data at a particular node, click the image icon on the toolbar at the top of the window. This will open an Image tab at the current node. The image is initially take from the last two dimensions of the node. A scrollbar is provided, which currently can be used to scroll through the first dimension of the node. You can alternatively change the slice manually and the scrollbar will move accordingly. You can have several image tabs open at once. Image tabs remember the node and slice if you switch to a different tab and back. Switching to a different node results in the default behaviour that the image shown is the last two dimensions of the first index of the first dimension.
+To display an image of a particular node, click the image icon on the toolbar at the top of the window. This will open an Image tab at the current node. You can have several image tabs open at once. Image tabs remember the node and slice if you switch to a different tab and back. Switching to a different node results in the default rendering behaviour for the image. The defaut image rendering is as follows: 
+
+* Greyscale: if the node has two or more dimensions and the shape of the last dimension is greater than 4. The image is initially taken from the last two dimensions of the node. A scrollbar is provided, which currently can be used to scroll through the first dimension of the node. This is useful for viewing a stack of greyscale images. You can alternatively change the slice manually and the scrollbar will move accordingly.
+
+* rgb or rgba: if the node has three or more dimensions and the shape of the last dimension is three or four. If the node has more than three dimensions, a scrollbar is provided, which can be used to scroll through the first dimension. This is useful for a stack of rgb or rgba images, for example.
 
 ## 4. Testing
 
 Currently there are no unit tests for this package. The gui has been tested with qtpy=2.2.0, pyqtgraph=0.12.4 and h5py=3.7.0 in combination with pyqt5=5.15.7, pyside2=5.15.2.1, pyqt6=6.3.1 and pyside6=6.3.2, and it works with all of the Qt API bindings.
 
 ## 5. Issues
```

### Comparing `hdf5view-0.0.6/README.md` & `hdf5view-0.0.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [![PyPI Version](https://img.shields.io/pypi/v/hdf5view.svg)](https://pypi.python.org/pypi/hdf5view/)
 [![Supported Python Versions](https://img.shields.io/pypi/pyversions/hdf5view.svg)](https://pypi.python.org/pypi/hdf5view/)
 
 # hdf5view
 
-Simple Qt/Python based viewer for HDF5 files. Displays a file tree, data tables and attributes and can render greyscale images of any nodes which have two or more dimensions. Everything is loaded dynamically, so hopefully it should be able to handle HDF5 files of any size and structure.
+Simple Qt/Python based viewer for HDF5 files. Displays a file tree, data tables and attributes and can render greyscale images of any nodes which have two or more dimensions, and rgb or rgba images of any nodes with three or more dimensions. Everything is loaded dynamically, so hopefully it should be able to handle HDF5 files of any size and structure.
 
 
 ## 1. Installing
 
 #### Qt API Bindings
 
 One of [pyqt5](https://www.riverbankcomputing.com/software/pyqt/), [pyside2](https://pyside.org), [pyqt6](https://www.riverbankcomputing.com/software/pyqt/) or [pyside6](https://pyside.org) is required in order to be able to run hdf5view. Please install one of these e.g. with pip:
@@ -126,15 +126,19 @@
 
 You can also create a desktop link to start the program for convenience. A Windows icon file hdf5view.ico is provided in the folder hdf5view/resources/images.
 
 ## 3. Usage
 
 The structure of the HDF5 file can be navigated using the tree view on the left hand side. The central panel displays a table of the data at the node selected. If the node has more than two dimensions, a 2D slice of the data is displayed in the table. On the right hand side you can see and modify the slice shown; and see details of the node and any associated attributes.
 
-To display a greyscale image of the data at a particular node, click the image icon on the toolbar at the top of the window. This will open an Image tab at the current node. The image is initially take from the last two dimensions of the node. A scrollbar is provided, which currently can be used to scroll through the first dimension of the node. You can alternatively change the slice manually and the scrollbar will move accordingly. You can have several image tabs open at once. Image tabs remember the node and slice if you switch to a different tab and back. Switching to a different node results in the default behaviour that the image shown is the last two dimensions of the first index of the first dimension.
+To display an image of a particular node, click the image icon on the toolbar at the top of the window. This will open an Image tab at the current node. You can have several image tabs open at once. Image tabs remember the node and slice if you switch to a different tab and back. Switching to a different node results in the default rendering behaviour for the image. The defaut image rendering is as follows: 
+
+* Greyscale: if the node has two or more dimensions and the shape of the last dimension is greater than 4. The image is initially taken from the last two dimensions of the node. A scrollbar is provided, which currently can be used to scroll through the first dimension of the node. This is useful for viewing a stack of greyscale images. You can alternatively change the slice manually and the scrollbar will move accordingly.
+
+* rgb or rgba: if the node has three or more dimensions and the shape of the last dimension is three or four. If the node has more than three dimensions, a scrollbar is provided, which can be used to scroll through the first dimension. This is useful for a stack of rgb or rgba images, for example.
 
 ## 4. Testing
 
 Currently there are no unit tests for this package. The gui has been tested with qtpy=2.2.0, pyqtgraph=0.12.4 and h5py=3.7.0 in combination with pyqt5=5.15.7, pyside2=5.15.2.1, pyqt6=6.3.1 and pyside6=6.3.2, and it works with all of the Qt API bindings.
 
 ## 5. Issues
```

### Comparing `hdf5view-0.0.6/pyproject.toml` & `hdf5view-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hdf5view-0.0.6/src/hdf5view/main.py` & `hdf5view-0.0.7/src/hdf5view/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 import os
 import sys
 import argparse
-#import traceback
+# import traceback
 
 # to force qtpy to use a particular Qt binding, uncomment the line below,
 # and set the string to your preferred binding i.e. 'pyqt5', 'pyside2',
 # 'pyqt6' or 'pyside6'. Otherwise, qtpy will take the first available of these.
 # os.environ['QT_API'] = 'pyqt5'
 
 import qtpy
```

### Comparing `hdf5view-0.0.6/src/hdf5view/mainwindow.py` & `hdf5view-0.0.7/src/hdf5view/mainwindow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # -*- coding: utf-8 -*-
 
 import os
 import h5py
 
+from qtpy import API_NAME
+
 from qtpy.QtCore import (
     Qt,
     QRect,
     QSettings,
 )
 
 from qtpy.QtGui import (
@@ -280,15 +282,18 @@
 
         # Restore the window geometry
         geometry = settings.value('geometry')
 
         if geometry and not geometry.isEmpty():
             self.restoreGeometry(geometry)
         else:
-            geometry = self.app.desktop().availableGeometry(self)
+            if API_NAME in ["PyQt6", "PySide6"]:
+                geometry = self.app.screens()[0].availableGeometry()
+            else:
+                geometry = self.app.desktop().availableGeometry(self)
             self.setGeometry(QRect(0,
                                    0,
                                    int(geometry.width() * 0.8),
                                    int(geometry.height() * 0.7)))
 
         # Restore the window state
         window_state = settings.value('windowState')
```

### Comparing `hdf5view-0.0.6/src/hdf5view/models.py` & `hdf5view-0.0.7/src/hdf5view/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -146,15 +146,18 @@
             column = index.column()
             row = index.row()
 
             if role in (Qt.DisplayRole, Qt.ToolTipRole):
                 if column == 0:
                     return self.keys[row]
                 elif column == 1:
-                    return str(self.values[row])
+                    try:
+                        return self.values[row].decode()
+                    except AttributeError:
+                        return str(self.values[row])
                 elif column == 2:
                     return str(type(self.values[row]))
 
 
 class DatasetTableModel(QAbstractTableModel):
 
     HEADERS = ('Name', 'Value')
@@ -252,23 +255,41 @@
 
             self.ndim = self.node.ndim
 
             shape = self.node.shape
 
             self.compound_names = self.node.dtype.names
 
-            if self.ndim == 1:
+            if self.ndim == 0:
+                self.row_count = 1
+                self.column_count = 1
+
+            elif self.ndim == 1:
                 self.row_count = shape[0]
 
                 if self.compound_names:
                     self.column_count = len(self.compound_names)
                 else:
                     self.column_count = 1
 
-            elif self.ndim >= 2:
+            elif self.ndim == 2:
+                self.row_count = shape[-2]
+                self.column_count = shape[-1]
+                self.dims = tuple([slice(None), slice(None)])
+                self.data_view = self.node[self.dims]
+
+            elif self.ndim > 2 and shape[-1] in [3, 4]:
+                self.row_count = shape[-3]
+                self.column_count = shape[-2]
+                self.dims = tuple(([0] * (self.ndim - 3)) + [slice(None),
+                                                             slice(None),
+                                                             slice(None)])
+                self.data_view = self.node[self.dims]
+
+            else:
                 self.row_count = shape[-2]
                 self.column_count = shape[-1]
                 self.dims = tuple(([0] * (self.ndim - 2)) + [slice(None), slice(None)])
                 self.data_view = self.node[self.dims]
 
         self.endResetModel()
 
@@ -283,35 +304,53 @@
             if self.compound_names and orientation == Qt.Horizontal:
                 return self.compound_names[section]
             else:
                 return str(section)
 
         super().headerData(section, orientation, role)
 
-    def data(self, index, role=Qt.DisplayRole):
 
+    def data(self, index, role=Qt.DisplayRole):
         if index.isValid():
             if role in (Qt.DisplayRole, Qt.ToolTipRole):
-                if self.ndim == 1:
+                if self.ndim == 0:
+                    try:
+                        q = str(self.node.asstr()[...])
+                    except TypeError:
+                        q = str(self.node[...])
+
+                elif self.ndim == 1:
                     if self.compound_names:
                         name = self.compound_names[index.column()]
-                        return str(self.node[index.row(), name])
+                        try:
+                            q = self.node[index.row(), name].decode()
+                        except AttributeError:
+                            q = str(self.node[index.row(), name])
                     else:
-                        return str(self.node[index.row()])
+                        try:
+                            q = self.node[index.row()].decode()
+                        except AttributeError:
+                            q = str(self.node[index.row()])
 
                 elif self.ndim == 2:
-                    return str(self.node[index.row(), index.column()])
+                    try:
+                        q = self.node[index.row(), index.column()].decode()
+                    except AttributeError:
+                        q = str(self.node[index.row(), index.column()])
 
                 elif self.ndim > 2:
                     if self.data_view.ndim == 0:
-                        return str(self.data_view)
+                        q = str(self.data_view)
                     elif self.data_view.ndim == 1:
-                        return str(self.data_view[index.row()])
+                        q = str(self.data_view[index.row()])
                     elif self.data_view.ndim >= 2:
-                        return str(self.data_view[index.row(), index.column()])
+                        q = str(self.data_view[index.row(), index.column()])
+
+                return q
+
 
     def set_dims(self, dims):
 
         self.beginResetModel()
 
         self.row_count = None
         self.column_count = None
@@ -384,26 +423,45 @@
 
             self.ndim = self.node.ndim
 
             shape = self.node.shape
 
             self.compound_names = self.node.dtype.names
 
-            if self.ndim == 1:
+            if self.ndim == 0:
+                self.row_count = 1
+                self.column_count = 1
+
+            elif self.ndim == 1:
                 self.row_count = shape[0]
 
                 if self.compound_names:
                     self.column_count = len(self.compound_names)
                 else:
                     self.column_count = 1
 
-            elif self.ndim >= 2:
+            elif self.ndim == 2:
                 self.row_count = shape[-2]
                 self.column_count = shape[-1]
-                self.dims = tuple(([0] * (self.ndim - 2)) + [slice(None), slice(None)])
+                self.dims = tuple([slice(None), slice(None)])
+                self.image_view = self.node[self.dims]
+
+            elif self.ndim > 2 and shape[-1] in [3, 4]:
+                self.row_count = shape[-3]
+                self.column_count = shape[-2]
+                self.dims = tuple(([0] * (self.ndim - 3)) + [slice(None),
+                                                             slice(None),
+                                                             slice(None)])
+                self.image_view = self.node[self.dims]
+
+            else:
+                self.row_count = shape[-2]
+                self.column_count = shape[-1]
+                self.dims = tuple(([0] * (self.ndim - 2)) + [slice(None),
+                                                             slice(None)])
                 self.image_view = self.node[self.dims]
 
         self.endResetModel()
 
     def parent(self, childIndex=QModelIndex()):
         return self.createIndex()
 
@@ -490,16 +548,21 @@
         self.column_count = 0
         self.shape = []
 
         self.beginResetModel()
         self.node = self.hdf[path]
 
         if isinstance(self.node, h5py.Dataset) and self.node.ndim > 2:
-            self.shape = (['0'] * (self.node.ndim - 2)) + [':', ':']
-            self.column_count = len(self.shape)
+            if self.node.shape[-1] in [3, 4]:
+                self.shape = (['0'] * (self.node.ndim - 3)) + [':', ':', ':']
+                self.column_count = len(self.shape)
+
+            else:
+                self.shape = (['0'] * (self.node.ndim - 2)) + [':', ':']
+                self.column_count = len(self.shape)
 
         self.endResetModel()
 
     def rowCount(self, parent=QModelIndex()):
         return self.row_count
 
     def columnCount(self, parent=QModelIndex()):
```

### Comparing `hdf5view-0.0.6/src/hdf5view/resources/images/dataset.svg` & `hdf5view-0.0.7/src/hdf5view/resources/images/dataset.svg`

 * *Files identical despite different names*

### Comparing `hdf5view-0.0.6/src/hdf5view/resources/images/folder-open.svg` & `hdf5view-0.0.7/src/hdf5view/resources/images/folder-open.svg`

 * *Files identical despite different names*

### Comparing `hdf5view-0.0.6/src/hdf5view/resources/images/folder.svg` & `hdf5view-0.0.7/src/hdf5view/resources/images/folder.svg`

 * *Files identical despite different names*

### Comparing `hdf5view-0.0.6/src/hdf5view/resources/images/hdf5view.ico` & `hdf5view-0.0.7/src/hdf5view/resources/images/hdf5view.ico`

 * *Files identical despite different names*

### Comparing `hdf5view-0.0.6/src/hdf5view/resources/images/hdf5view.svg` & `hdf5view-0.0.7/src/hdf5view/resources/images/hdf5view.svg`

 * *Files identical despite different names*

### Comparing `hdf5view-0.0.6/src/hdf5view/resources/images/image.svg` & `hdf5view-0.0.7/src/hdf5view/resources/images/image.svg`

 * *Files identical despite different names*

### Comparing `hdf5view-0.0.6/src/hdf5view/resources/images/plot.svg` & `hdf5view-0.0.7/src/hdf5view/resources/images/plot.svg`

 * *Files identical despite different names*

### Comparing `hdf5view-0.0.6/src/hdf5view/views.py` & `hdf5view-0.0.7/src/hdf5view/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -368,15 +368,16 @@
 
     def init_signals(self):
         self.image_item.scene().sigMouseMoved.connect(self.handle_mouse_moved)
         self.scrollbar.valueChanged.connect(self.handle_scroll)
 
 
     def update_image(self):
-        if len(self.model().dims) < 2:
+        small = self.model().ndim == 2 and any([i == 1 for i in self.model().node.shape])
+        if self.model().ndim < 2 or small:
             if self.viewbox.isVisible():
                 self.viewbox.setVisible(False)
 
             if self.scrollbar.isVisible():
                 self.scrollbar.blockSignals(True)
                 self.scrollbar.setVisible(False)
                 self.scrollbar.blockSignals(False)
@@ -418,24 +419,35 @@
 
     def handle_mouse_moved(self, pos):
         """
         Update the cursor position when the mouse moves
         in the image scene.
         """
         if self.image_item.image is not None and len(self.model().dims) >= 2:
-            max_y, max_x = self.image_item.image.shape
+            try:
+                max_y, max_x = self.image_item.image.shape
+            except ValueError:
+                max_y, max_x, max_z = self.image_item.image.shape
 
             scene_pos = self.viewbox.mapSceneToView(pos)
 
             x = int(scene_pos.x())
             y = int(scene_pos.y())
 
             if 0 <= x < max_x and 0 <= y < max_y:
                 I = self.model().image_view[y,x]
-                self.window().status.showMessage(f"X={x} Y={y}, value={I:.3e}")
+                msg1 = f"X={x} Y={y}, value="
+                try:
+                    msg2 = f"{I:.3e}"
+                except TypeError:
+                    try:
+                        msg2 = f"[{I[0]:.3e}, {I[1]:.3e}, {I[2]:.3e}, {I[3]:.3e}]"
+                    except IndexError:
+                        msg2 = f"[{I[0]:.3e}, {I[1]:.3e}, {I[2]:.3e}]"
+                self.window().status.showMessage(msg1 + msg2)
                 self.viewbox.setCursor(Qt.CrossCursor)
             else:
                 self.window().status.showMessage('')
                 self.viewbox.setCursor(Qt.ArrowCursor)
 
 
     def horizontalOffset(self):
```

### Comparing `hdf5view-0.0.6/src/hdf5view.egg-info/PKG-INFO` & `hdf5view-0.0.7/src/hdf5view.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdf5view
-Version: 0.0.6
+Version: 0.0.7
 Summary: HDF5View is a python based HDF5 file viewer built on PyQt5/PySide2/PyQt6/PySide6, QtPy, h5py and pyqtgraph.
 Author: Martin Swarbrick, Thomas G. Woodcock
 Maintainer: Thomas G. Woodcock
 License: MIT License
         
         Copyright (c) 2019 Martin Swarbrick
         
@@ -45,15 +45,15 @@
 License-File: LICENSE
 
 [![PyPI Version](https://img.shields.io/pypi/v/hdf5view.svg)](https://pypi.python.org/pypi/hdf5view/)
 [![Supported Python Versions](https://img.shields.io/pypi/pyversions/hdf5view.svg)](https://pypi.python.org/pypi/hdf5view/)
 
 # hdf5view
 
-Simple Qt/Python based viewer for HDF5 files. Displays a file tree, data tables and attributes and can render greyscale images of any nodes which have two or more dimensions. Everything is loaded dynamically, so hopefully it should be able to handle HDF5 files of any size and structure.
+Simple Qt/Python based viewer for HDF5 files. Displays a file tree, data tables and attributes and can render greyscale images of any nodes which have two or more dimensions, and rgb or rgba images of any nodes with three or more dimensions. Everything is loaded dynamically, so hopefully it should be able to handle HDF5 files of any size and structure.
 
 
 ## 1. Installing
 
 #### Qt API Bindings
 
 One of [pyqt5](https://www.riverbankcomputing.com/software/pyqt/), [pyside2](https://pyside.org), [pyqt6](https://www.riverbankcomputing.com/software/pyqt/) or [pyside6](https://pyside.org) is required in order to be able to run hdf5view. Please install one of these e.g. with pip:
@@ -172,15 +172,19 @@
 
 You can also create a desktop link to start the program for convenience. A Windows icon file hdf5view.ico is provided in the folder hdf5view/resources/images.
 
 ## 3. Usage
 
 The structure of the HDF5 file can be navigated using the tree view on the left hand side. The central panel displays a table of the data at the node selected. If the node has more than two dimensions, a 2D slice of the data is displayed in the table. On the right hand side you can see and modify the slice shown; and see details of the node and any associated attributes.
 
-To display a greyscale image of the data at a particular node, click the image icon on the toolbar at the top of the window. This will open an Image tab at the current node. The image is initially take from the last two dimensions of the node. A scrollbar is provided, which currently can be used to scroll through the first dimension of the node. You can alternatively change the slice manually and the scrollbar will move accordingly. You can have several image tabs open at once. Image tabs remember the node and slice if you switch to a different tab and back. Switching to a different node results in the default behaviour that the image shown is the last two dimensions of the first index of the first dimension.
+To display an image of a particular node, click the image icon on the toolbar at the top of the window. This will open an Image tab at the current node. You can have several image tabs open at once. Image tabs remember the node and slice if you switch to a different tab and back. Switching to a different node results in the default rendering behaviour for the image. The defaut image rendering is as follows: 
+
+* Greyscale: if the node has two or more dimensions and the shape of the last dimension is greater than 4. The image is initially taken from the last two dimensions of the node. A scrollbar is provided, which currently can be used to scroll through the first dimension of the node. This is useful for viewing a stack of greyscale images. You can alternatively change the slice manually and the scrollbar will move accordingly.
+
+* rgb or rgba: if the node has three or more dimensions and the shape of the last dimension is three or four. If the node has more than three dimensions, a scrollbar is provided, which can be used to scroll through the first dimension. This is useful for a stack of rgb or rgba images, for example.
 
 ## 4. Testing
 
 Currently there are no unit tests for this package. The gui has been tested with qtpy=2.2.0, pyqtgraph=0.12.4 and h5py=3.7.0 in combination with pyqt5=5.15.7, pyside2=5.15.2.1, pyqt6=6.3.1 and pyside6=6.3.2, and it works with all of the Qt API bindings.
 
 ## 5. Issues
```

### Comparing `hdf5view-0.0.6/src/hdf5view.egg-info/SOURCES.txt` & `hdf5view-0.0.7/src/hdf5view.egg-info/SOURCES.txt`

 * *Files identical despite different names*

