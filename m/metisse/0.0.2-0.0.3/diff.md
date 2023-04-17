# Comparing `tmp/metisse-0.0.2.tar.gz` & `tmp/metisse-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\metisse-0.0.2.tar", last modified: Mon Apr 17 07:20:16 2023, max compression
+gzip compressed data, was "dist\metisse-0.0.3.tar", last modified: Mon Apr 17 09:59:34 2023, max compression
```

## Comparing `metisse-0.0.2.tar` & `metisse-0.0.3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 07:20:16.093759 metisse-0.0.2/
--rw-rw-rw-   0        0        0     9787 2023-04-17 02:58:36.000000 metisse-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      415 2023-04-17 07:20:16.093759 metisse-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2736 2023-04-17 07:17:50.000000 metisse-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 07:20:16.036594 metisse-0.0.2/metisse/
--rw-rw-rw-   0        0        0        0 2023-04-17 02:58:36.000000 metisse-0.0.2/metisse/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 07:20:16.061530 metisse-0.0.2/metisse/clients/
--rw-rw-rw-   0        0        0        0 2023-04-17 02:58:36.000000 metisse-0.0.2/metisse/clients/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 07:20:16.062527 metisse-0.0.2/metisse/clients/android/
--rw-rw-rw-   0        0        0       26 2023-04-17 02:58:36.000000 metisse-0.0.2/metisse/clients/android/__init__.py
--rw-rw-rw-   0        0        0     1331 2023-04-17 02:58:36.000000 metisse-0.0.2/metisse/clients/android/adb.py
--rw-rw-rw-   0        0        0      701 2023-04-17 02:58:36.000000 metisse-0.0.2/metisse/clients/client.py
-drwxrwxrwx   0        0        0        0 2023-04-17 07:20:16.064522 metisse-0.0.2/metisse/clients/ios/
--rw-rw-rw-   0        0        0       26 2023-04-17 02:58:36.000000 metisse-0.0.2/metisse/clients/ios/__init__.py
--rw-rw-rw-   0        0        0     1853 2023-04-17 02:58:36.000000 metisse-0.0.2/metisse/clients/ios/wda.py
-drwxrwxrwx   0        0        0        0 2023-04-17 07:20:16.066516 metisse-0.0.2/metisse/example/
--rw-rw-rw-   0        0        0        0 2023-04-17 02:58:36.000000 metisse-0.0.2/metisse/example/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 07:20:16.028829 metisse-0.0.2/metisse/example/example_data/
-drwxrwxrwx   0        0        0        0 2023-04-17 07:20:16.068511 metisse-0.0.2/metisse/example/example_data/icon/
--rw-rw-rw-   0        0        0    90781 2023-04-17 02:58:36.000000 metisse-0.0.2/metisse/example/example_data/icon/example_template_face.png
--rw-rw-rw-   0        0        0    55904 2023-04-17 02:58:36.000000 metisse-0.0.2/metisse/example/example_data/icon/example_template_hand.png
-drwxrwxrwx   0        0        0        0 2023-04-17 07:20:16.069508 metisse-0.0.2/metisse/example/example_data/temp_image/
--rw-rw-rw-   0        0        0  2503418 2023-04-17 02:58:36.000000 metisse-0.0.2/metisse/example/example_data/temp_image/tmp0.png
-drwxrwxrwx   0        0        0        0 2023-04-17 07:20:16.084783 metisse-0.0.2/metisse/example/example_data/ui/
--rw-rw-rw-   0        0        0      313 2023-04-17 02:58:36.000000 metisse-0.0.2/metisse/example/example_data/ui/gui_settings.py
--rw-rw-rw-   0        0        0    16964 2023-04-17 02:58:36.000000 metisse-0.0.2/metisse/example/example_data/ui/script_gui.py
--rw-rw-rw-   0        0        0     3934 2023-04-17 02:58:36.000000 metisse-0.0.2/metisse/example/example_data/ui/universal_script_gui_main.ui
--rw-rw-rw-   0        0        0     4195 2023-04-17 02:59:18.000000 metisse-0.0.2/metisse/example/example_data/ui/universal_script_gui_main_ui.py
--rw-rw-rw-   0        0        0     2287 2023-04-17 02:58:36.000000 metisse-0.0.2/metisse/example/example_data/ui/universal_script_gui_sub.ui
--rw-rw-rw-   0        0        0     3568 2023-04-17 02:58:36.000000 metisse-0.0.2/metisse/example/example_data/ui/universal_script_gui_sub2.ui
--rw-rw-rw-   0        0        0     3740 2023-04-17 02:59:18.000000 metisse-0.0.2/metisse/example/example_data/ui/universal_script_gui_sub2_ui.py
--rw-rw-rw-   0        0        0      685 2023-04-17 02:58:36.000000 metisse-0.0.2/metisse/example/example_data/ui/universal_script_gui_sub3.ui
--rw-rw-rw-   0        0        0     1020 2023-04-17 02:59:18.000000 metisse-0.0.2/metisse/example/example_data/ui/universal_script_gui_sub3_ui.py
--rw-rw-rw-   0        0        0     2326 2023-04-17 02:59:18.000000 metisse-0.0.2/metisse/example/example_data/ui/universal_script_gui_sub_ui.py
--rw-rw-rw-   0        0        0     7059 2023-04-17 02:58:36.000000 metisse-0.0.2/metisse/example/generate_example.py
--rw-rw-rw-   0        0        0    22344 2023-04-17 02:58:36.000000 metisse-0.0.2/metisse/metisse.py
--rw-rw-rw-   0        0        0     1843 2023-04-17 02:58:36.000000 metisse-0.0.2/metisse/params.py
--rw-rw-rw-   0        0        0      205 2023-04-17 02:58:36.000000 metisse-0.0.2/metisse/settings.py
--rw-rw-rw-   0        0        0     2047 2023-04-17 02:58:36.000000 metisse-0.0.2/metisse/template_metis.py
-drwxrwxrwx   0        0        0        0 2023-04-17 07:20:16.092761 metisse-0.0.2/metisse/utils/
--rw-rw-rw-   0        0        0        0 2023-04-17 02:58:36.000000 metisse-0.0.2/metisse/utils/__init__.py
--rw-rw-rw-   0        0        0     1539 2023-04-17 02:58:36.000000 metisse-0.0.2/metisse/utils/image_recognition.py
--rw-rw-rw-   0        0        0     2190 2023-04-17 02:58:36.000000 metisse-0.0.2/metisse/utils/metisse_log.py
--rw-rw-rw-   0        0        0     6585 2023-04-17 02:58:36.000000 metisse-0.0.2/metisse/utils/metisse_path.py
--rw-rw-rw-   0        0        0      774 2023-04-17 02:58:36.000000 metisse-0.0.2/metisse/utils/opencv_utils.py
--rw-rw-rw-   0        0        0     1051 2023-04-17 02:58:36.000000 metisse-0.0.2/metisse/utils/ui_client.py
-drwxrwxrwx   0        0        0        0 2023-04-17 07:20:16.059571 metisse-0.0.2/metisse.egg-info/
--rw-rw-rw-   0        0        0      415 2023-04-17 07:20:15.000000 metisse-0.0.2/metisse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1465 2023-04-17 07:20:15.000000 metisse-0.0.2/metisse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 07:20:15.000000 metisse-0.0.2/metisse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       99 2023-04-17 07:20:15.000000 metisse-0.0.2/metisse.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-17 07:20:15.000000 metisse-0.0.2/metisse.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 07:20:16.093759 metisse-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      840 2023-04-17 02:58:36.000000 metisse-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 09:59:34.509864 metisse-0.0.3/
+-rw-rw-rw-   0        0        0     9787 2023-04-17 02:58:36.000000 metisse-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     3196 2023-04-17 09:59:34.508834 metisse-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2736 2023-04-17 07:32:05.000000 metisse-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 09:59:34.446863 metisse-0.0.3/metisse/
+-rw-rw-rw-   0        0        0        0 2023-04-17 02:58:36.000000 metisse-0.0.3/metisse/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 09:59:34.473846 metisse-0.0.3/metisse/clients/
+-rw-rw-rw-   0        0        0        0 2023-04-17 02:58:36.000000 metisse-0.0.3/metisse/clients/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 09:59:34.476838 metisse-0.0.3/metisse/clients/android/
+-rw-rw-rw-   0        0        0       26 2023-04-17 07:32:05.000000 metisse-0.0.3/metisse/clients/android/__init__.py
+-rw-rw-rw-   0        0        0     1331 2023-04-17 07:32:05.000000 metisse-0.0.3/metisse/clients/android/adb.py
+-rw-rw-rw-   0        0        0      701 2023-04-17 02:58:36.000000 metisse-0.0.3/metisse/clients/client.py
+drwxrwxrwx   0        0        0        0 2023-04-17 09:59:34.478832 metisse-0.0.3/metisse/clients/ios/
+-rw-rw-rw-   0        0        0       26 2023-04-17 02:58:36.000000 metisse-0.0.3/metisse/clients/ios/__init__.py
+-rw-rw-rw-   0        0        0     1853 2023-04-17 02:58:36.000000 metisse-0.0.3/metisse/clients/ios/wda.py
+drwxrwxrwx   0        0        0        0 2023-04-17 09:59:34.480906 metisse-0.0.3/metisse/example/
+-rw-rw-rw-   0        0        0        0 2023-04-17 02:58:36.000000 metisse-0.0.3/metisse/example/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 09:59:34.430906 metisse-0.0.3/metisse/example/example_data/
+drwxrwxrwx   0        0        0        0 2023-04-17 09:59:34.483899 metisse-0.0.3/metisse/example/example_data/icon/
+-rw-rw-rw-   0        0        0    90781 2023-04-17 02:58:36.000000 metisse-0.0.3/metisse/example/example_data/icon/example_template_face.png
+-rw-rw-rw-   0        0        0    55904 2023-04-17 02:58:36.000000 metisse-0.0.3/metisse/example/example_data/icon/example_template_hand.png
+drwxrwxrwx   0        0        0        0 2023-04-17 09:59:34.484898 metisse-0.0.3/metisse/example/example_data/temp_image/
+-rw-rw-rw-   0        0        0  2503418 2023-04-17 02:58:36.000000 metisse-0.0.3/metisse/example/example_data/temp_image/tmp0.png
+drwxrwxrwx   0        0        0        0 2023-04-17 09:59:34.500854 metisse-0.0.3/metisse/example/example_data/ui/
+-rw-rw-rw-   0        0        0      313 2023-04-17 02:58:36.000000 metisse-0.0.3/metisse/example/example_data/ui/gui_settings.py
+-rw-rw-rw-   0        0        0    16964 2023-04-17 02:58:36.000000 metisse-0.0.3/metisse/example/example_data/ui/script_gui.py
+-rw-rw-rw-   0        0        0     3934 2023-04-17 02:58:36.000000 metisse-0.0.3/metisse/example/example_data/ui/universal_script_gui_main.ui
+-rw-rw-rw-   0        0        0     4195 2023-04-17 02:59:18.000000 metisse-0.0.3/metisse/example/example_data/ui/universal_script_gui_main_ui.py
+-rw-rw-rw-   0        0        0     2287 2023-04-17 02:58:36.000000 metisse-0.0.3/metisse/example/example_data/ui/universal_script_gui_sub.ui
+-rw-rw-rw-   0        0        0     3568 2023-04-17 02:58:36.000000 metisse-0.0.3/metisse/example/example_data/ui/universal_script_gui_sub2.ui
+-rw-rw-rw-   0        0        0     3740 2023-04-17 02:59:18.000000 metisse-0.0.3/metisse/example/example_data/ui/universal_script_gui_sub2_ui.py
+-rw-rw-rw-   0        0        0      685 2023-04-17 02:58:36.000000 metisse-0.0.3/metisse/example/example_data/ui/universal_script_gui_sub3.ui
+-rw-rw-rw-   0        0        0     1020 2023-04-17 02:59:18.000000 metisse-0.0.3/metisse/example/example_data/ui/universal_script_gui_sub3_ui.py
+-rw-rw-rw-   0        0        0     2326 2023-04-17 02:59:18.000000 metisse-0.0.3/metisse/example/example_data/ui/universal_script_gui_sub_ui.py
+-rw-rw-rw-   0        0        0     7076 2023-04-17 09:46:50.000000 metisse-0.0.3/metisse/example/generate_example.py
+-rw-rw-rw-   0        0        0    22531 2023-04-17 09:49:38.000000 metisse-0.0.3/metisse/metisse.py
+-rw-rw-rw-   0        0        0     1843 2023-04-17 02:58:36.000000 metisse-0.0.3/metisse/params.py
+-rw-rw-rw-   0        0        0      205 2023-04-17 02:58:36.000000 metisse-0.0.3/metisse/settings.py
+-rw-rw-rw-   0        0        0     2047 2023-04-17 02:58:36.000000 metisse-0.0.3/metisse/template_metis.py
+drwxrwxrwx   0        0        0        0 2023-04-17 09:59:34.507866 metisse-0.0.3/metisse/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-17 02:58:36.000000 metisse-0.0.3/metisse/utils/__init__.py
+-rw-rw-rw-   0        0        0     1539 2023-04-17 02:58:36.000000 metisse-0.0.3/metisse/utils/image_recognition.py
+-rw-rw-rw-   0        0        0     2190 2023-04-17 07:32:05.000000 metisse-0.0.3/metisse/utils/metisse_log.py
+-rw-rw-rw-   0        0        0     6585 2023-04-17 09:13:34.000000 metisse-0.0.3/metisse/utils/metisse_path.py
+-rw-rw-rw-   0        0        0      774 2023-04-17 02:58:36.000000 metisse-0.0.3/metisse/utils/opencv_utils.py
+-rw-rw-rw-   0        0        0     1051 2023-04-17 02:58:36.000000 metisse-0.0.3/metisse/utils/ui_client.py
+drwxrwxrwx   0        0        0        0 2023-04-17 09:59:34.471880 metisse-0.0.3/metisse.egg-info/
+-rw-rw-rw-   0        0        0     3196 2023-04-17 09:59:34.000000 metisse-0.0.3/metisse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1465 2023-04-17 09:59:34.000000 metisse-0.0.3/metisse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 09:59:34.000000 metisse-0.0.3/metisse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       99 2023-04-17 09:59:34.000000 metisse-0.0.3/metisse.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-17 09:59:34.000000 metisse-0.0.3/metisse.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 09:59:34.509864 metisse-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1018 2023-04-17 09:50:52.000000 metisse-0.0.3/setup.py
```

### Comparing `metisse-0.0.2/LICENSE` & `metisse-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `metisse-0.0.2/README.md` & `metisse-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `metisse-0.0.2/metisse/clients/android/adb.py` & `metisse-0.0.3/metisse/clients/android/adb.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.2/metisse/clients/client.py` & `metisse-0.0.3/metisse/clients/client.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.2/metisse/clients/ios/wda.py` & `metisse-0.0.3/metisse/clients/ios/wda.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.2/metisse/example/example_data/icon/example_template_face.png` & `metisse-0.0.3/metisse/example/example_data/icon/example_template_face.png`

 * *Files identical despite different names*

### Comparing `metisse-0.0.2/metisse/example/example_data/icon/example_template_hand.png` & `metisse-0.0.3/metisse/example/example_data/icon/example_template_hand.png`

 * *Files identical despite different names*

### Comparing `metisse-0.0.2/metisse/example/example_data/temp_image/tmp0.png` & `metisse-0.0.3/metisse/example/example_data/temp_image/tmp0.png`

 * *Files identical despite different names*

### Comparing `metisse-0.0.2/metisse/example/example_data/ui/script_gui.py` & `metisse-0.0.3/metisse/example/example_data/ui/script_gui.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.2/metisse/example/example_data/ui/universal_script_gui_main.ui` & `metisse-0.0.3/metisse/example/example_data/ui/universal_script_gui_main.ui`

 * *Files identical despite different names*

### Comparing `metisse-0.0.2/metisse/example/example_data/ui/universal_script_gui_main_ui.py` & `metisse-0.0.3/metisse/example/example_data/ui/universal_script_gui_main_ui.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.2/metisse/example/example_data/ui/universal_script_gui_sub.ui` & `metisse-0.0.3/metisse/example/example_data/ui/universal_script_gui_sub.ui`

 * *Files identical despite different names*

### Comparing `metisse-0.0.2/metisse/example/example_data/ui/universal_script_gui_sub2.ui` & `metisse-0.0.3/metisse/example/example_data/ui/universal_script_gui_sub2.ui`

 * *Files identical despite different names*

### Comparing `metisse-0.0.2/metisse/example/example_data/ui/universal_script_gui_sub2_ui.py` & `metisse-0.0.3/metisse/example/example_data/ui/universal_script_gui_sub2_ui.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.2/metisse/example/example_data/ui/universal_script_gui_sub3.ui` & `metisse-0.0.3/metisse/example/example_data/ui/universal_script_gui_sub3.ui`

 * *Files identical despite different names*

### Comparing `metisse-0.0.2/metisse/example/example_data/ui/universal_script_gui_sub3_ui.py` & `metisse-0.0.3/metisse/example/example_data/ui/universal_script_gui_sub3_ui.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.2/metisse/example/example_data/ui/universal_script_gui_sub_ui.py` & `metisse-0.0.3/metisse/example/example_data/ui/universal_script_gui_sub_ui.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.2/metisse/example/generate_example.py` & `metisse-0.0.3/metisse/example/generate_example.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
             self,
             device_id=device_id,
             relatively_path=relatively_path,
             pyqt6_ui_label=pyqt6_ui_label,
             os_environment=os_environment,
         )
 
-    def __call__(self):
+    def __call__(self, *args, **kwargs):
         self.check_image_recognition(
             CustomImage(screen_image_name='tmp0',
                                    template_image_name='example_template_hand',
                                    is_refresh_screenshot=False))  # simulate image recognition hand icon
         print(f'hand pos = {self._img_recog_result.coordinate}')
 
         self.execute_time_sleep(1)  # wait 1 second
```

### Comparing `metisse-0.0.2/metisse/metisse.py` & `metisse-0.0.3/metisse/metisse.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         if not relatively_path:
             self._relatively_path = MetisseClass.get_current_path()
         else:
             self._relatively_path = relatively_path
 
         super(TemplateMetisClass, self).__init__()
 
-        self._device_id = device_id
+        self._device_id = self.check_device_id_path_valid(device_id)
         self._dev_path = DevPath(self._relatively_path)
         self._script_path = self._dev_path.create_extended_script_path(self._device_id)
         self._logger = MetisseLogger("MetisClass_logger",
                                      log_level=logging.DEBUG,
                                      log_file=os.path.join(self._script_path.device_id_path, "log",
                                                            self.get_time() + self._device_id + ".log"))
         assert os_environment in ST.OS_ENVIRONMENT
@@ -78,14 +78,19 @@
         return _path
 
     def execute_time_sleep(self, wait_time: float = 0):
         self._logger.info("execute_time_sleep : wait_time= %.2f", wait_time)
         self._ui_client.send_log_to_ui(f"execute_time_sleep method : \n wait_time= {wait_time:.2f}")
         time.sleep(wait_time)
 
+    def check_device_id_path_valid(self,input:str) -> str:
+        if ':' in input:
+            return input.replace(':', '_')
+        return input
+
     @property
     def get_device_id(self) -> str:
         if self._device_id:
             return ' -s ' + self._device_id
         return ''
 
     def check_gamelog(self, params: ImageRecognitionParams):
```

### Comparing `metisse-0.0.2/metisse/params.py` & `metisse-0.0.3/metisse/params.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.2/metisse/template_metis.py` & `metisse-0.0.3/metisse/template_metis.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.2/metisse/utils/image_recognition.py` & `metisse-0.0.3/metisse/utils/image_recognition.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.2/metisse/utils/metisse_log.py` & `metisse-0.0.3/metisse/utils/metisse_log.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.2/metisse/utils/metisse_path.py` & `metisse-0.0.3/metisse/utils/metisse_path.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.2/metisse/utils/opencv_utils.py` & `metisse-0.0.3/metisse/utils/opencv_utils.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.2/metisse/utils/ui_client.py` & `metisse-0.0.3/metisse/utils/ui_client.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.2/metisse.egg-info/SOURCES.txt` & `metisse-0.0.3/metisse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

