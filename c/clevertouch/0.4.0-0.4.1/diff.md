# Comparing `tmp/clevertouch-0.4.0.tar.gz` & `tmp/clevertouch-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clevertouch-0.4.0.tar", last modified: Sun Apr 16 12:47:19 2023, max compression
+gzip compressed data, was "clevertouch-0.4.1.tar", last modified: Mon Apr 17 17:34:54 2023, max compression
```

## Comparing `clevertouch-0.4.0.tar` & `clevertouch-0.4.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1064 2023-01-24 14:28:50.216215 clevertouch-0.4.0/LICENSE
--rw-r--r--   0        0        0     5073 2023-03-13 13:06:21.888575 clevertouch-0.4.0/README.md
--rw-r--r--   0        0        0     1022 2023-04-16 12:46:43.653638 clevertouch-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      183 2023-01-31 10:59:22.202682 clevertouch-0.4.0/src/clevertouch/__init__.py
--rw-r--r--   0        0        0     6679 2023-03-13 13:06:21.888575 clevertouch-0.4.0/src/clevertouch/api.py
--rw-r--r--   0        0        0      206 2023-03-09 11:16:19.367070 clevertouch-0.4.0/src/clevertouch/devices/__init__.py
--rw-r--r--   0        0        0      373 2023-03-13 13:06:21.888575 clevertouch-0.4.0/src/clevertouch/devices/const.py
--rw-r--r--   0        0        0     1193 2023-03-09 11:33:26.233110 clevertouch-0.4.0/src/clevertouch/devices/device.py
--rw-r--r--   0        0        0      900 2023-03-13 13:06:21.888575 clevertouch-0.4.0/src/clevertouch/devices/factory.py
--rw-r--r--   0        0        0     2023 2023-03-09 11:13:52.013655 clevertouch-0.4.0/src/clevertouch/devices/onoff.py
--rw-r--r--   0        0        0    11703 2023-04-15 06:05:19.193436 clevertouch-0.4.0/src/clevertouch/devices/radiator.py
--rw-r--r--   0        0        0     1522 2023-01-31 10:59:22.206682 clevertouch-0.4.0/src/clevertouch/info.py
--rw-r--r--   0        0        0     4214 2023-03-13 13:06:21.888575 clevertouch-0.4.0/src/clevertouch/objects.py
--rw-r--r--   0        0        0      836 2023-01-31 10:59:22.206682 clevertouch-0.4.0/src/clevertouch/util.py
--rw-r--r--   0        0        0       37 2023-01-24 22:11:22.095324 clevertouch-0.4.0/tests/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2023-01-24 22:11:22.095324 clevertouch-0.4.0/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2023-01-24 22:11:22.095324 clevertouch-0.4.0/tests/.pytest_cache/README.md
--rw-r--r--   0        0        0      103 2023-01-24 22:34:04.437950 clevertouch-0.4.0/tests/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      128 2023-01-24 22:34:04.437950 clevertouch-0.4.0/tests/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2023-01-24 22:34:04.437950 clevertouch-0.4.0/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0     1109 2023-01-31 10:59:22.206682 clevertouch-0.4.0/tests/authenticate_test.py
--rw-r--r--   0        0        0     5684 1970-01-01 00:00:00.000000 clevertouch-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-01-24 14:28:50.216215 clevertouch-0.4.1/LICENSE
+-rw-r--r--   0        0        0     5073 2023-03-13 13:06:21.888575 clevertouch-0.4.1/README.md
+-rw-r--r--   0        0        0     1022 2023-04-17 17:34:19.229298 clevertouch-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      183 2023-01-31 10:59:22.202682 clevertouch-0.4.1/src/clevertouch/__init__.py
+-rw-r--r--   0        0        0     6679 2023-03-13 13:06:21.888575 clevertouch-0.4.1/src/clevertouch/api.py
+-rw-r--r--   0        0        0      206 2023-03-09 11:16:19.367070 clevertouch-0.4.1/src/clevertouch/devices/__init__.py
+-rw-r--r--   0        0        0      373 2023-03-13 13:06:21.888575 clevertouch-0.4.1/src/clevertouch/devices/const.py
+-rw-r--r--   0        0        0     1193 2023-03-09 11:33:26.233110 clevertouch-0.4.1/src/clevertouch/devices/device.py
+-rw-r--r--   0        0        0      900 2023-03-13 13:06:21.888575 clevertouch-0.4.1/src/clevertouch/devices/factory.py
+-rw-r--r--   0        0        0     2023 2023-03-09 11:13:52.013655 clevertouch-0.4.1/src/clevertouch/devices/onoff.py
+-rw-r--r--   0        0        0    11467 2023-04-17 16:09:12.862617 clevertouch-0.4.1/src/clevertouch/devices/radiator.py
+-rw-r--r--   0        0        0     1522 2023-01-31 10:59:22.206682 clevertouch-0.4.1/src/clevertouch/info.py
+-rw-r--r--   0        0        0     4214 2023-03-13 13:06:21.888575 clevertouch-0.4.1/src/clevertouch/objects.py
+-rw-r--r--   0        0        0      836 2023-01-31 10:59:22.206682 clevertouch-0.4.1/src/clevertouch/util.py
+-rw-r--r--   0        0        0       37 2023-01-24 22:11:22.095324 clevertouch-0.4.1/tests/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2023-01-24 22:11:22.095324 clevertouch-0.4.1/tests/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2023-01-24 22:11:22.095324 clevertouch-0.4.1/tests/.pytest_cache/README.md
+-rw-r--r--   0        0        0      103 2023-01-24 22:34:04.437950 clevertouch-0.4.1/tests/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      128 2023-01-24 22:34:04.437950 clevertouch-0.4.1/tests/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2023-01-24 22:34:04.437950 clevertouch-0.4.1/tests/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0     1109 2023-01-31 10:59:22.206682 clevertouch-0.4.1/tests/authenticate_test.py
+-rw-r--r--   0        0        0     5684 1970-01-01 00:00:00.000000 clevertouch-0.4.1/PKG-INFO
```

### Comparing `clevertouch-0.4.0/LICENSE` & `clevertouch-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clevertouch-0.4.0/README.md` & `clevertouch-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `clevertouch-0.4.0/pyproject.toml` & `clevertouch-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 [tool.pytest.ini_options]
 log_cli = 1
 log_cli_level = "DEBUG"
 
 [project]
 name = "clevertouch"
-version = "0.4.0"
+version = "0.4.1"
 description = "A Python API for interacting with LVI/Purmo Touch E3-connected radiators"
 keywords = [
     "LVI",
     "home automation",
     "heating",
 ]
 authors = [
```

### Comparing `clevertouch-0.4.0/src/clevertouch/api.py` & `clevertouch-0.4.1/src/clevertouch/api.py`

 * *Files identical despite different names*

### Comparing `clevertouch-0.4.0/src/clevertouch/devices/device.py` & `clevertouch-0.4.1/src/clevertouch/devices/device.py`

 * *Files identical despite different names*

### Comparing `clevertouch-0.4.0/src/clevertouch/devices/factory.py` & `clevertouch-0.4.1/src/clevertouch/devices/factory.py`

 * *Files identical despite different names*

### Comparing `clevertouch-0.4.0/src/clevertouch/devices/onoff.py` & `clevertouch-0.4.1/src/clevertouch/devices/onoff.py`

 * *Files identical despite different names*

### Comparing `clevertouch-0.4.0/src/clevertouch/devices/radiator.py` & `clevertouch-0.4.1/src/clevertouch/devices/radiator.py`

 * *Files 3% similar despite different names*

```diff
@@ -143,33 +143,26 @@
             if self.temp_type == TempType.NONE
             else self.temperatures[self.temp_type].device,
             is_writable=False,
             name=TempType.TARGET,
         )
         # Read boost settings
         # 'boost_time' is the user writable boost time
-        try:
-            self.boost_time = int(data["time_boost"])
-        except KeyError:  # The key doesn't exist
-            self.boost_time = 0
-        except ValueError:  # The value can not be converted to an int
-            self.boost_time = 0
+        self.boost_time = int(data.get("time_boost") or 0)
         # 'time_boost_format_chrono' holds remaining boost time with higher resolution
-        try:
-            node = data["time_boost_format_chrono"]
+        node = data.get("time_boost_format_chrono")
+        if node:
             self.boost_remaining = (
-                int(node["d"]) * 24 * 60 * 60
-                + int(node["h"]) * 60 * 60
-                + int(node["m"]) * 60
-                + int(node["s"])
+                int(node.get("d") or 0) * 24 * 60 * 60
+                + int(node.get("h") or 0) * 60 * 60
+                + int(node.get("m") or 0) * 60
+                + int(node.get("s") or 0)
             )
-        except KeyError:
-            self.boost_remaining = 0
-        except ValueError:
-            self.boost_remaining = 0
+        else:
+            self.boost_remaining = None
 
     async def set_temperature(self, temp_type: str, temp_value: float, unit: str):
         """Set a specific temperature for a radiator"""
         if temp_type not in self._TEMP_TYPE_TO_DEVICE:
             raise ApiError(f"Temperature {temp_type} not available.")
         elif temp_type in self._READONLY_TEMP_TYPES:
             raise ApiError(f"Temperature {temp_type} is read-only.")
@@ -248,27 +241,27 @@
         Raises:
         ApiError
             If any of the arguments are invalid or incompatible.
         """
 
         if heat_mode not in self._HEAT_MODE_TO_DEVICE:
             raise ApiError(f"Heating mode {heat_mode} not available.")
-        if (temp_value or temp_unit) and (not temp_value or not temp_unit):
-            raise ApiError("Both temp value and unit must be set.")
+        if temp_value and not temp_unit:
+            raise ApiError("Unit must be set when a temp value is provided.")
         if temp_value and heat_mode not in self._HEAT_MODE_TO_WRITABLE_TEMP_TYPE:
             raise ApiError(f"Temperature can not be set for {heat_mode}.")
         if boost_time and heat_mode != HeatMode.BOOST:
             raise ApiError("Boost time can only be set for boost mode.")
 
         query_params = {}
         query_params["id_device"] = self.id_local
         query_params["gv_mode"] = self._HEAT_MODE_TO_DEVICE[heat_mode]
         query_params["nv_mode"] = self._HEAT_MODE_TO_DEVICE[heat_mode]
 
-        if temp_value:
+        if temp_value and temp_unit:
             temp_type = self._HEAT_MODE_TO_WRITABLE_TEMP_TYPE[heat_mode]
             new_temp = Temperature(
                 temp_value, temp_unit, is_writable=True, name=temp_type
             )
             query_params[self._TEMP_TYPE_TO_DEVICE[temp_type]] = new_temp.device
             # Debatable - see set_temperature
             self.temperatures[temp_type] = new_temp
```

### Comparing `clevertouch-0.4.0/src/clevertouch/info.py` & `clevertouch-0.4.1/src/clevertouch/info.py`

 * *Files identical despite different names*

### Comparing `clevertouch-0.4.0/src/clevertouch/objects.py` & `clevertouch-0.4.1/src/clevertouch/objects.py`

 * *Files identical despite different names*

### Comparing `clevertouch-0.4.0/src/clevertouch/util.py` & `clevertouch-0.4.1/src/clevertouch/util.py`

 * *Files identical despite different names*

### Comparing `clevertouch-0.4.0/tests/authenticate_test.py` & `clevertouch-0.4.1/tests/authenticate_test.py`

 * *Files identical despite different names*

### Comparing `clevertouch-0.4.0/PKG-INFO` & `clevertouch-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clevertouch
-Version: 0.4.0
+Version: 0.4.1
 Summary: A Python API for interacting with LVI/Purmo Touch E3-connected radiators
 License: MIT
 Keywords: LVI,home automation,heating
 Author-email: hemphen <michael.hemph@gmail.com>
 Requires-Python: >=3.8
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

