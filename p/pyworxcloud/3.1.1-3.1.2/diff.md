# Comparing `tmp/pyworxcloud-3.1.1.tar.gz` & `tmp/pyworxcloud-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyworxcloud-3.1.1.tar", max compression
+gzip compressed data, was "pyworxcloud-3.1.2.tar", max compression
```

## Comparing `pyworxcloud-3.1.1.tar` & `pyworxcloud-3.1.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    35149 2023-04-17 09:16:55.398923 pyworxcloud-3.1.1/LICENSE
--rw-r--r--   0        0        0      929 2023-04-17 09:16:55.398923 pyworxcloud-3.1.1/README.md
--rw-r--r--   0        0        0      610 2023-04-17 09:17:10.387114 pyworxcloud-3.1.1/pyproject.toml
--rw-r--r--   0        0        0    28745 2023-04-17 09:16:55.398923 pyworxcloud-3.1.1/pyworxcloud/__init__.py
--rw-r--r--   0        0        0     3751 2023-04-17 09:16:55.398923 pyworxcloud-3.1.1/pyworxcloud/api.py
--rw-r--r--   0        0        0     1134 2023-04-17 09:16:55.398923 pyworxcloud-3.1.1/pyworxcloud/clouds.py
--rw-r--r--   0        0        0      927 2023-04-17 09:16:55.398923 pyworxcloud-3.1.1/pyworxcloud/const.py
--rw-r--r--   0        0        0      204 2023-04-17 09:16:55.398923 pyworxcloud-3.1.1/pyworxcloud/day_map.py
--rw-r--r--   0        0        0     3647 2023-04-17 09:16:55.398923 pyworxcloud-3.1.1/pyworxcloud/events.py
--rw-r--r--   0        0        0     1826 2023-04-17 09:16:55.398923 pyworxcloud-3.1.1/pyworxcloud/exceptions.py
--rw-r--r--   0        0        0      204 2023-04-17 09:16:55.398923 pyworxcloud-3.1.1/pyworxcloud/helpers/__init__.py
--rw-r--r--   0        0        0      637 2023-04-17 09:16:55.398923 pyworxcloud-3.1.1/pyworxcloud/helpers/logger.py
--rw-r--r--   0        0        0     2794 2023-04-17 09:16:55.398923 pyworxcloud-3.1.1/pyworxcloud/helpers/time_format.py
--rw-r--r--   0        0        0      838 2023-04-17 09:16:55.398923 pyworxcloud-3.1.1/pyworxcloud/utils/__init__.py
--rw-r--r--   0        0        0     3338 2023-04-17 09:16:55.398923 pyworxcloud-3.1.1/pyworxcloud/utils/battery.py
--rw-r--r--   0        0        0     2091 2023-04-17 09:16:55.398923 pyworxcloud-3.1.1/pyworxcloud/utils/blades.py
--rw-r--r--   0        0        0     1924 2023-04-17 09:16:55.398923 pyworxcloud-3.1.1/pyworxcloud/utils/capability.py
--rw-r--r--   0        0        0     3838 2023-04-17 09:16:55.398923 pyworxcloud-3.1.1/pyworxcloud/utils/devices.py
--rw-r--r--   0        0        0      617 2023-04-17 09:16:55.402922 pyworxcloud-3.1.1/pyworxcloud/utils/firmware.py
--rw-r--r--   0        0        0      281 2023-04-17 09:16:55.402922 pyworxcloud-3.1.1/pyworxcloud/utils/landroid_class.py
--rw-r--r--   0        0        0      306 2023-04-17 09:16:55.402922 pyworxcloud-3.1.1/pyworxcloud/utils/lawn.py
--rw-r--r--   0        0        0      427 2023-04-17 09:16:55.402922 pyworxcloud-3.1.1/pyworxcloud/utils/location.py
--rw-r--r--   0        0        0     7538 2023-04-17 09:16:55.402922 pyworxcloud-3.1.1/pyworxcloud/utils/mqtt.py
--rw-r--r--   0        0        0      411 2023-04-17 09:16:55.402922 pyworxcloud-3.1.1/pyworxcloud/utils/orientation.py
--rw-r--r--   0        0        0     1348 2023-04-17 09:16:55.402922 pyworxcloud-3.1.1/pyworxcloud/utils/product.py
--rw-r--r--   0        0        0     1109 2023-04-17 09:16:55.402922 pyworxcloud-3.1.1/pyworxcloud/utils/rainsensor.py
--rw-r--r--   0        0        0     2410 2023-04-17 09:16:55.402922 pyworxcloud-3.1.1/pyworxcloud/utils/requests.py
--rw-r--r--   0        0        0     6375 2023-04-17 09:16:55.402922 pyworxcloud-3.1.1/pyworxcloud/utils/schedules.py
--rw-r--r--   0        0        0     2050 2023-04-17 09:16:55.402922 pyworxcloud-3.1.1/pyworxcloud/utils/state.py
--rw-r--r--   0        0        0      657 2023-04-17 09:16:55.402922 pyworxcloud-3.1.1/pyworxcloud/utils/statistics.py
--rw-r--r--   0        0        0      726 2023-04-17 09:16:55.402922 pyworxcloud-3.1.1/pyworxcloud/utils/warranty.py
--rw-r--r--   0        0        0     1423 2023-04-17 09:16:55.402922 pyworxcloud-3.1.1/pyworxcloud/utils/zone.py
--rw-r--r--   0        0        0     1698 1970-01-01 00:00:00.000000 pyworxcloud-3.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-17 10:21:38.844156 pyworxcloud-3.1.2/LICENSE
+-rw-r--r--   0        0        0      929 2023-04-17 10:21:38.844156 pyworxcloud-3.1.2/README.md
+-rw-r--r--   0        0        0      610 2023-04-17 10:21:52.648889 pyworxcloud-3.1.2/pyproject.toml
+-rw-r--r--   0        0        0    28730 2023-04-17 10:21:38.848156 pyworxcloud-3.1.2/pyworxcloud/__init__.py
+-rw-r--r--   0        0        0     3751 2023-04-17 10:21:38.848156 pyworxcloud-3.1.2/pyworxcloud/api.py
+-rw-r--r--   0        0        0     1134 2023-04-17 10:21:38.848156 pyworxcloud-3.1.2/pyworxcloud/clouds.py
+-rw-r--r--   0        0        0      927 2023-04-17 10:21:38.848156 pyworxcloud-3.1.2/pyworxcloud/const.py
+-rw-r--r--   0        0        0      204 2023-04-17 10:21:38.848156 pyworxcloud-3.1.2/pyworxcloud/day_map.py
+-rw-r--r--   0        0        0     3647 2023-04-17 10:21:38.848156 pyworxcloud-3.1.2/pyworxcloud/events.py
+-rw-r--r--   0        0        0     1826 2023-04-17 10:21:38.848156 pyworxcloud-3.1.2/pyworxcloud/exceptions.py
+-rw-r--r--   0        0        0      204 2023-04-17 10:21:38.848156 pyworxcloud-3.1.2/pyworxcloud/helpers/__init__.py
+-rw-r--r--   0        0        0      637 2023-04-17 10:21:38.848156 pyworxcloud-3.1.2/pyworxcloud/helpers/logger.py
+-rw-r--r--   0        0        0     2794 2023-04-17 10:21:38.848156 pyworxcloud-3.1.2/pyworxcloud/helpers/time_format.py
+-rw-r--r--   0        0        0      838 2023-04-17 10:21:38.848156 pyworxcloud-3.1.2/pyworxcloud/utils/__init__.py
+-rw-r--r--   0        0        0     3338 2023-04-17 10:21:38.848156 pyworxcloud-3.1.2/pyworxcloud/utils/battery.py
+-rw-r--r--   0        0        0     2091 2023-04-17 10:21:38.848156 pyworxcloud-3.1.2/pyworxcloud/utils/blades.py
+-rw-r--r--   0        0        0     1924 2023-04-17 10:21:38.848156 pyworxcloud-3.1.2/pyworxcloud/utils/capability.py
+-rw-r--r--   0        0        0     3838 2023-04-17 10:21:38.848156 pyworxcloud-3.1.2/pyworxcloud/utils/devices.py
+-rw-r--r--   0        0        0      617 2023-04-17 10:21:38.848156 pyworxcloud-3.1.2/pyworxcloud/utils/firmware.py
+-rw-r--r--   0        0        0      281 2023-04-17 10:21:38.848156 pyworxcloud-3.1.2/pyworxcloud/utils/landroid_class.py
+-rw-r--r--   0        0        0      306 2023-04-17 10:21:38.848156 pyworxcloud-3.1.2/pyworxcloud/utils/lawn.py
+-rw-r--r--   0        0        0      427 2023-04-17 10:21:38.848156 pyworxcloud-3.1.2/pyworxcloud/utils/location.py
+-rw-r--r--   0        0        0     7112 2023-04-17 10:21:38.848156 pyworxcloud-3.1.2/pyworxcloud/utils/mqtt.py
+-rw-r--r--   0        0        0      411 2023-04-17 10:21:38.848156 pyworxcloud-3.1.2/pyworxcloud/utils/orientation.py
+-rw-r--r--   0        0        0     1348 2023-04-17 10:21:38.848156 pyworxcloud-3.1.2/pyworxcloud/utils/product.py
+-rw-r--r--   0        0        0     1109 2023-04-17 10:21:38.848156 pyworxcloud-3.1.2/pyworxcloud/utils/rainsensor.py
+-rw-r--r--   0        0        0     2410 2023-04-17 10:21:38.848156 pyworxcloud-3.1.2/pyworxcloud/utils/requests.py
+-rw-r--r--   0        0        0     6375 2023-04-17 10:21:38.848156 pyworxcloud-3.1.2/pyworxcloud/utils/schedules.py
+-rw-r--r--   0        0        0     2050 2023-04-17 10:21:38.848156 pyworxcloud-3.1.2/pyworxcloud/utils/state.py
+-rw-r--r--   0        0        0      657 2023-04-17 10:21:38.848156 pyworxcloud-3.1.2/pyworxcloud/utils/statistics.py
+-rw-r--r--   0        0        0      726 2023-04-17 10:21:38.848156 pyworxcloud-3.1.2/pyworxcloud/utils/warranty.py
+-rw-r--r--   0        0        0     1423 2023-04-17 10:21:38.852156 pyworxcloud-3.1.2/pyworxcloud/utils/zone.py
+-rw-r--r--   0        0        0     1698 1970-01-01 00:00:00.000000 pyworxcloud-3.1.2/PKG-INFO
```

### Comparing `pyworxcloud-3.1.1/LICENSE` & `pyworxcloud-3.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.1/README.md` & `pyworxcloud-3.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.1/pyproject.toml` & `pyworxcloud-3.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pyworxcloud"
-version = "v3.1.1"
+version = "v3.1.2"
 description = "Landroid cloud (Positec) API library"
 authors = ["Malene Trab <malene@trab.dk>"]
 documentation = "https://github.com/mtrab/pyworxcloud"
 classifiers = [
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
```

### Comparing `pyworxcloud-3.1.1/pyworxcloud/__init__.py` & `pyworxcloud-3.1.2/pyworxcloud/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -245,15 +245,15 @@
             self._endpoint,
             self._user_id,
             self._log,
             self._on_update,
         )
 
         self.mqtt.connect()
-        while isinstance(self.mqtt.connected, type(None)):
+        while self.mqtt.connected is False:
             pass
 
         for mower in self._mowers:
             self.mqtt.subscribe(mower["mqtt_topics"]["command_out"])
 
         self._log.debug("MQTT connect done")
```

### Comparing `pyworxcloud-3.1.1/pyworxcloud/api.py` & `pyworxcloud-3.1.2/pyworxcloud/api.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.1/pyworxcloud/clouds.py` & `pyworxcloud-3.1.2/pyworxcloud/clouds.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.1/pyworxcloud/const.py` & `pyworxcloud-3.1.2/pyworxcloud/const.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.1/pyworxcloud/events.py` & `pyworxcloud-3.1.2/pyworxcloud/events.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.1/pyworxcloud/exceptions.py` & `pyworxcloud-3.1.2/pyworxcloud/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.1/pyworxcloud/helpers/logger.py` & `pyworxcloud-3.1.2/pyworxcloud/helpers/logger.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.1/pyworxcloud/helpers/time_format.py` & `pyworxcloud-3.1.2/pyworxcloud/helpers/time_format.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.1/pyworxcloud/utils/__init__.py` & `pyworxcloud-3.1.2/pyworxcloud/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.1/pyworxcloud/utils/battery.py` & `pyworxcloud-3.1.2/pyworxcloud/utils/battery.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.1/pyworxcloud/utils/blades.py` & `pyworxcloud-3.1.2/pyworxcloud/utils/blades.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.1/pyworxcloud/utils/capability.py` & `pyworxcloud-3.1.2/pyworxcloud/utils/capability.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.1/pyworxcloud/utils/devices.py` & `pyworxcloud-3.1.2/pyworxcloud/utils/devices.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.1/pyworxcloud/utils/firmware.py` & `pyworxcloud-3.1.2/pyworxcloud/utils/firmware.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.1/pyworxcloud/utils/mqtt.py` & `pyworxcloud-3.1.2/pyworxcloud/utils/mqtt.py`

 * *Files 15% similar despite different names*

```diff
@@ -159,55 +159,43 @@
         client: mqtt.Client | None,
         userdata: Any | None,
         flags: Any | None,
         rc: int | None,
         properties: Any | None = None,  # pylint: disable=unused-argument,invalid-name
     ) -> None:
         """MQTT callback method."""
-        self._log.debug(connack_string(rc))
+        logger = self._log.getChild("Conn_State")
+        logger.debug(connack_string(rc))
         if rc == 0:
             self._disconnected = False
-            self._log.debug("MQTT connected")
+            logger.debug("MQTT connected")
             self._events.call(
                 LandroidEvent.MQTT_CONNECTION, state=self.client.is_connected()
             )
         else:
-            self._log.debug("MQTT connection failed")
+            logger.debug("MQTT connection failed")
             self._events.call(
                 LandroidEvent.MQTT_CONNECTION, state=self.client.is_connected()
             )
 
     def _on_disconnect(
         self,
         client: mqtt.Client | None,
         userdata: Any | None,
         rc: int | None,
         properties: Any | None = None,  # pylint: disable=unused-argument,invalid-name
     ) -> None:
         """MQTT callback method."""
-        logger = self._log.getChild("mqtt.disconnected")
+        logger = self._log.getChild("Conn_State")
         if rc > 0:
-            if rc == 7:
-                if not self.client.is_connected():
-                    raise MQTTException(
-                        "Unexpected MQTT disconnect - were you perhaps banned?"
-                    )
-            if self.client.is_connected():
-                logger.debug("MQTT connection was lost! (%s)", error_string(rc))
-
             logger.debug(
-                "Setting MQTT connected flag FALSE and unsubscribing from topics"
-            )
-
-            self._events.call(
-                LandroidEvent.MQTT_CONNECTION, state=self.client.is_connected()
+                "Unexpected MQTT disconnect (%s) - retrying", connack_string(rc)
             )
-
-            for topic in self._topic:
-                client.unsubscribe(self._topic.pop(topic))
+            self.client.reconnect_delay_set(min_delay=1, max_delay=120)
+            self.client.reconnect()
 
     def disconnect(
         self, reasoncode=None, properties=None  # pylint: disable=unused-argument
     ):
         """Disconnect from AWSIoT MQTT server."""
         self._disconnected = True
         self.client.loop_stop()
```

### Comparing `pyworxcloud-3.1.1/pyworxcloud/utils/product.py` & `pyworxcloud-3.1.2/pyworxcloud/utils/product.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.1/pyworxcloud/utils/rainsensor.py` & `pyworxcloud-3.1.2/pyworxcloud/utils/rainsensor.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.1/pyworxcloud/utils/requests.py` & `pyworxcloud-3.1.2/pyworxcloud/utils/requests.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.1/pyworxcloud/utils/schedules.py` & `pyworxcloud-3.1.2/pyworxcloud/utils/schedules.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.1/pyworxcloud/utils/state.py` & `pyworxcloud-3.1.2/pyworxcloud/utils/state.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.1/pyworxcloud/utils/statistics.py` & `pyworxcloud-3.1.2/pyworxcloud/utils/statistics.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.1/pyworxcloud/utils/warranty.py` & `pyworxcloud-3.1.2/pyworxcloud/utils/warranty.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.1/pyworxcloud/utils/zone.py` & `pyworxcloud-3.1.2/pyworxcloud/utils/zone.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.1/PKG-INFO` & `pyworxcloud-3.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyworxcloud
-Version: 3.1.1
+Version: 3.1.2
 Summary: Landroid cloud (Positec) API library
 License: MIT
 Author: Malene Trab
 Author-email: malene@trab.dk
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyworxcloud Version: 3.1.1 Summary: Landroid cloud
+Metadata-Version: 2.1 Name: pyworxcloud Version: 3.1.2 Summary: Landroid cloud
 (Positec) API library License: MIT Author: Malene Trab Author-email:
 malene@trab.dk Requires-Python: >=3.10,<4.0 Classifier: License :: OSI Approved
 :: MIT License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Topic :: Software Development :: Libraries :: Python
 Modules Requires-Dist: paho-mqtt (>=1.6.1,<2.0.0) Requires-Dist: requests
 (>=2.26.0,<3.0.0) Requires-Dist: urllib3 (>=1.26.10,<2.0.0) Project-URL: Bug
```

