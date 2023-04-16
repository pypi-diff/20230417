# Comparing `tmp/mqtt-entity-0.0.1.tar.gz` & `tmp/mqtt-entity-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mqtt-entity-0.0.1.tar", last modified: Sat Apr 15 20:42:40 2023, max compression
+gzip compressed data, was "mqtt-entity-0.0.2.tar", last modified: Sun Apr 16 22:23:41 2023, max compression
```

## Comparing `mqtt-entity-0.0.1.tar` & `mqtt-entity-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 20:42:40.072272 mqtt-entity-0.0.1/
--rw-rw-rw-   0        0        0     1073 2023-01-01 19:33:39.000000 mqtt-entity-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       85 2023-04-15 20:19:26.000000 mqtt-entity-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1700 2023-04-15 20:42:40.073278 mqtt-entity-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      913 2023-04-15 20:42:35.000000 mqtt-entity-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-15 20:42:40.038272 mqtt-entity-0.0.1/mqtt_entity/
--rw-rw-rw-   0        0        0      249 2023-04-15 20:25:17.000000 mqtt-entity-0.0.1/mqtt_entity/__init__.py
--rw-rw-rw-   0        0        0     7453 2023-04-15 20:32:06.000000 mqtt-entity-0.0.1/mqtt_entity/client.py
--rw-rw-rw-   0        0        0     4834 2023-04-15 20:32:20.000000 mqtt-entity-0.0.1/mqtt_entity/entities.py
--rw-rw-rw-   0        0        0      287 2023-04-15 16:27:56.000000 mqtt-entity-0.0.1/mqtt_entity/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-15 20:42:40.061275 mqtt-entity-0.0.1/mqtt_entity.egg-info/
--rw-rw-rw-   0        0        0     1700 2023-04-15 20:42:39.000000 mqtt-entity-0.0.1/mqtt_entity.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      382 2023-04-15 20:42:39.000000 mqtt-entity-0.0.1/mqtt_entity.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 20:42:39.000000 mqtt-entity-0.0.1/mqtt_entity.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      129 2023-04-15 20:42:39.000000 mqtt-entity-0.0.1/mqtt_entity.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-15 20:42:39.000000 mqtt-entity-0.0.1/mqtt_entity.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-04-15 20:19:34.000000 mqtt-entity-0.0.1/mqtt_entity.egg-info/zip-safe
--rw-rw-rw-   0        0        0     1343 2023-04-15 20:42:40.076274 mqtt-entity-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      124 2023-04-15 20:19:27.000000 mqtt-entity-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-15 20:42:40.068273 mqtt-entity-0.0.1/tests/
--rw-rw-rw-   0        0        0     1179 2023-04-15 18:18:13.000000 mqtt-entity-0.0.1/tests/conftest.py
--rw-rw-rw-   0        0        0     5693 2023-04-15 20:25:17.000000 mqtt-entity-0.0.1/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:41.242721 mqtt-entity-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-16 22:23:32.000000 mqtt-entity-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-16 22:23:32.000000 mqtt-entity-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-16 22:23:41.242721 mqtt-entity-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-16 22:23:32.000000 mqtt-entity-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:41.242721 mqtt-entity-0.0.2/mqtt_entity/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-16 22:23:32.000000 mqtt-entity-0.0.2/mqtt_entity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7453 2023-04-16 22:23:32.000000 mqtt-entity-0.0.2/mqtt_entity/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-04-16 22:23:32.000000 mqtt-entity-0.0.2/mqtt_entity/entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-16 22:23:32.000000 mqtt-entity-0.0.2/mqtt_entity/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-16 22:23:32.000000 mqtt-entity-0.0.2/mqtt_entity/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:41.242721 mqtt-entity-0.0.2/mqtt_entity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-16 22:23:41.000000 mqtt-entity-0.0.2/mqtt_entity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-16 22:23:41.000000 mqtt-entity-0.0.2/mqtt_entity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 22:23:41.000000 mqtt-entity-0.0.2/mqtt_entity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-16 22:23:41.000000 mqtt-entity-0.0.2/mqtt_entity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-16 22:23:41.000000 mqtt-entity-0.0.2/mqtt_entity.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 22:23:41.000000 mqtt-entity-0.0.2/mqtt_entity.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-04-16 22:23:41.242721 mqtt-entity-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-16 22:23:32.000000 mqtt-entity-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:41.242721 mqtt-entity-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-16 22:23:32.000000 mqtt-entity-0.0.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-04-16 22:23:32.000000 mqtt-entity-0.0.2/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-04-16 22:23:32.000000 mqtt-entity-0.0.2/tests/test_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-16 22:23:32.000000 mqtt-entity-0.0.2/tests/test_helpers.py
```

### Comparing `mqtt-entity-0.0.1/LICENSE` & `mqtt-entity-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mqtt-entity-0.0.1/PKG-INFO` & `mqtt-entity-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,50 @@
-Metadata-Version: 2.1
-Name: mqtt-entity
-Version: 0.0.1
-Summary: MQTT client to manage Home Assistant entities via MQTT
-Home-page: https://github.com/kellerza/mqtt-entity/
-Author: Johann Kellerman
-Author-email: kellerza@gmail.com
-License: MIT
-Keywords: home-assistant,mqtt,library,discovery,asyncio
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: tests
-License-File: LICENSE
-
-# MQTT Entity helper library for Home Assistant
-
-A Python helper library to manage Home Assistant entities over MQTT.
-
-Features:
-- MQTT entity discovery info (persistent messages)
-- Option to remove persistent discovery info
-- Availability management
-- Manage entities per device
-- Entities modelled as classes
-- Supported entities:
-  - Read-only: Sensor, BinarySensor
-  - Read & write: Select, Switch, Number
-- Asyncio based
-
-MQTTClient based on paho-mqtt.
-
-## Why?
-
-This MQTT code was included in several of my home Assistant addons (SMA-EM / Sunsynk) and finally decided to extract it in a separate library to leverage recent updates & features like discovery removal.
-
-Alternatives options (not based on asyncio)
-- https://pypi.org/project/ha-mqtt-discoverable/
-- https://pypi.org/project/homeassistant-mqtt-binding/
-
-## Credits
-
-@Ivan-L contributed some of the writable entities to the Sunsynk addon project
+Metadata-Version: 2.1
+Name: mqtt-entity
+Version: 0.0.2
+Summary: MQTT client to manage Home Assistant entities via MQTT
+Home-page: https://github.com/kellerza/mqtt-entity/
+Author: Johann Kellerman
+Author-email: kellerza@gmail.com
+License: MIT
+Keywords: home-assistant,mqtt,library,discovery,asyncio
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: tests
+License-File: LICENSE
+
+# MQTT Entity helper library for Home Assistant
+[![codecov](https://codecov.io/gh/kellerza/mqtt_entity/branch/main/graph/badge.svg?token=PG4N1YBUGW)](https://codecov.io/gh/kellerza/mqtt_entity)
+
+A Python helper library to manage Home Assistant entities over MQTT.
+
+Features:
+- MQTT entity discovery info (persistent messages)
+- Option to remove persistent discovery info
+- Availability management
+- Manage entities per device
+- Entities modelled as classes
+- Supported entities:
+  - Read-only: Sensor, BinarySensor
+  - Read & write: Select, Switch, Number
+- Asyncio based
+
+MQTTClient based on paho-mqtt.
+
+## Why?
+
+This MQTT code was included in several of my home Assistant addons (SMA-EM / Sunsynk) and finally decided to extract it in a separate library to leverage recent updates & features like discovery removal.
+
+Alternatives options (not based on asyncio)
+- https://pypi.org/project/ha-mqtt-discoverable/
+- https://pypi.org/project/homeassistant-mqtt-binding/
+
+## Credits
+
+@Ivan-L contributed some of the writable entities to the Sunsynk addon project
```

### Comparing `mqtt-entity-0.0.1/README.md` & `mqtt-entity-0.0.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # MQTT Entity helper library for Home Assistant
+[![codecov](https://codecov.io/gh/kellerza/mqtt_entity/branch/main/graph/badge.svg?token=PG4N1YBUGW)](https://codecov.io/gh/kellerza/mqtt_entity)
 
 A Python helper library to manage Home Assistant entities over MQTT.
 
 Features:
 - MQTT entity discovery info (persistent messages)
 - Option to remove persistent discovery info
 - Availability management
```

### Comparing `mqtt-entity-0.0.1/mqtt_entity/client.py` & `mqtt-entity-0.0.2/mqtt_entity/client.py`

 * *Files identical despite different names*

### Comparing `mqtt-entity-0.0.1/mqtt_entity/entities.py` & `mqtt-entity-0.0.2/mqtt_entity/entities.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 """MQTT entities."""
 import inspect
 import logging
-from typing import Any, Callable, Sequence, Union
+from typing import Any, Callable, Optional, Sequence, Union
 
 import attr
+from attrs import validators
 
 from mqtt_entity.utils import required
 
 _LOGGER = logging.getLogger(__name__)
 
 # pylint: disable=too-few-public-methods, too-many-instance-attributes
 
 
 @attr.define
 class Device:
     """A Home Assistant Device, used to group entities."""
 
-    identifiers: list[Union[str, tuple[str, Any]]] = attr.field(validator=required)
+    identifiers: list[Union[str, tuple[str, Any]]] = attr.field(
+        validator=[validators.instance_of(list), validators.min_len(1)]
+    )
     connections: list[str] = attr.field(factory=list)
     configuration_url: str = attr.field(default="")
     manufacturer: str = attr.field(default="")
     model: str = attr.field(default="")
     name: str = attr.field(default="")
     suggested_area: str = attr.field(default="")
     sw_version: str = attr.field(default="")
@@ -61,14 +64,16 @@
     entity_category: str = attr.field(default="")
     icon: str = attr.field(default="")
 
     _path = ""
 
     def __attrs_post_init__(self) -> None:
         """Init the class."""
+        if not self._path:
+            raise TypeError(f"Do not instantiate {self.__class__.__name__} directly")
         if not self.state_class and self.device_class == "energy":
             self.state_class = "total_increasing"
 
     @property
     def asdict(self) -> dict:
         """Represent the entity as a dictionary, without empty values and defaults."""
 
@@ -102,68 +107,46 @@
     payload_on: str = attr.field(default="ON")
     payload_off: str = attr.field(default="OFF")
 
     _path = "binary_sensor"
 
 
 @attr.define
-class SelectEntity(Entity):
+class RWEntity(Entity):
+    """Read/Write entity base class."""
+
+    command_topic: str = attr.field(
+        default="", validator=(validators.instance_of(str), validators.min_len(2))
+    )
+
+    on_change: Optional[Callable] = attr.field(default=None)
+
+
+@attr.define
+class SelectEntity(RWEntity):
     """A HomeAssistant Select entity."""
 
-    command_topic: str = attr.field(default=None, validator=required)
     options: Sequence[str] = attr.field(default=None, validator=required)
 
-    on_change: Callable = attr.field(default=None)
-
     _path = "select"
 
 
 @attr.define
-class SwitchEntity(Entity):
+class SwitchEntity(RWEntity):
     """A Home Assistant Binary Sensor entity."""
 
     payload_on: Union[str, int] = attr.field(default=1)
     payload_off: Union[str, int] = attr.field(default=0)
-    command_topic: str = attr.field(default=None, validator=required)
 
-    on_change: Callable = attr.field(default=None)
     _path = "switch"
 
 
 @attr.define
-class NumberEntity(Entity):
+class NumberEntity(RWEntity):
     """A HomeAssistant Number entity."""
 
-    command_topic: str = attr.field(default=None, validator=required)
     min: float = attr.field(default=0.0)
     max: float = attr.field(default=100.0)
     mode: str = attr.field(default="auto")
     step: float = attr.field(default=1.0)
 
-    on_change: Callable = attr.field(default=None)
-
     _path = "number"
-
-
-def hass_device_class(*, unit: str) -> str:
-    """Get the HASS device_class from the unit."""
-    return {
-        "W": "power",
-        "kW": "power",
-        "kVA": "apparent_power",
-        "V": "voltage",
-        "kWh": "energy",
-        "kVah": "",  # Not energy
-        "A": "current",
-        "°C": "temperature",
-        "%": "battery",
-    }.get(unit, "")
-
-
-def hass_default_rw_icon(*, unit: str) -> str:
-    """Get the HASS default icon from the unit."""
-    return {
-        "W": "mdi:flash",
-        "V": "mdi:sine-wave",
-        "A": "mdi:current-ac",
-        "%": "mdi:battery-lock",
-    }.get(unit, "")
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mqtt-entity-0.0.1/mqtt_entity.egg-info/PKG-INFO` & `mqtt-entity-0.0.2/mqtt_entity.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,50 @@
-Metadata-Version: 2.1
-Name: mqtt-entity
-Version: 0.0.1
-Summary: MQTT client to manage Home Assistant entities via MQTT
-Home-page: https://github.com/kellerza/mqtt-entity/
-Author: Johann Kellerman
-Author-email: kellerza@gmail.com
-License: MIT
-Keywords: home-assistant,mqtt,library,discovery,asyncio
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: tests
-License-File: LICENSE
-
-# MQTT Entity helper library for Home Assistant
-
-A Python helper library to manage Home Assistant entities over MQTT.
-
-Features:
-- MQTT entity discovery info (persistent messages)
-- Option to remove persistent discovery info
-- Availability management
-- Manage entities per device
-- Entities modelled as classes
-- Supported entities:
-  - Read-only: Sensor, BinarySensor
-  - Read & write: Select, Switch, Number
-- Asyncio based
-
-MQTTClient based on paho-mqtt.
-
-## Why?
-
-This MQTT code was included in several of my home Assistant addons (SMA-EM / Sunsynk) and finally decided to extract it in a separate library to leverage recent updates & features like discovery removal.
-
-Alternatives options (not based on asyncio)
-- https://pypi.org/project/ha-mqtt-discoverable/
-- https://pypi.org/project/homeassistant-mqtt-binding/
-
-## Credits
-
-@Ivan-L contributed some of the writable entities to the Sunsynk addon project
+Metadata-Version: 2.1
+Name: mqtt-entity
+Version: 0.0.2
+Summary: MQTT client to manage Home Assistant entities via MQTT
+Home-page: https://github.com/kellerza/mqtt-entity/
+Author: Johann Kellerman
+Author-email: kellerza@gmail.com
+License: MIT
+Keywords: home-assistant,mqtt,library,discovery,asyncio
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: tests
+License-File: LICENSE
+
+# MQTT Entity helper library for Home Assistant
+[![codecov](https://codecov.io/gh/kellerza/mqtt_entity/branch/main/graph/badge.svg?token=PG4N1YBUGW)](https://codecov.io/gh/kellerza/mqtt_entity)
+
+A Python helper library to manage Home Assistant entities over MQTT.
+
+Features:
+- MQTT entity discovery info (persistent messages)
+- Option to remove persistent discovery info
+- Availability management
+- Manage entities per device
+- Entities modelled as classes
+- Supported entities:
+  - Read-only: Sensor, BinarySensor
+  - Read & write: Select, Switch, Number
+- Asyncio based
+
+MQTTClient based on paho-mqtt.
+
+## Why?
+
+This MQTT code was included in several of my home Assistant addons (SMA-EM / Sunsynk) and finally decided to extract it in a separate library to leverage recent updates & features like discovery removal.
+
+Alternatives options (not based on asyncio)
+- https://pypi.org/project/ha-mqtt-discoverable/
+- https://pypi.org/project/homeassistant-mqtt-binding/
+
+## Credits
+
+@Ivan-L contributed some of the writable entities to the Sunsynk addon project
```

### Comparing `mqtt-entity-0.0.1/tests/conftest.py` & `mqtt-entity-0.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mqtt-entity-0.0.1/tests/test_client.py` & `mqtt-entity-0.0.2/tests/test_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,53 +3,22 @@
 import logging
 from unittest.mock import MagicMock, Mock, patch
 
 import pytest
 
 import mqtt_entity
 from mqtt_entity.client import _mqtt_on_connect
-from mqtt_entity.entities import hass_default_rw_icon, hass_device_class
 
 _LOGGER = logging.getLogger(__name__)
 
 MQTT_HOST = "192.168.1.8"
 MQTT_PASS = "hass123"
 MQTT_USER = "hass"
 
 
-def test_mqtt():
-    """Test MQTT."""
-    assert hass_device_class(unit="kWh") == "energy"
-    assert hass_default_rw_icon(unit="W") == "mdi:flash"
-
-
-def test_mqtt_entity():
-    """Test MQTT."""
-    dev = mqtt_entity.Device(identifiers=["123"])
-
-    ava = mqtt_entity.Availability(topic="/blah")
-
-    ent = mqtt_entity.SensorEntity(
-        name="test1",
-        unique_id="789",
-        device=dev,
-        availability=[ava],
-        state_topic="/test/a",
-    )
-    assert ent.asdict == {
-        "name": "test1",
-        "unique_id": "789",
-        "device": {"identifiers": ["123"]},
-        "availability": [{"topic": "/blah"}],
-        "state_topic": "/test/a",
-    }
-
-    assert ent.topic == "homeassistant/sensor/123/789/config"
-
-
 @pytest.mark.asyncio
 @pytest.mark.mqtt
 async def test_mqtt_server():
     """Test MQTT."""
     mqc = mqtt_entity.MQTTClient()
     mqc.availability_topic = "test/available"
     await mqc.connect(username="hass", password="hass123", host="192.168.1.8")
```

