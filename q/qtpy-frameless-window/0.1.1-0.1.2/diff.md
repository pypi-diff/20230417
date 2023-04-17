# Comparing `tmp/QtPy-Frameless-Window-0.1.1.tar.gz` & `tmp/QtPy-Frameless-Window-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QtPy-Frameless-Window-0.1.1.tar", last modified: Sun Apr 16 19:35:36 2023, max compression
+gzip compressed data, was "QtPy-Frameless-Window-0.1.2.tar", last modified: Mon Apr 17 09:54:29 2023, max compression
```

## Comparing `QtPy-Frameless-Window-0.1.1.tar` & `QtPy-Frameless-Window-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    35823 2023-04-16 18:25:23.998258 QtPy-Frameless-Window-0.1.1/LICENSE
--rw-r--r--   0        0        0      961 2023-04-16 19:35:27.472871 QtPy-Frameless-Window-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      334 2023-04-16 18:25:24.013718 QtPy-Frameless-Window-0.1.1/qt_api/__init__.py
--rw-r--r--   0        0        0      174 2023-04-16 18:25:24.013718 QtPy-Frameless-Window-0.1.1/qtframelesswindow/__init__.py
--rw-r--r--   0        0        0     6143 2023-04-16 18:25:24.014611 QtPy-Frameless-Window-0.1.1/qtframelesswindow/buttons.py
--rw-r--r--   0        0        0     1739 2023-04-16 19:05:07.126941 QtPy-Frameless-Window-0.1.1/qtframelesswindow/manager.py
--rw-r--r--   0        0        0     7048 2023-04-16 19:34:31.149864 QtPy-Frameless-Window-0.1.1/qtframelesswindow/resource.py
--rw-r--r--   0        0        0     7111 2023-04-16 18:25:24.028639 QtPy-Frameless-Window-0.1.1/qtframelesswindow/window.py
--rw-r--r--   0        0        0     1763 2023-04-16 18:25:23.998258 QtPy-Frameless-Window-0.1.1/README.md
--rw-r--r--   0        0        0     2253 1970-01-01 00:00:00.000000 QtPy-Frameless-Window-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35823 2023-04-16 18:25:23.998258 QtPy-Frameless-Window-0.1.2/LICENSE
+-rw-r--r--   0        0        0      961 2023-04-17 09:54:22.591746 QtPy-Frameless-Window-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      334 2023-04-16 18:25:24.013718 QtPy-Frameless-Window-0.1.2/qt_api/__init__.py
+-rw-r--r--   0        0        0      146 2023-04-17 09:47:28.476630 QtPy-Frameless-Window-0.1.2/qtframelesswindow/__init__.py
+-rw-r--r--   0        0        0     6101 2023-04-17 09:50:47.880145 QtPy-Frameless-Window-0.1.2/qtframelesswindow/buttons.py
+-rw-r--r--   0        0        0     1681 2023-04-17 09:51:46.518997 QtPy-Frameless-Window-0.1.2/qtframelesswindow/manager.py
+-rw-r--r--   0        0        0     7048 2023-04-16 19:34:31.149864 QtPy-Frameless-Window-0.1.2/qtframelesswindow/resource.py
+-rw-r--r--   0        0        0     7103 2023-04-17 09:49:44.801034 QtPy-Frameless-Window-0.1.2/qtframelesswindow/window.py
+-rw-r--r--   0        0        0     1763 2023-04-16 18:25:23.998258 QtPy-Frameless-Window-0.1.2/README.md
+-rw-r--r--   0        0        0     2253 1970-01-01 00:00:00.000000 QtPy-Frameless-Window-0.1.2/PKG-INFO
```

### Comparing `QtPy-Frameless-Window-0.1.1/LICENSE` & `QtPy-Frameless-Window-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.1.1/pyproject.toml` & `QtPy-Frameless-Window-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 description = "A cross-platform frameless window based on QtPy."
 keywords = [
     "pyqt frameless",
 ]
 name = "QtPy-Frameless-Window"
 readme = "README.md"
 requires-python = ">=3.7,<3.10"
-version = "0.1.1"
+version = "0.1.2"
 
 [project.license]
 text = "GPLv3"
 
 [project.urls]
 Homepage = "https://github.com/TaoChenyue/QtPy-Frameless-Window.git"
```

### Comparing `QtPy-Frameless-Window-0.1.1/qtframelesswindow/buttons.py` & `QtPy-Frameless-Window-0.1.2/qtframelesswindow/buttons.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 from qtpy.QtGui import QPaintEvent,QMouseEvent,QColor,QFont
 from qtpy.QtWidgets import QPushButton,QWidget,QHBoxLayout,QLabel,QSizePolicy
-from .manager import StyleManager,IconManager,Theme,style_mapdict
+from .manager import StyleManager,IconManager,style_mapdict
 from typing import List
 
 BTN_H=30
 BTN_W=45
 
 class WindowButton(QPushButton):
-    def __init__(self,parent,theme:Theme=Theme.LIGHT):
+    def __init__(self,parent,theme:str="light"):
         super().__init__(parent)
         self.setSizePolicy(QSizePolicy.Policy.Preferred,QSizePolicy.Policy.Preferred)
         self.style_manager=StyleManager.BUTTON
         self.set_theme(theme)
         
-    def set_theme(self,theme:Theme):
+    def set_theme(self,theme:str="light"):
         self.theme=theme
         self.style_manager.set(self,theme)
         
 class MinimizeButton(WindowButton):
-    def __init__(self, parent, theme: Theme = Theme.LIGHT):
+    def __init__(self, parent, theme:str="light"):
         self.icon_manager=IconManager.MINIMIZE
         super().__init__(parent, theme)
         self.clicked.connect(self.window().showMinimized)
         
-    def set_theme(self, theme: Theme):
+    def set_theme(self, theme:str="light"):
         self.icon_manager.set(self,theme)
         return super().set_theme(theme)
     
 class CloseButton(WindowButton):
-    def __init__(self, parent, theme: Theme = Theme.LIGHT):
+    def __init__(self, parent, theme:str="light"):
         self.icon_manager=IconManager.CLOSE
         super().__init__(parent, theme)
         self.style_manager=StyleManager.BUTTON_CLOSE
         self.style_manager.set(self,theme)
         self.clicked.connect(self.window().close)
-    def set_theme(self, theme: Theme):
+    def set_theme(self, theme:str="light"):
         self.icon_manager.set(self,theme)
         return super().set_theme(theme)
     
 class ToggleButton(WindowButton):
-    def __init__(self, parent, theme: Theme = Theme.LIGHT):
+    def __init__(self, parent, theme:str="light"):
         super().__init__(parent, theme)
         self.icon_manager={
             "max":IconManager.MAXIMIZE,
             "normal":IconManager.NORMALIZE
         }
         self.clicked.connect(self.__toggle)
         
@@ -54,15 +54,15 @@
             self.window().showMaximized()
     
     def paintEvent(self, arg__1: QPaintEvent) -> None:
         self.icon_manager["normal" if self.window().isMaximized() else "max"].set(self,self.theme)
         return super().paintEvent(arg__1)
     
 class WindowIcon(WindowButton):
-    def __init__(self, parent, theme: Theme = Theme.LIGHT):
+    def __init__(self, parent, theme:str="light"):
         super().__init__(parent, theme)
         self.icon_manager=IconManager.CLOSE
         self.icon_manager.set(self)
            
     def mouseMoveEvent(self, arg__1: QMouseEvent) -> None:
         self.window().windowHandle().startSystemMove()
         return super().mouseMoveEvent(arg__1)
@@ -71,15 +71,15 @@
         if self.window().isMaximized():
             self.window().showNormal()
         else:
             self.window().showMaximized()
         return super().mouseDoubleClickEvent(event)
     
 class WindowButtons(QWidget):
-    def __init__(self, parent=None,theme:Theme=Theme.LIGHT) -> None:
+    def __init__(self, parent=None,theme:str="light") -> None:
         super().__init__(parent)
         self.setupUi()
         self.setFixedWidth(BTN_W*3)
         
     def setupUi(self):
         self.setLayout(QHBoxLayout())
         self.layout().setContentsMargins(0,0,0,0)
@@ -87,15 +87,15 @@
         self.minBtn=MinimizeButton(self)
         self.toggleBtn=ToggleButton(self)
         self.closeBtn=CloseButton(self)
         self.layout().addWidget(self.minBtn)
         self.layout().addWidget(self.toggleBtn)
         self.layout().addWidget(self.closeBtn)
         
-    def set_theme(self,theme:Theme):
+    def set_theme(self,theme:str="light"):
         self.minBtn.set_theme(theme)
         self.toggleBtn.set_theme(theme)
         self.closeBtn.set_theme(theme)
         
     def set_color(self,color:QColor):
         style_mapdict["--R"]=color.red()
         style_mapdict["--G"]=color.blue()
@@ -124,16 +124,16 @@
 class WindowTitle(QLabel):
     def __init__(self,parent):
         super().__init__(parent)
         self.setFont(QFont("Segoe UI",10))
         # self.setAlignment(Qt.AlignmentFlag.AlignCenter)
         self.setSizePolicy(QSizePolicy.Policy.Ignored,QSizePolicy.Policy.Fixed)
         
-    def set_theme(self,theme:Theme=Theme.LIGHT):
-        if theme==Theme.LIGHT:
+    def set_theme(self,theme:str="light"):
+        if theme=="light":
             self.setStyleSheet("color:black;")
         else:
             self.setStyleSheet("color:white")
         
     def mouseDoubleClickEvent(self, event: QMouseEvent) -> None:
         if self.window().isMaximized():
             self.window().showNormal()
```

### Comparing `QtPy-Frameless-Window-0.1.1/qtframelesswindow/manager.py` & `QtPy-Frameless-Window-0.1.2/qtframelesswindow/manager.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,64 +1,61 @@
 from enum import Enum
 from qtpy.QtCore import QFile
 from qtpy.QtGui import QIcon
 from qtpy.QtWidgets import QWidget,QAbstractButton
 from . import resource
-
-class Theme(Enum):
-    DARK="dark"
-    LIGHT="light"
     
 style_mapdict={
     "--R":255,
     "--G":255,
     "--B":255,
 }
     
 class ResourceManager(Enum):
     
-    def path(self,theme:Theme):
+    def path(self,theme:str='light'):
         raise NotImplementedError
     
-    def get(self,theme:Theme):
+    def get(self,theme:str='light'):
         raise NotImplementedError
     
-    def set(self,obj:QWidget,theme:Theme=Theme.LIGHT):
+    def set(self,obj:QWidget,theme:str='light'):
         raise NotImplementedError
     
 class StyleManager(ResourceManager):
     BUTTON="button"
     BUTTON_CLOSE="button_close"
     
     
-    def path(self,theme:Theme):
+    def path(self,theme):
         return f":/qtframelesswindow/qss/{self.value}.qss"
     
-    def get(self, theme: Theme):
+    def get(self,theme):
         f=QFile(self.path(theme))
         f.open(QFile.OpenModeFlag.ReadOnly)
         content=str(f.readAll(),encoding="utf-8")
         f.close()
         for k,v in style_mapdict.items():
             content=content.replace(k,str(v))
         return content
     
-    def set(self,obj:QWidget,theme:Theme=Theme.LIGHT):
+    def set(self,obj:QWidget,theme):
+        self.theme=theme
         obj.setStyleSheet(self.get(theme))
         
     
 class IconManager(ResourceManager):
     CLOSE="close"
     MAXIMIZE="maximize"
     MINIMIZE="minimize"
     NORMALIZE="normalize"
     
-    def path(self,theme:Theme):
-        dir_name="black" if theme==Theme.LIGHT else "white"
+    def path(self,theme:str='light'):
+        dir_name="black" if theme=="light" else "white"
         return f":/qtframelesswindow/images/{dir_name}/{self.value}.svg"
     
-    def get(self, theme: Theme):
+    def get(self, theme:str='light'):
         return QIcon(self.path(theme))
     
-    def set(self, obj: QWidget, theme: Theme=Theme.LIGHT):
+    def set(self, obj: QWidget, theme:str='light'):
         if isinstance(obj,QAbstractButton):
             obj.setIcon(self.get(theme))
```

### Comparing `QtPy-Frameless-Window-0.1.1/qtframelesswindow/resource.py` & `QtPy-Frameless-Window-0.1.2/qtframelesswindow/resource.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.1.1/qtframelesswindow/window.py` & `QtPy-Frameless-Window-0.1.2/qtframelesswindow/window.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from qtpy.QtCore import Qt, QCoreApplication, QEvent, QPropertyAnimation, QRect
 from qtpy.QtGui import QPaintEvent, QPainter, QColor
 from qtpy.QtWidgets import QWidget, QVBoxLayout, QMainWindow, QDialog
 from .buttons import TitleBar
-from .manager import Theme
 import math
 
 
 
 BORDER = 5
 
 
@@ -28,30 +27,31 @@
         self.titlebar = TitleBar(self)
         self.main_window = QWidget(self)
         self.client_window.setLayout(QVBoxLayout())
         self.client_window.layout().setSpacing(0)
         self.client_window.layout().setContentsMargins(0, 0, 0, 0)
         self.client_window.layout().addWidget(self.titlebar)
         self.client_window.layout().addWidget(self.main_window)
+        self.resize(400,400)
 
     def __set_frameless(self):
         self.setWindowFlag(Qt.WindowType.FramelessWindowHint, True)
         self.setAttribute(Qt.WidgetAttribute.WA_TranslucentBackground, True)
         # style sheet
         self.client_window.setObjectName("__window")
         self.set_border_radius(BORDER)
         # resize
         QCoreApplication.instance().installEventFilter(self)
 
     def set_border_radius(self, radius: int):
         self.__radius=radius
         self.update_stylesheet()
         
-    def set_theme(self,theme:Theme=Theme.LIGHT,bg_color:str=None):
-        if theme==Theme.LIGHT:
+    def set_theme(self,theme:str="light",bg_color:str=None):
+        if theme=="light":
             self.__background="white" if bg_color is None else bg_color
         else:
             self.__background="#383838" if bg_color is None else bg_color
         self.update_stylesheet()
         self.titlebar.title.set_theme(theme)
         self.titlebar.buttons.set_theme(theme)
```

### Comparing `QtPy-Frameless-Window-0.1.1/README.md` & `QtPy-Frameless-Window-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.1.1/PKG-INFO` & `QtPy-Frameless-Window-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QtPy-Frameless-Window
-Version: 0.1.1
+Version: 0.1.2
 Summary: A cross-platform frameless window based on QtPy.
 License: GPLv3
 Keywords: pyqt frameless
 Author-email: TaoChenyue <3038816978@qq.com>
 Requires-Python: >=3.7,<3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

