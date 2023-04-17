# Comparing `tmp/metisse-0.0.3.tar.gz` & `tmp/metisse-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\metisse-0.0.3.tar", last modified: Mon Apr 17 09:59:34 2023, max compression
+gzip compressed data, was "dist\metisse-0.0.4.tar", last modified: Mon Apr 17 10:06:49 2023, max compression
```

## Comparing `metisse-0.0.3.tar` & `metisse-0.0.4.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 09:59:34.509864 metisse-0.0.3/
--rw-rw-rw-   0        0        0     9787 2023-04-17 02:58:36.000000 metisse-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     3196 2023-04-17 09:59:34.508834 metisse-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2736 2023-04-17 07:32:05.000000 metisse-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 09:59:34.446863 metisse-0.0.3/metisse/
--rw-rw-rw-   0        0        0        0 2023-04-17 02:58:36.000000 metisse-0.0.3/metisse/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 09:59:34.473846 metisse-0.0.3/metisse/clients/
--rw-rw-rw-   0        0        0        0 2023-04-17 02:58:36.000000 metisse-0.0.3/metisse/clients/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 09:59:34.476838 metisse-0.0.3/metisse/clients/android/
--rw-rw-rw-   0        0        0       26 2023-04-17 07:32:05.000000 metisse-0.0.3/metisse/clients/android/__init__.py
--rw-rw-rw-   0        0        0     1331 2023-04-17 07:32:05.000000 metisse-0.0.3/metisse/clients/android/adb.py
--rw-rw-rw-   0        0        0      701 2023-04-17 02:58:36.000000 metisse-0.0.3/metisse/clients/client.py
-drwxrwxrwx   0        0        0        0 2023-04-17 09:59:34.478832 metisse-0.0.3/metisse/clients/ios/
--rw-rw-rw-   0        0        0       26 2023-04-17 02:58:36.000000 metisse-0.0.3/metisse/clients/ios/__init__.py
--rw-rw-rw-   0        0        0     1853 2023-04-17 02:58:36.000000 metisse-0.0.3/metisse/clients/ios/wda.py
-drwxrwxrwx   0        0        0        0 2023-04-17 09:59:34.480906 metisse-0.0.3/metisse/example/
--rw-rw-rw-   0        0        0        0 2023-04-17 02:58:36.000000 metisse-0.0.3/metisse/example/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 09:59:34.430906 metisse-0.0.3/metisse/example/example_data/
-drwxrwxrwx   0        0        0        0 2023-04-17 09:59:34.483899 metisse-0.0.3/metisse/example/example_data/icon/
--rw-rw-rw-   0        0        0    90781 2023-04-17 02:58:36.000000 metisse-0.0.3/metisse/example/example_data/icon/example_template_face.png
--rw-rw-rw-   0        0        0    55904 2023-04-17 02:58:36.000000 metisse-0.0.3/metisse/example/example_data/icon/example_template_hand.png
-drwxrwxrwx   0        0        0        0 2023-04-17 09:59:34.484898 metisse-0.0.3/metisse/example/example_data/temp_image/
--rw-rw-rw-   0        0        0  2503418 2023-04-17 02:58:36.000000 metisse-0.0.3/metisse/example/example_data/temp_image/tmp0.png
-drwxrwxrwx   0        0        0        0 2023-04-17 09:59:34.500854 metisse-0.0.3/metisse/example/example_data/ui/
--rw-rw-rw-   0        0        0      313 2023-04-17 02:58:36.000000 metisse-0.0.3/metisse/example/example_data/ui/gui_settings.py
--rw-rw-rw-   0        0        0    16964 2023-04-17 02:58:36.000000 metisse-0.0.3/metisse/example/example_data/ui/script_gui.py
--rw-rw-rw-   0        0        0     3934 2023-04-17 02:58:36.000000 metisse-0.0.3/metisse/example/example_data/ui/universal_script_gui_main.ui
--rw-rw-rw-   0        0        0     4195 2023-04-17 02:59:18.000000 metisse-0.0.3/metisse/example/example_data/ui/universal_script_gui_main_ui.py
--rw-rw-rw-   0        0        0     2287 2023-04-17 02:58:36.000000 metisse-0.0.3/metisse/example/example_data/ui/universal_script_gui_sub.ui
--rw-rw-rw-   0        0        0     3568 2023-04-17 02:58:36.000000 metisse-0.0.3/metisse/example/example_data/ui/universal_script_gui_sub2.ui
--rw-rw-rw-   0        0        0     3740 2023-04-17 02:59:18.000000 metisse-0.0.3/metisse/example/example_data/ui/universal_script_gui_sub2_ui.py
--rw-rw-rw-   0        0        0      685 2023-04-17 02:58:36.000000 metisse-0.0.3/metisse/example/example_data/ui/universal_script_gui_sub3.ui
--rw-rw-rw-   0        0        0     1020 2023-04-17 02:59:18.000000 metisse-0.0.3/metisse/example/example_data/ui/universal_script_gui_sub3_ui.py
--rw-rw-rw-   0        0        0     2326 2023-04-17 02:59:18.000000 metisse-0.0.3/metisse/example/example_data/ui/universal_script_gui_sub_ui.py
--rw-rw-rw-   0        0        0     7076 2023-04-17 09:46:50.000000 metisse-0.0.3/metisse/example/generate_example.py
--rw-rw-rw-   0        0        0    22531 2023-04-17 09:49:38.000000 metisse-0.0.3/metisse/metisse.py
--rw-rw-rw-   0        0        0     1843 2023-04-17 02:58:36.000000 metisse-0.0.3/metisse/params.py
--rw-rw-rw-   0        0        0      205 2023-04-17 02:58:36.000000 metisse-0.0.3/metisse/settings.py
--rw-rw-rw-   0        0        0     2047 2023-04-17 02:58:36.000000 metisse-0.0.3/metisse/template_metis.py
-drwxrwxrwx   0        0        0        0 2023-04-17 09:59:34.507866 metisse-0.0.3/metisse/utils/
--rw-rw-rw-   0        0        0        0 2023-04-17 02:58:36.000000 metisse-0.0.3/metisse/utils/__init__.py
--rw-rw-rw-   0        0        0     1539 2023-04-17 02:58:36.000000 metisse-0.0.3/metisse/utils/image_recognition.py
--rw-rw-rw-   0        0        0     2190 2023-04-17 07:32:05.000000 metisse-0.0.3/metisse/utils/metisse_log.py
--rw-rw-rw-   0        0        0     6585 2023-04-17 09:13:34.000000 metisse-0.0.3/metisse/utils/metisse_path.py
--rw-rw-rw-   0        0        0      774 2023-04-17 02:58:36.000000 metisse-0.0.3/metisse/utils/opencv_utils.py
--rw-rw-rw-   0        0        0     1051 2023-04-17 02:58:36.000000 metisse-0.0.3/metisse/utils/ui_client.py
-drwxrwxrwx   0        0        0        0 2023-04-17 09:59:34.471880 metisse-0.0.3/metisse.egg-info/
--rw-rw-rw-   0        0        0     3196 2023-04-17 09:59:34.000000 metisse-0.0.3/metisse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1465 2023-04-17 09:59:34.000000 metisse-0.0.3/metisse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 09:59:34.000000 metisse-0.0.3/metisse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       99 2023-04-17 09:59:34.000000 metisse-0.0.3/metisse.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-17 09:59:34.000000 metisse-0.0.3/metisse.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 09:59:34.509864 metisse-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1018 2023-04-17 09:50:52.000000 metisse-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 10:06:49.637830 metisse-0.0.4/
+-rw-rw-rw-   0        0        0     9787 2023-04-17 02:58:36.000000 metisse-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     3196 2023-04-17 10:06:49.636833 metisse-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2736 2023-04-17 07:32:05.000000 metisse-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 10:06:49.583973 metisse-0.0.4/metisse/
+-rw-rw-rw-   0        0        0        0 2023-04-17 02:58:36.000000 metisse-0.0.4/metisse/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 10:06:49.600928 metisse-0.0.4/metisse/clients/
+-rw-rw-rw-   0        0        0        0 2023-04-17 02:58:36.000000 metisse-0.0.4/metisse/clients/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 10:06:49.602924 metisse-0.0.4/metisse/clients/android/
+-rw-rw-rw-   0        0        0       26 2023-04-17 07:32:05.000000 metisse-0.0.4/metisse/clients/android/__init__.py
+-rw-rw-rw-   0        0        0     1331 2023-04-17 07:32:05.000000 metisse-0.0.4/metisse/clients/android/adb.py
+-rw-rw-rw-   0        0        0      701 2023-04-17 02:58:36.000000 metisse-0.0.4/metisse/clients/client.py
+drwxrwxrwx   0        0        0        0 2023-04-17 10:06:49.604918 metisse-0.0.4/metisse/clients/ios/
+-rw-rw-rw-   0        0        0       26 2023-04-17 02:58:36.000000 metisse-0.0.4/metisse/clients/ios/__init__.py
+-rw-rw-rw-   0        0        0     1853 2023-04-17 02:58:36.000000 metisse-0.0.4/metisse/clients/ios/wda.py
+drwxrwxrwx   0        0        0        0 2023-04-17 10:06:49.606912 metisse-0.0.4/metisse/example/
+-rw-rw-rw-   0        0        0        0 2023-04-17 02:58:36.000000 metisse-0.0.4/metisse/example/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 10:06:49.564349 metisse-0.0.4/metisse/example/example_data/
+drwxrwxrwx   0        0        0        0 2023-04-17 10:06:49.610902 metisse-0.0.4/metisse/example/example_data/icon/
+-rw-rw-rw-   0        0        0    90781 2023-04-17 02:58:36.000000 metisse-0.0.4/metisse/example/example_data/icon/example_template_face.png
+-rw-rw-rw-   0        0        0    55904 2023-04-17 02:58:36.000000 metisse-0.0.4/metisse/example/example_data/icon/example_template_hand.png
+drwxrwxrwx   0        0        0        0 2023-04-17 10:06:49.611899 metisse-0.0.4/metisse/example/example_data/temp_image/
+-rw-rw-rw-   0        0        0  2503418 2023-04-17 02:58:36.000000 metisse-0.0.4/metisse/example/example_data/temp_image/tmp0.png
+drwxrwxrwx   0        0        0        0 2023-04-17 10:06:49.628855 metisse-0.0.4/metisse/example/example_data/ui/
+-rw-rw-rw-   0        0        0      313 2023-04-17 02:58:36.000000 metisse-0.0.4/metisse/example/example_data/ui/gui_settings.py
+-rw-rw-rw-   0        0        0    16964 2023-04-17 02:58:36.000000 metisse-0.0.4/metisse/example/example_data/ui/script_gui.py
+-rw-rw-rw-   0        0        0     3934 2023-04-17 02:58:36.000000 metisse-0.0.4/metisse/example/example_data/ui/universal_script_gui_main.ui
+-rw-rw-rw-   0        0        0     4195 2023-04-17 02:59:18.000000 metisse-0.0.4/metisse/example/example_data/ui/universal_script_gui_main_ui.py
+-rw-rw-rw-   0        0        0     2287 2023-04-17 02:58:36.000000 metisse-0.0.4/metisse/example/example_data/ui/universal_script_gui_sub.ui
+-rw-rw-rw-   0        0        0     3568 2023-04-17 02:58:36.000000 metisse-0.0.4/metisse/example/example_data/ui/universal_script_gui_sub2.ui
+-rw-rw-rw-   0        0        0     3740 2023-04-17 02:59:18.000000 metisse-0.0.4/metisse/example/example_data/ui/universal_script_gui_sub2_ui.py
+-rw-rw-rw-   0        0        0      685 2023-04-17 02:58:36.000000 metisse-0.0.4/metisse/example/example_data/ui/universal_script_gui_sub3.ui
+-rw-rw-rw-   0        0        0     1020 2023-04-17 02:59:18.000000 metisse-0.0.4/metisse/example/example_data/ui/universal_script_gui_sub3_ui.py
+-rw-rw-rw-   0        0        0     2326 2023-04-17 02:59:18.000000 metisse-0.0.4/metisse/example/example_data/ui/universal_script_gui_sub_ui.py
+-rw-rw-rw-   0        0        0     7076 2023-04-17 10:04:33.000000 metisse-0.0.4/metisse/example/generate_example.py
+-rw-rw-rw-   0        0        0    22532 2023-04-17 10:04:58.000000 metisse-0.0.4/metisse/metisse.py
+-rw-rw-rw-   0        0        0     1843 2023-04-17 02:58:36.000000 metisse-0.0.4/metisse/params.py
+-rw-rw-rw-   0        0        0      205 2023-04-17 02:58:36.000000 metisse-0.0.4/metisse/settings.py
+-rw-rw-rw-   0        0        0     2047 2023-04-17 02:58:36.000000 metisse-0.0.4/metisse/template_metis.py
+drwxrwxrwx   0        0        0        0 2023-04-17 10:06:49.635836 metisse-0.0.4/metisse/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-17 02:58:36.000000 metisse-0.0.4/metisse/utils/__init__.py
+-rw-rw-rw-   0        0        0     1539 2023-04-17 02:58:36.000000 metisse-0.0.4/metisse/utils/image_recognition.py
+-rw-rw-rw-   0        0        0     2190 2023-04-17 07:32:05.000000 metisse-0.0.4/metisse/utils/metisse_log.py
+-rw-rw-rw-   0        0        0     6585 2023-04-17 09:13:34.000000 metisse-0.0.4/metisse/utils/metisse_path.py
+-rw-rw-rw-   0        0        0      774 2023-04-17 02:58:36.000000 metisse-0.0.4/metisse/utils/opencv_utils.py
+-rw-rw-rw-   0        0        0     1051 2023-04-17 02:58:36.000000 metisse-0.0.4/metisse/utils/ui_client.py
+drwxrwxrwx   0        0        0        0 2023-04-17 10:06:49.598934 metisse-0.0.4/metisse.egg-info/
+-rw-rw-rw-   0        0        0     3196 2023-04-17 10:06:49.000000 metisse-0.0.4/metisse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1465 2023-04-17 10:06:49.000000 metisse-0.0.4/metisse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 10:06:49.000000 metisse-0.0.4/metisse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       99 2023-04-17 10:06:49.000000 metisse-0.0.4/metisse.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-17 10:06:49.000000 metisse-0.0.4/metisse.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 10:06:49.637830 metisse-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1018 2023-04-17 10:05:37.000000 metisse-0.0.4/setup.py
```

### Comparing `metisse-0.0.3/LICENSE` & `metisse-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `metisse-0.0.3/PKG-INFO` & `metisse-0.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metisse
-Version: 0.0.3
+Version: 0.0.4
 Summary: A versatile and automated testing framework for games and apps on Android and iOS platforms
 Author: Henry Chen
 Author-email: weekand7@gmail.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `metisse-0.0.3/README.md` & `metisse-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `metisse-0.0.3/metisse/clients/android/adb.py` & `metisse-0.0.4/metisse/clients/android/adb.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.3/metisse/clients/client.py` & `metisse-0.0.4/metisse/clients/client.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.3/metisse/clients/ios/wda.py` & `metisse-0.0.4/metisse/clients/ios/wda.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.3/metisse/example/example_data/icon/example_template_face.png` & `metisse-0.0.4/metisse/example/example_data/icon/example_template_face.png`

 * *Files identical despite different names*

### Comparing `metisse-0.0.3/metisse/example/example_data/icon/example_template_hand.png` & `metisse-0.0.4/metisse/example/example_data/icon/example_template_hand.png`

 * *Files identical despite different names*

### Comparing `metisse-0.0.3/metisse/example/example_data/temp_image/tmp0.png` & `metisse-0.0.4/metisse/example/example_data/temp_image/tmp0.png`

 * *Files identical despite different names*

### Comparing `metisse-0.0.3/metisse/example/example_data/ui/script_gui.py` & `metisse-0.0.4/metisse/example/example_data/ui/script_gui.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.3/metisse/example/example_data/ui/universal_script_gui_main.ui` & `metisse-0.0.4/metisse/example/example_data/ui/universal_script_gui_main.ui`

 * *Files identical despite different names*

### Comparing `metisse-0.0.3/metisse/example/example_data/ui/universal_script_gui_main_ui.py` & `metisse-0.0.4/metisse/example/example_data/ui/universal_script_gui_main_ui.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.3/metisse/example/example_data/ui/universal_script_gui_sub.ui` & `metisse-0.0.4/metisse/example/example_data/ui/universal_script_gui_sub.ui`

 * *Files identical despite different names*

### Comparing `metisse-0.0.3/metisse/example/example_data/ui/universal_script_gui_sub2.ui` & `metisse-0.0.4/metisse/example/example_data/ui/universal_script_gui_sub2.ui`

 * *Files identical despite different names*

### Comparing `metisse-0.0.3/metisse/example/example_data/ui/universal_script_gui_sub2_ui.py` & `metisse-0.0.4/metisse/example/example_data/ui/universal_script_gui_sub2_ui.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.3/metisse/example/example_data/ui/universal_script_gui_sub3.ui` & `metisse-0.0.4/metisse/example/example_data/ui/universal_script_gui_sub3.ui`

 * *Files identical despite different names*

### Comparing `metisse-0.0.3/metisse/example/example_data/ui/universal_script_gui_sub3_ui.py` & `metisse-0.0.4/metisse/example/example_data/ui/universal_script_gui_sub3_ui.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.3/metisse/example/example_data/ui/universal_script_gui_sub_ui.py` & `metisse-0.0.4/metisse/example/example_data/ui/universal_script_gui_sub_ui.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.3/metisse/example/generate_example.py` & `metisse-0.0.4/metisse/example/generate_example.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.3/metisse/metisse.py` & `metisse-0.0.4/metisse/metisse.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,15 +181,15 @@
                                                                           params.accuracy_val)
 
                 self._logger.info("image_recognition method : template_name=%s  prob=%.4f accuracy_val=%.4f %s",
                                   params.template_image_name, self._img_recog_result.recognition_threshold, params.accuracy_val,
                                   self._img_recog_result.is_recognized)
                 self._ui_client.send_image_path_to_ui(_image_path=_template_image_path)
                 self._ui_client.send_log_to_ui(
-                    "image_recognition method : \n template_name={params.template_image_name}  \n prob={self._img_recog_result.recognition_threshold:.4f} \n accuracy_val={params.accuracy_val:.4f} \n {self._img_recog_result.is_recognized}"
+                    f"image_recognition method : \n template_name={params.template_image_name}  \n prob={self._img_recog_result.recognition_threshold:.4f} \n accuracy_val={params.accuracy_val:.4f} \n {self._img_recog_result.is_recognized}"
                 )
                 if self._img_recog_result.is_recognized:
                     if self.is_backup and params.is_backup:
                         self.save_screenshot_compression(save_params)
                     return True
             return False
```

### Comparing `metisse-0.0.3/metisse/params.py` & `metisse-0.0.4/metisse/params.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.3/metisse/template_metis.py` & `metisse-0.0.4/metisse/template_metis.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.3/metisse/utils/image_recognition.py` & `metisse-0.0.4/metisse/utils/image_recognition.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.3/metisse/utils/metisse_log.py` & `metisse-0.0.4/metisse/utils/metisse_log.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.3/metisse/utils/metisse_path.py` & `metisse-0.0.4/metisse/utils/metisse_path.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.3/metisse/utils/opencv_utils.py` & `metisse-0.0.4/metisse/utils/opencv_utils.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.3/metisse/utils/ui_client.py` & `metisse-0.0.4/metisse/utils/ui_client.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.3/metisse.egg-info/PKG-INFO` & `metisse-0.0.4/metisse.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metisse
-Version: 0.0.3
+Version: 0.0.4
 Summary: A versatile and automated testing framework for games and apps on Android and iOS platforms
 Author: Henry Chen
 Author-email: weekand7@gmail.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `metisse-0.0.3/metisse.egg-info/SOURCES.txt` & `metisse-0.0.4/metisse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metisse-0.0.3/setup.py` & `metisse-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setup(
     name='metisse',
-    version="0.0.3",
+    version="0.0.4",
     description="A versatile and automated testing framework for games and apps on Android and iOS platforms",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Henry Chen',
     author_email='weekand7@gmail.com',
     license='Apache License 2.0',
     packages=find_packages(exclude=['unit_tests', 'unit_tests.*']),
```

