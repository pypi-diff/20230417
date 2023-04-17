# Comparing `tmp/PySideSix-Frameless-Window-0.0.6.tar.gz` & `tmp/PySideSix-Frameless-Window-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PySideSix-Frameless-Window-0.0.6.tar", last modified: Mon Apr 10 14:42:55 2023, max compression
+gzip compressed data, was "dist\PySideSix-Frameless-Window-0.1.0.tar", last modified: Mon Apr 17 07:24:01 2023, max compression
```

## Comparing `PySideSix-Frameless-Window-0.0.6.tar` & `PySideSix-Frameless-Window-0.1.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 14:42:55.264169 PySideSix-Frameless-Window-0.0.6/
--rw-rw-rw-   0        0        0     7815 2023-04-10 14:32:17.000000 PySideSix-Frameless-Window-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     5519 2023-04-10 14:42:55.261655 PySideSix-Frameless-Window-0.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-10 14:42:55.216259 PySideSix-Frameless-Window-0.0.6/PySideSix_Frameless_Window.egg-info/
--rw-rw-rw-   0        0        0     5519 2023-04-10 14:42:54.000000 PySideSix-Frameless-Window-0.0.6/PySideSix_Frameless_Window.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      868 2023-04-10 14:42:55.000000 PySideSix-Frameless-Window-0.0.6/PySideSix_Frameless_Window.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 14:42:54.000000 PySideSix-Frameless-Window-0.0.6/PySideSix_Frameless_Window.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-04-10 14:42:54.000000 PySideSix-Frameless-Window-0.0.6/PySideSix_Frameless_Window.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-04-10 14:42:54.000000 PySideSix-Frameless-Window-0.0.6/PySideSix_Frameless_Window.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4927 2023-04-10 14:32:17.000000 PySideSix-Frameless-Window-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 14:42:55.223871 PySideSix-Frameless-Window-0.0.6/qframelesswindow/
--rw-rw-rw-   0        0        0     1614 2023-04-10 14:32:17.000000 PySideSix-Frameless-Window-0.0.6/qframelesswindow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 14:42:55.225068 PySideSix-Frameless-Window-0.0.6/qframelesswindow/_rc/
--rw-rw-rw-   0        0        0        0 2023-01-28 14:21:55.000000 PySideSix-Frameless-Window-0.0.6/qframelesswindow/_rc/__init__.py
--rw-rw-rw-   0        0        0     1477 2023-04-10 14:32:17.000000 PySideSix-Frameless-Window-0.0.6/qframelesswindow/_rc/resource.py
-drwxrwxrwx   0        0        0        0 2023-04-10 14:42:55.231841 PySideSix-Frameless-Window-0.0.6/qframelesswindow/linux/
--rw-rw-rw-   0        0        0     4320 2023-04-10 14:32:17.000000 PySideSix-Frameless-Window-0.0.6/qframelesswindow/linux/__init__.py
--rw-rw-rw-   0        0        0     2918 2023-04-10 14:32:17.000000 PySideSix-Frameless-Window-0.0.6/qframelesswindow/linux/window_effect.py
-drwxrwxrwx   0        0        0        0 2023-04-10 14:42:55.231841 PySideSix-Frameless-Window-0.0.6/qframelesswindow/mac/
--rw-rw-rw-   0        0        0     4529 2023-04-10 14:32:17.000000 PySideSix-Frameless-Window-0.0.6/qframelesswindow/mac/__init__.py
--rw-rw-rw-   0        0        0     4320 2023-04-10 14:32:17.000000 PySideSix-Frameless-Window-0.0.6/qframelesswindow/mac/window_effect.py
-drwxrwxrwx   0        0        0        0 2023-04-10 14:42:55.240337 PySideSix-Frameless-Window-0.0.6/qframelesswindow/titlebar/
--rw-rw-rw-   0        0        0     5062 2023-04-10 14:32:17.000000 PySideSix-Frameless-Window-0.0.6/qframelesswindow/titlebar/__init__.py
--rw-rw-rw-   0        0        0     9039 2023-04-10 14:32:17.000000 PySideSix-Frameless-Window-0.0.6/qframelesswindow/titlebar/title_bar_buttons.py
-drwxrwxrwx   0        0        0        0 2023-04-10 14:42:55.247404 PySideSix-Frameless-Window-0.0.6/qframelesswindow/utils/
--rw-rw-rw-   0        0        0      885 2022-07-25 01:20:40.000000 PySideSix-Frameless-Window-0.0.6/qframelesswindow/utils/__init__.py
--rw-rw-rw-   0        0        0     1216 2023-04-10 14:32:17.000000 PySideSix-Frameless-Window-0.0.6/qframelesswindow/utils/linux_utils.py
--rw-rw-rw-   0        0        0     1844 2023-04-10 14:32:17.000000 PySideSix-Frameless-Window-0.0.6/qframelesswindow/utils/mac_utils.py
--rw-rw-rw-   0        0        0     7143 2023-04-10 14:32:17.000000 PySideSix-Frameless-Window-0.0.6/qframelesswindow/utils/win32_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-10 14:42:55.259186 PySideSix-Frameless-Window-0.0.6/qframelesswindow/windows/
--rw-rw-rw-   0        0        0     8180 2023-04-10 14:32:17.000000 PySideSix-Frameless-Window-0.0.6/qframelesswindow/windows/__init__.py
--rw-rw-rw-   0        0        0     4261 2023-04-10 14:32:17.000000 PySideSix-Frameless-Window-0.0.6/qframelesswindow/windows/c_structures.py
--rw-rw-rw-   0        0        0     8905 2023-04-10 14:32:17.000000 PySideSix-Frameless-Window-0.0.6/qframelesswindow/windows/window_effect.py
--rw-rw-rw-   0        0        0       42 2023-04-10 14:42:55.264169 PySideSix-Frameless-Window-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1003 2023-04-10 14:32:17.000000 PySideSix-Frameless-Window-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 07:24:01.418397 PySideSix-Frameless-Window-0.1.0/
+-rw-rw-rw-   0        0        0     7815 2023-04-17 07:22:03.000000 PySideSix-Frameless-Window-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     5519 2023-04-17 07:24:01.417322 PySideSix-Frameless-Window-0.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-17 07:24:01.377817 PySideSix-Frameless-Window-0.1.0/PySideSix_Frameless_Window.egg-info/
+-rw-rw-rw-   0        0        0     5519 2023-04-17 07:24:01.000000 PySideSix-Frameless-Window-0.1.0/PySideSix_Frameless_Window.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      868 2023-04-17 07:24:01.000000 PySideSix-Frameless-Window-0.1.0/PySideSix_Frameless_Window.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 07:24:01.000000 PySideSix-Frameless-Window-0.1.0/PySideSix_Frameless_Window.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-04-17 07:24:01.000000 PySideSix-Frameless-Window-0.1.0/PySideSix_Frameless_Window.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-04-17 07:24:01.000000 PySideSix-Frameless-Window-0.1.0/PySideSix_Frameless_Window.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4927 2023-04-17 07:22:03.000000 PySideSix-Frameless-Window-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 07:24:01.379900 PySideSix-Frameless-Window-0.1.0/qframelesswindow/
+-rw-rw-rw-   0        0        0     1614 2023-04-17 07:22:33.000000 PySideSix-Frameless-Window-0.1.0/qframelesswindow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 07:24:01.384387 PySideSix-Frameless-Window-0.1.0/qframelesswindow/_rc/
+-rw-rw-rw-   0        0        0        0 2023-01-28 14:21:55.000000 PySideSix-Frameless-Window-0.1.0/qframelesswindow/_rc/__init__.py
+-rw-rw-rw-   0        0        0     1477 2023-04-17 07:22:03.000000 PySideSix-Frameless-Window-0.1.0/qframelesswindow/_rc/resource.py
+drwxrwxrwx   0        0        0        0 2023-04-17 07:24:01.388872 PySideSix-Frameless-Window-0.1.0/qframelesswindow/linux/
+-rw-rw-rw-   0        0        0     4320 2023-04-17 07:22:03.000000 PySideSix-Frameless-Window-0.1.0/qframelesswindow/linux/__init__.py
+-rw-rw-rw-   0        0        0     2918 2023-04-17 07:22:03.000000 PySideSix-Frameless-Window-0.1.0/qframelesswindow/linux/window_effect.py
+drwxrwxrwx   0        0        0        0 2023-04-17 07:24:01.394310 PySideSix-Frameless-Window-0.1.0/qframelesswindow/mac/
+-rw-rw-rw-   0        0        0     4529 2023-04-17 07:22:03.000000 PySideSix-Frameless-Window-0.1.0/qframelesswindow/mac/__init__.py
+-rw-rw-rw-   0        0        0     4320 2023-04-17 07:22:03.000000 PySideSix-Frameless-Window-0.1.0/qframelesswindow/mac/window_effect.py
+drwxrwxrwx   0        0        0        0 2023-04-17 07:24:01.398503 PySideSix-Frameless-Window-0.1.0/qframelesswindow/titlebar/
+-rw-rw-rw-   0        0        0     5062 2023-04-17 07:22:03.000000 PySideSix-Frameless-Window-0.1.0/qframelesswindow/titlebar/__init__.py
+-rw-rw-rw-   0        0        0     9039 2023-04-17 07:22:03.000000 PySideSix-Frameless-Window-0.1.0/qframelesswindow/titlebar/title_bar_buttons.py
+drwxrwxrwx   0        0        0        0 2023-04-17 07:24:01.407557 PySideSix-Frameless-Window-0.1.0/qframelesswindow/utils/
+-rw-rw-rw-   0        0        0      885 2022-07-25 01:20:40.000000 PySideSix-Frameless-Window-0.1.0/qframelesswindow/utils/__init__.py
+-rw-rw-rw-   0        0        0     1216 2023-04-17 07:22:03.000000 PySideSix-Frameless-Window-0.1.0/qframelesswindow/utils/linux_utils.py
+-rw-rw-rw-   0        0        0     1844 2023-04-17 07:22:03.000000 PySideSix-Frameless-Window-0.1.0/qframelesswindow/utils/mac_utils.py
+-rw-rw-rw-   0        0        0     8093 2023-04-17 07:22:38.000000 PySideSix-Frameless-Window-0.1.0/qframelesswindow/utils/win32_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-17 07:24:01.415177 PySideSix-Frameless-Window-0.1.0/qframelesswindow/windows/
+-rw-rw-rw-   0        0        0     8180 2023-04-17 07:22:03.000000 PySideSix-Frameless-Window-0.1.0/qframelesswindow/windows/__init__.py
+-rw-rw-rw-   0        0        0     4261 2023-04-17 07:22:03.000000 PySideSix-Frameless-Window-0.1.0/qframelesswindow/windows/c_structures.py
+-rw-rw-rw-   0        0        0     8905 2023-04-17 07:22:03.000000 PySideSix-Frameless-Window-0.1.0/qframelesswindow/windows/window_effect.py
+-rw-rw-rw-   0        0        0       42 2023-04-17 07:24:01.418397 PySideSix-Frameless-Window-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1003 2023-04-17 07:22:24.000000 PySideSix-Frameless-Window-0.1.0/setup.py
```

### Comparing `PySideSix-Frameless-Window-0.0.6/LICENSE` & `PySideSix-Frameless-Window-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.0.6/PKG-INFO` & `PySideSix-Frameless-Window-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySideSix-Frameless-Window
-Version: 0.0.6
+Version: 0.1.0
 Summary: A cross-platform frameless window based on pyside6, support Win32, Linux and macOS.
 Home-page: https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/PySide6
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: LGPLv3
 Keywords: pyside6 frameless
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PySideSix-Frameless-Window-0.0.6/PySideSix_Frameless_Window.egg-info/PKG-INFO` & `PySideSix-Frameless-Window-0.1.0/PySideSix_Frameless_Window.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySideSix-Frameless-Window
-Version: 0.0.6
+Version: 0.1.0
 Summary: A cross-platform frameless window based on pyside6, support Win32, Linux and macOS.
 Home-page: https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/PySide6
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: LGPLv3
 Keywords: pyside6 frameless
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PySideSix-Frameless-Window-0.0.6/PySideSix_Frameless_Window.egg-info/SOURCES.txt` & `PySideSix-Frameless-Window-0.1.0/PySideSix_Frameless_Window.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.0.6/README.md` & `PySideSix-Frameless-Window-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.0.6/qframelesswindow/__init__.py` & `PySideSix-Frameless-Window-0.1.0/qframelesswindow/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 Examples are available at https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/PySide6/examples.
 
 :copyright: (c) 2021 by zhiyiYo.
 :license: LGPLv3, see LICENSE for more details.
 """
 
-__version__ = "0.0.6"
+__version__ = "0.1.0"
 
 import sys
 
 from PySide6.QtCore import Qt
 from PySide6.QtWidgets import QDialog, QMainWindow
 
 from .titlebar import TitleBar, TitleBarButton, SvgTitleBarButton, StandardTitleBar
```

### Comparing `PySideSix-Frameless-Window-0.0.6/qframelesswindow/_rc/resource.py` & `PySideSix-Frameless-Window-0.1.0/qframelesswindow/_rc/resource.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.0.6/qframelesswindow/linux/__init__.py` & `PySideSix-Frameless-Window-0.1.0/qframelesswindow/linux/__init__.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.0.6/qframelesswindow/linux/window_effect.py` & `PySideSix-Frameless-Window-0.1.0/qframelesswindow/linux/window_effect.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.0.6/qframelesswindow/mac/__init__.py` & `PySideSix-Frameless-Window-0.1.0/qframelesswindow/mac/__init__.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.0.6/qframelesswindow/mac/window_effect.py` & `PySideSix-Frameless-Window-0.1.0/qframelesswindow/mac/window_effect.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.0.6/qframelesswindow/titlebar/__init__.py` & `PySideSix-Frameless-Window-0.1.0/qframelesswindow/titlebar/__init__.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.0.6/qframelesswindow/titlebar/title_bar_buttons.py` & `PySideSix-Frameless-Window-0.1.0/qframelesswindow/titlebar/title_bar_buttons.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.0.6/qframelesswindow/utils/__init__.py` & `PySideSix-Frameless-Window-0.1.0/qframelesswindow/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.0.6/qframelesswindow/utils/linux_utils.py` & `PySideSix-Frameless-Window-0.1.0/qframelesswindow/utils/linux_utils.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.0.6/qframelesswindow/utils/mac_utils.py` & `PySideSix-Frameless-Window-0.1.0/qframelesswindow/utils/mac_utils.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.0.6/qframelesswindow/utils/win32_utils.py` & `PySideSix-Frameless-Window-0.1.0/qframelesswindow/utils/win32_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from ctypes.wintypes import DWORD, HWND, LPARAM, RECT, UINT
 from platform import platform
 import sys
 
 import win32api
 import win32con
 import win32gui
+import win32print
 from PySide6.QtCore import QOperatingSystemVersion, QVersionNumber
 from PySide6.QtGui import QGuiApplication
 
 
 ABM_GETSTATE = 4
 ABS_AUTOHIDE = 1
 ABM_GETTASKBARPOS = 5
@@ -91,27 +92,62 @@
     dpiScale: bool
         whether to use dpi scale
     """
     window = findWindow(hWnd)
     if not window:
         return 0
 
-    user32 = windll.user32
-
     frame = win32con.SM_CXSIZEFRAME if horizontal else win32con.SM_CYSIZEFRAME
-    dpi = user32.GetDpiForWindow(hWnd)
-    result = user32.GetSystemMetricsForDpi(frame, dpi) + user32.GetSystemMetricsForDpi(92, dpi)
+    result = getSystemMetrics(hWnd, frame, horizontal) + getSystemMetrics(hWnd, 92, horizontal)
 
     if result > 0:
         return result
 
     thickness = 8 if isCompositionEnabled() else 4
     return round(thickness*window.devicePixelRatio())
 
 
+def getSystemMetrics(hWnd, index, horizontal):
+    """ get system metrics """
+    if not hasattr(windll.user32, 'GetSystemMetricsForDpi'):
+        return win32api.GetSystemMetrics(index)
+
+    dpi = getDpiForWindow(hWnd, horizontal)
+    return windll.user32.GetSystemMetricsForDpi(index, dpi)
+
+
+def getDpiForWindow(hWnd, horizontal=True):
+    """ get dpi for window
+
+    Parameters
+    ----------
+    hWnd: int or `sip.voidptr`
+        window handle
+
+    dpiScale: bool
+        whether to use dpi scale
+    """
+    if hasattr(windll.user32, 'GetDpiForWindow'):
+        return windll.user32.GetDpiForWindow(hWnd)
+
+    hdc = win32gui.GetDC(hWnd)
+    if not hdc:
+        return 96
+
+    dpiX = win32print.GetDeviceCaps(hdc, win32con.LOGPIXELSX)
+    dpiY = win32print.GetDeviceCaps(hdc, win32con.LOGPIXELSY)
+    win32gui.ReleaseDC(hWnd, hdc)
+    if dpiX > 0 and horizontal:
+        return dpiX
+    elif dpiY > 0 and not horizontal:
+        return dpiY
+
+    return 96
+
+
 def findWindow(hWnd):
     """ find window by hWnd, return `None` if not found
 
     Parameters
     ----------
     hWnd: int or `sip.voidptr`
         window handle
```

### Comparing `PySideSix-Frameless-Window-0.0.6/qframelesswindow/windows/__init__.py` & `PySideSix-Frameless-Window-0.1.0/qframelesswindow/windows/__init__.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.0.6/qframelesswindow/windows/c_structures.py` & `PySideSix-Frameless-Window-0.1.0/qframelesswindow/windows/c_structures.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.0.6/qframelesswindow/windows/window_effect.py` & `PySideSix-Frameless-Window-0.1.0/qframelesswindow/windows/window_effect.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.0.6/setup.py` & `PySideSix-Frameless-Window-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="PySideSix-Frameless-Window",
-    version="0.0.6",
+    version="0.1.0",
     keywords="pyside6 frameless",
     author="zhiyiYo",
     author_email="shokokawaii@outlook.com",
     description="A cross-platform frameless window based on pyside6, support Win32, Linux and macOS.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="LGPLv3",
```

