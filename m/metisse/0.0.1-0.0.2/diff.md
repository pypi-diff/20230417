# Comparing `tmp/metisse-0.0.1.tar.gz` & `tmp/metisse-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metisse-0.0.1.tar", last modified: Sun Apr 16 10:27:48 2023, max compression
+gzip compressed data, was "dist\metisse-0.0.2.tar", last modified: Mon Apr 17 07:20:16 2023, max compression
```

## Comparing `metisse-0.0.1.tar` & `metisse-0.0.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 10:27:48.892690 metisse-0.0.1/
--rw-rw-rw-   0        0        0     9787 2023-04-14 10:23:54.000000 metisse-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      453 2023-04-16 10:27:48.892690 metisse-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2724 2023-04-16 10:24:33.000000 metisse-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-16 10:27:48.844626 metisse-0.0.1/metisse/
--rw-rw-rw-   0        0        0        0 2023-04-14 10:23:54.000000 metisse-0.0.1/metisse/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-16 10:27:48.862669 metisse-0.0.1/metisse/clients/
--rw-rw-rw-   0        0        0        0 2023-04-14 10:23:54.000000 metisse-0.0.1/metisse/clients/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-16 10:27:48.862669 metisse-0.0.1/metisse/clients/andriod/
--rw-rw-rw-   0        0        0       26 2023-04-14 10:23:54.000000 metisse-0.0.1/metisse/clients/andriod/__init__.py
--rw-rw-rw-   0        0        0     1331 2023-04-14 10:23:54.000000 metisse-0.0.1/metisse/clients/andriod/adb.py
--rw-rw-rw-   0        0        0      701 2023-04-14 10:23:54.000000 metisse-0.0.1/metisse/clients/client.py
-drwxrwxrwx   0        0        0        0 2023-04-16 10:27:48.862669 metisse-0.0.1/metisse/clients/ios/
--rw-rw-rw-   0        0        0       26 2023-04-14 10:23:54.000000 metisse-0.0.1/metisse/clients/ios/__init__.py
--rw-rw-rw-   0        0        0     1853 2023-04-14 10:23:54.000000 metisse-0.0.1/metisse/clients/ios/wda.py
-drwxrwxrwx   0        0        0        0 2023-04-16 10:27:48.876676 metisse-0.0.1/metisse/example/
--rw-rw-rw-   0        0        0        0 2023-04-14 10:23:54.000000 metisse-0.0.1/metisse/example/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-16 10:27:48.828981 metisse-0.0.1/metisse/example/example_data/
-drwxrwxrwx   0        0        0        0 2023-04-16 10:27:48.876676 metisse-0.0.1/metisse/example/example_data/icon/
--rw-rw-rw-   0        0        0    90781 2023-04-14 10:23:54.000000 metisse-0.0.1/metisse/example/example_data/icon/example_template_face.png
--rw-rw-rw-   0        0        0    55904 2023-04-14 10:23:54.000000 metisse-0.0.1/metisse/example/example_data/icon/example_template_hand.png
-drwxrwxrwx   0        0        0        0 2023-04-16 10:27:48.876676 metisse-0.0.1/metisse/example/example_data/temp_image/
--rw-rw-rw-   0        0        0  2503418 2023-04-14 10:23:54.000000 metisse-0.0.1/metisse/example/example_data/temp_image/tmp0.png
-drwxrwxrwx   0        0        0        0 2023-04-16 10:27:48.891184 metisse-0.0.1/metisse/example/example_data/ui/
--rw-rw-rw-   0        0        0      313 2023-04-14 10:23:54.000000 metisse-0.0.1/metisse/example/example_data/ui/gui_settings.py
--rw-rw-rw-   0        0        0    16964 2023-04-16 09:48:20.000000 metisse-0.0.1/metisse/example/example_data/ui/script_gui.py
--rw-rw-rw-   0        0        0     3934 2023-04-14 10:23:54.000000 metisse-0.0.1/metisse/example/example_data/ui/universal_script_gui_main.ui
--rw-rw-rw-   0        0        0     4195 2023-04-16 10:24:11.000000 metisse-0.0.1/metisse/example/example_data/ui/universal_script_gui_main_ui.py
--rw-rw-rw-   0        0        0     2287 2023-04-14 10:23:54.000000 metisse-0.0.1/metisse/example/example_data/ui/universal_script_gui_sub.ui
--rw-rw-rw-   0        0        0     3568 2023-04-14 10:23:54.000000 metisse-0.0.1/metisse/example/example_data/ui/universal_script_gui_sub2.ui
--rw-rw-rw-   0        0        0     3740 2023-04-16 10:24:11.000000 metisse-0.0.1/metisse/example/example_data/ui/universal_script_gui_sub2_ui.py
--rw-rw-rw-   0        0        0      685 2023-04-14 10:23:54.000000 metisse-0.0.1/metisse/example/example_data/ui/universal_script_gui_sub3.ui
--rw-rw-rw-   0        0        0     1020 2023-04-16 10:24:11.000000 metisse-0.0.1/metisse/example/example_data/ui/universal_script_gui_sub3_ui.py
--rw-rw-rw-   0        0        0     2326 2023-04-16 10:24:11.000000 metisse-0.0.1/metisse/example/example_data/ui/universal_script_gui_sub_ui.py
--rw-rw-rw-   0        0        0     7059 2023-04-16 10:24:33.000000 metisse-0.0.1/metisse/example/generate_example.py
--rw-rw-rw-   0        0        0    22330 2023-04-16 10:24:33.000000 metisse-0.0.1/metisse/metisse.py
--rw-rw-rw-   0        0        0     1843 2023-04-14 10:23:54.000000 metisse-0.0.1/metisse/params.py
--rw-rw-rw-   0        0        0      205 2023-04-14 10:23:54.000000 metisse-0.0.1/metisse/settings.py
--rw-rw-rw-   0        0        0     2047 2023-04-16 08:54:16.000000 metisse-0.0.1/metisse/template_metis.py
-drwxrwxrwx   0        0        0        0 2023-04-16 10:27:48.892690 metisse-0.0.1/metisse/utils/
--rw-rw-rw-   0        0        0        0 2023-04-14 10:23:54.000000 metisse-0.0.1/metisse/utils/__init__.py
--rw-rw-rw-   0        0        0     1539 2023-04-14 10:23:54.000000 metisse-0.0.1/metisse/utils/image_recognition.py
--rw-rw-rw-   0        0        0     2188 2023-04-14 10:23:54.000000 metisse-0.0.1/metisse/utils/metis_log.py
--rw-rw-rw-   0        0        0     6585 2023-04-14 10:23:54.000000 metisse-0.0.1/metisse/utils/metis_path.py
--rw-rw-rw-   0        0        0      774 2023-04-14 10:23:54.000000 metisse-0.0.1/metisse/utils/opencv_utils.py
--rw-rw-rw-   0        0        0     1051 2023-04-14 10:23:54.000000 metisse-0.0.1/metisse/utils/ui_client.py
-drwxrwxrwx   0        0        0        0 2023-04-16 10:27:48.862669 metisse-0.0.1/metisse.egg-info/
--rw-rw-rw-   0        0        0      453 2023-04-16 10:27:48.000000 metisse-0.0.1/metisse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1461 2023-04-16 10:27:48.000000 metisse-0.0.1/metisse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 10:27:48.000000 metisse-0.0.1/metisse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       99 2023-04-16 10:27:48.000000 metisse-0.0.1/metisse.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-16 10:27:48.000000 metisse-0.0.1/metisse.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 10:27:48.892690 metisse-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      840 2023-04-16 10:26:30.000000 metisse-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 07:20:16.093759 metisse-0.0.2/
+-rw-rw-rw-   0        0        0     9787 2023-04-17 02:58:36.000000 metisse-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      415 2023-04-17 07:20:16.093759 metisse-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2736 2023-04-17 07:17:50.000000 metisse-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 07:20:16.036594 metisse-0.0.2/metisse/
+-rw-rw-rw-   0        0        0        0 2023-04-17 02:58:36.000000 metisse-0.0.2/metisse/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 07:20:16.061530 metisse-0.0.2/metisse/clients/
+-rw-rw-rw-   0        0        0        0 2023-04-17 02:58:36.000000 metisse-0.0.2/metisse/clients/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 07:20:16.062527 metisse-0.0.2/metisse/clients/android/
+-rw-rw-rw-   0        0        0       26 2023-04-17 02:58:36.000000 metisse-0.0.2/metisse/clients/android/__init__.py
+-rw-rw-rw-   0        0        0     1331 2023-04-17 02:58:36.000000 metisse-0.0.2/metisse/clients/android/adb.py
+-rw-rw-rw-   0        0        0      701 2023-04-17 02:58:36.000000 metisse-0.0.2/metisse/clients/client.py
+drwxrwxrwx   0        0        0        0 2023-04-17 07:20:16.064522 metisse-0.0.2/metisse/clients/ios/
+-rw-rw-rw-   0        0        0       26 2023-04-17 02:58:36.000000 metisse-0.0.2/metisse/clients/ios/__init__.py
+-rw-rw-rw-   0        0        0     1853 2023-04-17 02:58:36.000000 metisse-0.0.2/metisse/clients/ios/wda.py
+drwxrwxrwx   0        0        0        0 2023-04-17 07:20:16.066516 metisse-0.0.2/metisse/example/
+-rw-rw-rw-   0        0        0        0 2023-04-17 02:58:36.000000 metisse-0.0.2/metisse/example/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 07:20:16.028829 metisse-0.0.2/metisse/example/example_data/
+drwxrwxrwx   0        0        0        0 2023-04-17 07:20:16.068511 metisse-0.0.2/metisse/example/example_data/icon/
+-rw-rw-rw-   0        0        0    90781 2023-04-17 02:58:36.000000 metisse-0.0.2/metisse/example/example_data/icon/example_template_face.png
+-rw-rw-rw-   0        0        0    55904 2023-04-17 02:58:36.000000 metisse-0.0.2/metisse/example/example_data/icon/example_template_hand.png
+drwxrwxrwx   0        0        0        0 2023-04-17 07:20:16.069508 metisse-0.0.2/metisse/example/example_data/temp_image/
+-rw-rw-rw-   0        0        0  2503418 2023-04-17 02:58:36.000000 metisse-0.0.2/metisse/example/example_data/temp_image/tmp0.png
+drwxrwxrwx   0        0        0        0 2023-04-17 07:20:16.084783 metisse-0.0.2/metisse/example/example_data/ui/
+-rw-rw-rw-   0        0        0      313 2023-04-17 02:58:36.000000 metisse-0.0.2/metisse/example/example_data/ui/gui_settings.py
+-rw-rw-rw-   0        0        0    16964 2023-04-17 02:58:36.000000 metisse-0.0.2/metisse/example/example_data/ui/script_gui.py
+-rw-rw-rw-   0        0        0     3934 2023-04-17 02:58:36.000000 metisse-0.0.2/metisse/example/example_data/ui/universal_script_gui_main.ui
+-rw-rw-rw-   0        0        0     4195 2023-04-17 02:59:18.000000 metisse-0.0.2/metisse/example/example_data/ui/universal_script_gui_main_ui.py
+-rw-rw-rw-   0        0        0     2287 2023-04-17 02:58:36.000000 metisse-0.0.2/metisse/example/example_data/ui/universal_script_gui_sub.ui
+-rw-rw-rw-   0        0        0     3568 2023-04-17 02:58:36.000000 metisse-0.0.2/metisse/example/example_data/ui/universal_script_gui_sub2.ui
+-rw-rw-rw-   0        0        0     3740 2023-04-17 02:59:18.000000 metisse-0.0.2/metisse/example/example_data/ui/universal_script_gui_sub2_ui.py
+-rw-rw-rw-   0        0        0      685 2023-04-17 02:58:36.000000 metisse-0.0.2/metisse/example/example_data/ui/universal_script_gui_sub3.ui
+-rw-rw-rw-   0        0        0     1020 2023-04-17 02:59:18.000000 metisse-0.0.2/metisse/example/example_data/ui/universal_script_gui_sub3_ui.py
+-rw-rw-rw-   0        0        0     2326 2023-04-17 02:59:18.000000 metisse-0.0.2/metisse/example/example_data/ui/universal_script_gui_sub_ui.py
+-rw-rw-rw-   0        0        0     7059 2023-04-17 02:58:36.000000 metisse-0.0.2/metisse/example/generate_example.py
+-rw-rw-rw-   0        0        0    22344 2023-04-17 02:58:36.000000 metisse-0.0.2/metisse/metisse.py
+-rw-rw-rw-   0        0        0     1843 2023-04-17 02:58:36.000000 metisse-0.0.2/metisse/params.py
+-rw-rw-rw-   0        0        0      205 2023-04-17 02:58:36.000000 metisse-0.0.2/metisse/settings.py
+-rw-rw-rw-   0        0        0     2047 2023-04-17 02:58:36.000000 metisse-0.0.2/metisse/template_metis.py
+drwxrwxrwx   0        0        0        0 2023-04-17 07:20:16.092761 metisse-0.0.2/metisse/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-17 02:58:36.000000 metisse-0.0.2/metisse/utils/__init__.py
+-rw-rw-rw-   0        0        0     1539 2023-04-17 02:58:36.000000 metisse-0.0.2/metisse/utils/image_recognition.py
+-rw-rw-rw-   0        0        0     2190 2023-04-17 02:58:36.000000 metisse-0.0.2/metisse/utils/metisse_log.py
+-rw-rw-rw-   0        0        0     6585 2023-04-17 02:58:36.000000 metisse-0.0.2/metisse/utils/metisse_path.py
+-rw-rw-rw-   0        0        0      774 2023-04-17 02:58:36.000000 metisse-0.0.2/metisse/utils/opencv_utils.py
+-rw-rw-rw-   0        0        0     1051 2023-04-17 02:58:36.000000 metisse-0.0.2/metisse/utils/ui_client.py
+drwxrwxrwx   0        0        0        0 2023-04-17 07:20:16.059571 metisse-0.0.2/metisse.egg-info/
+-rw-rw-rw-   0        0        0      415 2023-04-17 07:20:15.000000 metisse-0.0.2/metisse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1465 2023-04-17 07:20:15.000000 metisse-0.0.2/metisse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 07:20:15.000000 metisse-0.0.2/metisse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       99 2023-04-17 07:20:15.000000 metisse-0.0.2/metisse.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-17 07:20:15.000000 metisse-0.0.2/metisse.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 07:20:16.093759 metisse-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      840 2023-04-17 02:58:36.000000 metisse-0.0.2/setup.py
```

### Comparing `metisse-0.0.1/LICENSE` & `metisse-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `metisse-0.0.1/README.md` & `metisse-0.0.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-# Metis
+# Metisse
 
-Metis is a powerful image recognition and automation package designed to facilitate the development of scripts for mobile devices. It provides an extensive set of tools for image recognition, screenshot manipulation, and user interaction, such as tapping, swiping, and pressing.
+Metisse is a powerful image recognition and automation package designed to facilitate the development of scripts for mobile devices. It provides an extensive set of tools for image recognition, screenshot manipulation, and user interaction, such as tapping, swiping, and pressing.
 
 ## Features
 
 - Image recognition using template matching
 - Screenshot manipulation, including cropping and saving
 - Automation of user interactions, such as tapping, swiping, and pressing
 - Customizable parameters for image recognition and automation tasks
 - Easy integration with existing automation frameworks
 
 ## Installation
 
-To install Metis, run the following command in your terminal:
+To install Metisse, run the following command in your terminal:
 
 ```bash
 pip install metisse
 ```
 Usage
-Here's a simple example demonstrating how to use Metis for image recognition and user interaction:
+Here's a simple example demonstrating how to use Metisse for image recognition and user interaction:
 
 python
 Copy code
 ```bash
 from metisse.metisse import MetisseClass
 from metisse.params import ImageRecognitionParams, SaveParams
 
@@ -53,17 +53,17 @@
     ex.create_example_py_file()
 ```
 
 
 For more detailed information about the available methods and their usage, please refer to the MetisseClass Methods documentation.
 
 ## Contributing
-We welcome contributions to Metis! If you'd like to contribute, please follow these steps:
+We welcome contributions to Metisse! If you'd like to contribute, please follow these steps:
 - Fork the repository
 - Create a new branch for your changes
 - Make your changes and test them thoroughly
 - Commit your changes and push them to your forked repository
 - Create a pull request with a detailed description of your changes
 - Please make sure to follow the code style and conventions used in the project.
 
 ## License
-Metis is licensed under the Apache License 2.0.
+Metisse is licensed under the Apache License 2.0.
```

### Comparing `metisse-0.0.1/metisse/clients/andriod/adb.py` & `metisse-0.0.2/metisse/clients/android/adb.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.1/metisse/clients/client.py` & `metisse-0.0.2/metisse/clients/client.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.1/metisse/clients/ios/wda.py` & `metisse-0.0.2/metisse/clients/ios/wda.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.1/metisse/example/example_data/icon/example_template_face.png` & `metisse-0.0.2/metisse/example/example_data/icon/example_template_face.png`

 * *Files identical despite different names*

### Comparing `metisse-0.0.1/metisse/example/example_data/icon/example_template_hand.png` & `metisse-0.0.2/metisse/example/example_data/icon/example_template_hand.png`

 * *Files identical despite different names*

### Comparing `metisse-0.0.1/metisse/example/example_data/temp_image/tmp0.png` & `metisse-0.0.2/metisse/example/example_data/temp_image/tmp0.png`

 * *Files identical despite different names*

### Comparing `metisse-0.0.1/metisse/example/example_data/ui/script_gui.py` & `metisse-0.0.2/metisse/example/example_data/ui/script_gui.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.1/metisse/example/example_data/ui/universal_script_gui_main.ui` & `metisse-0.0.2/metisse/example/example_data/ui/universal_script_gui_main.ui`

 * *Files identical despite different names*

### Comparing `metisse-0.0.1/metisse/example/example_data/ui/universal_script_gui_main_ui.py` & `metisse-0.0.2/metisse/example/example_data/ui/universal_script_gui_main_ui.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.1/metisse/example/example_data/ui/universal_script_gui_sub.ui` & `metisse-0.0.2/metisse/example/example_data/ui/universal_script_gui_sub.ui`

 * *Files identical despite different names*

### Comparing `metisse-0.0.1/metisse/example/example_data/ui/universal_script_gui_sub2.ui` & `metisse-0.0.2/metisse/example/example_data/ui/universal_script_gui_sub2.ui`

 * *Files identical despite different names*

### Comparing `metisse-0.0.1/metisse/example/example_data/ui/universal_script_gui_sub2_ui.py` & `metisse-0.0.2/metisse/example/example_data/ui/universal_script_gui_sub2_ui.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.1/metisse/example/example_data/ui/universal_script_gui_sub3.ui` & `metisse-0.0.2/metisse/example/example_data/ui/universal_script_gui_sub3.ui`

 * *Files identical despite different names*

### Comparing `metisse-0.0.1/metisse/example/example_data/ui/universal_script_gui_sub3_ui.py` & `metisse-0.0.2/metisse/example/example_data/ui/universal_script_gui_sub3_ui.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.1/metisse/example/example_data/ui/universal_script_gui_sub_ui.py` & `metisse-0.0.2/metisse/example/example_data/ui/universal_script_gui_sub_ui.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.1/metisse/example/generate_example.py` & `metisse-0.0.2/metisse/example/generate_example.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.1/metisse/metisse.py` & `metisse-0.0.2/metisse/metisse.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 from typing import Tuple
 # pylint: disable=no-member
 from PIL import Image
 import inspect
 from .params import ImageRecognitionParams, SaveParams, DeviceParams, UiClientParams, ImageRecognitionResult
 from .template_metis import TemplateMetisClass
 from .clients.ios.wda import WdaClient
-from .clients.andriod.adb import AdbClient
-from .utils.metis_path import DevPath
+from .clients.android.adb import AdbClient
+from .utils.metisse_path import DevPath
 from .utils.opencv_utils import Opencv_utils
 from .utils.ui_client import UiClient
-from .utils.metis_log import MetisLogger
+from .utils.metisse_log import MetisseLogger
 from .utils import image_recognition
 from .settings import Settings as ST
 
 
 class MetisseClass(TemplateMetisClass):
 
     def __init__(self, device_id: str, relatively_path: str, pyqt6_ui_label: UiClientParams, os_environment: str = 'android'):
@@ -39,18 +39,18 @@
             self._relatively_path = relatively_path
 
         super(TemplateMetisClass, self).__init__()
 
         self._device_id = device_id
         self._dev_path = DevPath(self._relatively_path)
         self._script_path = self._dev_path.create_extended_script_path(self._device_id)
-        self._logger = MetisLogger("MetisClass_logger",
-                                   log_level=logging.DEBUG,
-                                   log_file=os.path.join(self._script_path.device_id_path, "log",
-                                                         self.get_time() + self._device_id + ".log"))
+        self._logger = MetisseLogger("MetisClass_logger",
+                                     log_level=logging.DEBUG,
+                                     log_file=os.path.join(self._script_path.device_id_path, "log",
+                                                           self.get_time() + self._device_id + ".log"))
         assert os_environment in ST.OS_ENVIRONMENT
         self._os_environment = os_environment  # android , ios
         self.ios_device_scale = 2  # init var
 
         if self._os_environment == 'ios':
             self._client = WdaClient(DeviceParams(device_id, os_environment))
         elif self._os_environment == 'android':
```

### Comparing `metisse-0.0.1/metisse/params.py` & `metisse-0.0.2/metisse/params.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.1/metisse/template_metis.py` & `metisse-0.0.2/metisse/template_metis.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.1/metisse/utils/image_recognition.py` & `metisse-0.0.2/metisse/utils/image_recognition.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.1/metisse/utils/metis_log.py` & `metisse-0.0.2/metisse/utils/metisse_log.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 import os
 
 
-class MetisLogger(logging.Logger):
+class MetisseLogger(logging.Logger):
 
     def __init__(self, logger_name, log_level=logging.INFO, log_file=None):
         self.logger = logging.getLogger(logger_name)
         self.logger.setLevel(log_level)
 
         formatter = logging.Formatter(
             "%(asctime)s - %(name)s - %(levelname)s - %(message)s",
```

### Comparing `metisse-0.0.1/metisse/utils/metis_path.py` & `metisse-0.0.2/metisse/utils/metisse_path.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.1/metisse/utils/opencv_utils.py` & `metisse-0.0.2/metisse/utils/opencv_utils.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.1/metisse/utils/ui_client.py` & `metisse-0.0.2/metisse/utils/ui_client.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.1/metisse.egg-info/SOURCES.txt` & `metisse-0.0.2/metisse.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 metisse.egg-info/PKG-INFO
 metisse.egg-info/SOURCES.txt
 metisse.egg-info/dependency_links.txt
 metisse.egg-info/requires.txt
 metisse.egg-info/top_level.txt
 metisse/clients/__init__.py
 metisse/clients/client.py
-metisse/clients/andriod/__init__.py
-metisse/clients/andriod/adb.py
+metisse/clients/android/__init__.py
+metisse/clients/android/adb.py
 metisse/clients/ios/__init__.py
 metisse/clients/ios/wda.py
 metisse/example/__init__.py
 metisse/example/generate_example.py
 metisse/example/example_data/icon/example_template_face.png
 metisse/example/example_data/icon/example_template_hand.png
 metisse/example/example_data/temp_image/tmp0.png
@@ -30,11 +30,11 @@
 metisse/example/example_data/ui/universal_script_gui_sub2.ui
 metisse/example/example_data/ui/universal_script_gui_sub2_ui.py
 metisse/example/example_data/ui/universal_script_gui_sub3.ui
 metisse/example/example_data/ui/universal_script_gui_sub3_ui.py
 metisse/example/example_data/ui/universal_script_gui_sub_ui.py
 metisse/utils/__init__.py
 metisse/utils/image_recognition.py
-metisse/utils/metis_log.py
-metisse/utils/metis_path.py
+metisse/utils/metisse_log.py
+metisse/utils/metisse_path.py
 metisse/utils/opencv_utils.py
 metisse/utils/ui_client.py
```

### Comparing `metisse-0.0.1/setup.py` & `metisse-0.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='metisse',
-    version="0.0.1",
+    version="0.0.2",
     description="A versatile and automated testing framework for games and apps on Android and iOS platforms",
     author='Henry Chen',
     author_email='weekand7@gmail.com',
     license='Apache License 2.0',
     packages=find_packages(exclude=['unit_tests', 'unit_tests.*']),
     package_data={
         'metisse': ['example/example_data/**/*'],
```

