# Comparing `tmp/PyQt5-Frameless-Window-0.2.4.tar.gz` & `tmp/PyQt5-Frameless-Window-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PyQt5-Frameless-Window-0.2.4.tar", last modified: Tue Mar 28 02:20:34 2023, max compression
+gzip compressed data, was "dist\PyQt5-Frameless-Window-0.2.5.tar", last modified: Mon Apr 17 07:13:39 2023, max compression
```

## Comparing `PyQt5-Frameless-Window-0.2.4.tar` & `PyQt5-Frameless-Window-0.2.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-03-28 02:20:34.032613 PyQt5-Frameless-Window-0.2.4/
--rw-rw-rw-   0        0        0    35823 2023-03-28 01:52:53.000000 PyQt5-Frameless-Window-0.2.4/LICENSE
--rw-rw-rw-   0        0        0     5508 2023-03-28 02:20:34.029994 PyQt5-Frameless-Window-0.2.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-03-28 02:20:33.981958 PyQt5-Frameless-Window-0.2.4/PyQt5_Frameless_Window.egg-info/
--rw-rw-rw-   0        0        0     5508 2023-03-28 02:20:33.000000 PyQt5-Frameless-Window-0.2.4/PyQt5_Frameless_Window.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      848 2023-03-28 02:20:33.000000 PyQt5-Frameless-Window-0.2.4/PyQt5_Frameless_Window.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-28 02:20:33.000000 PyQt5-Frameless-Window-0.2.4/PyQt5_Frameless_Window.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      126 2023-03-28 02:20:33.000000 PyQt5-Frameless-Window-0.2.4/PyQt5_Frameless_Window.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-03-28 02:20:33.000000 PyQt5-Frameless-Window-0.2.4/PyQt5_Frameless_Window.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4938 2023-03-28 02:19:14.000000 PyQt5-Frameless-Window-0.2.4/README.md
-drwxrwxrwx   0        0        0        0 2023-03-28 02:20:33.994082 PyQt5-Frameless-Window-0.2.4/qframelesswindow/
--rw-rw-rw-   0        0        0     1616 2023-03-28 02:07:59.000000 PyQt5-Frameless-Window-0.2.4/qframelesswindow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-28 02:20:33.998759 PyQt5-Frameless-Window-0.2.4/qframelesswindow/_rc/
--rw-rw-rw-   0        0        0        0 2023-01-28 14:21:55.000000 PyQt5-Frameless-Window-0.2.4/qframelesswindow/_rc/__init__.py
--rw-rw-rw-   0        0        0     2728 2023-03-12 04:01:36.000000 PyQt5-Frameless-Window-0.2.4/qframelesswindow/_rc/resource.py
-drwxrwxrwx   0        0        0        0 2023-03-28 02:20:34.002620 PyQt5-Frameless-Window-0.2.4/qframelesswindow/linux/
--rw-rw-rw-   0        0        0     2891 2023-03-12 04:01:36.000000 PyQt5-Frameless-Window-0.2.4/qframelesswindow/linux/__init__.py
--rw-rw-rw-   0        0        0     2683 2023-03-12 03:51:48.000000 PyQt5-Frameless-Window-0.2.4/qframelesswindow/linux/window_effect.py
-drwxrwxrwx   0        0        0        0 2023-03-28 02:20:34.007043 PyQt5-Frameless-Window-0.2.4/qframelesswindow/mac/
--rw-rw-rw-   0        0        0     2994 2023-03-12 04:01:36.000000 PyQt5-Frameless-Window-0.2.4/qframelesswindow/mac/__init__.py
--rw-rw-rw-   0        0        0     3898 2023-03-12 04:01:36.000000 PyQt5-Frameless-Window-0.2.4/qframelesswindow/mac/window_effect.py
-drwxrwxrwx   0        0        0        0 2023-03-28 02:20:34.012248 PyQt5-Frameless-Window-0.2.4/qframelesswindow/titlebar/
--rw-rw-rw-   0        0        0     4984 2023-03-12 04:01:36.000000 PyQt5-Frameless-Window-0.2.4/qframelesswindow/titlebar/__init__.py
--rw-rw-rw-   0        0        0     9057 2023-03-12 04:01:36.000000 PyQt5-Frameless-Window-0.2.4/qframelesswindow/titlebar/title_bar_buttons.py
-drwxrwxrwx   0        0        0        0 2023-03-28 02:20:34.021377 PyQt5-Frameless-Window-0.2.4/qframelesswindow/utils/
--rw-rw-rw-   0        0        0      885 2022-07-25 01:20:40.000000 PyQt5-Frameless-Window-0.2.4/qframelesswindow/utils/__init__.py
--rw-rw-rw-   0        0        0     5299 2023-03-12 04:01:36.000000 PyQt5-Frameless-Window-0.2.4/qframelesswindow/utils/linux_utils.py
--rw-rw-rw-   0        0        0     1850 2023-03-12 04:01:36.000000 PyQt5-Frameless-Window-0.2.4/qframelesswindow/utils/mac_utils.py
--rw-rw-rw-   0        0        0     7240 2023-03-12 04:01:36.000000 PyQt5-Frameless-Window-0.2.4/qframelesswindow/utils/win32_utils.py
-drwxrwxrwx   0        0        0        0 2023-03-28 02:20:34.027408 PyQt5-Frameless-Window-0.2.4/qframelesswindow/windows/
--rw-rw-rw-   0        0        0     6715 2023-03-20 16:32:46.000000 PyQt5-Frameless-Window-0.2.4/qframelesswindow/windows/__init__.py
--rw-rw-rw-   0        0        0     4013 2023-03-12 03:51:48.000000 PyQt5-Frameless-Window-0.2.4/qframelesswindow/windows/c_structures.py
--rw-rw-rw-   0        0        0     8344 2023-03-12 04:01:36.000000 PyQt5-Frameless-Window-0.2.4/qframelesswindow/windows/window_effect.py
--rw-rw-rw-   0        0        0       42 2023-03-28 02:20:34.032613 PyQt5-Frameless-Window-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0     1023 2023-03-28 02:05:46.000000 PyQt5-Frameless-Window-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 07:13:39.696361 PyQt5-Frameless-Window-0.2.5/
+-rw-rw-rw-   0        0        0    35823 2023-04-14 02:47:40.000000 PyQt5-Frameless-Window-0.2.5/LICENSE
+-rw-rw-rw-   0        0        0     5051 2023-04-17 07:13:39.695228 PyQt5-Frameless-Window-0.2.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-17 07:13:39.654105 PyQt5-Frameless-Window-0.2.5/PyQt5_Frameless_Window.egg-info/
+-rw-rw-rw-   0        0        0     5051 2023-04-17 07:13:39.000000 PyQt5-Frameless-Window-0.2.5/PyQt5_Frameless_Window.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      848 2023-04-17 07:13:39.000000 PyQt5-Frameless-Window-0.2.5/PyQt5_Frameless_Window.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 07:13:39.000000 PyQt5-Frameless-Window-0.2.5/PyQt5_Frameless_Window.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      126 2023-04-17 07:13:39.000000 PyQt5-Frameless-Window-0.2.5/PyQt5_Frameless_Window.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-04-17 07:13:39.000000 PyQt5-Frameless-Window-0.2.5/PyQt5_Frameless_Window.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4481 2023-04-14 02:48:03.000000 PyQt5-Frameless-Window-0.2.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 07:13:39.656305 PyQt5-Frameless-Window-0.2.5/qframelesswindow/
+-rw-rw-rw-   0        0        0     1616 2023-04-17 07:12:34.000000 PyQt5-Frameless-Window-0.2.5/qframelesswindow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 07:13:39.660694 PyQt5-Frameless-Window-0.2.5/qframelesswindow/_rc/
+-rw-rw-rw-   0        0        0        0 2023-01-28 14:21:55.000000 PyQt5-Frameless-Window-0.2.5/qframelesswindow/_rc/__init__.py
+-rw-rw-rw-   0        0        0     2728 2023-04-14 02:47:40.000000 PyQt5-Frameless-Window-0.2.5/qframelesswindow/_rc/resource.py
+drwxrwxrwx   0        0        0        0 2023-04-17 07:13:39.665463 PyQt5-Frameless-Window-0.2.5/qframelesswindow/linux/
+-rw-rw-rw-   0        0        0     2891 2023-04-14 02:47:40.000000 PyQt5-Frameless-Window-0.2.5/qframelesswindow/linux/__init__.py
+-rw-rw-rw-   0        0        0     2683 2023-04-14 02:47:40.000000 PyQt5-Frameless-Window-0.2.5/qframelesswindow/linux/window_effect.py
+drwxrwxrwx   0        0        0        0 2023-04-17 07:13:39.670902 PyQt5-Frameless-Window-0.2.5/qframelesswindow/mac/
+-rw-rw-rw-   0        0        0     2994 2023-04-14 02:47:40.000000 PyQt5-Frameless-Window-0.2.5/qframelesswindow/mac/__init__.py
+-rw-rw-rw-   0        0        0     3898 2023-04-14 02:47:40.000000 PyQt5-Frameless-Window-0.2.5/qframelesswindow/mac/window_effect.py
+drwxrwxrwx   0        0        0        0 2023-04-17 07:13:39.674582 PyQt5-Frameless-Window-0.2.5/qframelesswindow/titlebar/
+-rw-rw-rw-   0        0        0     4984 2023-04-14 02:47:40.000000 PyQt5-Frameless-Window-0.2.5/qframelesswindow/titlebar/__init__.py
+-rw-rw-rw-   0        0        0     9057 2023-04-14 02:47:40.000000 PyQt5-Frameless-Window-0.2.5/qframelesswindow/titlebar/title_bar_buttons.py
+drwxrwxrwx   0        0        0        0 2023-04-17 07:13:39.684873 PyQt5-Frameless-Window-0.2.5/qframelesswindow/utils/
+-rw-rw-rw-   0        0        0      885 2022-07-25 01:20:40.000000 PyQt5-Frameless-Window-0.2.5/qframelesswindow/utils/__init__.py
+-rw-rw-rw-   0        0        0     5299 2023-04-14 02:47:40.000000 PyQt5-Frameless-Window-0.2.5/qframelesswindow/utils/linux_utils.py
+-rw-rw-rw-   0        0        0     1850 2023-04-14 02:47:40.000000 PyQt5-Frameless-Window-0.2.5/qframelesswindow/utils/mac_utils.py
+-rw-rw-rw-   0        0        0     8190 2023-04-17 06:53:54.000000 PyQt5-Frameless-Window-0.2.5/qframelesswindow/utils/win32_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-17 07:13:39.692056 PyQt5-Frameless-Window-0.2.5/qframelesswindow/windows/
+-rw-rw-rw-   0        0        0     6715 2023-04-14 02:47:40.000000 PyQt5-Frameless-Window-0.2.5/qframelesswindow/windows/__init__.py
+-rw-rw-rw-   0        0        0     4013 2023-04-14 02:47:40.000000 PyQt5-Frameless-Window-0.2.5/qframelesswindow/windows/c_structures.py
+-rw-rw-rw-   0        0        0     8344 2023-04-14 02:47:40.000000 PyQt5-Frameless-Window-0.2.5/qframelesswindow/windows/window_effect.py
+-rw-rw-rw-   0        0        0       42 2023-04-17 07:13:39.696361 PyQt5-Frameless-Window-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     1023 2023-04-17 07:12:27.000000 PyQt5-Frameless-Window-0.2.5/setup.py
```

### Comparing `PyQt5-Frameless-Window-0.2.4/LICENSE` & `PyQt5-Frameless-Window-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.4/PKG-INFO` & `PyQt5-Frameless-Window-0.2.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: PyQt5-Frameless-Window
-Version: 0.2.4
+Version: 0.2.5
 Summary: A cross-platform frameless window based on pyqt5, support Win32, X11, Wayland and macOS.
 Home-page: https://github.com/zhiyiYo/PyQt-Frameless-Window
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Keywords: pyqt frameless
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
-  <img width="15%" align="center" src="https://raw.githubusercontent.com/zhiyiYo/PyQt-Frameless-Window/master/screenshot/logo.png" alt="logo">
+  <img width="15%" align="center" src="screenshot/logo.png" alt="logo">
 </p>
   <h1 align="center">
   PyQt-Frameless-Window
 </h1>
 <p align="center">
   A cross-platform frameless window based on PyQt5
 </p>
@@ -29,19 +29,19 @@
   </a>
 
   <a style="text-decoration:none">
     <img src="https://static.pepy.tech/personalized-badge/pyqt5-frameless-window?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads" alt="Download"/>
   </a>
 
   <a style="text-decoration:none">
-    <img src="https://img.shields.io/badge/License-MIT-blue?color=#4ec820" alt="MIT"/>
+    <img src="https://img.shields.io/badge/License-GPLv3-blue?color=#4ec820" alt="GPLv3"/>
   </a>
 </p>
 
-![Cover](https://raw.githubusercontent.com/zhiyiYo/PyQt-Frameless-Window/master/screenshot/cover.jpg)
+![Cover](screenshot/cover.jpg)
 
 
 ## Features
 * Moving
 * Stretching
 * Window shadow
 * Window animation
@@ -90,29 +90,29 @@
 
 if __name__ == '__main__':
     app = QApplication(sys.argv)
     demo = Window()
     demo.show()
     sys.exit(app.exec_())
 ```
-For more complex requirements, see [demo.py](https://github.com/zhiyiYo/PyQt-Frameless-Window/blob/master/examples/demo.py) and [main_window.py](https://github.com/zhiyiYo/PyQt-Frameless-Window/blob/master/examples/main_window.py).
+For more complex requirements, see [demo.py](./examples/demo.py) and [main_window.py](./examples/main_window.py).
 
 ## Examples
 * Normal frameless window
-![Normal Frameless Window](https://raw.githubusercontent.com/zhiyiYo/PyQt-Frameless-Window/master/screenshot/normal_frameless_window.gif)
+![Normal Frameless Window](screenshot/normal_frameless_window.gif)
 * Acrylic frameless window
-![Acrylic Frameless Window](https://raw.githubusercontent.com/zhiyiYo/PyQt-Frameless-Window/master/screenshot/acrylic_window.jpg)
+![Acrylic Frameless Window](screenshot/acrylic_window.jpg)
 
 
 ## Document
 Want to know more about PyQt-Frameless-Window? Please read the [help document](https://pyqt-frameless-window.readthedocs.io/) 👈
 
 
 ## Notes
-1. `FramelessWindow` provides a default custom title bar. If you don't like it, just rewrite it as [demo.py](https://github.com/zhiyiYo/PyQt-Frameless-Window/blob/master/examples/demo.py) does.
+1. `FramelessWindow` provides a default custom title bar. If you don't like it, just rewrite it as [demo.py](./examples/demo.py) does.
 
 2. Moving the acrylic window on Win10 may get stuck. At present, there is no good solution. Maybe you can disable the acrylic effect when moving the window, but I haven't done this in the source code.
 3. Snap layout is not enabled by default. See [#56](https://github.com/zhiyiYo/PyQt-Frameless-Window/issues/56) to learn how to enable it.
 
 4. If you encounter this problem on Windows:
    > ImportError: DLL load failed while importing win32api
```

### Comparing `PyQt5-Frameless-Window-0.2.4/PyQt5_Frameless_Window.egg-info/PKG-INFO` & `PyQt5-Frameless-Window-0.2.5/PyQt5_Frameless_Window.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: PyQt5-Frameless-Window
-Version: 0.2.4
+Version: 0.2.5
 Summary: A cross-platform frameless window based on pyqt5, support Win32, X11, Wayland and macOS.
 Home-page: https://github.com/zhiyiYo/PyQt-Frameless-Window
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Keywords: pyqt frameless
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
-  <img width="15%" align="center" src="https://raw.githubusercontent.com/zhiyiYo/PyQt-Frameless-Window/master/screenshot/logo.png" alt="logo">
+  <img width="15%" align="center" src="screenshot/logo.png" alt="logo">
 </p>
   <h1 align="center">
   PyQt-Frameless-Window
 </h1>
 <p align="center">
   A cross-platform frameless window based on PyQt5
 </p>
@@ -29,19 +29,19 @@
   </a>
 
   <a style="text-decoration:none">
     <img src="https://static.pepy.tech/personalized-badge/pyqt5-frameless-window?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads" alt="Download"/>
   </a>
 
   <a style="text-decoration:none">
-    <img src="https://img.shields.io/badge/License-MIT-blue?color=#4ec820" alt="MIT"/>
+    <img src="https://img.shields.io/badge/License-GPLv3-blue?color=#4ec820" alt="GPLv3"/>
   </a>
 </p>
 
-![Cover](https://raw.githubusercontent.com/zhiyiYo/PyQt-Frameless-Window/master/screenshot/cover.jpg)
+![Cover](screenshot/cover.jpg)
 
 
 ## Features
 * Moving
 * Stretching
 * Window shadow
 * Window animation
@@ -90,29 +90,29 @@
 
 if __name__ == '__main__':
     app = QApplication(sys.argv)
     demo = Window()
     demo.show()
     sys.exit(app.exec_())
 ```
-For more complex requirements, see [demo.py](https://github.com/zhiyiYo/PyQt-Frameless-Window/blob/master/examples/demo.py) and [main_window.py](https://github.com/zhiyiYo/PyQt-Frameless-Window/blob/master/examples/main_window.py).
+For more complex requirements, see [demo.py](./examples/demo.py) and [main_window.py](./examples/main_window.py).
 
 ## Examples
 * Normal frameless window
-![Normal Frameless Window](https://raw.githubusercontent.com/zhiyiYo/PyQt-Frameless-Window/master/screenshot/normal_frameless_window.gif)
+![Normal Frameless Window](screenshot/normal_frameless_window.gif)
 * Acrylic frameless window
-![Acrylic Frameless Window](https://raw.githubusercontent.com/zhiyiYo/PyQt-Frameless-Window/master/screenshot/acrylic_window.jpg)
+![Acrylic Frameless Window](screenshot/acrylic_window.jpg)
 
 
 ## Document
 Want to know more about PyQt-Frameless-Window? Please read the [help document](https://pyqt-frameless-window.readthedocs.io/) 👈
 
 
 ## Notes
-1. `FramelessWindow` provides a default custom title bar. If you don't like it, just rewrite it as [demo.py](https://github.com/zhiyiYo/PyQt-Frameless-Window/blob/master/examples/demo.py) does.
+1. `FramelessWindow` provides a default custom title bar. If you don't like it, just rewrite it as [demo.py](./examples/demo.py) does.
 
 2. Moving the acrylic window on Win10 may get stuck. At present, there is no good solution. Maybe you can disable the acrylic effect when moving the window, but I haven't done this in the source code.
 3. Snap layout is not enabled by default. See [#56](https://github.com/zhiyiYo/PyQt-Frameless-Window/issues/56) to learn how to enable it.
 
 4. If you encounter this problem on Windows:
    > ImportError: DLL load failed while importing win32api
```

### Comparing `PyQt5-Frameless-Window-0.2.4/PyQt5_Frameless_Window.egg-info/SOURCES.txt` & `PyQt5-Frameless-Window-0.2.5/PyQt5_Frameless_Window.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.4/qframelesswindow/__init__.py` & `PyQt5-Frameless-Window-0.2.5/qframelesswindow/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 Examples are available at https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/master/examples.
 
 :copyright: (c) 2021 by zhiyiYo.
 :license: GPLv3, see LICENSE for more details.
 """
 
-__version__ = "0.2.4"
+__version__ = "0.2.5"
 
 import sys
 
 from PyQt5.QtWidgets import QDialog, QMainWindow
 
 from .titlebar import TitleBar, TitleBarButton, SvgTitleBarButton, StandardTitleBar
```

### Comparing `PyQt5-Frameless-Window-0.2.4/qframelesswindow/_rc/resource.py` & `PyQt5-Frameless-Window-0.2.5/qframelesswindow/_rc/resource.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.4/qframelesswindow/linux/__init__.py` & `PyQt5-Frameless-Window-0.2.5/qframelesswindow/linux/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.4/qframelesswindow/linux/window_effect.py` & `PyQt5-Frameless-Window-0.2.5/qframelesswindow/linux/window_effect.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.4/qframelesswindow/mac/__init__.py` & `PyQt5-Frameless-Window-0.2.5/qframelesswindow/mac/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.4/qframelesswindow/mac/window_effect.py` & `PyQt5-Frameless-Window-0.2.5/qframelesswindow/mac/window_effect.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.4/qframelesswindow/titlebar/__init__.py` & `PyQt5-Frameless-Window-0.2.5/qframelesswindow/titlebar/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.4/qframelesswindow/titlebar/title_bar_buttons.py` & `PyQt5-Frameless-Window-0.2.5/qframelesswindow/titlebar/title_bar_buttons.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.4/qframelesswindow/utils/__init__.py` & `PyQt5-Frameless-Window-0.2.5/qframelesswindow/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.4/qframelesswindow/utils/linux_utils.py` & `PyQt5-Frameless-Window-0.2.5/qframelesswindow/utils/linux_utils.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.4/qframelesswindow/utils/mac_utils.py` & `PyQt5-Frameless-Window-0.2.5/qframelesswindow/utils/mac_utils.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.4/qframelesswindow/utils/win32_utils.py` & `PyQt5-Frameless-Window-0.2.5/qframelesswindow/utils/win32_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from ctypes.wintypes import DWORD, HWND, LPARAM, RECT, UINT
 from platform import platform
 import sys
 
 import win32api
 import win32con
 import win32gui
+import win32print
 from PyQt5.QtCore import QOperatingSystemVersion
 from PyQt5.QtGui import QGuiApplication
 from PyQt5.QtWinExtras import QtWin
 from win32comext.shell import shellcon
 
 
 def isMaximized(hWnd):
@@ -81,27 +82,62 @@
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
 
     thickness = 8 if QtWin.isCompositionEnabled() else 4
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

### Comparing `PyQt5-Frameless-Window-0.2.4/qframelesswindow/windows/__init__.py` & `PyQt5-Frameless-Window-0.2.5/qframelesswindow/windows/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.4/qframelesswindow/windows/c_structures.py` & `PyQt5-Frameless-Window-0.2.5/qframelesswindow/windows/c_structures.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.4/qframelesswindow/windows/window_effect.py` & `PyQt5-Frameless-Window-0.2.5/qframelesswindow/windows/window_effect.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.4/setup.py` & `PyQt5-Frameless-Window-0.2.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="PyQt5-Frameless-Window",
-    version="0.2.4",
+    version="0.2.5",
     keywords="pyqt frameless",
     author="zhiyiYo",
     author_email="shokokawaii@outlook.com",
     description="A cross-platform frameless window based on pyqt5, support Win32, X11, Wayland and macOS.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="GPLv3",
```

