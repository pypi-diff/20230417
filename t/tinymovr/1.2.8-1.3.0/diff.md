# Comparing `tmp/tinymovr-1.2.8.tar.gz` & `tmp/tinymovr-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinymovr-1.2.8.tar", last modified: Mon Apr 10 19:15:29 2023, max compression
+gzip compressed data, was "tinymovr-1.3.0.tar", last modified: Mon Apr 17 16:52:37 2023, max compression
```

## Comparing `tinymovr-1.2.8.tar` & `tinymovr-1.3.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-10 19:15:29.511173 tinymovr-1.2.8/
--rw-r--r--   0 yanconst   (501) staff       (20)       87 2023-04-10 19:14:46.000000 tinymovr-1.2.8/MANIFEST.in
--rw-r--r--   0 yanconst   (501) staff       (20)     2144 2023-04-10 19:15:29.510793 tinymovr-1.2.8/PKG-INFO
--rw-r--r--   0 yanconst   (501) staff       (20)     1689 2023-04-08 07:47:15.000000 tinymovr-1.2.8/README.md
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-10 19:15:29.489743 tinymovr-1.2.8/resources/
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-10 19:15:29.494096 tinymovr-1.2.8/resources/icons/
--rw-r--r--   0 yanconst   (501) staff       (20)     3184 2023-04-08 07:47:15.000000 tinymovr-1.2.8/resources/icons/call.png
--rw-r--r--   0 yanconst   (501) staff       (20)       38 2023-04-10 19:15:29.511263 tinymovr-1.2.8/setup.cfg
--rw-r--r--   0 yanconst   (501) staff       (20)     2326 2023-04-10 19:14:46.000000 tinymovr-1.2.8/setup.py
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-10 19:15:29.498489 tinymovr-1.2.8/tinymovr/
--rw-r--r--   0 yanconst   (501) staff       (20)       55 2023-04-08 07:47:15.000000 tinymovr-1.2.8/tinymovr/__init__.py
--rw-r--r--   0 yanconst   (501) staff       (20)     3529 2023-04-08 07:47:15.000000 tinymovr-1.2.8/tinymovr/channel.py
--rw-r--r--   0 yanconst   (501) staff       (20)     2882 2023-04-10 19:03:18.000000 tinymovr-1.2.8/tinymovr/cli.py
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-10 19:15:29.504777 tinymovr-1.2.8/tinymovr/codec/
--rw-r--r--   0 yanconst   (501) staff       (20)       65 2022-02-09 17:27:03.000000 tinymovr-1.2.8/tinymovr/codec/__init__.py
--rw-r--r--   0 yanconst   (501) staff       (20)     2944 2023-04-08 07:47:15.000000 tinymovr-1.2.8/tinymovr/codec/codec.py
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-10 19:15:29.506866 tinymovr-1.2.8/tinymovr/config/
--rw-r--r--   0 yanconst   (501) staff       (20)      160 2023-04-08 07:47:15.000000 tinymovr-1.2.8/tinymovr/config/__init__.py
--rw-r--r--   0 yanconst   (501) staff       (20)     3358 2023-04-08 07:47:15.000000 tinymovr-1.2.8/tinymovr/config/config.py
--rw-r--r--   0 yanconst   (501) staff       (20)    15484 2023-04-08 07:47:15.000000 tinymovr-1.2.8/tinymovr/config/device.yaml
--rw-r--r--   0 yanconst   (501) staff       (20)     1075 2023-04-08 07:47:15.000000 tinymovr-1.2.8/tinymovr/constants.py
--rw-r--r--   0 yanconst   (501) staff       (20)     3292 2023-04-08 07:47:15.000000 tinymovr-1.2.8/tinymovr/discovery.py
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-10 19:15:29.510094 tinymovr-1.2.8/tinymovr/gui/
--rw-r--r--   0 yanconst   (501) staff       (20)      411 2023-04-08 07:47:15.000000 tinymovr-1.2.8/tinymovr/gui/__init__.py
--rw-r--r--   0 yanconst   (501) staff       (20)     1718 2023-04-10 19:03:18.000000 tinymovr-1.2.8/tinymovr/gui/gui.py
--rw-r--r--   0 yanconst   (501) staff       (20)     8904 2023-04-08 07:47:15.000000 tinymovr-1.2.8/tinymovr/gui/helpers.py
--rw-r--r--   0 yanconst   (501) staff       (20)    12186 2023-04-08 07:47:15.000000 tinymovr-1.2.8/tinymovr/gui/window.py
--rw-r--r--   0 yanconst   (501) staff       (20)     4472 2023-04-08 07:47:15.000000 tinymovr-1.2.8/tinymovr/gui/worker.py
--rw-r--r--   0 yanconst   (501) staff       (20)     3088 2023-04-08 07:47:15.000000 tinymovr-1.2.8/tinymovr/tee.py
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-10 19:15:29.503719 tinymovr-1.2.8/tinymovr.egg-info/
--rw-r--r--   0 yanconst   (501) staff       (20)     2144 2023-04-10 19:15:29.000000 tinymovr-1.2.8/tinymovr.egg-info/PKG-INFO
--rw-r--r--   0 yanconst   (501) staff       (20)      614 2023-04-10 19:15:29.000000 tinymovr-1.2.8/tinymovr.egg-info/SOURCES.txt
--rw-r--r--   0 yanconst   (501) staff       (20)        1 2023-04-10 19:15:29.000000 tinymovr-1.2.8/tinymovr.egg-info/dependency_links.txt
--rw-r--r--   0 yanconst   (501) staff       (20)       82 2023-04-10 19:15:29.000000 tinymovr-1.2.8/tinymovr.egg-info/entry_points.txt
--rw-r--r--   0 yanconst   (501) staff       (20)      158 2023-04-10 19:15:29.000000 tinymovr-1.2.8/tinymovr.egg-info/requires.txt
--rw-r--r--   0 yanconst   (501) staff       (20)        9 2023-04-10 19:15:29.000000 tinymovr-1.2.8/tinymovr.egg-info/top_level.txt
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-17 16:52:37.496353 tinymovr-1.3.0/
+-rw-r--r--   0 yanconst   (501) staff       (20)       87 2023-04-10 19:14:46.000000 tinymovr-1.3.0/MANIFEST.in
+-rw-r--r--   0 yanconst   (501) staff       (20)     2144 2023-04-17 16:52:37.496191 tinymovr-1.3.0/PKG-INFO
+-rw-r--r--   0 yanconst   (501) staff       (20)     1689 2023-04-08 07:47:15.000000 tinymovr-1.3.0/README.md
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-17 16:52:37.490282 tinymovr-1.3.0/resources/
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-17 16:52:37.491283 tinymovr-1.3.0/resources/icons/
+-rw-r--r--   0 yanconst   (501) staff       (20)     3184 2023-04-08 07:47:15.000000 tinymovr-1.3.0/resources/icons/call.png
+-rw-r--r--   0 yanconst   (501) staff       (20)       38 2023-04-17 16:52:37.496399 tinymovr-1.3.0/setup.cfg
+-rw-r--r--   0 yanconst   (501) staff       (20)     2334 2023-04-17 16:47:58.000000 tinymovr-1.3.0/setup.py
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-17 16:52:37.492837 tinymovr-1.3.0/tinymovr/
+-rw-r--r--   0 yanconst   (501) staff       (20)       55 2023-04-08 07:47:15.000000 tinymovr-1.3.0/tinymovr/__init__.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     3529 2023-04-08 07:47:15.000000 tinymovr-1.3.0/tinymovr/channel.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     2882 2023-04-10 19:03:18.000000 tinymovr-1.3.0/tinymovr/cli.py
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-17 16:52:37.494371 tinymovr-1.3.0/tinymovr/codec/
+-rw-r--r--   0 yanconst   (501) staff       (20)       65 2022-02-09 17:27:03.000000 tinymovr-1.3.0/tinymovr/codec/__init__.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     2944 2023-04-08 07:47:15.000000 tinymovr-1.3.0/tinymovr/codec/codec.py
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-17 16:52:37.494898 tinymovr-1.3.0/tinymovr/config/
+-rw-r--r--   0 yanconst   (501) staff       (20)      160 2023-04-08 07:47:15.000000 tinymovr-1.3.0/tinymovr/config/__init__.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     3358 2023-04-08 07:47:15.000000 tinymovr-1.3.0/tinymovr/config/config.py
+-rw-r--r--   0 yanconst   (501) staff       (20)    15484 2023-04-08 07:47:15.000000 tinymovr-1.3.0/tinymovr/config/device.yaml
+-rw-r--r--   0 yanconst   (501) staff       (20)     1075 2023-04-08 07:47:15.000000 tinymovr-1.3.0/tinymovr/constants.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     3292 2023-04-08 07:47:15.000000 tinymovr-1.3.0/tinymovr/discovery.py
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-17 16:52:37.495977 tinymovr-1.3.0/tinymovr/gui/
+-rw-r--r--   0 yanconst   (501) staff       (20)      411 2023-04-08 07:47:15.000000 tinymovr-1.3.0/tinymovr/gui/__init__.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     1718 2023-04-17 16:47:58.000000 tinymovr-1.3.0/tinymovr/gui/gui.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     8904 2023-04-17 16:47:58.000000 tinymovr-1.3.0/tinymovr/gui/helpers.py
+-rw-r--r--   0 yanconst   (501) staff       (20)    12207 2023-04-17 16:47:58.000000 tinymovr-1.3.0/tinymovr/gui/window.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     4472 2023-04-17 16:47:58.000000 tinymovr-1.3.0/tinymovr/gui/worker.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     3088 2023-04-08 07:47:15.000000 tinymovr-1.3.0/tinymovr/tee.py
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-17 16:52:37.493975 tinymovr-1.3.0/tinymovr.egg-info/
+-rw-r--r--   0 yanconst   (501) staff       (20)     2144 2023-04-17 16:52:37.000000 tinymovr-1.3.0/tinymovr.egg-info/PKG-INFO
+-rw-r--r--   0 yanconst   (501) staff       (20)      614 2023-04-17 16:52:37.000000 tinymovr-1.3.0/tinymovr.egg-info/SOURCES.txt
+-rw-r--r--   0 yanconst   (501) staff       (20)        1 2023-04-17 16:52:37.000000 tinymovr-1.3.0/tinymovr.egg-info/dependency_links.txt
+-rw-r--r--   0 yanconst   (501) staff       (20)       82 2023-04-17 16:52:37.000000 tinymovr-1.3.0/tinymovr.egg-info/entry_points.txt
+-rw-r--r--   0 yanconst   (501) staff       (20)      166 2023-04-17 16:52:37.000000 tinymovr-1.3.0/tinymovr.egg-info/requires.txt
+-rw-r--r--   0 yanconst   (501) staff       (20)        9 2023-04-17 16:52:37.000000 tinymovr-1.3.0/tinymovr.egg-info/top_level.txt
```

### Comparing `tinymovr-1.2.8/PKG-INFO` & `tinymovr-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinymovr
-Version: 1.2.8
+Version: 1.3.0
 Summary: Tinymovr Studio
 Home-page: https://github.com/yconst/Tinymovr
 Author: Yannis Chatzikonstantinou
 Author-email: info@tinymovr.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `tinymovr-1.2.8/README.md` & `tinymovr-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `tinymovr-1.2.8/resources/icons/call.png` & `tinymovr-1.3.0/resources/icons/call.png`

 * *Files identical despite different names*

### Comparing `tinymovr-1.2.8/setup.py` & `tinymovr-1.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         "pyserial",
         "pyusb",
         "pyyaml",
         "docopt",
         "flatten-dict",
         "pint",
     ],
-    extras_require={"gui": ["pyside2", "pyqtgraph"]},
+    extras_require={"gui": ["pyside6", "pyqtgraph>=0.13.3"]},
     entry_points={
         "console_scripts": [
             "tinymovr_cli=tinymovr.cli:spawn",
             "tinymovr=tinymovr.gui:spawn",
         ]
     },
 )
```

### Comparing `tinymovr-1.2.8/tinymovr/channel.py` & `tinymovr-1.3.0/tinymovr/channel.py`

 * *Files identical despite different names*

### Comparing `tinymovr-1.2.8/tinymovr/cli.py` & `tinymovr-1.3.0/tinymovr/cli.py`

 * *Files identical despite different names*

### Comparing `tinymovr-1.2.8/tinymovr/codec/codec.py` & `tinymovr-1.3.0/tinymovr/codec/codec.py`

 * *Files identical despite different names*

### Comparing `tinymovr-1.2.8/tinymovr/config/config.py` & `tinymovr-1.3.0/tinymovr/config/config.py`

 * *Files identical despite different names*

### Comparing `tinymovr-1.2.8/tinymovr/config/device.yaml` & `tinymovr-1.3.0/tinymovr/config/device.yaml`

 * *Files identical despite different names*

### Comparing `tinymovr-1.2.8/tinymovr/constants.py` & `tinymovr-1.3.0/tinymovr/constants.py`

 * *Files identical despite different names*

### Comparing `tinymovr-1.2.8/tinymovr/discovery.py` & `tinymovr-1.3.0/tinymovr/discovery.py`

 * *Files identical despite different names*

### Comparing `tinymovr-1.2.8/tinymovr/gui/gui.py` & `tinymovr-1.3.0/tinymovr/gui/gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     --chan=<chan>  The bus device "channel".
     --bitrate=<bitrate>  CAN bitrate [default: 1000000].
 """
 
 import sys
 import pkg_resources
 from docopt import docopt
-from PySide2.QtWidgets import QApplication
+from PySide6.QtWidgets import QApplication
 from tinymovr.gui import MainWindow, app_stylesheet
 from tinymovr.constants import app_name
 
 
 """
 Tinymovr Studio GUI
 Copyright Ioannis Chatzikonstantinou 2020-2023
```

### Comparing `tinymovr-1.2.8/tinymovr/gui/helpers.py` & `tinymovr-1.3.0/tinymovr/gui/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 this program. If not, see <http://www.gnu.org/licenses/>.
 """
 
 import time
 import os
 import enum
 import pint
-from PySide2 import QtGui, QtCore
-from PySide2.QtWidgets import QMessageBox, QFileDialog
+from PySide6 import QtGui, QtCore
+from PySide6.QtWidgets import QMessageBox, QFileDialog
 from avlos.definitions import RemoteAttribute
 
 
 app_stylesheet = """
 
 /* --------------------------------------- QPushButton -----------------------------------*/
```

### Comparing `tinymovr-1.2.8/tinymovr/gui/window.py` & `tinymovr-1.3.0/tinymovr/gui/window.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,31 +15,31 @@
 this program. If not, see <http://www.gnu.org/licenses/>.
 """
 
 import time
 from functools import partial
 from contextlib import suppress
 import json
-from PySide2 import QtCore
-from PySide2.QtCore import Signal
-from PySide2.QtWidgets import (
+from PySide6 import QtCore
+from PySide6.QtCore import Signal
+from PySide6.QtWidgets import (
     QMainWindow,
     QMenu,
     QMenuBar,
-    QAction,
     QWidget,
     QFrame,
     QHBoxLayout,
     QVBoxLayout,
     QHeaderView,
     QLabel,
     QTreeWidget,
     QTreeWidgetItem,
     QPushButton,
 )
+from PySide6.QtGui import QAction
 import pyqtgraph as pg
 from tinymovr.constants import app_name
 from tinymovr.channel import ResponseError as ChannelResponseError
 from tinymovr.config import get_bus_config, configure_logging
 from avlos import get_registry
 from avlos.json_codec import AvlosEncoder
 from tinymovr.gui import (
```

### Comparing `tinymovr-1.2.8/tinymovr/gui/worker.py` & `tinymovr-1.3.0/tinymovr/gui/worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 You should have received a copy of the GNU General Public License along with
 this program. If not, see <http://www.gnu.org/licenses/>.
 """
 
 import time
 import can
 from canine import CANineBus
-from PySide2 import QtCore
-from PySide2.QtCore import QObject
-from PySide2.QtWidgets import (
+from PySide6 import QtCore
+from PySide6.QtCore import QObject
+from PySide6.QtWidgets import (
     QApplication,
 )
 from tinymovr.gui import TimedGetter, RateLimitedFunction, get_dynamic_attrs
 from tinymovr.tee import init_tee, destroy_tee
 from tinymovr.discovery import Discovery
 from tinymovr.constants import base_node_name
```

### Comparing `tinymovr-1.2.8/tinymovr/tee.py` & `tinymovr-1.3.0/tinymovr/tee.py`

 * *Files identical despite different names*

### Comparing `tinymovr-1.2.8/tinymovr.egg-info/PKG-INFO` & `tinymovr-1.3.0/tinymovr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinymovr
-Version: 1.2.8
+Version: 1.3.0
 Summary: Tinymovr Studio
 Home-page: https://github.com/yconst/Tinymovr
 Author: Yannis Chatzikonstantinou
 Author-email: info@tinymovr.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `tinymovr-1.2.8/tinymovr.egg-info/SOURCES.txt` & `tinymovr-1.3.0/tinymovr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

