# Comparing `tmp/napari-vodex-1.0.11.tar.gz` & `tmp/napari-vodex-1.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-vodex-1.0.11.tar", last modified: Sat Feb  4 00:21:35 2023, max compression
+gzip compressed data, was "napari-vodex-1.0.12.tar", last modified: Mon Apr 17 01:30:46 2023, max compression
```

## Comparing `napari-vodex-1.0.11.tar` & `napari-vodex-1.0.12.tar`

### file list

```diff
@@ -1,34 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 00:21:35.528872 napari-vodex-1.0.11/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 00:21:35.520872 napari-vodex-1.0.11/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 00:21:35.524872 napari-vodex-1.0.11/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-02-04 00:21:08.000000 napari-vodex-1.0.11/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-02-04 00:21:08.000000 napari-vodex-1.0.11/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 00:21:35.524872 napari-vodex-1.0.11/.napari-hub/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-02-04 00:21:08.000000 napari-vodex-1.0.11/.napari-hub/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-02-04 00:21:08.000000 napari-vodex-1.0.11/.napari-hub/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-02-04 00:21:08.000000 napari-vodex-1.0.11/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-02-04 00:21:08.000000 napari-vodex-1.0.11/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-04 00:21:08.000000 napari-vodex-1.0.11/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-02-04 00:21:35.528872 napari-vodex-1.0.11/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-02-04 00:21:08.000000 napari-vodex-1.0.11/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-02-04 00:21:08.000000 napari-vodex-1.0.11/desktop.ini
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-02-04 00:21:08.000000 napari-vodex-1.0.11/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-02-04 00:21:35.528872 napari-vodex-1.0.11/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 00:21:35.520872 napari-vodex-1.0.11/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 00:21:35.528872 napari-vodex-1.0.11/src/napari_vodex/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-02-04 00:21:08.000000 napari-vodex-1.0.11/src/napari_vodex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 00:21:35.528872 napari-vodex-1.0.11/src/napari_vodex/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-04 00:21:08.000000 napari-vodex-1.0.11/src/napari_vodex/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-04 00:21:08.000000 napari-vodex-1.0.11/src/napari_vodex/_tests/test_VodexModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-02-04 00:21:08.000000 napari-vodex-1.0.11/src/napari_vodex/_tests/test_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-02-04 00:21:35.000000 napari-vodex-1.0.11/src/napari_vodex/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    66517 2023-02-04 00:21:08.000000 napari-vodex-1.0.11/src/napari_vodex/_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-02-04 00:21:08.000000 napari-vodex-1.0.11/src/napari_vodex/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 00:21:35.528872 napari-vodex-1.0.11/src/napari_vodex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-02-04 00:21:35.000000 napari-vodex-1.0.11/src/napari_vodex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-02-04 00:21:35.000000 napari-vodex-1.0.11/src/napari_vodex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-04 00:21:35.000000 napari-vodex-1.0.11/src/napari_vodex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-02-04 00:21:35.000000 napari-vodex-1.0.11/src/napari_vodex.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-02-04 00:21:35.000000 napari-vodex-1.0.11/src/napari_vodex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-04 00:21:35.000000 napari-vodex-1.0.11/src/napari_vodex.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-02-04 00:21:08.000000 napari-vodex-1.0.11/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 01:30:46.025181 napari-vodex-1.0.12/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 01:30:46.021181 napari-vodex-1.0.12/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 01:30:46.021181 napari-vodex-1.0.12/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-04-17 01:30:25.000000 napari-vodex-1.0.12/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-17 01:30:25.000000 napari-vodex-1.0.12/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 01:30:46.021181 napari-vodex-1.0.12/.napari-hub/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-17 01:30:25.000000 napari-vodex-1.0.12/.napari-hub/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-17 01:30:25.000000 napari-vodex-1.0.12/.napari-hub/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-17 01:30:25.000000 napari-vodex-1.0.12/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-17 01:30:25.000000 napari-vodex-1.0.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-17 01:30:25.000000 napari-vodex-1.0.12/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-04-17 01:30:46.025181 napari-vodex-1.0.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-04-17 01:30:25.000000 napari-vodex-1.0.12/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-17 01:30:25.000000 napari-vodex-1.0.12/desktop.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-17 01:30:25.000000 napari-vodex-1.0.12/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-17 01:30:46.025181 napari-vodex-1.0.12/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 01:30:46.021181 napari-vodex-1.0.12/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 01:30:46.025181 napari-vodex-1.0.12/src/napari_vodex/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-17 01:30:25.000000 napari-vodex-1.0.12/src/napari_vodex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23792 2023-04-17 01:30:25.000000 napari-vodex-1.0.12/src/napari_vodex/_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7834 2023-04-17 01:30:25.000000 napari-vodex-1.0.12/src/napari_vodex/_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 01:30:46.025181 napari-vodex-1.0.12/src/napari_vodex/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 01:30:25.000000 napari-vodex-1.0.12/src/napari_vodex/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 01:30:25.000000 napari-vodex-1.0.12/src/napari_vodex/_tests/test_VodexModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-17 01:30:25.000000 napari-vodex-1.0.12/src/napari_vodex/_tests/test_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-17 01:30:45.000000 napari-vodex-1.0.12/src/napari_vodex/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42391 2023-04-17 01:30:25.000000 napari-vodex-1.0.12/src/napari_vodex/_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-17 01:30:25.000000 napari-vodex-1.0.12/src/napari_vodex/_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-17 01:30:25.000000 napari-vodex-1.0.12/src/napari_vodex/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 01:30:46.025181 napari-vodex-1.0.12/src/napari_vodex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-04-17 01:30:45.000000 napari-vodex-1.0.12/src/napari_vodex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-17 01:30:46.000000 napari-vodex-1.0.12/src/napari_vodex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 01:30:45.000000 napari-vodex-1.0.12/src/napari_vodex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-17 01:30:45.000000 napari-vodex-1.0.12/src/napari_vodex.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-17 01:30:45.000000 napari-vodex-1.0.12/src/napari_vodex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-17 01:30:45.000000 napari-vodex-1.0.12/src/napari_vodex.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-17 01:30:25.000000 napari-vodex-1.0.12/tox.ini
```

### Comparing `napari-vodex-1.0.11/.github/workflows/test_and_deploy.yml` & `napari-vodex-1.0.12/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `napari-vodex-1.0.11/.gitignore` & `napari-vodex-1.0.12/.gitignore`

 * *Files identical despite different names*

### Comparing `napari-vodex-1.0.11/.napari-hub/config.yml` & `napari-vodex-1.0.12/.napari-hub/config.yml`

 * *Files identical despite different names*

### Comparing `napari-vodex-1.0.11/.pre-commit-config.yaml` & `napari-vodex-1.0.12/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `napari-vodex-1.0.11/LICENSE` & `napari-vodex-1.0.12/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-vodex-1.0.11/PKG-INFO` & `napari-vodex-1.0.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: napari-vodex
-Version: 1.0.11
+Version: 1.0.12
 Summary: A napari plugin for VoDEx : Volumetric Data and Experiment Manager. Allows to load volumetric data based on experimental conditions.
 Home-page: https://github.com/LemonJust/napari-vodex
 Author: Anna Nadtochiy
 Author-email: lemonjustgithub@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/LemonJust/napari-vodex/issues
 Project-URL: Documentation, https://lemonjust.github.io/vodex/napari/
 Project-URL: Source Code, https://github.com/LemonJust/napari-vodex
 Project-URL: User Support, https://github.com/LemonJust/napari-vodex/issues
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: napari
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `napari-vodex-1.0.11/README.md` & `napari-vodex-1.0.12/README.md`

 * *Files identical despite different names*

### Comparing `napari-vodex-1.0.11/setup.cfg` & `napari-vodex-1.0.12/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 long_description_content_type = text/markdown
 url = https://github.com/LemonJust/napari-vodex
 author = Anna Nadtochiy
 author_email = lemonjustgithub@gmail.com
 license = BSD-3-Clause
 license_files = LICENSE
 classifiers = 
-	Development Status :: 2 - Pre-Alpha
+	Development Status :: 3 - Alpha
 	Framework :: napari
 	Intended Audience :: Developers
 	License :: OSI Approved :: BSD License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
@@ -26,15 +26,15 @@
 	Documentation = https://lemonjust.github.io/vodex/napari/
 	Source Code = https://github.com/LemonJust/napari-vodex
 	User Support = https://github.com/LemonJust/napari-vodex/issues
 
 [options]
 packages = find:
 install_requires = 
-	vodex >=1.0.7
+	vodex >=1.0.12
 	numpy
 	magicgui
 	qtpy
 python_requires = >=3.8
 include_package_data = True
 package_dir = 
 	=src
```

### Comparing `napari-vodex-1.0.11/src/napari_vodex/_tests/test_widget.py` & `napari-vodex-1.0.12/src/napari_vodex/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari-vodex-1.0.11/src/napari_vodex/_widget.py` & `napari-vodex-1.0.12/src/napari_vodex/_view.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,9 @@
-"""
-This module is an example of a barebones QWidget plugin for napari
-
-For Widget specification see: https://napari.org/stable/plugins/guides.html?#widgets
-
-"""
-from typing import TYPE_CHECKING, List, Union
-from pathlib import Path
-
-from magicgui import magic_factory
-from qtpy.QtWidgets import \
-    QHBoxLayout, QPushButton, QWidget
-
-if TYPE_CHECKING:
-    import napari
-
-# imports info: https://napari.org/stable/plugins/best_practices.html :
-# Don’t import from PyQt5 or PySide2 in your plugin: use qtpy. If you use from PyQt5 import QtCore (or similar) in
-# your plugin, but the end-user has chosen to use PySide2 for their Qt backend — or vice versa — then your plugin
-# will fail to import. Instead use from qtpy import   QtCore. qtpy is a Qt compatibility layer that will import from
-# whatever backend is installed in the environment.
-
-
+from typing import List
 from pathlib import Path
-from typing import Union
 
 from qtpy.QtCore import Qt, QRegExp, QModelIndex
 from qtpy.QtGui import QRegExpValidator
 from qtpy.QtWidgets import (
 
     QAbstractItemView,
     QComboBox,
@@ -49,31 +26,30 @@
     QStyledItemDelegate,
     QStyle,
     QCheckBox,
     QPushButton,
     QVBoxLayout,
     QHBoxLayout,
     QFrame,
-    QLabel,
-    QApplication
+    QLabel
 )
 
 import vodex as vx
-import napari
 
 
 # _______________________________________________________________________________
 # Collapsable implementation can be also found
 # https://stackoverflow.com/questions/52615115/how-to-create-collapsible-box-in-pyqt
 
+
 def horizontal_line():
     line = QFrame()
     # line.setGeometry(QRect(60, 110, 751, 20))
     line.setFrameShape(QFrame.HLine)
-    line.setFrameShadow(QFrame.Sunken)
+    # line.setFrameShadow(QFrame.Sunken)
     return line
 
 
 def clear_layout(layout, keep=0):
     # from https://stackoverflow.com/questions/4528347/clear-all-widgets-in-a-layout-in-pyqt
     while layout.count() - keep:
         child = layout.takeAt(0)
@@ -82,14 +58,15 @@
 
 
 class InputError(QMessageBox):
     def __init__(self, title="Input Error"):
         super().__init__()
         # tutorial on message boxes: https://www.techwithtim.net/tutorials/pyqt5-tutorial/messageboxes/
         self.setWindowTitle(title)
+        # self.setTextFormat(Qt.RichText)
         self.setStandardButtons(QMessageBox.Ok)  # | QMessageBox.Cancel) if adding more buttons, separate with "|"
         self.setDefaultButton(QMessageBox.Ok)  # setting default button to Cancel
         self.buttonClicked.connect(self.popup_clicked)
 
     def popup_clicked(self, i):
         return i.text()
 
@@ -330,16 +307,16 @@
         # Create a top-level layout
         main_layout = QVBoxLayout()
         self.setLayout(main_layout)
 
         # Add volumes info layout
         self.fpv = QSpinBox()
         self.fgf = QSpinBox()
-        self.fpv.setRange(1, 100000000)  # if range is not set, the maximum is 100, which can be not enough,
-        self.fgf.setRange(0, 100000000)  # 100000000 is well within integer range, and hopefully is enough for anyone
+        self.fpv.setRange(1, 1000000000)  # if range is not set, the maximum is 100, which can be not enough,
+        self.fgf.setRange(0, 1000000000)  # 100000000 is well within integer range, and hopefully is enough for anyone
         self.fgf.setValue(0)
         volume_info_lo = QFormLayout()
         volume_info_lo.addRow("Frames per volume:", self.fpv)
         volume_info_lo.addRow("First good frame:", self.fgf)
         main_layout.addLayout(volume_info_lo)
 
         # get volumes button
@@ -379,15 +356,16 @@
         # 1. save FileTab and VolumeTab into a database)
         main_layout = QVBoxLayout()
         self.setLayout(main_layout)
         main_layout.addWidget(horizontal_line())
 
         self.save_pb = QPushButton("Save")
         self.save_le = QLineEdit()
-        self.info_label = QLabel("Save experiment to a database file:")
+        self.info_label = QLabel("[SAVE] Save experiment to a database file:")
+        main_layout.addWidget(QLabel("____________________________________________________"))
         main_layout.addWidget(self.info_label)
         main_layout.addWidget(self.save_le)
         main_layout.addWidget(self.save_pb)
 
     def get_save_filename(self):
         """
         Returns a filename to save the database or None.
@@ -619,15 +597,15 @@
         main_lo.addLayout(table_lo)
 
         self.msg = InputError()
 
     def set_up_table(self):
         self.table.setColumnCount(2)
         self.table.setColumnWidth(0, 150)
-        self.table.setHorizontalHeaderLabels(["Label name", "Duration"])
+        self.table.setHorizontalHeaderLabels(["Label name", "Duration (in frames!)"])
         self.table.setSelectionBehavior(QAbstractItemView.SelectRows)
         self.table.setSelectionMode(QAbstractItemView.SingleSelection)
         h_header = self.table.horizontalHeader()
         h_header.setSectionResizeMode(1, QHeaderView.ResizeMode.Stretch)
 
     def add_row(self, labels: List[str], label_name: str = None, duration: int = None):
         """
@@ -640,14 +618,15 @@
         Learning Resources:
             Instead of setting widgets for each cell,
             a better way would be to use a delegate https://forum.qt.io/topic/88486/dropdown-in-qtablewdget
         """
         # create the elements to insert
         label_choice = QComboBox()
         label_duration = QSpinBox()
+        label_duration.setRange(1, 1000000000)
         label_choice.addItems(labels)
         label_duration.setMinimum(1)
 
         n_rows = self.table.rowCount()
         self.table.insertRow(n_rows)
         self.table.setRowHeight(n_rows, self.ROW_HEIGHT)
 
@@ -880,38 +859,80 @@
 
         self.ROW_HEIGHT = 30
         # Create a top-level layout
         self.main_layout = QVBoxLayout()
         self.setLayout(self.main_layout)
 
         # 1. Individual volumes
+        section1_title = QLabel("[LOAD OPTION 1] Load based on volumes/slices IDs")
+        self.main_layout.addWidget(QLabel("____________________________________________________"))
+        self.main_layout.addWidget(section1_title)
+
         self.v_info_pb = QPushButton("")
         self.v_info_pb.setIcon(self.style().standardIcon(getattr(QStyle, "SP_MessageBoxInformation")))
         self.v_info_pb.clicked.connect(self.how_to_volumes)
         v_label = QLabel("Volumes: ")
         self.volumes = QLineEdit()
         # Regex explanation :
         # this allows integers separated by , and slices : .
         # For example: 12, 34, 4:56 , 72  : 34 is a valid input
         # (although slice 72:34 is invalid, it will be filtered out later)
         # but this: 4, 5, 6:7 : 8 is invalid because of two consecutive ":"
         reg_ex = QRegExp(r"^ *(\d{1,}|\d{1,} *: *\d{1,})( *|, *\d{1,}|, *\d{1,} *: *\d{1,}| *)*$")
         input_validator = QRegExpValidator(reg_ex, self.volumes)
         self.volumes.setValidator(input_validator)
 
+        #    slice input
+        #    TODO: add check if the slices are valid for the current dataset (use Signals?) (low priority)
+        self.s_info_pb = QPushButton("")
+        self.s_info_pb.setIcon(self.style().standardIcon(getattr(QStyle, "SP_MessageBoxInformation")))
+        self.s_info_pb.clicked.connect(self.how_to_slices)
+        s_label = QLabel("Slices: ")
+        self.slices = QLineEdit()
+        self.slices.setValidator(input_validator)
+
         volume_lo = QHBoxLayout()
         volume_lo.addWidget(v_label)
         volume_lo.addWidget(self.volumes)
         volume_lo.addWidget(self.v_info_pb)
-        self.main_layout.addLayout(volume_lo)
+        slice_lo = QHBoxLayout()
+        slice_lo.addWidget(s_label)
+        slice_lo.addWidget(self.slices)
+        slice_lo.addWidget(self.s_info_pb)
+        volume_slice_lo = QVBoxLayout()
+        volume_slice_lo.addLayout(volume_lo)
+        volume_slice_lo.addLayout(slice_lo)
+
+        # 2 checkboxes whether to consider the head and the tail of the dataset
+        self.head_cb = QCheckBox("Head")
+        self.tail_cb = QCheckBox("Tail")
+        head_tail_lo = QVBoxLayout()
+        head_tail_lo.addWidget(self.head_cb)
+        head_tail_lo.addWidget(self.tail_cb)
+
+        volume_slice_checkbox_lo = QHBoxLayout()
+        volume_slice_checkbox_lo.addLayout(volume_slice_lo)
+        volume_slice_checkbox_lo.addLayout(head_tail_lo)
+
+        self.main_layout.addLayout(volume_slice_checkbox_lo)
         self.load_volumes_pb = QPushButton("Load")
         self.main_layout.addWidget(self.load_volumes_pb)
         self.main_layout.addWidget(horizontal_line())
 
         # 2. Annotation list
+        self.main_layout.addWidget(QLabel("____________________________________________________"))
+        section2_title = QLabel("[LOAD OPTION 2] Load based on experimental conditions")
+        self.a_info_pb = QPushButton("")
+        self.a_info_pb.setIcon(self.style().standardIcon(getattr(QStyle, "SP_MessageBoxInformation")))
+        self.a_info_pb.clicked.connect(self.how_to_annotations)
+        intro_lo = QHBoxLayout()
+        intro_lo.addWidget(section2_title)
+        intro_lo.addWidget(self.a_info_pb)
+        self.main_layout.addLayout(intro_lo)
+
         self.annotations = {}
 
         self.checkbox_lo = QHBoxLayout()
         self.checkboxes = []
         self.info_text = QLabel("Add time annotation to the experiment\nto see the options.")
         self.checkbox_lo.addWidget(self.info_text)
 
@@ -958,18 +979,64 @@
             if annotation_name not in self.annotations:
                 self.annotations[annotation_name] = AnnotationCheckboxes(annotation_name, label_names)
                 self.checkbox_lo.addWidget(self.annotations[annotation_name])
             else:
                 self.annotations[annotation_name].update_labels(label_names)
 
     def how_to_volumes(self):
-        text = "Enter the indeces for the volumes you would like to load.\nValid inputs are individual indexes, " \
-               "separated by a comma:\n2, 4  , 6, (all spaces are ignored)\nor slices, to load volumes 9, 10, 11, " \
-               "12 one can write:\n9:12 (Important! Volume number 12 WILL BE LOADED) \nAny combination of these two " \
-               "inputs will work:\n2, 4, 6, 9:12, 19 (loads volumes 2, 4, 6, 9, 10, 11, 12 and 19 ) "
+        text = "Enter the indices for the volumes you would like to load. " \
+               "Valid inputs include individual indices, comma-separated lists, or ranges using a colon. " \
+               "Spaces are ignored. The volumes are loaded in ascending order. For example:\n" \
+               "• Individual indices: 0, 4, 6\n" \
+               "• Ranges: 9:12 (note that volume 12 will be loaded)\n" \
+               "• Combined inputs: 2, 4, 6, 9:12, 19 (loads volumes 2, 4, 6, 9, 10, 11, 12, and 19)\n" \
+               "Use the examples shown to specify the desired volumes to load.\n\n" \
+               "If slices to load are specified, you can leave the volumes empty. " \
+               "Then the specified slices will be loaded for all volumes.\n\n" \
+               "If the dataset has unfilled volumes at the beginning or end of the recording, " \
+               "you can include/exclude them by checking the Head and Tail checkboxes. " \
+               "This might be important if you are trying to load a set of slices that " \
+               "are not present in the Head or Tail of the dataset."
+
+        self.launch_popup(text=text)
+
+    def how_to_slices(self):
+        text = "Enter the indices for the slices you would like to load. " \
+               "Valid inputs include individual slices, " \
+               "comma-separated, or ranges using a colon. Spaces are ignored. " \
+               "ORDER IS IGNORED ( loaded in ascending order! ) " \
+               "For example:\n" \
+               "• Individual slices: 0, 2, 5\n" \
+               "• Ranges: 0:5 (note that volume 5 WILL BE LOADED)\n" \
+               "• Combined inputs: 0, 2, 5:7, 9 (loads slices 0, 2, 5, 6, 7, 9)\n" \
+               "Use the format shown in the examples to specify the desired slices to load.\n\n" \
+               "If slices to volumes are specified, you can leave the slices empty. " \
+               "Then all the slices will be loaded for the specified volumes.\n\n" \
+               "If the dataset has unfilled volumes at the beginning or end of the recording, " \
+               "you can include/exclude them by checking the Head and Tail checkboxes." \
+               "This might be important if you are trying to load a set of slices that " \
+               "are not present in the Head or Tail of the dataset."
+
+        self.launch_popup(text=text)
+
+    def how_to_annotations(self):
+        text = "If you have added time annotations to the experiment, you will see the annotation's names and labels. " \
+               "Check the checkboxes by the labels for which you want to get the volumes, " \
+               "and choose how to combine them with a logical OR or a logical AND. " \
+               "Then, click the 'Find volumes' button to get a list of volume IDs that " \
+               "correspond to the chosen conditions or 'Load' to load all such volumes into napari.\n\n" \
+               "When you are choosing 'OR', all the conditions you picked will be combined with a logical OR." \
+               " This means that vodex will pick volumes with slices that correspond " \
+               "to at least one of the conditions " \
+               "that you picked. It does not mean that the whole volume corresponds to one of the conditions. " \
+               "Half of the slices in the volume can correspond to one condition and the other half to another.\n\n" \
+               "When you are choosing 'AND', vodex will pick volumes with slices that correspond to all the " \
+               "conditions that you picked at the same time. If at least one slice in a volume does not correspond" \
+               " to all the conditions, such volume will not be picked."
+
         self.launch_popup(text=text)
 
     def get_volumes(self):
         """
         Gets volumes from text.
         """
         requested_volumes = self.volumes.text()
@@ -981,14 +1048,30 @@
                     assert start < end, f"The slice start {start} must be smaller than the end {end}"
                     volumes.extend(range(int(start.strip()), (int(end.strip()) + 1)))
                 else:
                     volumes.append(int(vol.strip()))
             # TODO: check for repeats ?
         return volumes, requested_volumes
 
+    def get_slices(self):
+        """
+        Gets slices from text.
+        """
+        requested_slices = self.slices.text()
+        slices = []
+        if requested_slices:
+            for sl in requested_slices.split(","):
+                if ":" in sl:
+                    start, end = sl.split(":")
+                    assert start < end, f"The slice start {start} must be smaller than the end {end}"
+                    slices.extend(range(int(start.strip()), (int(end.strip()) + 1)))
+                else:
+                    slices.append(int(sl.strip()))
+        return slices, requested_slices
+
 
 class VodexView(QWidget):
     """
     Does everything about the GUI View.
     """
 
     def __init__(self, viewer):
@@ -1058,713 +1141,7 @@
         # 3. Load/Save Tab
         splitter_3 = QSplitter(Qt.Vertical)
         splitter_3.addWidget(self.dt)
         splitter_3.addWidget(self.st)
         tabs.addTab(splitter_3, "Load/Save Data")
 
         self.main_layout.addWidget(tabs)
-
-
-class VodexModel:
-    """
-    Does everything on the vodex side.
-    """
-
-    def __init__(self):
-
-        self.fm = None
-        self.vm = None
-
-        self.annotations = {}
-        self.labels = {}
-        self.cycles = {}
-        self.timelines = {}
-
-        self.experiment = None
-        self.experiment_saved = False
-
-    def crete_fm(self, data_dir, file_type, file_names=None):
-        """
-        Creates the FileManager.
-        """
-        self.fm = vx.FileManager(data_dir, file_type=file_type, file_names=file_names)
-
-    def remove_fm(self):
-        """
-        Removes the FileManager.
-        """
-        self.annotations = {}
-
-    def create_vm(self, fpv, fgf):
-        """
-        Creates the VolumeManager.
-        """
-        self.vm = vx.VolumeManager(fpv, vx.FrameManager(self.fm), fgf=fgf)
-
-    def remove_vm(self):
-        """
-        Removes the VolumeManager.
-        """
-        self.vm = None
-
-    def create_annotation(self, group: str, state_names: List[str], state_info: dict,
-                          labels_order: List[str], duration: List[int], an_type: str):
-        """
-        Creates an annotation.
-
-        Args:
-            group: Group name ( the same as annotation name)
-            state_names: a list of unique label names used to create the annotation
-            state_info: description of the state_names
-            labels_order: label names in the order as they follow in the annotation
-            duration: duration of the labels in the order as they follow in the annotation
-            an_type: whether annotation os created from Cycle or from Timeline
-        """
-        n_frames = self.vm.n_frames
-        self.labels[group] = vx.Labels(group, state_names, state_info=state_info)
-        label_order = [vx.TimeLabel(name, description=state_info[name], group=group) for name in labels_order]
-
-        if an_type == 'Timeline':
-            self.timelines[group] = vx.Timeline(label_order, duration)
-            annotation = vx.Annotation.from_timeline(n_frames, self.labels[group], self.timelines[group], info=None)
-        elif an_type == 'Cycle':
-            self.cycles[group] = vx.Cycle(label_order, duration)
-            annotation = vx.Annotation.from_cycle(n_frames, self.labels[group], self.cycles[group], info=None)
-        else:
-            annotation = None
-        self.annotations[group] = annotation
-
-        # add to the experiment
-        self.experiment.add_annotations([annotation])
-
-        # indicate that there are some unsaved changes
-        self.experiment_saved = False
-
-    def remove_annotation(self, group):
-        """
-        Removes an annotation from the experiment and from the model.
-        """
-        self.labels.pop(group)
-        self.cycles.pop(group, None)
-        self.timelines.pop(group, None)
-        self.annotations.pop(group)
-
-        # finally, remove from the experiment
-        self.experiment.delete_annotations([group])
-        # indicate that there are some unsaved changes
-        self.experiment_saved = False
-
-    def create_experiment(self):
-        """
-        Initialises the experiment from VolumeManager, no annotations added at this point.
-        """
-        # check that the vm is not empty ( no creating empty tables )
-        self.experiment = vx.Experiment.create(self.vm, [])
-
-    def remove_experiment(self):
-        """
-        Removes experiment from the model,
-        also resets annotations, labels, cycles and timelines.
-        Setting the model into the initial state.
-        """
-
-        self.annotations = {}
-        self.labels = {}
-        self.cycles = {}
-        self.timelines = {}
-
-        self.experiment = None
-        self.experiment_saved = False
-
-    def save_experiment(self, file_name: str):
-        """
-        Saves experiment to file.
-        """
-        self.experiment.save(file_name)
-        self.experiment_saved = True
-
-    def load_experiment(self, file_name: str):
-        """
-        Loads experiment to file.
-        """
-        # this makes sure annotations and all the managers
-        # are already in experiment
-        self.experiment = vx.Experiment.load(file_name)
-        self.experiment_saved = True
-
-        # populate the model to reflect the experiment
-        db_exporter = vx.DbExporter(self.experiment.db)
-        self.fm = db_exporter.reconstruct_file_manager()
-        self.vm = db_exporter.reconstruct_volume_manager()
-        self.load_annotation_info(db_exporter)
-
-    def load_annotation_info(self, db_exporter):
-        """
-        Creates annotations, cycles, timelines and labels from the database records.
-        """
-        # get the names of all the available annotations from the db
-        annotation_names = self.experiment.db.get_Names_from_AnnotationTypes()
-
-        # get the total number of frames in the recording
-        n_frames = self.vm.n_frames
-
-        for group in annotation_names:
-            # reconstruct Labels for the group
-            labels = db_exporter.reconstruct_labels(group)
-            self.labels[group] = labels
-
-            # create the annotation based on the annotation type
-            cycle = db_exporter.reconstruct_cycle(group)
-            if cycle is not None:
-                self.cycles[group] = cycle
-                self.annotations[group] = vx.Annotation.from_cycle(n_frames, labels, cycle)
-            else:
-                timeline = db_exporter.reconstruct_timeline(group)
-                self.timelines[group] = timeline
-                self.annotations[group] = vx.Annotation.from_timeline(n_frames, labels, timeline)
-
-    def choose_volumes(self, conditions: Union[tuple, List[tuple]], logic: str):
-        """
-        Selects only full volumes that correspond to specified conditions;
-        Uses "or" or "and" between the conditions depending on logic.
-        To load the selected volumes, use load_volumes()
-
-        Args:
-            conditions: a list of conditions on the annotation labels
-                in a form [(group, name),(group, name), ...] where group is a string for the annotation type
-                and name is the name of the label of that annotation type. For example [('light', 'on'), ('shape','c')]
-            logic: "and" or "or" , default is "and".
-        Returns:
-            list of volumes and list of frame ids that were chosen.
-            Remember that frame numbers start at 1, but volumes start at 0.
-        """
-        volume_list = self.experiment.choose_volumes(conditions, logic)
-        return volume_list
-
-    def load_volumes(self, volumes: List[int]):
-        """
-        Loads volumes.
-        """
-        assert self.experiment is not None, "Error when loading volumes: " \
-                                            "experiment is not initialized."
-        volumes_img = self.experiment.load_volumes(volumes)
-        return volumes_img
-
-    def save_volumes(self, volumes_img: List[int]):
-        pass
-
-
-class VodexController:
-    """
-    Controller class for the GUI (following the MVC schema).
-    """
-
-    def __init__(self, model, view):
-
-        self._model = model
-        self._view = view
-
-        self._connectDisplaySignalsAndSlots()
-        self.msg = InputError(title="Error!")
-
-    def launch_popup(self, text):
-        self.msg.setText(text)
-        x = self.msg.exec_()
-
-    def initialize_fm(self):
-        """
-        Executed when [Get Files] button is pressed.
-        Initialises FileManager with all the files retrieved from the data directory
-        and adds the files to the list to inspect.
-        """
-        data_dir_str = self._view.nt.dir_location.text()
-        if data_dir_str == "":
-            self.launch_popup(f"Enter directory!")
-        else:
-            data_dir = Path(data_dir_str)
-            # check that the location is a directory
-            if data_dir.is_dir():
-                try:
-                    # create FileManager
-                    file_type = self._view.nt.file_types.currentText()
-                    self._model.crete_fm(data_dir, file_type)
-                    # update list of files
-                    self._view.nt.list_widget.fill_list(self._model.fm.file_names)
-                    # freeze dir
-                    self._view.nt.freeze_dir()
-                    # unfreeze file list
-                    self._view.nt.list_widget.setEnabled(True)
-                except Exception as initialize_fm_exception:
-                    self.launch_popup(str(initialize_fm_exception))
-                    self._model.remove_fm()
-                # # if file names are not empty
-                # if self._model.fm is not None:
-                #     # update list of files
-                #     self._view.ft.list_widget.fill_list(self._model.fm.file_names)
-                #     # freeze dir
-                #     self._view.ft.freeze_dir()
-                #     # unfreeze file list
-                #     self._view.ft.list_widget.setEnabled(True)
-            else:
-                self.launch_popup(f"Directory {data_dir} does not exist!")
-
-    def update_and_freeze_fm(self):
-        """
-        Executed when [Save File Order] button is pressed.
-        Updates a FileManager with the edited files and freezes it.
-        Unfreezes the volue manager step.
-        """
-        try:
-            data_dir = self._view.nt.dir_location.text()
-            file_type = self._view.nt.file_types.currentText()
-            file_names = self._view.nt.list_widget.get_file_names()
-            # if file names are empty
-            if file_names:
-                # create new FileManager from updated file list
-                self._model.crete_fm(data_dir, file_type, file_names=file_names)
-                # freeze files list
-                self._view.nt.list_widget.freeze()
-                # unfreeze vm
-                self._view.vt.setEnabled(True)
-                self._view.vt.unfreeze_vm()
-            else:
-                self.launch_popup("File names are empty!\n"
-                                  "To repopulate the files, press Fetch files again!")
-
-        except Exception as e:
-            self.launch_popup(e)
-
-    def remove_fm(self):
-        """
-        Executed when the [Change Directory] button is pressed.
-        Deletes existing FileManager and clears file list.
-        """
-        # clear dependent managers
-        self.remove_vm()
-
-        try:
-            # remove FileManager from the model
-            self._model.remove_fm()
-            # clear files from list and make it active
-            self._view.nt.list_widget.list_widget.clear()
-            self._view.nt.list_widget.unfreeze()
-        except Exception as e:
-            self._view.error_dialog.showMessage(e)
-
-    def initialize_vm(self):
-        """
-        Executed when [Save Volume Info] button is pressed.
-        Initialises VolumeManager and outputs the recording summary to inspect.
-        """
-
-        # must save files before adding vm
-        if self._view.nt.list_widget.list_widget.isEnabled():
-            self._view.vt.volume_info_string.setText("Save changes to the files first!")
-        else:
-            # create new VolumeManager from updated file list
-            fpv = self._view.vt.fpv.value()
-            fgf = self._view.vt.fgf.value()
-            try:
-                self._model.create_vm(fpv, fgf)
-                # freeze vm
-                self._view.vt.freeze_vm()
-                # update the volume info summary
-                self._view.vt.volume_info_string.setText(str(self._model.vm))
-
-                # show the info for the next step
-                self._view.it.show()
-
-            except Exception as vm_e:
-                self.launch_popup(vm_e)
-
-    def create_experiment(self):
-        """
-        Executed when [Create Experiment] button is pressed.
-        Initialises Experiment and freezes the first tab.
-        """
-        if self._model.vm is None:
-            self.launch_popup("Save volume information first!")
-        else:
-            self._model.create_experiment()
-
-            # swap the button to edit
-            self._view.it.create_experiment.hide()
-            self._view.it.edit_experiment.show()
-            self._view.it.next_step.show()
-
-            # freeze all the first tab
-            self._view.nt.setEnabled(False)
-            self._view.vt.setEnabled(False)
-
-            # allow to save ( on the Load/Save tab ):
-            self._view.st.setEnabled(True)
-
-    def edit_experiment(self):
-
-        # switch all annotations into "in edit" mode
-        for annotation in list(self._model.annotations.keys()):
-            self.edit_annotation(annotation)
-
-        # remove experiment
-        self._model.remove_experiment()
-
-        # unfreeze all the first tab
-        self._view.nt.setEnabled(True)
-        self._view.vt.setEnabled(True)
-
-        # swap the button to show on the first tab
-        self._view.it.create_experiment.show()
-        self._view.it.edit_experiment.hide()
-        self._view.it.next_step.hide()
-
-    def remove_vm(self):
-        """
-        Executed when the [Change Directory] of [Edit Volume Info] button is pressed.
-        Deletes existing VolumeManager and clears file list.
-        """
-        self._model.remove_vm()
-
-        # remove the volume info summary
-        self._view.vt.volume_info_string.setText("")
-
-        # sets the volume info inputs to enabled
-
-        # remove the save button:
-        self._view.st.hide()
-
-    def add_annotation(self, annotation_name):
-        if self._model.experiment is None:
-            self.launch_popup("Create Experiment First!")
-        else:
-            # get information to create annotation
-            group = annotation_name
-            state_names = self._view.at.annotations[annotation_name].labels.get_names()
-            state_info = self._view.at.annotations[annotation_name].labels.get_descriptions()
-            labels_order = self._view.at.annotations[annotation_name].timing.get_names_sequence()
-            duration = self._view.at.annotations[annotation_name].timing.get_duration_sequence()
-            an_type = self._view.at.annotations[annotation_name].timing.annotation_type.currentText()
-
-            if an_type == "Timeline" and sum(duration) != self._model.vm.n_frames:
-                self.launch_popup("The number of frames in a Timeline "
-                                  "must exactly match the total number of frames in the recording.")
-            elif an_type == "Cycle" and sum(duration) > self._model.vm.n_frames:
-                self.launch_popup("The number of frames in a Cycle "
-                                  "must be less or equal to the total number of frames in the recording.")
-            else:
-                # change the tab view
-                self._view.at.annotations[annotation_name].freeze()
-
-                # create annotation and add it to the experiment
-                self._model.create_annotation(group, state_names, state_info, labels_order, duration, an_type)
-
-                # update the Load/Save Tab
-                self._view.dt.update_labels(self._get_label_names())
-
-    def remove_annotation(self, annotation_name):
-        # remove the tab from view
-        self._view.at.annotations[annotation_name].setParent(None)
-        self._view.at.annotations[annotation_name].deleteLater()
-        self._view.at.pageCombo.removeItem(self._view.at.pageCombo.currentIndex())
-
-        # remove annotation from model and from experiment
-        self._model.remove_annotation(annotation_name)
-
-        # update the Load/Save Tab
-        self._view.dt.update_labels(self._get_label_names())
-
-    def edit_annotation(self, annotation_name):
-        # change the tab view
-        self._view.at.annotations[annotation_name].unfreeze()
-
-        # remove annotation from model and from experiment
-        self._model.remove_annotation(annotation_name)
-
-        # update the Load/Save Tab
-        self._view.dt.update_labels(self._get_label_names())
-
-    def initialize_at(self):
-        """
-        Executed when [Add annotation] button is pressed.
-        Initialises the annotation tab.
-        """
-        if self._model.experiment is None:
-            self.launch_popup("Create Experiment first!")
-        else:
-            if self._view.at.pageCombo is None:
-                self._view.at.initialize_annotation_list()
-                self._view.at.pageCombo.activated.connect(self._view.at.switchPage)
-
-    def initialize_ap(self, annotation_name=None):
-        """
-        Executed when [Add annotation] button is pressed.
-        Initialises the annotation page and adds it to the annotation tab.
-        """
-        if self._model.experiment is not None:
-            if annotation_name is None:
-                # check if the name is unique
-                annotation_name = self._view.at.get_annotation_name()
-            # create ap
-            if annotation_name is not None:
-                self._view.at.create_ap(annotation_name)
-                self._connectAnnotationPageSignalsAndSlots(annotation_name)
-
-    def save_experiment(self):
-        """
-        Executed when [Load volumes] button is pressed.
-        Initialises the experiment.
-        """
-        # launch a pop-up that the db will be created and saved.
-        file_name = self._view.st.get_save_filename()
-        if file_name is not None:
-            # attempt to save
-            self._model.save_experiment(file_name)
-
-    def load_volumes(self):
-        """
-        Executed when [Load volumes] is pressed.
-        """
-        # check that experiment has been saved:
-        if self._model.experiment is not None:
-            # get volume indeces
-            volumes, requested_volumes = self._view.dt.get_volumes()
-            if volumes:
-                # load images
-                volumes_img = self._model.load_volumes(volumes)
-                # finally add loaded data to napari viewer
-                self._view.napari.add_image(volumes_img, name=requested_volumes)
-            else:
-                self.launch_popup("Enter the IDs of volumes to load!")
-        else:
-            self.launch_popup("You must create the experiment to load the volumes.\n"
-                              "See Image Data tab.")
-
-    def load_volumes_for_conditions(self):
-        """
-        Executed when [Load volumes] is pressed.
-        """
-        # rerun the choosing part in case anything changed
-        # TODO : make sure nothing can change from choosing to loading
-        search_results = self._find_volumes()
-        # will be none if experiment is not defined or no annotations added
-        if search_results is not None:
-            conditions, logic, volumes = search_results
-            if volumes:
-                # construct the name
-                name = f"_{logic}_".join(f"{condition[0]}-{condition[1]}" for condition in conditions)
-
-                # load images
-                volumes_img = self._model.load_volumes(volumes)
-                # finally add loaded data to napari viewer
-                self._view.napari.add_image(volumes_img, name=name)
-
-    def load_experiment(self):
-        # browse for the db
-        self._view.lt.browse()
-        db_name = self._view.lt.db_location.text()
-        self._model.load_experiment(db_name)
-
-        # update the info about the fm and vm
-        self._view.lt.fm_info_string.setText(str(self._model.fm))
-        self._view.lt.vm_info_string.setText(str(self._model.vm))
-        self._view.lt.setEnabled(False)
-        self._load_annotations()
-
-    def _get_label_names(self):
-        """
-        Replaces Labels in the _model.labels to their names.
-        Such that the resulting dictionary is annotation names as keys, label names as values.
-        """
-        label_names = {}
-        for annotation_name, labels in self._model.labels.items():
-            label_names[annotation_name] = labels.state_names
-        return label_names
-
-    def _load_annotations(self):
-        """
-        create the annotation tab and annotation pages and fill out
-        """
-        self.initialize_at()
-        for annotation_name in self._model.annotations.keys():
-            self.initialize_ap(annotation_name=annotation_name)
-            self._load_labels(annotation_name)
-            self._load_timing(annotation_name)
-
-            self._view.at.annotations[annotation_name].freeze()
-
-        # update the Load/Save Tab
-        self._view.dt.update_labels(self._get_label_names())
-
-    def _load_labels(self, annotation_name):
-        # TODO: test with empty labels in the db ? Is it possible?
-        labels = self._model.labels[annotation_name]
-        for label in labels.states:
-            self._view.at.annotations[annotation_name].labels.add_row(label_name=label.name,
-                                                                      description=label.description)
-
-    def _load_timing(self, annotation_name):
-        labels = self._view.at.annotations[annotation_name].labels.label_names
-        # decide if it's a cycle or a timeline
-        if annotation_name in self._model.cycles.keys():
-            self._view.at.annotations[annotation_name].timing.annotation_type.setCurrentText("Cycle")
-            timing = self._model.cycles[annotation_name]
-        elif annotation_name in self._model.timelines.keys():
-            self._view.at.annotations[annotation_name].timing.annotation_type.setCurrentText("Timeline")
-            timing = self._model.timelines[annotation_name]
-        # fill out the table
-        for label, duration in zip(timing.label_order, timing.duration):
-            self._view.at.annotations[annotation_name].timing.add_row(labels,
-                                                                      label_name=label.name,
-                                                                      duration=duration)
-
-    def _find_volumes(self):
-        if self._model.experiment is None:
-            self.launch_popup("Create Experiment First!")
-            return
-        elif not self._model.annotations:
-            self.launch_popup("Add an Annotation to Experiment First!")
-            return
-        else:
-            # collect conditions info
-            conditions = []
-            for annotation in self._view.dt.annotations.values():
-                an_conditions = annotation.get_checked_conditions()
-                if an_conditions:
-                    conditions.extend(annotation.get_checked_conditions())
-            logic = self._view.dt.logic_box.currentText()
-
-            # get volumes
-            volumes_ids = self._model.experiment.choose_volumes(conditions, logic=logic)
-
-            # print volumes to text field
-            if volumes_ids:
-                self._view.dt.volumes_info.setText(','.join(str(volume) for volume in volumes_ids))
-            else:
-                self._view.dt.volumes_info.setText("No full volumes satisfy the conditions.")
-
-            return conditions, logic, volumes_ids
-
-    def _connectAnnotationPageSignalsAndSlots(self, annotation_name):
-        # 0. Connect tab controls
-        # [Add annotation] button
-        self._view.at.annotations[annotation_name].add_pb.clicked.connect(lambda:
-                                                                          self.add_annotation(annotation_name))
-        # [Delete annotation] button
-        self._view.at.annotations[annotation_name].delete_pb.clicked.connect(lambda:
-                                                                             self.remove_annotation(annotation_name))
-        # [Edit annotation] button
-        self._view.at.annotations[annotation_name].edit_pb.clicked.connect(lambda:
-                                                                           self.edit_annotation(annotation_name))
-        # 1. connect LabelsTab
-        # [Add label] button:
-        # add a new label and update the choices in conditions tab
-        self._view.at.annotations[annotation_name].labels.add_label.clicked.connect(
-            lambda: self._view.at.annotations[annotation_name].labels.add_row())
-        self._view.at.annotations[annotation_name].labels.add_label.clicked.connect(
-            lambda: self._view.at.annotations[annotation_name].timing.update_choices(
-                self._view.at.annotations[annotation_name].labels.label_names
-            ))
-        # [Delete selected] button:
-        # if selected label is not used in the conditions tab delete selected row from the table
-        self._view.at.annotations[annotation_name].labels.delete_selected.clicked.connect(
-            lambda: self._view.at.annotations[annotation_name].labels.delete_row(
-                self._view.at.annotations[annotation_name].timing.check_in_use(
-                    self._view.at.annotations[annotation_name].labels.get_selected_name()
-                )))
-        self._view.at.annotations[annotation_name].labels.delete_selected.clicked.connect(
-            lambda: self._view.at.annotations[annotation_name].timing.update_choices(
-                self._view.at.annotations[annotation_name].labels.label_names
-            ))
-        # 2. connect TimingTab
-        self._view.at.annotations[annotation_name].timing.add_button.clicked.connect(
-            lambda: self._view.at.annotations[annotation_name].timing.add_row(
-                self._view.at.annotations[annotation_name].labels.get_names()))
-        self._view.at.annotations[annotation_name].timing.del_button.clicked.connect(
-            self._view.at.annotations[annotation_name].timing.delete_row)
-
-    def _connectFirstTabSignalsAndSlots(self):
-        # 1. connect FileTab
-        # _______________________________________________________________________________________________
-        # [Browse] button in New Experiment
-        self._view.nt.browse_button.clicked.connect(self._view.nt.browse)
-        # [Load] button in Load Experiment
-        self._view.lt.load_db_pb.clicked.connect(self.load_experiment)
-
-        # [Fetch files] button
-        self._view.nt.files_button.clicked.connect(self.initialize_fm)
-
-        # [Edit] button
-        self._view.nt.edit_dir_button.clicked.connect(self.remove_fm)
-        self._view.nt.edit_dir_button.clicked.connect(self._view.nt.unfreeze_dir)
-
-        # [Delete File] button
-        self._view.nt.list_widget.delete_button.clicked.connect(self._view.nt.list_widget.delete_file)
-
-        # [Save File Order] button
-        self._view.nt.list_widget.save_button.clicked.connect(self.update_and_freeze_fm)
-
-        # [Edit Files] button
-        self._view.nt.list_widget.edit_button.clicked.connect(self._view.nt.list_widget.unfreeze)
-        self._view.nt.list_widget.edit_button.clicked.connect(self.remove_vm)
-
-        # 2. connect VolumeTab
-        # _______________________________________________________________________________________________
-        # [Save Volume Info] button
-        # update the volume info summary
-        self._view.vt.volumes_button.clicked.connect(self.initialize_vm)
-
-        # [Edit Volume Info] button
-        self._view.vt.edit_vol_button.clicked.connect(self.remove_vm)
-        self._view.vt.edit_vol_button.clicked.connect(self._view.vt.unfreeze_vm)
-
-        # 3. connect InitialiseTab
-        self._view.it.create_experiment.clicked.connect(self.create_experiment)
-        self._view.it.edit_experiment.clicked.connect(self.edit_experiment)
-
-    def _connectDisplaySignalsAndSlots(self):
-
-        # 0. Connect intro Tab
-        # _______________________________________________________________________________________________
-        self._view.nt_pb.clicked.connect(self._view.initialize_new_experiment)
-        self._view.lt_pb.clicked.connect(self._view.initialize_load_experiment)
-
-        self._connectFirstTabSignalsAndSlots()
-
-        # 3. connect SaveTab
-        # _______________________________________________________________________________________________
-        # [Save] button
-        self._view.st.save_pb.clicked.connect(self.save_experiment)
-
-        # 4. connect AnnotationTab
-        # _______________________________________________________________________________________________
-        # [Add Annotation] button
-        self._view.at.add_annotation_pb.clicked.connect(self.initialize_at)
-        # initialize_ap connects all the buttons for the individual pages
-        self._view.at.add_annotation_pb.clicked.connect(lambda: self.initialize_ap())
-
-        # 5. connect DataReaderWriterTab
-        # _______________________________________________________________________________________________
-        # [Load volumes] button
-        self._view.dt.load_volumes_pb.clicked.connect(self.load_volumes)
-        self._view.dt.find_volumes.clicked.connect(self._find_volumes)
-        self._view.dt.load_conditions_pb.clicked.connect(self.load_volumes_for_conditions)
-
-
-class VodexWidget(VodexView):
-    # your QWidget.__init__ can optionally request the napari viewer instance
-    # in one of two ways:
-    # 1. use a parameter called `napari_viewer`
-    # 2. use a type annotation of 'napari.viewer.Viewer' for any parameter
-
-    def __init__(self, viewer: 'napari.viewer.Viewer' = None):
-        super().__init__(viewer)
-
-        self._model = VodexModel()
-        self._controller = VodexController(model=self._model, view=self)
-
-
-if __name__ == "__main__":
-    import sys
-
-    app = QApplication(sys.argv)
-    window = VodexWidget()
-    window.show()
-    sys.exit(app.exec_())
```

### Comparing `napari-vodex-1.0.11/src/napari_vodex.egg-info/PKG-INFO` & `napari-vodex-1.0.12/src/napari_vodex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: napari-vodex
-Version: 1.0.11
+Version: 1.0.12
 Summary: A napari plugin for VoDEx : Volumetric Data and Experiment Manager. Allows to load volumetric data based on experimental conditions.
 Home-page: https://github.com/LemonJust/napari-vodex
 Author: Anna Nadtochiy
 Author-email: lemonjustgithub@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/LemonJust/napari-vodex/issues
 Project-URL: Documentation, https://lemonjust.github.io/vodex/napari/
 Project-URL: Source Code, https://github.com/LemonJust/napari-vodex
 Project-URL: User Support, https://github.com/LemonJust/napari-vodex/issues
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: napari
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `napari-vodex-1.0.11/src/napari_vodex.egg-info/SOURCES.txt` & `napari-vodex-1.0.12/src/napari_vodex.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -7,15 +7,18 @@
 pyproject.toml
 setup.cfg
 tox.ini
 .github/workflows/test_and_deploy.yml
 .napari-hub/DESCRIPTION.md
 .napari-hub/config.yml
 src/napari_vodex/__init__.py
+src/napari_vodex/_controller.py
+src/napari_vodex/_model.py
 src/napari_vodex/_version.py
+src/napari_vodex/_view.py
 src/napari_vodex/_widget.py
 src/napari_vodex/napari.yaml
 src/napari_vodex.egg-info/PKG-INFO
 src/napari_vodex.egg-info/SOURCES.txt
 src/napari_vodex.egg-info/dependency_links.txt
 src/napari_vodex.egg-info/entry_points.txt
 src/napari_vodex.egg-info/requires.txt
```

### Comparing `napari-vodex-1.0.11/tox.ini` & `napari-vodex-1.0.12/tox.ini`

 * *Files identical despite different names*

