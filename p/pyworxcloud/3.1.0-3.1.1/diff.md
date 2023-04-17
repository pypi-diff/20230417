# Comparing `tmp/pyworxcloud-3.1.0.tar.gz` & `tmp/pyworxcloud-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyworxcloud-3.1.0.tar", max compression
+gzip compressed data, was "pyworxcloud-3.1.1.tar", max compression
```

## Comparing `pyworxcloud-3.1.0.tar` & `pyworxcloud-3.1.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    35149 2023-04-15 21:26:39.145454 pyworxcloud-3.1.0/LICENSE
--rw-r--r--   0        0        0      929 2023-04-15 21:26:39.145454 pyworxcloud-3.1.0/README.md
--rw-r--r--   0        0        0      610 2023-04-15 21:26:50.221668 pyworxcloud-3.1.0/pyproject.toml
--rw-r--r--   0        0        0    28745 2023-04-15 21:26:39.145454 pyworxcloud-3.1.0/pyworxcloud/__init__.py
--rw-r--r--   0        0        0     3751 2023-04-15 21:26:39.145454 pyworxcloud-3.1.0/pyworxcloud/api.py
--rw-r--r--   0        0        0     1134 2023-04-15 21:26:39.145454 pyworxcloud-3.1.0/pyworxcloud/clouds.py
--rw-r--r--   0        0        0      927 2023-04-15 21:26:39.145454 pyworxcloud-3.1.0/pyworxcloud/const.py
--rw-r--r--   0        0        0      204 2023-04-15 21:26:39.145454 pyworxcloud-3.1.0/pyworxcloud/day_map.py
--rw-r--r--   0        0        0     3647 2023-04-15 21:26:39.145454 pyworxcloud-3.1.0/pyworxcloud/events.py
--rw-r--r--   0        0        0     1756 2023-04-15 21:26:39.145454 pyworxcloud-3.1.0/pyworxcloud/exceptions.py
--rw-r--r--   0        0        0      204 2023-04-15 21:26:39.145454 pyworxcloud-3.1.0/pyworxcloud/helpers/__init__.py
--rw-r--r--   0        0        0      637 2023-04-15 21:26:39.145454 pyworxcloud-3.1.0/pyworxcloud/helpers/logger.py
--rw-r--r--   0        0        0     2794 2023-04-15 21:26:39.145454 pyworxcloud-3.1.0/pyworxcloud/helpers/time_format.py
--rw-r--r--   0        0        0      838 2023-04-15 21:26:39.145454 pyworxcloud-3.1.0/pyworxcloud/utils/__init__.py
--rw-r--r--   0        0        0     3338 2023-04-15 21:26:39.145454 pyworxcloud-3.1.0/pyworxcloud/utils/battery.py
--rw-r--r--   0        0        0     2091 2023-04-15 21:26:39.145454 pyworxcloud-3.1.0/pyworxcloud/utils/blades.py
--rw-r--r--   0        0        0     1924 2023-04-15 21:26:39.145454 pyworxcloud-3.1.0/pyworxcloud/utils/capability.py
--rw-r--r--   0        0        0     3838 2023-04-15 21:26:39.145454 pyworxcloud-3.1.0/pyworxcloud/utils/devices.py
--rw-r--r--   0        0        0      617 2023-04-15 21:26:39.145454 pyworxcloud-3.1.0/pyworxcloud/utils/firmware.py
--rw-r--r--   0        0        0      281 2023-04-15 21:26:39.145454 pyworxcloud-3.1.0/pyworxcloud/utils/landroid_class.py
--rw-r--r--   0        0        0      306 2023-04-15 21:26:39.145454 pyworxcloud-3.1.0/pyworxcloud/utils/lawn.py
--rw-r--r--   0        0        0      427 2023-04-15 21:26:39.149454 pyworxcloud-3.1.0/pyworxcloud/utils/location.py
--rw-r--r--   0        0        0     6150 2023-04-15 21:26:39.149454 pyworxcloud-3.1.0/pyworxcloud/utils/mqtt.py
--rw-r--r--   0        0        0      411 2023-04-15 21:26:39.149454 pyworxcloud-3.1.0/pyworxcloud/utils/orientation.py
--rw-r--r--   0        0        0     1348 2023-04-15 21:26:39.149454 pyworxcloud-3.1.0/pyworxcloud/utils/product.py
--rw-r--r--   0        0        0     1109 2023-04-15 21:26:39.149454 pyworxcloud-3.1.0/pyworxcloud/utils/rainsensor.py
--rw-r--r--   0        0        0     2410 2023-04-15 21:26:39.149454 pyworxcloud-3.1.0/pyworxcloud/utils/requests.py
--rw-r--r--   0        0        0     6375 2023-04-15 21:26:39.149454 pyworxcloud-3.1.0/pyworxcloud/utils/schedules.py
--rw-r--r--   0        0        0     2050 2023-04-15 21:26:39.149454 pyworxcloud-3.1.0/pyworxcloud/utils/state.py
--rw-r--r--   0        0        0      657 2023-04-15 21:26:39.149454 pyworxcloud-3.1.0/pyworxcloud/utils/statistics.py
--rw-r--r--   0        0        0      726 2023-04-15 21:26:39.149454 pyworxcloud-3.1.0/pyworxcloud/utils/warranty.py
--rw-r--r--   0        0        0     1423 2023-04-15 21:26:39.149454 pyworxcloud-3.1.0/pyworxcloud/utils/zone.py
--rw-r--r--   0        0        0     1698 1970-01-01 00:00:00.000000 pyworxcloud-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-17 09:16:55.398923 pyworxcloud-3.1.1/LICENSE
+-rw-r--r--   0        0        0      929 2023-04-17 09:16:55.398923 pyworxcloud-3.1.1/README.md
+-rw-r--r--   0        0        0      610 2023-04-17 09:17:10.387114 pyworxcloud-3.1.1/pyproject.toml
+-rw-r--r--   0        0        0    28745 2023-04-17 09:16:55.398923 pyworxcloud-3.1.1/pyworxcloud/__init__.py
+-rw-r--r--   0        0        0     3751 2023-04-17 09:16:55.398923 pyworxcloud-3.1.1/pyworxcloud/api.py
+-rw-r--r--   0        0        0     1134 2023-04-17 09:16:55.398923 pyworxcloud-3.1.1/pyworxcloud/clouds.py
+-rw-r--r--   0        0        0      927 2023-04-17 09:16:55.398923 pyworxcloud-3.1.1/pyworxcloud/const.py
+-rw-r--r--   0        0        0      204 2023-04-17 09:16:55.398923 pyworxcloud-3.1.1/pyworxcloud/day_map.py
+-rw-r--r--   0        0        0     3647 2023-04-17 09:16:55.398923 pyworxcloud-3.1.1/pyworxcloud/events.py
+-rw-r--r--   0        0        0     1826 2023-04-17 09:16:55.398923 pyworxcloud-3.1.1/pyworxcloud/exceptions.py
+-rw-r--r--   0        0        0      204 2023-04-17 09:16:55.398923 pyworxcloud-3.1.1/pyworxcloud/helpers/__init__.py
+-rw-r--r--   0        0        0      637 2023-04-17 09:16:55.398923 pyworxcloud-3.1.1/pyworxcloud/helpers/logger.py
+-rw-r--r--   0        0        0     2794 2023-04-17 09:16:55.398923 pyworxcloud-3.1.1/pyworxcloud/helpers/time_format.py
+-rw-r--r--   0        0        0      838 2023-04-17 09:16:55.398923 pyworxcloud-3.1.1/pyworxcloud/utils/__init__.py
+-rw-r--r--   0        0        0     3338 2023-04-17 09:16:55.398923 pyworxcloud-3.1.1/pyworxcloud/utils/battery.py
+-rw-r--r--   0        0        0     2091 2023-04-17 09:16:55.398923 pyworxcloud-3.1.1/pyworxcloud/utils/blades.py
+-rw-r--r--   0        0        0     1924 2023-04-17 09:16:55.398923 pyworxcloud-3.1.1/pyworxcloud/utils/capability.py
+-rw-r--r--   0        0        0     3838 2023-04-17 09:16:55.398923 pyworxcloud-3.1.1/pyworxcloud/utils/devices.py
+-rw-r--r--   0        0        0      617 2023-04-17 09:16:55.402922 pyworxcloud-3.1.1/pyworxcloud/utils/firmware.py
+-rw-r--r--   0        0        0      281 2023-04-17 09:16:55.402922 pyworxcloud-3.1.1/pyworxcloud/utils/landroid_class.py
+-rw-r--r--   0        0        0      306 2023-04-17 09:16:55.402922 pyworxcloud-3.1.1/pyworxcloud/utils/lawn.py
+-rw-r--r--   0        0        0      427 2023-04-17 09:16:55.402922 pyworxcloud-3.1.1/pyworxcloud/utils/location.py
+-rw-r--r--   0        0        0     7538 2023-04-17 09:16:55.402922 pyworxcloud-3.1.1/pyworxcloud/utils/mqtt.py
+-rw-r--r--   0        0        0      411 2023-04-17 09:16:55.402922 pyworxcloud-3.1.1/pyworxcloud/utils/orientation.py
+-rw-r--r--   0        0        0     1348 2023-04-17 09:16:55.402922 pyworxcloud-3.1.1/pyworxcloud/utils/product.py
+-rw-r--r--   0        0        0     1109 2023-04-17 09:16:55.402922 pyworxcloud-3.1.1/pyworxcloud/utils/rainsensor.py
+-rw-r--r--   0        0        0     2410 2023-04-17 09:16:55.402922 pyworxcloud-3.1.1/pyworxcloud/utils/requests.py
+-rw-r--r--   0        0        0     6375 2023-04-17 09:16:55.402922 pyworxcloud-3.1.1/pyworxcloud/utils/schedules.py
+-rw-r--r--   0        0        0     2050 2023-04-17 09:16:55.402922 pyworxcloud-3.1.1/pyworxcloud/utils/state.py
+-rw-r--r--   0        0        0      657 2023-04-17 09:16:55.402922 pyworxcloud-3.1.1/pyworxcloud/utils/statistics.py
+-rw-r--r--   0        0        0      726 2023-04-17 09:16:55.402922 pyworxcloud-3.1.1/pyworxcloud/utils/warranty.py
+-rw-r--r--   0        0        0     1423 2023-04-17 09:16:55.402922 pyworxcloud-3.1.1/pyworxcloud/utils/zone.py
+-rw-r--r--   0        0        0     1698 1970-01-01 00:00:00.000000 pyworxcloud-3.1.1/PKG-INFO
```

### Comparing `pyworxcloud-3.1.0/LICENSE` & `pyworxcloud-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.0/README.md` & `pyworxcloud-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.0/pyproject.toml` & `pyworxcloud-3.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pyworxcloud"
-version = "v3.1.0"
+version = "v3.1.1"
 description = "Landroid cloud (Positec) API library"
 authors = ["Malene Trab <malene@trab.dk>"]
 documentation = "https://github.com/mtrab/pyworxcloud"
 classifiers = [
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
```

### Comparing `pyworxcloud-3.1.0/pyworxcloud/__init__.py` & `pyworxcloud-3.1.1/pyworxcloud/__init__.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.0/pyworxcloud/api.py` & `pyworxcloud-3.1.1/pyworxcloud/api.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.0/pyworxcloud/clouds.py` & `pyworxcloud-3.1.1/pyworxcloud/clouds.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.0/pyworxcloud/const.py` & `pyworxcloud-3.1.1/pyworxcloud/const.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.0/pyworxcloud/events.py` & `pyworxcloud-3.1.1/pyworxcloud/events.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.0/pyworxcloud/exceptions.py` & `pyworxcloud-3.1.1/pyworxcloud/exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,14 +35,18 @@
 
     def __init__(self, message):
         """Custom ratelimit exception class"""
         super(RateLimit, self).__init__(message)
         self.message = message
 
 
+class MQTTException(Exception):
+    """Defines a MQTT exception."""
+
+
 # Exception classes for URL requests
 class RequestError(Exception):
     """Define a bad request error (400)."""
 
 
 class AuthorizationError(Exception):
     """Represents an authorization error (401)."""
```

### Comparing `pyworxcloud-3.1.0/pyworxcloud/helpers/logger.py` & `pyworxcloud-3.1.1/pyworxcloud/helpers/logger.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.0/pyworxcloud/helpers/time_format.py` & `pyworxcloud-3.1.1/pyworxcloud/helpers/time_format.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.0/pyworxcloud/utils/__init__.py` & `pyworxcloud-3.1.1/pyworxcloud/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.0/pyworxcloud/utils/battery.py` & `pyworxcloud-3.1.1/pyworxcloud/utils/battery.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.0/pyworxcloud/utils/blades.py` & `pyworxcloud-3.1.1/pyworxcloud/utils/blades.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.0/pyworxcloud/utils/capability.py` & `pyworxcloud-3.1.1/pyworxcloud/utils/capability.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.0/pyworxcloud/utils/devices.py` & `pyworxcloud-3.1.1/pyworxcloud/utils/devices.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.0/pyworxcloud/utils/firmware.py` & `pyworxcloud-3.1.1/pyworxcloud/utils/firmware.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.0/pyworxcloud/utils/mqtt.py` & `pyworxcloud-3.1.1/pyworxcloud/utils/mqtt.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,19 +7,23 @@
 import urllib.parse
 from datetime import datetime
 from logging import Logger
 from typing import Any
 from uuid import uuid4
 
 import paho.mqtt.client as mqtt
-from paho.mqtt.client import connack_string
+from paho.mqtt.client import connack_string, error_string
 
-from ..events import EventHandler
+from ..exceptions import MQTTException
+
+from ..events import EventHandler, LandroidEvent
 from .landroid_class import LDict
 
+QOS_FLAG = 1
+
 
 class MQTTMsgType(LDict):
     """Define specific message type data."""
 
     def __init__(self) -> dict:
         super().__init__()
 
@@ -93,37 +97,44 @@
         """Initialize AWSIoT MQTT handler."""
         super().__init__()
         # self.client = None
         self._events = EventHandler()
         self._on_update = callback
         self._endpoint = endpoint
         self._log = logger.getChild("MQTT")
-
-        self.connected: bool | None = None
+        self._disconnected = False
+        self._topic: list = []
 
         accesstokenparts = token.replace("_", "/").replace("-", "+").split(".")
 
         self._uuid = uuid4()
 
         self.client = mqtt.Client(
             client_id=f"{brandprefix}/USER/{user_id}/bot/{self._uuid}",
             clean_session=False,
             userdata=None,
+            reconnect_on_failure=True,
         )
         self.client.username_pw_set(
             username=f"bot?jwt={urllib.parse.quote(accesstokenparts[0])}.{urllib.parse.quote(accesstokenparts[1])}&x-amz-customauthorizer-name=''&x-amz-customauthorizer-signature={urllib.parse.quote(accesstokenparts[2])}",
             password=None,
         )
 
         ssl_context = ssl.create_default_context()
         ssl_context.set_alpn_protocols(["mqtt"])
         self.client.tls_set_context(context=ssl_context)
 
         self.client.on_connect = self._on_connect
         self.client.on_message = self._forward_on_message
+        self.client.on_disconnect = self._on_disconnect
+
+    @property
+    def connected(self) -> bool:
+        """Returns the MQTT connection state."""
+        return self.client.is_connected()
 
     def _forward_on_message(
         self,
         client: mqtt.Client | None,
         userdata: Any | None,
         message: Any | None,
         properties: Any | None = None,  # pylint: disable=unused-argument
@@ -131,15 +142,16 @@
         """MQTT callback method definition."""
         msg = message.payload.decode("utf-8")
         self._log.debug("Received MQTT message:\n%s", msg)
         self._on_update(msg)
 
     def subscribe(self, topic: str) -> None:
         """Subscribe to MQTT updates."""
-        self.client.subscribe(topic=topic)
+        self._topic.append(topic)
+        self.client.subscribe(topic=topic, qos=QOS_FLAG)
 
     def connect(self) -> None:
         """Connect to the MQTT service."""
         self.client.connect(self._endpoint, 443, 45)
         self.client.loop_start()
 
     def _on_connect(
@@ -149,50 +161,80 @@
         flags: Any | None,
         rc: int | None,
         properties: Any | None = None,  # pylint: disable=unused-argument,invalid-name
     ) -> None:
         """MQTT callback method."""
         self._log.debug(connack_string(rc))
         if rc == 0:
-            self.connected = True
+            self._disconnected = False
             self._log.debug("MQTT connected")
+            self._events.call(
+                LandroidEvent.MQTT_CONNECTION, state=self.client.is_connected()
+            )
         else:
-            self.connected = False
             self._log.debug("MQTT connection failed")
+            self._events.call(
+                LandroidEvent.MQTT_CONNECTION, state=self.client.is_connected()
+            )
+
+    def _on_disconnect(
+        self,
+        client: mqtt.Client | None,
+        userdata: Any | None,
+        rc: int | None,
+        properties: Any | None = None,  # pylint: disable=unused-argument,invalid-name
+    ) -> None:
+        """MQTT callback method."""
+        logger = self._log.getChild("mqtt.disconnected")
+        if rc > 0:
+            if rc == 7:
+                if not self.client.is_connected():
+                    raise MQTTException(
+                        "Unexpected MQTT disconnect - were you perhaps banned?"
+                    )
+            if self.client.is_connected():
+                logger.debug("MQTT connection was lost! (%s)", error_string(rc))
+
+            logger.debug(
+                "Setting MQTT connected flag FALSE and unsubscribing from topics"
+            )
+
+            self._events.call(
+                LandroidEvent.MQTT_CONNECTION, state=self.client.is_connected()
+            )
+
+            for topic in self._topic:
+                client.unsubscribe(self._topic.pop(topic))
 
     def disconnect(
         self, reasoncode=None, properties=None  # pylint: disable=unused-argument
     ):
         """Disconnect from AWSIoT MQTT server."""
+        self._disconnected = True
+        self.client.loop_stop()
         self.client.disconnect()
-        # self._configuration.disconnect()
 
     def ping(self, serial_number: str, topic: str) -> None:
         """Ping (update) the mower."""
         cmd = self.format_message(serial_number, {"cmd": Command.FORCE_REFRESH})
         self._log.debug("Sending '%s' on topic '%s'", cmd, topic)
-        self.client.publish(topic, cmd, 0)
-        # self._configuration.publish(topic, cmd, mqtt.QoS.AT_LEAST_ONCE)
+        self.client.publish(topic, cmd, QOS_FLAG)
 
     def command(self, serial_number: str, topic: str, action: Command) -> None:
         """Send a specific command to the mower."""
         cmd = self.format_message(serial_number, {"cmd": action})
         self._log.debug("Sending '%s' on topic '%s'", cmd, topic)
-        self.client.publish(topic, cmd, 0)
-        # self._configuration.publish(topic, cmd, mqtt.QoS.AT_LEAST_ONCE)
+        self.client.publish(topic, cmd, QOS_FLAG)
 
     def publish(self, serial_number: str, topic: str, message: dict) -> None:
         """Publish message to the mower."""
         self._log.debug("Publishing message '%s'", message)
-        self.client.publish(topic, self.format_message(serial_number, message), 0)
-        # self._configuration.publish(
-        #     topic,
-        #     self.format_message(serial_number, message),
-        #     mqtt.QoS.AT_LEAST_ONCE,
-        # )
+        self.client.publish(
+            topic, self.format_message(serial_number, message), QOS_FLAG
+        )
 
     def format_message(self, serial_number: str, message: dict) -> str:
         """
         Format a message.
         Message is expected to be a dict like this: {"cmd": 1}
         """
         now = datetime.now()
```

### Comparing `pyworxcloud-3.1.0/pyworxcloud/utils/product.py` & `pyworxcloud-3.1.1/pyworxcloud/utils/product.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.0/pyworxcloud/utils/rainsensor.py` & `pyworxcloud-3.1.1/pyworxcloud/utils/rainsensor.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.0/pyworxcloud/utils/requests.py` & `pyworxcloud-3.1.1/pyworxcloud/utils/requests.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.0/pyworxcloud/utils/schedules.py` & `pyworxcloud-3.1.1/pyworxcloud/utils/schedules.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.0/pyworxcloud/utils/state.py` & `pyworxcloud-3.1.1/pyworxcloud/utils/state.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.0/pyworxcloud/utils/statistics.py` & `pyworxcloud-3.1.1/pyworxcloud/utils/statistics.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.0/pyworxcloud/utils/warranty.py` & `pyworxcloud-3.1.1/pyworxcloud/utils/warranty.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.0/pyworxcloud/utils/zone.py` & `pyworxcloud-3.1.1/pyworxcloud/utils/zone.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.0/PKG-INFO` & `pyworxcloud-3.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyworxcloud
-Version: 3.1.0
+Version: 3.1.1
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
-Metadata-Version: 2.1 Name: pyworxcloud Version: 3.1.0 Summary: Landroid cloud
+Metadata-Version: 2.1 Name: pyworxcloud Version: 3.1.1 Summary: Landroid cloud
 (Positec) API library License: MIT Author: Malene Trab Author-email:
 malene@trab.dk Requires-Python: >=3.10,<4.0 Classifier: License :: OSI Approved
 :: MIT License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Topic :: Software Development :: Libraries :: Python
 Modules Requires-Dist: paho-mqtt (>=1.6.1,<2.0.0) Requires-Dist: requests
 (>=2.26.0,<3.0.0) Requires-Dist: urllib3 (>=1.26.10,<2.0.0) Project-URL: Bug
```

