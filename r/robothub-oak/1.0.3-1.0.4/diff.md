# Comparing `tmp/robothub_oak-1.0.3.tar.gz` & `tmp/robothub_oak-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robothub_oak-1.0.3.tar", last modified: Thu Apr  6 00:21:50 2023, max compression
+gzip compressed data, was "robothub_oak-1.0.4.tar", last modified: Mon Apr 17 09:24:45 2023, max compression
```

## Comparing `robothub_oak-1.0.3.tar` & `robothub_oak-1.0.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:21:50.509091 robothub_oak-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-06 00:21:11.000000 robothub_oak-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-06 00:21:11.000000 robothub_oak-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-06 00:21:50.509091 robothub_oak-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-06 00:21:11.000000 robothub_oak-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 00:21:50.509091 robothub_oak-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-06 00:21:11.000000 robothub_oak-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:21:50.501092 robothub_oak-1.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:21:50.505092 robothub_oak-1.0.3/src/robothub_oak/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-06 00:21:11.000000 robothub_oak-1.0.3/src/robothub_oak/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      423 2023-04-06 00:21:11.000000 robothub_oak-1.0.3/src/robothub_oak/app.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2225 2023-04-06 00:21:11.000000 robothub_oak-1.0.3/src/robothub_oak/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-04-06 00:21:11.000000 robothub_oak-1.0.3/src/robothub_oak/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:21:50.505092 robothub_oak-1.0.3/src/robothub_oak/components/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-06 00:21:11.000000 robothub_oak-1.0.3/src/robothub_oak/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-04-06 00:21:11.000000 robothub_oak-1.0.3/src/robothub_oak/components/camera.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 00:21:11.000000 robothub_oak-1.0.3/src/robothub_oak/components/imu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-06 00:21:11.000000 robothub_oak-1.0.3/src/robothub_oak/components/neural_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-06 00:21:11.000000 robothub_oak-1.0.3/src/robothub_oak/components/stereo.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-06 00:21:11.000000 robothub_oak-1.0.3/src/robothub_oak/components/streamable.py
--rw-r--r--   0 runner    (1001) docker     (123)     5978 2023-04-06 00:21:11.000000 robothub_oak-1.0.3/src/robothub_oak/device.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13079 2023-04-06 00:21:11.000000 robothub_oak-1.0.3/src/robothub_oak/hub_camera.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7994 2023-04-06 00:21:11.000000 robothub_oak-1.0.3/src/robothub_oak/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-06 00:21:11.000000 robothub_oak-1.0.3/src/robothub_oak/packets.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-06 00:21:11.000000 robothub_oak-1.0.3/src/robothub_oak/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:21:50.505092 robothub_oak-1.0.3/src/robothub_oak.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-06 00:21:50.000000 robothub_oak-1.0.3/src/robothub_oak.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-06 00:21:50.000000 robothub_oak-1.0.3/src/robothub_oak.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 00:21:50.000000 robothub_oak-1.0.3/src/robothub_oak.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-06 00:21:50.000000 robothub_oak-1.0.3/src/robothub_oak.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:21:50.509091 robothub_oak-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-06 00:21:11.000000 robothub_oak-1.0.3/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 00:21:11.000000 robothub_oak-1.0.3/tests/test_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 00:21:11.000000 robothub_oak-1.0.3/tests/test_hub_camera.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 00:21:11.000000 robothub_oak-1.0.3/tests/test_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:24:45.817186 robothub_oak-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-17 09:24:05.000000 robothub_oak-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-17 09:24:05.000000 robothub_oak-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-17 09:24:45.817186 robothub_oak-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-17 09:24:05.000000 robothub_oak-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 09:24:45.817186 robothub_oak-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-17 09:24:05.000000 robothub_oak-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:24:45.809186 robothub_oak-1.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:24:45.813186 robothub_oak-1.0.4/src/robothub_oak/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-17 09:24:05.000000 robothub_oak-1.0.4/src/robothub_oak/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      423 2023-04-17 09:24:05.000000 robothub_oak-1.0.4/src/robothub_oak/app.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2225 2023-04-17 09:24:05.000000 robothub_oak-1.0.4/src/robothub_oak/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-04-17 09:24:05.000000 robothub_oak-1.0.4/src/robothub_oak/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:24:45.817186 robothub_oak-1.0.4/src/robothub_oak/components/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-17 09:24:05.000000 robothub_oak-1.0.4/src/robothub_oak/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-04-17 09:24:05.000000 robothub_oak-1.0.4/src/robothub_oak/components/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 09:24:05.000000 robothub_oak-1.0.4/src/robothub_oak/components/imu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-17 09:24:05.000000 robothub_oak-1.0.4/src/robothub_oak/components/neural_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-17 09:24:05.000000 robothub_oak-1.0.4/src/robothub_oak/components/stereo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-17 09:24:05.000000 robothub_oak-1.0.4/src/robothub_oak/components/streamable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5978 2023-04-17 09:24:05.000000 robothub_oak-1.0.4/src/robothub_oak/device.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13238 2023-04-17 09:24:05.000000 robothub_oak-1.0.4/src/robothub_oak/hub_camera.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7990 2023-04-17 09:24:05.000000 robothub_oak-1.0.4/src/robothub_oak/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-17 09:24:05.000000 robothub_oak-1.0.4/src/robothub_oak/packets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-17 09:24:05.000000 robothub_oak-1.0.4/src/robothub_oak/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:24:45.813186 robothub_oak-1.0.4/src/robothub_oak.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-17 09:24:45.000000 robothub_oak-1.0.4/src/robothub_oak.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-17 09:24:45.000000 robothub_oak-1.0.4/src/robothub_oak.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 09:24:45.000000 robothub_oak-1.0.4/src/robothub_oak.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-17 09:24:45.000000 robothub_oak-1.0.4/src/robothub_oak.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:24:45.817186 robothub_oak-1.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-17 09:24:05.000000 robothub_oak-1.0.4/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 09:24:05.000000 robothub_oak-1.0.4/tests/test_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 09:24:05.000000 robothub_oak-1.0.4/tests/test_hub_camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 09:24:05.000000 robothub_oak-1.0.4/tests/test_manager.py
```

### Comparing `robothub_oak-1.0.3/LICENSE` & `robothub_oak-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `robothub_oak-1.0.3/PKG-INFO` & `robothub_oak-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robothub_oak
-Version: 1.0.3
+Version: 1.0.4
 Summary: RobotHub-OAK integration library
 Home-page: https://www.luxonis.com/
 Author: Luxonis
 Author-email: support@luxonis.com
 License: MIT
 Project-URL: Homepage, https://github.com/luxonis/robothub-oak/
 Project-URL: Documentation, https://hub-docs.luxonis.com/
```

### Comparing `robothub_oak-1.0.3/README.md` & `robothub_oak-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `robothub_oak-1.0.3/setup.py` & `robothub_oak-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 
 long_description = io.open('README.md', encoding='utf-8').read()
 
 setup(
     name='robothub_oak',
-    version='1.0.3',
+    version='1.0.4',
     description='RobotHub-OAK integration library',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://www.luxonis.com/',
     license='MIT',
     keywords='robothub robot hub connect agent depthai oak sdk',
     author='Luxonis',
```

### Comparing `robothub_oak-1.0.3/src/robothub_oak/callbacks.py` & `robothub_oak-1.0.4/src/robothub_oak/callbacks.py`

 * *Files identical despite different names*

### Comparing `robothub_oak-1.0.3/src/robothub_oak/commands.py` & `robothub_oak-1.0.4/src/robothub_oak/commands.py`

 * *Files identical despite different names*

### Comparing `robothub_oak-1.0.3/src/robothub_oak/components/camera.py` & `robothub_oak-1.0.4/src/robothub_oak/components/camera.py`

 * *Files identical despite different names*

### Comparing `robothub_oak-1.0.3/src/robothub_oak/components/neural_network.py` & `robothub_oak-1.0.4/src/robothub_oak/components/neural_network.py`

 * *Files identical despite different names*

### Comparing `robothub_oak-1.0.3/src/robothub_oak/components/stereo.py` & `robothub_oak-1.0.4/src/robothub_oak/components/stereo.py`

 * *Files identical despite different names*

### Comparing `robothub_oak-1.0.3/src/robothub_oak/device.py` & `robothub_oak-1.0.4/src/robothub_oak/device.py`

 * *Files identical despite different names*

### Comparing `robothub_oak-1.0.3/src/robothub_oak/hub_camera.py` & `robothub_oak-1.0.4/src/robothub_oak/hub_camera.py`

 * *Files 1% similar despite different names*

```diff
@@ -217,20 +217,27 @@
     def stop(self) -> None:
         """
         Stops the device and sets the state to disconnected.
         """
         self.stop_event.set()
 
         for stream in self.streams.values():
-            robothub.STREAMS.destroy(stream)
+            try:
+                robothub.STREAMS.destroy(stream)
+            except ValueError:
+                pass
+
+        self.streams.clear()
+        self.state = robothub.DeviceState.DISCONNECTED
 
         self.streams.clear()
 
         if self.oak_camera:
             self.oak_camera.device.close()
+
         self.oak_camera = None
 
     def stats_report(self) -> Dict[str, Any]:
         """
         Returns a dictionary with statistics about the device.
         """
         stats = {'mxid': self.device.getMxId()}
```

### Comparing `robothub_oak-1.0.3/src/robothub_oak/manager.py` & `robothub_oak-1.0.4/src/robothub_oak/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,24 +71,24 @@
         self.__graceful_thread_join(self.connection_thread)
         self.__graceful_thread_join(self.reporting_thread)
         self.__graceful_thread_join(self.polling_thread)
 
         try:
             robothub.STREAMS.destroy_all_streams()
         except BaseException as e:
-            raise Exception(f'Destroy all streams excepted with: {e}.')
+            logging.debug(f'Destroy all streams excepted with: {e}.')
 
         for camera in self._hub_cameras:
             try:
                 if camera.state != robothub.DeviceState.DISCONNECTED:
                     with open(os.devnull, 'w') as devnull:
                         with contextlib.redirect_stdout(devnull):
                             camera.stop()
             except BaseException as e:
-                raise Exception(f'Device {camera.device_name}: could not exit with exception: {e}.')
+                logging.debug(f'Device {camera.device_name}: could not exit with exception: {e}.')
 
         log.info('App: stopped successfully.')
 
     def add_device(self, device: 'Device') -> None:
         """
         Add a camera to the list of cameras.
         """
```

### Comparing `robothub_oak-1.0.3/src/robothub_oak/packets.py` & `robothub_oak-1.0.4/src/robothub_oak/packets.py`

 * *Files identical despite different names*

### Comparing `robothub_oak-1.0.3/src/robothub_oak.egg-info/PKG-INFO` & `robothub_oak-1.0.4/src/robothub_oak.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robothub-oak
-Version: 1.0.3
+Version: 1.0.4
 Summary: RobotHub-OAK integration library
 Home-page: https://www.luxonis.com/
 Author: Luxonis
 Author-email: support@luxonis.com
 License: MIT
 Project-URL: Homepage, https://github.com/luxonis/robothub-oak/
 Project-URL: Documentation, https://hub-docs.luxonis.com/
```

### Comparing `robothub_oak-1.0.3/src/robothub_oak.egg-info/SOURCES.txt` & `robothub_oak-1.0.4/src/robothub_oak.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robothub_oak-1.0.3/tests/test_app.py` & `robothub_oak-1.0.4/tests/test_app.py`

 * *Files identical despite different names*

