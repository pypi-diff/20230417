# Comparing `tmp/Termighty-3.0.4.tar.gz` & `tmp/Termighty-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Termighty-3.0.4.tar", last modified: Sun Apr 16 13:54:54 2023, max compression
+gzip compressed data, was "Termighty-3.0.5.tar", last modified: Mon Apr 17 20:44:01 2023, max compression
```

## Comparing `Termighty-3.0.4.tar` & `Termighty-3.0.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 13:54:54.928257 Termighty-3.0.4/
--rw-rw-rw-   0        0        0    35823 2022-09-11 20:43:48.000000 Termighty-3.0.4/LICENSE
--rw-rw-rw-   0        0        0    21213 2023-04-16 13:54:54.928758 Termighty-3.0.4/PKG-INFO
--rw-rw-rw-   0        0        0    20657 2023-04-16 13:48:14.000000 Termighty-3.0.4/README.md
--rw-rw-rw-   0        0        0       93 2023-04-13 17:22:56.000000 Termighty-3.0.4/pyproject.toml
--rw-rw-rw-   0        0        0      130 2023-04-16 13:54:54.931256 Termighty-3.0.4/setup.cfg
--rw-rw-rw-   0        0        0      929 2023-04-16 12:50:11.000000 Termighty-3.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-16 13:54:54.859757 Termighty-3.0.4/source/
-drwxrwxrwx   0        0        0        0 2023-04-16 13:54:54.883757 Termighty-3.0.4/source/Termighty.egg-info/
--rw-rw-rw-   0        0        0    21213 2023-04-16 13:54:54.000000 Termighty-3.0.4/source/Termighty.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      900 2023-04-16 13:54:54.000000 Termighty-3.0.4/source/Termighty.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 13:54:54.000000 Termighty-3.0.4/source/Termighty.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-16 13:54:54.000000 Termighty-3.0.4/source/Termighty.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-16 13:54:54.000000 Termighty-3.0.4/source/Termighty.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-16 13:54:54.887256 Termighty-3.0.4/source/termighty/
--rw-rw-rw-   0        0        0      115 2022-09-11 20:43:48.000000 Termighty-3.0.4/source/termighty/__init__.py
--rw-rw-rw-   0        0        0      403 2022-09-17 22:33:08.000000 Termighty-3.0.4/source/termighty/config.ini
-drwxrwxrwx   0        0        0        0 2023-04-16 13:54:54.894757 Termighty-3.0.4/source/termighty/data/
--rw-rw-rw-   0        0        0     7971 2022-09-17 14:02:53.000000 Termighty-3.0.4/source/termighty/data/keymaps.json
--rw-rw-rw-   0        0        0    66090 2022-09-11 20:43:48.000000 Termighty-3.0.4/source/termighty/data/rgb.json
--rw-rw-rw-   0        0        0      216 2022-09-11 20:43:48.000000 Termighty-3.0.4/source/termighty/data/styles.json
-drwxrwxrwx   0        0        0        0 2023-04-16 13:54:54.901257 Termighty-3.0.4/source/termighty/obj/
--rw-rw-rw-   0        0        0       54 2022-09-11 20:43:48.000000 Termighty-3.0.4/source/termighty/obj/__init__.py
--rw-rw-rw-   0        0        0    15095 2022-09-18 18:49:31.000000 Termighty-3.0.4/source/termighty/obj/color.py
--rw-rw-rw-   0        0        0    17757 2022-09-18 14:21:27.000000 Termighty-3.0.4/source/termighty/obj/string.py
-drwxrwxrwx   0        0        0        0 2023-04-16 13:54:54.909257 Termighty-3.0.4/source/termighty/settings/
--rw-rw-rw-   0        0        0       80 2022-09-11 20:43:48.000000 Termighty-3.0.4/source/termighty/settings/__init__.py
--rw-rw-rw-   0        0        0     1737 2022-09-17 22:33:43.000000 Termighty-3.0.4/source/termighty/settings/config.py
--rw-rw-rw-   0        0        0     1010 2022-09-18 14:22:15.000000 Termighty-3.0.4/source/termighty/settings/data.py
--rw-rw-rw-   0        0        0     1458 2023-04-13 13:51:49.000000 Termighty-3.0.4/source/termighty/settings/system.py
-drwxrwxrwx   0        0        0        0 2023-04-16 13:54:54.918757 Termighty-3.0.4/source/termighty/utils/
--rw-rw-rw-   0        0        0       97 2022-09-18 19:41:57.000000 Termighty-3.0.4/source/termighty/utils/__init__.py
--rw-rw-rw-   0        0        0    45164 2023-04-15 22:32:49.000000 Termighty-3.0.4/source/termighty/utils/key_processor.py
--rw-rw-rw-   0        0        0    10100 2023-04-13 14:40:44.000000 Termighty-3.0.4/source/termighty/utils/listener.py
--rw-rw-rw-   0        0        0     5463 2023-04-13 14:00:48.000000 Termighty-3.0.4/source/termighty/utils/term.py
-drwxrwxrwx   0        0        0        0 2023-04-16 13:54:54.925257 Termighty-3.0.4/source/termighty/widgets/
--rw-rw-rw-   0        0        0       68 2022-09-12 19:41:55.000000 Termighty-3.0.4/source/termighty/widgets/__init__.py
--rw-rw-rw-   0        0        0    18807 2023-04-16 13:27:48.000000 Termighty-3.0.4/source/termighty/widgets/text_box.py
--rw-rw-rw-   0        0        0    16942 2023-04-16 12:49:28.000000 Termighty-3.0.4/source/termighty/widgets/text_editor.py
+drwxrwxrwx   0        0        0        0 2023-04-17 20:44:01.961016 Termighty-3.0.5/
+-rw-rw-rw-   0        0        0    35823 2022-09-11 20:43:48.000000 Termighty-3.0.5/LICENSE
+-rw-rw-rw-   0        0        0    23343 2023-04-17 20:44:01.961516 Termighty-3.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0    22787 2023-04-16 14:04:47.000000 Termighty-3.0.5/README.md
+-rw-rw-rw-   0        0        0       93 2023-04-13 17:22:56.000000 Termighty-3.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0      130 2023-04-17 20:44:01.964017 Termighty-3.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      929 2023-04-17 20:43:47.000000 Termighty-3.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 20:44:01.775507 Termighty-3.0.5/source/
+drwxrwxrwx   0        0        0        0 2023-04-17 20:44:01.801007 Termighty-3.0.5/source/Termighty.egg-info/
+-rw-rw-rw-   0        0        0    23343 2023-04-17 20:44:01.000000 Termighty-3.0.5/source/Termighty.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      900 2023-04-17 20:44:01.000000 Termighty-3.0.5/source/Termighty.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 20:44:01.000000 Termighty-3.0.5/source/Termighty.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-17 20:44:01.000000 Termighty-3.0.5/source/Termighty.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-17 20:44:01.000000 Termighty-3.0.5/source/Termighty.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 20:44:01.805508 Termighty-3.0.5/source/termighty/
+-rw-rw-rw-   0        0        0      115 2022-09-11 20:43:48.000000 Termighty-3.0.5/source/termighty/__init__.py
+-rw-rw-rw-   0        0        0      403 2022-09-17 22:33:08.000000 Termighty-3.0.5/source/termighty/config.ini
+drwxrwxrwx   0        0        0        0 2023-04-17 20:44:01.813007 Termighty-3.0.5/source/termighty/data/
+-rw-rw-rw-   0        0        0     7971 2022-09-17 14:02:53.000000 Termighty-3.0.5/source/termighty/data/keymaps.json
+-rw-rw-rw-   0        0        0    66090 2022-09-11 20:43:48.000000 Termighty-3.0.5/source/termighty/data/rgb.json
+-rw-rw-rw-   0        0        0      216 2022-09-11 20:43:48.000000 Termighty-3.0.5/source/termighty/data/styles.json
+drwxrwxrwx   0        0        0        0 2023-04-17 20:44:01.823506 Termighty-3.0.5/source/termighty/obj/
+-rw-rw-rw-   0        0        0       54 2022-09-11 20:43:48.000000 Termighty-3.0.5/source/termighty/obj/__init__.py
+-rw-rw-rw-   0        0        0    15095 2022-09-18 18:49:31.000000 Termighty-3.0.5/source/termighty/obj/color.py
+-rw-rw-rw-   0        0        0    17757 2022-09-18 14:21:27.000000 Termighty-3.0.5/source/termighty/obj/string.py
+drwxrwxrwx   0        0        0        0 2023-04-17 20:44:01.882506 Termighty-3.0.5/source/termighty/settings/
+-rw-rw-rw-   0        0        0       80 2022-09-11 20:43:48.000000 Termighty-3.0.5/source/termighty/settings/__init__.py
+-rw-rw-rw-   0        0        0     1737 2022-09-17 22:33:43.000000 Termighty-3.0.5/source/termighty/settings/config.py
+-rw-rw-rw-   0        0        0     1010 2022-09-18 14:22:15.000000 Termighty-3.0.5/source/termighty/settings/data.py
+-rw-rw-rw-   0        0        0     1458 2023-04-13 13:51:49.000000 Termighty-3.0.5/source/termighty/settings/system.py
+drwxrwxrwx   0        0        0        0 2023-04-17 20:44:01.950517 Termighty-3.0.5/source/termighty/utils/
+-rw-rw-rw-   0        0        0       97 2022-09-18 19:41:57.000000 Termighty-3.0.5/source/termighty/utils/__init__.py
+-rw-rw-rw-   0        0        0    45164 2023-04-15 22:32:49.000000 Termighty-3.0.5/source/termighty/utils/key_processor.py
+-rw-rw-rw-   0        0        0    10100 2023-04-13 14:40:44.000000 Termighty-3.0.5/source/termighty/utils/listener.py
+-rw-rw-rw-   0        0        0     5463 2023-04-13 14:00:48.000000 Termighty-3.0.5/source/termighty/utils/term.py
+drwxrwxrwx   0        0        0        0 2023-04-17 20:44:01.958017 Termighty-3.0.5/source/termighty/widgets/
+-rw-rw-rw-   0        0        0       68 2022-09-12 19:41:55.000000 Termighty-3.0.5/source/termighty/widgets/__init__.py
+-rw-rw-rw-   0        0        0    18767 2023-04-17 20:35:34.000000 Termighty-3.0.5/source/termighty/widgets/text_box.py
+-rw-rw-rw-   0        0        0    16935 2023-04-17 20:41:56.000000 Termighty-3.0.5/source/termighty/widgets/text_editor.py
```

### Comparing `Termighty-3.0.4/LICENSE` & `Termighty-3.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `Termighty-3.0.4/PKG-INFO` & `Termighty-3.0.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-Metadata-Version: 2.1
-Name: Termighty
-Version: 3.0.4
-Summary: Cross-Platform Terminal Coloring, Formatting, and Management Utilities.
-Home-page: https://github.com/GabrielSCabrera/Termighty
-Download-URL: https://github.com/GabrielSCabrera/Termightyarchive/v3.0.4.tar.gz
-Author: Gabriel S. Cabrera
-Author-email: gabriel.sigurd.cabrera@gmail.com
-Keywords: terminal,xterm,gui,windows,linux
-Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
 # Termighty
+### High-level utilities for cross-platform terminal interaction.
+
+Termighty is a Python package that provides a comprehensive set of tools for managing and customizing the terminal environment, as well as handling user inputs and creating dynamic text displays. It consists of several classes, each serving specific purposes.
+
+The Term class offers commands for modifying the terminal state, managing multiple buffers, and controlling terminal output. It includes methods for initializing the class, playing the terminal bell sound, clearing the terminal screen, hiding and showing the cursor, moving and saving the cursor position, and writing to the terminal.
+
+The String class is an advanced version of Python's built-in str class, designed to handle ANSI Escape Sequences for custom text and background colors, as well as text styles. It provides methods for listing available styles, creating instances with specific colors and styles, and implementing magic methods to use the String class like a built-in string.
+
+The Color class manages colors in RGB format and can be used in conjunction with the String class or for modifying terminal background and foreground colors directly. It supports many operations between colors, unary operations on colors, and color instantiation from a comprehensive catalog of colors.
+
+The GetchIterator class is designed to iterate over a Listener's history, yielding all new additions to the history until the Listener is stopped. The Listener class, a superclass that must be inherited before instantiation, allows users to display live, dynamic text on the terminal while simultaneously accepting user inputs.
+
+The TextBox class provides a base for rectangular shapes (with or without text) that display on the terminal. It simplifies and standardizes the creation of more complex objects. The TextEditor class, a subclass of TextBox, emulates a fully-functional word processor with advanced features such as cursor positioning, and text selection.
 
-High-level utilities for cross-platform terminal interaction.
+In summary, Termighty is a powerful package that enables developers to create customized terminal experiences with enhanced text manipulation, user input handling, and dynamic displays.
 
 # Class Documentation: System
 
 The `System` class is used to keep track of the terminal dimensions and detect the current OS. It also contains the `kill_all` class attribute, which is by default set to `False`. If it is set to `True`, all active Termighty threads will be killed.
 
 ## Attributes
```

### Comparing `Termighty-3.0.4/README.md` & `Termighty-3.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,37 @@
+Metadata-Version: 2.1
+Name: Termighty
+Version: 3.0.5
+Summary: Cross-Platform Terminal Coloring, Formatting, and Management Utilities.
+Home-page: https://github.com/GabrielSCabrera/Termighty
+Download-URL: https://github.com/GabrielSCabrera/Termightyarchive/v3.0.5.tar.gz
+Author: Gabriel S. Cabrera
+Author-email: gabriel.sigurd.cabrera@gmail.com
+Keywords: terminal,xterm,gui,windows,linux
+Classifier: Development Status :: 3 - Alpha
+Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
 # Termighty
+### High-level utilities for cross-platform terminal interaction.
+
+Termighty is a Python package that provides a comprehensive set of tools for managing and customizing the terminal environment, as well as handling user inputs and creating dynamic text displays. It consists of several classes, each serving specific purposes.
+
+The Term class offers commands for modifying the terminal state, managing multiple buffers, and controlling terminal output. It includes methods for initializing the class, playing the terminal bell sound, clearing the terminal screen, hiding and showing the cursor, moving and saving the cursor position, and writing to the terminal.
+
+The String class is an advanced version of Python's built-in str class, designed to handle ANSI Escape Sequences for custom text and background colors, as well as text styles. It provides methods for listing available styles, creating instances with specific colors and styles, and implementing magic methods to use the String class like a built-in string.
+
+The Color class manages colors in RGB format and can be used in conjunction with the String class or for modifying terminal background and foreground colors directly. It supports many operations between colors, unary operations on colors, and color instantiation from a comprehensive catalog of colors.
+
+The GetchIterator class is designed to iterate over a Listener's history, yielding all new additions to the history until the Listener is stopped. The Listener class, a superclass that must be inherited before instantiation, allows users to display live, dynamic text on the terminal while simultaneously accepting user inputs.
+
+The TextBox class provides a base for rectangular shapes (with or without text) that display on the terminal. It simplifies and standardizes the creation of more complex objects. The TextEditor class, a subclass of TextBox, emulates a fully-functional word processor with advanced features such as cursor positioning, and text selection.
 
-High-level utilities for cross-platform terminal interaction.
+In summary, Termighty is a powerful package that enables developers to create customized terminal experiences with enhanced text manipulation, user input handling, and dynamic displays.
 
 # Class Documentation: System
 
 The `System` class is used to keep track of the terminal dimensions and detect the current OS. It also contains the `kill_all` class attribute, which is by default set to `False`. If it is set to `True`, all active Termighty threads will be killed.
 
 ## Attributes
```

### Comparing `Termighty-3.0.4/setup.py` & `Termighty-3.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 
 setup(
     name="Termighty",
     packages=find_packages(where="source"),
     package_dir={"": "source"},
     include_package_data=True,
     package_data={"": ["data/*.json", "config.ini"]},
-    version="3.0.4",
+    version="3.0.5",
     description="Cross-Platform Terminal Coloring, Formatting, and Management Utilities.",
     long_description=long_description,
     author="Gabriel S. Cabrera",
     author_email="gabriel.sigurd.cabrera@gmail.com",
     url=url,
-    download_url=url + "archive/v3.0.4.tar.gz",
+    download_url=url + "archive/v3.0.5.tar.gz",
     keywords=["terminal", "xterm", "gui", "windows", "linux"],
     install_requires=dependencies,
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Programming Language :: Python :: 3.10",
     ],
 )
```

### Comparing `Termighty-3.0.4/source/Termighty.egg-info/PKG-INFO` & `Termighty-3.0.5/source/Termighty.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,37 @@
 Metadata-Version: 2.1
 Name: Termighty
-Version: 3.0.4
+Version: 3.0.5
 Summary: Cross-Platform Terminal Coloring, Formatting, and Management Utilities.
 Home-page: https://github.com/GabrielSCabrera/Termighty
-Download-URL: https://github.com/GabrielSCabrera/Termightyarchive/v3.0.4.tar.gz
+Download-URL: https://github.com/GabrielSCabrera/Termightyarchive/v3.0.5.tar.gz
 Author: Gabriel S. Cabrera
 Author-email: gabriel.sigurd.cabrera@gmail.com
 Keywords: terminal,xterm,gui,windows,linux
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 # Termighty
+### High-level utilities for cross-platform terminal interaction.
 
-High-level utilities for cross-platform terminal interaction.
+Termighty is a Python package that provides a comprehensive set of tools for managing and customizing the terminal environment, as well as handling user inputs and creating dynamic text displays. It consists of several classes, each serving specific purposes.
+
+The Term class offers commands for modifying the terminal state, managing multiple buffers, and controlling terminal output. It includes methods for initializing the class, playing the terminal bell sound, clearing the terminal screen, hiding and showing the cursor, moving and saving the cursor position, and writing to the terminal.
+
+The String class is an advanced version of Python's built-in str class, designed to handle ANSI Escape Sequences for custom text and background colors, as well as text styles. It provides methods for listing available styles, creating instances with specific colors and styles, and implementing magic methods to use the String class like a built-in string.
+
+The Color class manages colors in RGB format and can be used in conjunction with the String class or for modifying terminal background and foreground colors directly. It supports many operations between colors, unary operations on colors, and color instantiation from a comprehensive catalog of colors.
+
+The GetchIterator class is designed to iterate over a Listener's history, yielding all new additions to the history until the Listener is stopped. The Listener class, a superclass that must be inherited before instantiation, allows users to display live, dynamic text on the terminal while simultaneously accepting user inputs.
+
+The TextBox class provides a base for rectangular shapes (with or without text) that display on the terminal. It simplifies and standardizes the creation of more complex objects. The TextEditor class, a subclass of TextBox, emulates a fully-functional word processor with advanced features such as cursor positioning, and text selection.
+
+In summary, Termighty is a powerful package that enables developers to create customized terminal experiences with enhanced text manipulation, user input handling, and dynamic displays.
 
 # Class Documentation: System
 
 The `System` class is used to keep track of the terminal dimensions and detect the current OS. It also contains the `kill_all` class attribute, which is by default set to `False`. If it is set to `True`, all active Termighty threads will be killed.
 
 ## Attributes
```

### Comparing `Termighty-3.0.4/source/Termighty.egg-info/SOURCES.txt` & `Termighty-3.0.5/source/Termighty.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Termighty-3.0.4/source/termighty/data/keymaps.json` & `Termighty-3.0.5/source/termighty/data/keymaps.json`

 * *Files identical despite different names*

### Comparing `Termighty-3.0.4/source/termighty/data/rgb.json` & `Termighty-3.0.5/source/termighty/data/rgb.json`

 * *Files identical despite different names*

### Comparing `Termighty-3.0.4/source/termighty/obj/color.py` & `Termighty-3.0.5/source/termighty/obj/color.py`

 * *Files identical despite different names*

### Comparing `Termighty-3.0.4/source/termighty/obj/string.py` & `Termighty-3.0.5/source/termighty/obj/string.py`

 * *Files identical despite different names*

### Comparing `Termighty-3.0.4/source/termighty/settings/config.py` & `Termighty-3.0.5/source/termighty/settings/config.py`

 * *Files identical despite different names*

### Comparing `Termighty-3.0.4/source/termighty/settings/data.py` & `Termighty-3.0.5/source/termighty/settings/data.py`

 * *Files identical despite different names*

### Comparing `Termighty-3.0.4/source/termighty/settings/system.py` & `Termighty-3.0.5/source/termighty/settings/system.py`

 * *Files identical despite different names*

### Comparing `Termighty-3.0.4/source/termighty/utils/key_processor.py` & `Termighty-3.0.5/source/termighty/utils/key_processor.py`

 * *Files identical despite different names*

### Comparing `Termighty-3.0.4/source/termighty/utils/listener.py` & `Termighty-3.0.5/source/termighty/utils/listener.py`

 * *Files identical despite different names*

### Comparing `Termighty-3.0.4/source/termighty/utils/term.py` & `Termighty-3.0.5/source/termighty/utils/term.py`

 * *Files identical despite different names*

### Comparing `Termighty-3.0.4/source/termighty/widgets/text_box.py` & `Termighty-3.0.5/source/termighty/widgets/text_box.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,14 @@
 
         self._active: bool = False
         self._view_changed: bool = False
         self._text: list[str, ...] = None  # [""]
 
         # Whether the text should wrap to the next line if a line exceeds the width of the underlying TextBox.
         self._wrap_text: bool = wrap_text
-        self._wrap_text_width: int = self._shape[1]
         self._wrap_subsequent_indent: str = wrap_subsequent_indent
         self._wrap_text_break_on_hyphens: bool = wrap_text_break_on_hyphens
         self._wrap_text_break_long_words: bool = wrap_text_break_long_words
         self._process_text_wrapper()
 
     """MAGIC METHODS"""
 
@@ -105,20 +104,19 @@
         """
         Justify the raw text given to the __call__ method such that all lines of text are equally-sized, and wide enough
         to allow for the view of the text to be moved left, right, up, and down, until the text is just out of view.
 
         Takes the `self._alignment` attribute into account, aligning the text either to the left, right, or center of
         the TextBox.
         """
-        self._process_text_wrapper()
         if self._wrap_text:
             self._new_line: list[bool, ...] = [
                 i == 0 for row in self._text for i in range(len(self._text_wrapper.wrap(row)))
             ]
-            text: list[str, ...] = [line for row in self._text for line in self._text_wrapper.wrap(row)]
+            text: list[str, ...] = [line.strip() for row in self._text for line in self._text_wrapper.wrap(row)]
         else:
             self._new_line: list[bool] = [True for i in range(self._shape[0])]
             text: list[str, ...] = self._text
 
         rows: int = len(text)
         cols: int = max(len(row) for row in text) if len(text) > 0 else 0
 
@@ -196,15 +194,15 @@
         self._terminal_size: tuple[int, int] = System.terminal_size
 
         self._origin: tuple[int, int] = view
         self._current_output: list[str, ...] = None
 
     def _process_text_wrapper(self):
         self._text_wrapper = TextWrapper(
-            width=self._wrap_text_width,
+            width=self._shape[1],
             subsequent_indent=self._wrap_subsequent_indent,
             break_on_hyphens=self._wrap_text_break_on_hyphens,
             break_long_words=self._wrap_text_break_long_words,
         )
 
     def _init_arguments(
         self,
@@ -289,14 +287,15 @@
             # Reformat the contents of the TextBox due to a change in terminal dimensions.
             if self._terminal_size != (terminal_size := System.terminal_size):
                 self._terminal_size: tuple[int, int] = terminal_size
                 # Repeat the reset process three times in order to account for lag in the terminal as it is resized.
                 # Two iterations usually is enough, but three seems to always prevent issues.
                 for i in range(3):
                     time.sleep(0.01)
+                    self._process_text_wrapper()
                     self._set_shape()
                     self._set_view()
                     self._process_text()
 
             if self._view_changed:
                 self._view_changed: bool = False
                 self.write()
```

### Comparing `Termighty-3.0.4/source/termighty/widgets/text_editor.py` & `Termighty-3.0.5/source/termighty/widgets/text_editor.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,15 +176,15 @@
 
     def _process_text_wrapper(self):
         if not self._line_numbers or self._text is None:
             w = 0
         else:
             w = max(Config.line_numbers_width, int(np.log10(len(self._text))) + 2)
         self._text_wrapper = TextWrapper(
-            width=self._wrap_text_width - w,
+            width=self._shape[1] - w,
             expand_tabs=False,
             replace_whitespace=False,
             fix_sentence_endings=False,
             break_long_words=False,
             drop_whitespace=False,
             break_on_hyphens=False,
             subsequent_indent=self._wrap_subsequent_indent,
```

