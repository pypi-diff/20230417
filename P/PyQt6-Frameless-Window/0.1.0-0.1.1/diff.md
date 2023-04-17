# Comparing `tmp/PyQt6-Frameless-Window-0.1.0.tar.gz` & `tmp/PyQt6-Frameless-Window-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PyQt6-Frameless-Window-0.1.0.tar", last modified: Thu Mar 30 01:27:48 2023, max compression
+gzip compressed data, was "dist\PyQt6-Frameless-Window-0.1.1.tar", last modified: Mon Apr 17 07:16:57 2023, max compression
```

## Comparing `PyQt6-Frameless-Window-0.1.0.tar` & `PyQt6-Frameless-Window-0.1.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-03-30 01:27:48.032519 PyQt6-Frameless-Window-0.1.0/
--rw-rw-rw-   0        0        0    35823 2023-03-28 03:37:30.000000 PyQt6-Frameless-Window-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     5582 2023-03-30 01:27:48.032519 PyQt6-Frameless-Window-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-03-30 01:27:47.999737 PyQt6-Frameless-Window-0.1.0/PyQt6_Frameless_Window.egg-info/
--rw-rw-rw-   0        0        0     5582 2023-03-30 01:27:47.000000 PyQt6-Frameless-Window-0.1.0/PyQt6_Frameless_Window.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      848 2023-03-30 01:27:47.000000 PyQt6-Frameless-Window-0.1.0/PyQt6_Frameless_Window.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-30 01:27:47.000000 PyQt6-Frameless-Window-0.1.0/PyQt6_Frameless_Window.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-03-30 01:27:47.000000 PyQt6-Frameless-Window-0.1.0/PyQt6_Frameless_Window.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-03-30 01:27:47.000000 PyQt6-Frameless-Window-0.1.0/PyQt6_Frameless_Window.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5007 2023-03-30 01:25:46.000000 PyQt6-Frameless-Window-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-03-30 01:27:48.001760 PyQt6-Frameless-Window-0.1.0/qframelesswindow/
--rw-rw-rw-   0        0        0     1615 2023-03-30 01:26:14.000000 PyQt6-Frameless-Window-0.1.0/qframelesswindow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-30 01:27:48.005746 PyQt6-Frameless-Window-0.1.0/qframelesswindow/_rc/
--rw-rw-rw-   0        0        0        0 2023-01-28 14:21:55.000000 PyQt6-Frameless-Window-0.1.0/qframelesswindow/_rc/__init__.py
--rw-rw-rw-   0        0        0     2728 2023-03-30 01:22:17.000000 PyQt6-Frameless-Window-0.1.0/qframelesswindow/_rc/resource.py
-drwxrwxrwx   0        0        0        0 2023-03-30 01:27:48.010290 PyQt6-Frameless-Window-0.1.0/qframelesswindow/linux/
--rw-rw-rw-   0        0        0     3110 2023-03-30 01:22:17.000000 PyQt6-Frameless-Window-0.1.0/qframelesswindow/linux/__init__.py
--rw-rw-rw-   0        0        0     2920 2023-03-30 01:22:17.000000 PyQt6-Frameless-Window-0.1.0/qframelesswindow/linux/window_effect.py
-drwxrwxrwx   0        0        0        0 2023-03-30 01:27:48.013988 PyQt6-Frameless-Window-0.1.0/qframelesswindow/mac/
--rw-rw-rw-   0        0        0     3015 2023-03-30 01:22:17.000000 PyQt6-Frameless-Window-0.1.0/qframelesswindow/mac/__init__.py
--rw-rw-rw-   0        0        0     4095 2023-03-30 01:22:17.000000 PyQt6-Frameless-Window-0.1.0/qframelesswindow/mac/window_effect.py
-drwxrwxrwx   0        0        0        0 2023-03-30 01:27:48.017930 PyQt6-Frameless-Window-0.1.0/qframelesswindow/titlebar/
--rw-rw-rw-   0        0        0     5083 2023-03-30 01:22:17.000000 PyQt6-Frameless-Window-0.1.0/qframelesswindow/titlebar/__init__.py
--rw-rw-rw-   0        0        0     9205 2023-03-30 01:22:17.000000 PyQt6-Frameless-Window-0.1.0/qframelesswindow/titlebar/title_bar_buttons.py
-drwxrwxrwx   0        0        0        0 2023-03-30 01:27:48.024942 PyQt6-Frameless-Window-0.1.0/qframelesswindow/utils/
--rw-rw-rw-   0        0        0      885 2022-07-25 01:20:40.000000 PyQt6-Frameless-Window-0.1.0/qframelesswindow/utils/__init__.py
--rw-rw-rw-   0        0        0      644 2023-03-30 01:22:17.000000 PyQt6-Frameless-Window-0.1.0/qframelesswindow/utils/linux_utils.py
--rw-rw-rw-   0        0        0     1850 2023-03-30 01:22:41.000000 PyQt6-Frameless-Window-0.1.0/qframelesswindow/utils/mac_utils.py
--rw-rw-rw-   0        0        0     7402 2023-03-30 01:22:17.000000 PyQt6-Frameless-Window-0.1.0/qframelesswindow/utils/win32_utils.py
-drwxrwxrwx   0        0        0        0 2023-03-30 01:27:48.030116 PyQt6-Frameless-Window-0.1.0/qframelesswindow/windows/
--rw-rw-rw-   0        0        0     6624 2023-03-30 01:22:17.000000 PyQt6-Frameless-Window-0.1.0/qframelesswindow/windows/__init__.py
--rw-rw-rw-   0        0        0     4261 2023-03-30 01:22:17.000000 PyQt6-Frameless-Window-0.1.0/qframelesswindow/windows/c_structures.py
--rw-rw-rw-   0        0        0     8949 2023-03-30 01:22:17.000000 PyQt6-Frameless-Window-0.1.0/qframelesswindow/windows/window_effect.py
--rw-rw-rw-   0        0        0       42 2023-03-30 01:27:48.033920 PyQt6-Frameless-Window-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      984 2023-03-30 01:22:55.000000 PyQt6-Frameless-Window-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 07:16:57.759624 PyQt6-Frameless-Window-0.1.1/
+-rw-rw-rw-   0        0        0    35823 2023-04-14 02:47:40.000000 PyQt6-Frameless-Window-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     5582 2023-04-17 07:16:57.758530 PyQt6-Frameless-Window-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-17 07:16:57.718817 PyQt6-Frameless-Window-0.1.1/PyQt6_Frameless_Window.egg-info/
+-rw-rw-rw-   0        0        0     5582 2023-04-17 07:16:57.000000 PyQt6-Frameless-Window-0.1.1/PyQt6_Frameless_Window.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      848 2023-04-17 07:16:57.000000 PyQt6-Frameless-Window-0.1.1/PyQt6_Frameless_Window.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 07:16:57.000000 PyQt6-Frameless-Window-0.1.1/PyQt6_Frameless_Window.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-04-17 07:16:57.000000 PyQt6-Frameless-Window-0.1.1/PyQt6_Frameless_Window.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-04-17 07:16:57.000000 PyQt6-Frameless-Window-0.1.1/PyQt6_Frameless_Window.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5007 2023-04-17 07:14:43.000000 PyQt6-Frameless-Window-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 07:16:57.721387 PyQt6-Frameless-Window-0.1.1/qframelesswindow/
+-rw-rw-rw-   0        0        0     1615 2023-04-17 07:15:33.000000 PyQt6-Frameless-Window-0.1.1/qframelesswindow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 07:16:57.725809 PyQt6-Frameless-Window-0.1.1/qframelesswindow/_rc/
+-rw-rw-rw-   0        0        0        0 2023-01-28 14:21:55.000000 PyQt6-Frameless-Window-0.1.1/qframelesswindow/_rc/__init__.py
+-rw-rw-rw-   0        0        0     2728 2023-04-17 07:14:43.000000 PyQt6-Frameless-Window-0.1.1/qframelesswindow/_rc/resource.py
+drwxrwxrwx   0        0        0        0 2023-04-17 07:16:57.730780 PyQt6-Frameless-Window-0.1.1/qframelesswindow/linux/
+-rw-rw-rw-   0        0        0     3110 2023-04-17 07:14:43.000000 PyQt6-Frameless-Window-0.1.1/qframelesswindow/linux/__init__.py
+-rw-rw-rw-   0        0        0     2920 2023-04-17 07:14:43.000000 PyQt6-Frameless-Window-0.1.1/qframelesswindow/linux/window_effect.py
+drwxrwxrwx   0        0        0        0 2023-04-17 07:16:57.735564 PyQt6-Frameless-Window-0.1.1/qframelesswindow/mac/
+-rw-rw-rw-   0        0        0     3015 2023-04-17 07:14:44.000000 PyQt6-Frameless-Window-0.1.1/qframelesswindow/mac/__init__.py
+-rw-rw-rw-   0        0        0     4095 2023-04-17 07:14:44.000000 PyQt6-Frameless-Window-0.1.1/qframelesswindow/mac/window_effect.py
+drwxrwxrwx   0        0        0        0 2023-04-17 07:16:57.739746 PyQt6-Frameless-Window-0.1.1/qframelesswindow/titlebar/
+-rw-rw-rw-   0        0        0     5083 2023-04-17 07:14:44.000000 PyQt6-Frameless-Window-0.1.1/qframelesswindow/titlebar/__init__.py
+-rw-rw-rw-   0        0        0     9205 2023-04-17 07:14:44.000000 PyQt6-Frameless-Window-0.1.1/qframelesswindow/titlebar/title_bar_buttons.py
+drwxrwxrwx   0        0        0        0 2023-04-17 07:16:57.749907 PyQt6-Frameless-Window-0.1.1/qframelesswindow/utils/
+-rw-rw-rw-   0        0        0      885 2022-07-25 01:20:40.000000 PyQt6-Frameless-Window-0.1.1/qframelesswindow/utils/__init__.py
+-rw-rw-rw-   0        0        0      644 2023-04-17 07:14:44.000000 PyQt6-Frameless-Window-0.1.1/qframelesswindow/utils/linux_utils.py
+-rw-rw-rw-   0        0        0     1850 2023-04-17 07:14:44.000000 PyQt6-Frameless-Window-0.1.1/qframelesswindow/utils/mac_utils.py
+-rw-rw-rw-   0        0        0     8352 2023-04-17 07:15:38.000000 PyQt6-Frameless-Window-0.1.1/qframelesswindow/utils/win32_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-17 07:16:57.756301 PyQt6-Frameless-Window-0.1.1/qframelesswindow/windows/
+-rw-rw-rw-   0        0        0     6624 2023-04-17 07:14:44.000000 PyQt6-Frameless-Window-0.1.1/qframelesswindow/windows/__init__.py
+-rw-rw-rw-   0        0        0     4261 2023-04-17 07:14:44.000000 PyQt6-Frameless-Window-0.1.1/qframelesswindow/windows/c_structures.py
+-rw-rw-rw-   0        0        0     8949 2023-04-17 07:14:44.000000 PyQt6-Frameless-Window-0.1.1/qframelesswindow/windows/window_effect.py
+-rw-rw-rw-   0        0        0       42 2023-04-17 07:16:57.759624 PyQt6-Frameless-Window-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      984 2023-04-17 07:15:25.000000 PyQt6-Frameless-Window-0.1.1/setup.py
```

### Comparing `PyQt6-Frameless-Window-0.1.0/LICENSE` & `PyQt6-Frameless-Window-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.0/PKG-INFO` & `PyQt6-Frameless-Window-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQt6-Frameless-Window
-Version: 0.1.0
+Version: 0.1.1
 Summary: A cross-platform frameless window based on pyqt6, support Win32, Linux and macOS.
 Home-page: https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/PyQt6
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Keywords: pyqt6 frameless
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PyQt6-Frameless-Window-0.1.0/PyQt6_Frameless_Window.egg-info/PKG-INFO` & `PyQt6-Frameless-Window-0.1.1/PyQt6_Frameless_Window.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQt6-Frameless-Window
-Version: 0.1.0
+Version: 0.1.1
 Summary: A cross-platform frameless window based on pyqt6, support Win32, Linux and macOS.
 Home-page: https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/PyQt6
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Keywords: pyqt6 frameless
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PyQt6-Frameless-Window-0.1.0/PyQt6_Frameless_Window.egg-info/SOURCES.txt` & `PyQt6-Frameless-Window-0.1.1/PyQt6_Frameless_Window.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.0/README.md` & `PyQt6-Frameless-Window-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.0/qframelesswindow/__init__.py` & `PyQt6-Frameless-Window-0.1.1/qframelesswindow/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 Examples are available at https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/PyQt6/examples.
 
 :copyright: (c) 2021 by zhiyiYo.
 :license: GPLv3, see LICENSE for more details.
 """
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 
 import sys
 
 from PyQt6.QtWidgets import QDialog, QMainWindow
 
 from .titlebar import TitleBar, TitleBarButton, SvgTitleBarButton, StandardTitleBar
```

### Comparing `PyQt6-Frameless-Window-0.1.0/qframelesswindow/_rc/resource.py` & `PyQt6-Frameless-Window-0.1.1/qframelesswindow/_rc/resource.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.0/qframelesswindow/linux/__init__.py` & `PyQt6-Frameless-Window-0.1.1/qframelesswindow/linux/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.0/qframelesswindow/linux/window_effect.py` & `PyQt6-Frameless-Window-0.1.1/qframelesswindow/linux/window_effect.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.0/qframelesswindow/mac/__init__.py` & `PyQt6-Frameless-Window-0.1.1/qframelesswindow/mac/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.0/qframelesswindow/mac/window_effect.py` & `PyQt6-Frameless-Window-0.1.1/qframelesswindow/mac/window_effect.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.0/qframelesswindow/titlebar/__init__.py` & `PyQt6-Frameless-Window-0.1.1/qframelesswindow/titlebar/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.0/qframelesswindow/titlebar/title_bar_buttons.py` & `PyQt6-Frameless-Window-0.1.1/qframelesswindow/titlebar/title_bar_buttons.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.0/qframelesswindow/utils/__init__.py` & `PyQt6-Frameless-Window-0.1.1/qframelesswindow/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.0/qframelesswindow/utils/linux_utils.py` & `PyQt6-Frameless-Window-0.1.1/qframelesswindow/utils/linux_utils.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.0/qframelesswindow/utils/mac_utils.py` & `PyQt6-Frameless-Window-0.1.1/qframelesswindow/utils/mac_utils.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.0/qframelesswindow/utils/win32_utils.py` & `PyQt6-Frameless-Window-0.1.1/qframelesswindow/utils/win32_utils.py`

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
 from PyQt6.QtCore import QOperatingSystemVersion
 from PyQt6.QtGui import QGuiApplication
 from win32comext.shell import shellcon
 
 
 def isMaximized(hWnd):
     """ Determine whether the window is maximized
@@ -80,27 +81,62 @@
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
 
     thickness = 8 if IsCompositionEnabled() else 4
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

### Comparing `PyQt6-Frameless-Window-0.1.0/qframelesswindow/windows/__init__.py` & `PyQt6-Frameless-Window-0.1.1/qframelesswindow/windows/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.0/qframelesswindow/windows/c_structures.py` & `PyQt6-Frameless-Window-0.1.1/qframelesswindow/windows/c_structures.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.0/qframelesswindow/windows/window_effect.py` & `PyQt6-Frameless-Window-0.1.1/qframelesswindow/windows/window_effect.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.0/setup.py` & `PyQt6-Frameless-Window-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="PyQt6-Frameless-Window",
-    version="0.1.0",
+    version="0.1.1",
     keywords="pyqt6 frameless",
     author="zhiyiYo",
     author_email="shokokawaii@outlook.com",
     description="A cross-platform frameless window based on pyqt6, support Win32, Linux and macOS.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="GPLv3",
```

