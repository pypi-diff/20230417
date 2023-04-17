# Comparing `tmp/aiopioneer-0.4.1.tar.gz` & `tmp/aiopioneer-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiopioneer-0.4.1.tar", last modified: Sun Apr  9 09:23:07 2023, max compression
+gzip compressed data, was "aiopioneer-0.4.2.tar", last modified: Mon Apr 17 19:55:52 2023, max compression
```

## Comparing `aiopioneer-0.4.1.tar` & `aiopioneer-0.4.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwx---   0 root         (0) adm          (4)        0 2023-04-09 09:23:07.931850 aiopioneer-0.4.1/
--rw-rw----   0 root         (0) adm          (4)    11357 2022-11-17 13:13:29.000000 aiopioneer-0.4.1/LICENSE
--rw-rw----   0 root         (0) adm          (4)    13768 2023-04-09 09:23:07.933886 aiopioneer-0.4.1/PKG-INFO
--rw-rw----   0 root         (0) adm          (4)    13119 2023-04-07 14:25:01.000000 aiopioneer-0.4.1/README.md
-drwxrwx---   0 root         (0) adm          (4)        0 2023-04-09 09:23:07.551855 aiopioneer-0.4.1/aiopioneer/
--rw-rw----   0 root         (0) adm          (4)       68 2022-11-17 13:13:41.000000 aiopioneer-0.4.1/aiopioneer/__init__.py
--rw-rw----   0 root         (0) adm          (4)     9864 2023-03-11 16:24:54.000000 aiopioneer-0.4.1/aiopioneer/cli.py
--rw-rw----   0 root         (0) adm          (4)    12266 2023-04-09 09:09:39.000000 aiopioneer-0.4.1/aiopioneer/commands.py
--rw-rw----   0 root         (0) adm          (4)    14911 2023-04-09 09:21:39.000000 aiopioneer-0.4.1/aiopioneer/const.py
--rw-rw----   0 root         (0) adm          (4)    43747 2023-04-07 14:25:01.000000 aiopioneer-0.4.1/aiopioneer/param.py
-drwxrwx---   0 root         (0) adm          (4)        0 2023-04-09 09:23:07.901851 aiopioneer-0.4.1/aiopioneer/parsers/
--rw-rw----   0 root         (0) adm          (4)       35 2023-04-07 14:25:01.000000 aiopioneer-0.4.1/aiopioneer/parsers/__init__.py
--rw-rw----   0 root         (0) adm          (4)     3205 2023-04-07 14:25:01.000000 aiopioneer-0.4.1/aiopioneer/parsers/audio.py
--rw-rw----   0 root         (0) adm          (4)       41 2023-04-07 14:25:01.000000 aiopioneer-0.4.1/aiopioneer/parsers/const.py
--rw-rw----   0 root         (0) adm          (4)    20107 2023-04-07 14:25:01.000000 aiopioneer-0.4.1/aiopioneer/parsers/dsp.py
--rw-rw----   0 root         (0) adm          (4)    26292 2023-04-07 14:25:01.000000 aiopioneer-0.4.1/aiopioneer/parsers/information.py
--rw-rw----   0 root         (0) adm          (4)     7566 2023-04-07 14:25:01.000000 aiopioneer-0.4.1/aiopioneer/parsers/parse.py
--rw-rw----   0 root         (0) adm          (4)      630 2023-04-07 14:25:01.000000 aiopioneer-0.4.1/aiopioneer/parsers/response.py
--rw-rw----   0 root         (0) adm          (4)    23791 2023-04-07 14:25:01.000000 aiopioneer-0.4.1/aiopioneer/parsers/settings.py
--rw-rw----   0 root         (0) adm          (4)    15501 2023-04-07 14:25:01.000000 aiopioneer-0.4.1/aiopioneer/parsers/system.py
--rw-rw----   0 root         (0) adm          (4)     3667 2023-04-07 14:25:01.000000 aiopioneer-0.4.1/aiopioneer/parsers/tuner.py
--rw-rw----   0 root         (0) adm          (4)     8753 2023-04-07 14:25:01.000000 aiopioneer-0.4.1/aiopioneer/parsers/video.py
--rw-rw----   0 root         (0) adm          (4)    75319 2023-04-09 09:09:39.000000 aiopioneer-0.4.1/aiopioneer/pioneer_avr.py
--rw-rw----   0 root         (0) adm          (4)     5015 2023-03-29 19:15:30.000000 aiopioneer-0.4.1/aiopioneer/util.py
-drwxrwx---   0 root         (0) adm          (4)        0 2023-04-09 09:23:07.641854 aiopioneer-0.4.1/aiopioneer.egg-info/
--rw-rw----   0 root         (0) adm          (4)    13768 2023-04-09 09:23:07.000000 aiopioneer-0.4.1/aiopioneer.egg-info/PKG-INFO
--rw-rw----   0 root         (0) adm          (4)      670 2023-04-09 09:23:07.000000 aiopioneer-0.4.1/aiopioneer.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) adm          (4)        1 2023-04-09 09:23:07.000000 aiopioneer-0.4.1/aiopioneer.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) adm          (4)       51 2023-04-09 09:23:07.000000 aiopioneer-0.4.1/aiopioneer.egg-info/entry_points.txt
--rw-rw----   0 root         (0) adm          (4)       11 2023-04-09 09:23:07.000000 aiopioneer-0.4.1/aiopioneer.egg-info/top_level.txt
--rw-rw----   0 root         (0) adm          (4)       38 2023-04-09 09:23:07.945261 aiopioneer-0.4.1/setup.cfg
--rw-rw----   0 root         (0) adm          (4)     1100 2023-03-10 20:49:55.000000 aiopioneer-0.4.1/setup.py
+drwxrwx---   0 root         (0) adm          (4)        0 2023-04-17 19:55:52.917482 aiopioneer-0.4.2/
+-rw-rw----   0 root         (0) adm          (4)    11357 2022-11-17 13:13:29.000000 aiopioneer-0.4.2/LICENSE
+-rw-rw----   0 root         (0) adm          (4)    13768 2023-04-17 19:55:52.924227 aiopioneer-0.4.2/PKG-INFO
+-rw-rw----   0 root         (0) adm          (4)    13119 2023-04-07 14:25:01.000000 aiopioneer-0.4.2/README.md
+drwxrwx---   0 root         (0) adm          (4)        0 2023-04-17 19:55:52.637485 aiopioneer-0.4.2/aiopioneer/
+-rw-rw----   0 root         (0) adm          (4)       68 2022-11-17 13:13:41.000000 aiopioneer-0.4.2/aiopioneer/__init__.py
+-rw-rw----   0 root         (0) adm          (4)    10142 2023-04-16 20:13:15.000000 aiopioneer-0.4.2/aiopioneer/cli.py
+-rw-rw----   0 root         (0) adm          (4)    12269 2023-04-16 20:13:15.000000 aiopioneer-0.4.2/aiopioneer/commands.py
+-rw-rw----   0 root         (0) adm          (4)    14927 2023-04-17 19:55:12.000000 aiopioneer-0.4.2/aiopioneer/const.py
+-rw-rw----   0 root         (0) adm          (4)    43845 2023-04-16 20:13:15.000000 aiopioneer-0.4.2/aiopioneer/param.py
+drwxrwx---   0 root         (0) adm          (4)        0 2023-04-17 19:55:52.887482 aiopioneer-0.4.2/aiopioneer/parsers/
+-rw-rw----   0 root         (0) adm          (4)       35 2023-04-07 14:25:01.000000 aiopioneer-0.4.2/aiopioneer/parsers/__init__.py
+-rw-rw----   0 root         (0) adm          (4)     3205 2023-04-07 14:25:01.000000 aiopioneer-0.4.2/aiopioneer/parsers/audio.py
+-rw-rw----   0 root         (0) adm          (4)       41 2023-04-07 14:25:01.000000 aiopioneer-0.4.2/aiopioneer/parsers/const.py
+-rw-rw----   0 root         (0) adm          (4)    20107 2023-04-07 14:25:01.000000 aiopioneer-0.4.2/aiopioneer/parsers/dsp.py
+-rw-rw----   0 root         (0) adm          (4)    26292 2023-04-07 14:25:01.000000 aiopioneer-0.4.2/aiopioneer/parsers/information.py
+-rw-rw----   0 root         (0) adm          (4)     8010 2023-04-16 20:13:15.000000 aiopioneer-0.4.2/aiopioneer/parsers/parse.py
+-rw-rw----   0 root         (0) adm          (4)      630 2023-04-07 14:25:01.000000 aiopioneer-0.4.2/aiopioneer/parsers/response.py
+-rw-rw----   0 root         (0) adm          (4)    23791 2023-04-07 14:25:01.000000 aiopioneer-0.4.2/aiopioneer/parsers/settings.py
+-rw-rw----   0 root         (0) adm          (4)    16160 2023-04-16 20:13:15.000000 aiopioneer-0.4.2/aiopioneer/parsers/system.py
+-rw-rw----   0 root         (0) adm          (4)     3667 2023-04-07 14:25:01.000000 aiopioneer-0.4.2/aiopioneer/parsers/tuner.py
+-rw-rw----   0 root         (0) adm          (4)     8753 2023-04-07 14:25:01.000000 aiopioneer-0.4.2/aiopioneer/parsers/video.py
+-rw-rw----   0 root         (0) adm          (4)    78131 2023-04-16 20:13:15.000000 aiopioneer-0.4.2/aiopioneer/pioneer_avr.py
+-rw-rw----   0 root         (0) adm          (4)     5297 2023-04-16 20:13:15.000000 aiopioneer-0.4.2/aiopioneer/util.py
+drwxrwx---   0 root         (0) adm          (4)        0 2023-04-17 19:55:52.717484 aiopioneer-0.4.2/aiopioneer.egg-info/
+-rw-rw----   0 root         (0) adm          (4)    13768 2023-04-17 19:55:52.000000 aiopioneer-0.4.2/aiopioneer.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) adm          (4)      670 2023-04-17 19:55:52.000000 aiopioneer-0.4.2/aiopioneer.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) adm          (4)        1 2023-04-17 19:55:52.000000 aiopioneer-0.4.2/aiopioneer.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) adm          (4)       51 2023-04-17 19:55:52.000000 aiopioneer-0.4.2/aiopioneer.egg-info/entry_points.txt
+-rw-rw----   0 root         (0) adm          (4)       11 2023-04-17 19:55:52.000000 aiopioneer-0.4.2/aiopioneer.egg-info/top_level.txt
+-rw-rw----   0 root         (0) adm          (4)       38 2023-04-17 19:55:52.934653 aiopioneer-0.4.2/setup.cfg
+-rw-rw----   0 root         (0) adm          (4)     1100 2023-03-10 20:49:55.000000 aiopioneer-0.4.2/setup.py
```

### Comparing `aiopioneer-0.4.1/LICENSE` & `aiopioneer-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.4.1/PKG-INFO` & `aiopioneer-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiopioneer
-Version: 0.4.1
+Version: 0.4.2
 Summary: Asyncio Python library for controlling a Pioneer AVR via its API
 Home-page: https://github.com/crowbarz/aiopioneer.git
 Author: Crowbar Z
 Author-email: crowbarz@outlook.com
 Keywords: pioneer avr asyncio
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
```

### Comparing `aiopioneer-0.4.1/README.md` & `aiopioneer-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.4.1/aiopioneer/cli.py` & `aiopioneer-0.4.2/aiopioneer/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,16 +212,23 @@
             print(f"Executing command {cmd}")
             cur_zone = zone
             if (
                 not isinstance(PIONEER_COMMANDS[cmd], dict)
                 or zone not in PIONEER_COMMANDS[cmd]
             ):
                 cur_zone = "1"
-            prefix = arg if arg else ""
-            await pioneer.send_command(cmd, zone=cur_zone, prefix=prefix)
+            prefix = (suffix := "")
+            if arg:
+                prefix, _, suffix = arg.partition("|")
+            print(
+                f"Sending command {cmd}"
+                + (f", prefix {prefix}" if prefix else "")
+                + (f", suffix {suffix}" if suffix else "")
+            )
+            await pioneer.send_command(cmd, zone=cur_zone, prefix=prefix, suffix=suffix)
         else:
             print(f"ERROR: Unknown command {cmd}")
 
     await pioneer.shutdown()
     return True
```

### Comparing `aiopioneer-0.4.1/aiopioneer/commands.py` & `aiopioneer-0.4.2/aiopioneer/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -284,10 +284,10 @@
     "operation_amp_cursor_return": {"1": "CRT"},
     "operation_amp_audio_parameter": {"1": "ATA"},
     "operation_amp_output_parameter": {"1": "HPA"},
     "operation_amp_video_parameter": {"1": "VPA"},
     "operation_amp_channel_select": {"1": "CLC"},
     "operation_amp_home_menu": {"1": "HM"},
     "operation_amp_key_off": {"1": "KOF"},
-    "set_input_name": {"1": ["1RGB", "RGB"]},
-    "set_default_input_name": {"1": ["0RGB", "RGB"]}
+    "set_source_name": {"1": ["1RGB", "RGB"]},
+    "set_default_source_name": {"1": ["0RGB", "RGB"]},
 }
```

### Comparing `aiopioneer-0.4.1/aiopioneer/const.py` & `aiopioneer-0.4.2/aiopioneer/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """Constants for aiopioneer."""
 
 from enum import Enum
 
 DEFAULT_PORT = 8102
-VERSION = "0.4.1"
+VERSION = "0.4.2"
 
 
 class Zones(Enum):
     """Valid aiopioneer zones"""
 
+    ALL = "ALL"
     Z1 = "1"
     Z2 = "2"
     Z3 = "3"
     HDZ = "Z"
 
     def __str__(self):
         return self.value
```

### Comparing `aiopioneer-0.4.1/aiopioneer/param.py` & `aiopioneer-0.4.2/aiopioneer/param.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 PARAM_POWER_ON_VOLUME_BOUNCE = "power_on_volume_bounce"
 PARAM_VOLUME_STEP_ONLY = "volume_step_only"
 PARAM_IGNORE_VOLUME_CHECK = "ignore_volume_check"
 PARAM_DEBUG_LISTENER = "debug_listener"
 PARAM_DEBUG_RESPONDER = "debug_responder"
 PARAM_DEBUG_UPDATER = "debug_updater"
 PARAM_DEBUG_COMMAND = "debug_command"
+PARAM_QUERY_SOURCES = "query_sources"
 PARAM_ZONE_1_SOURCES = "zone_1_sources"  ## All possible valid input sources for Zone 1
 PARAM_ZONE_2_SOURCES = "zone_2_sources"  ## All possible valid input sources for Zone 2
 PARAM_ZONE_3_SOURCES = "zone_3_sources"  ## All possible valid input sources for Zone 3
 PARAM_HDZONE_SOURCES = "hdzone_sources"  ## All possible valid input sources for HDZone
 PARAM_ZONE_SOURCES = {
     Zones.Z1: PARAM_ZONE_1_SOURCES,
     Zones.Z2: PARAM_ZONE_2_SOURCES,
@@ -40,14 +41,18 @@
 ## categories, instead we rely on the AVR returning them as they are changed.
 PARAM_DISABLE_AUTO_QUERY = "disable_autoquery"
 ## A list containing all the IDs of listening modes that should be disabled
 PARAM_DISABLED_LISTENING_MODES = "disabled_amplifier_listening_modes"
 ## Tuner step for AM frequencies. If None, calculate automatically when tuner is first used
 PARAM_TUNER_AM_FREQ_STEP = "am_frequency_step"
 
+PARAM_DEFAULTS_SYSTEM = {
+    PARAM_QUERY_SOURCES: None,
+}
+
 PARAM_DEFAULTS = {
     PARAM_IGNORED_ZONES: [],
     PARAM_COMMAND_DELAY: 0.1,
     PARAM_MAX_SOURCE_ID: 60,
     PARAM_MAX_VOLUME: 185,
     PARAM_MAX_VOLUME_ZONEX: 81,
     PARAM_POWER_ON_VOLUME_BOUNCE: False,
```

### Comparing `aiopioneer-0.4.1/aiopioneer/parsers/audio.py` & `aiopioneer-0.4.2/aiopioneer/parsers/audio.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.4.1/aiopioneer/parsers/dsp.py` & `aiopioneer-0.4.2/aiopioneer/parsers/dsp.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.4.1/aiopioneer/parsers/information.py` & `aiopioneer-0.4.2/aiopioneer/parsers/information.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.4.1/aiopioneer/parsers/response.py` & `aiopioneer-0.4.2/aiopioneer/parsers/response.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.4.1/aiopioneer/parsers/settings.py` & `aiopioneer-0.4.2/aiopioneer/parsers/settings.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.4.1/aiopioneer/parsers/system.py` & `aiopioneer-0.4.2/aiopioneer/parsers/system.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 """Core system related parsers for Pioneer AVRs."""
 
 import re
 
-from aiopioneer.param import PARAM_TUNER_AM_FREQ_STEP, PARAM_MHL_SOURCE, PARAM_SPEAKER_SYSTEM_MODES
+from aiopioneer.param import (
+    PARAM_QUERY_SOURCES,
+    PARAM_TUNER_AM_FREQ_STEP,
+    PARAM_MHL_SOURCE,
+    PARAM_SPEAKER_SYSTEM_MODES,
+)
 from aiopioneer.const import (
     MEDIA_CONTROL_SOURCES,
     SPEAKER_MODES,
     HDMI_AUDIO_MODES,
     HDMI_OUT_MODES,
     PQLS_MODES,
     AMP_MODES,
@@ -320,20 +325,32 @@
                                 zone=zone,
                                 value="unknown",
                                 queue_commands=None))
 
         return parsed
 
     @staticmethod
-    def input_name(raw: str, _param: dict, zone = None, command = "RGB") -> list:
+    def input_name(raw: str, params: dict, zone = None, command = "RGB") -> list:
         """Input name parser. Applies system wide."""
         source_number = raw[:2]
         source_name = raw[3:]
 
         parsed = []
+        if not params[PARAM_QUERY_SOURCES]:
+            ## Only update AVR source mappings if AVR sources are being queried
+            return parsed
+        ## Clear current source ID from source mappings via PioneerAVR.clear_source_id
+        parsed.append(Response(raw=raw,
+                            response_command=command,
+                            base_property=lambda self: self.clear_source_id(source_number),
+                            property_name=source_name,
+                            zone=zone,
+                            value=source_number,
+                            queue_commands=None))
+
         parsed.append(Response(raw=raw,
                             response_command=command,
                             base_property="_source_name_to_id",
                             property_name=source_name,
                             zone=zone,
                             value=source_number,
                             queue_commands=None))
```

### Comparing `aiopioneer-0.4.1/aiopioneer/parsers/tuner.py` & `aiopioneer-0.4.2/aiopioneer/parsers/tuner.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.4.1/aiopioneer/parsers/video.py` & `aiopioneer-0.4.2/aiopioneer/parsers/video.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.4.1/aiopioneer/pioneer_avr.py` & `aiopioneer-0.4.2/aiopioneer/pioneer_avr.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,28 +3,34 @@
 
 
 import asyncio
 import time
 import logging
 import re
 import math
+
+from collections.abc import Callable
+from inspect import isfunction
+
 from .param import (
     PARAM_IGNORED_ZONES,
     PARAM_COMMAND_DELAY,
     PARAM_MAX_SOURCE_ID,
     PARAM_MAX_VOLUME,
     PARAM_MAX_VOLUME_ZONEX,
     PARAM_POWER_ON_VOLUME_BOUNCE,
     PARAM_VOLUME_STEP_ONLY,
     PARAM_IGNORE_VOLUME_CHECK,
     PARAM_DEBUG_LISTENER,
     PARAM_DEBUG_RESPONDER,
     PARAM_DEBUG_UPDATER,
     PARAM_DEBUG_COMMAND,
+    PARAM_QUERY_SOURCES,
     PARAM_DEFAULTS,
+    PARAM_DEFAULTS_SYSTEM,
     PARAM_MODEL_DEFAULTS,
     PARAM_DISABLED_LISTENING_MODES,
     PARAM_VIDEO_RESOLUTION_MODES,
     PARAM_ZONE_SOURCES,
     PARAM_ENABLED_FUNCTIONS,
     PARAM_DISABLE_AUTO_QUERY,
     PARAM_TUNER_AM_FREQ_STEP,
@@ -124,28 +130,29 @@
         self.dsp = {}
         self.video = {}
         self.system = {}
         self.audio = {}
 
         # Parameters
         self._default_params = PARAM_DEFAULTS
+        self._system_params = PARAM_DEFAULTS_SYSTEM
         self._user_params = None
         self._params = None
         self.set_user_params(params)
 
         # Internal state
         self._connect_lock = asyncio.Lock()
         self._disconnect_lock = asyncio.Lock()
         self._update_lock = asyncio.Lock()
         self._request_lock = asyncio.Lock()
         self._update_event = asyncio.Event()
         self._reconnect = True
         self._full_update = True
-        self._last_updated = 0.0
-        self._last_command = 0.0
+        self._last_updated = None
+        self._last_command = None
         self._reader = None
         self._writer = None
         self._listener_task = None
         self._responder_task = None
         self._reconnect_task = None
         self._updater_task = None
         self._command_queue_task = None
@@ -157,24 +164,34 @@
         self._source_id_to_name = {}
         self._zone_callback = {}
         # self._update_callback = None
 
     def __del__(self):
         _LOGGER.debug(">> PioneerAVR.__del__()")
 
+    @property
+    def query_sources(self) -> bool:
+        """Whether sources have been queried from AVR."""
+        return self._system_params.get(PARAM_QUERY_SOURCES)
+
+    def _set_query_sources(self, value: bool) -> None:
+        self._system_params[PARAM_QUERY_SOURCES] = value
+        self._update_params()
+
     def get_unique_id(self):
         """Get unique identifier for this instance."""
         return self._host + ":" + str(self._port)
 
     # Parameter management functions
     def _update_params(self):
         """Set current parameters."""
         self._params = {}
         merge(self._params, self._default_params)
         merge(self._params, self._user_params, force_overwrite=True)
+        merge(self._params, self._system_params)
 
     def set_user_params(self, params=None):
         """Set parameters and merge with defaults."""
         _LOGGER.debug(">> PioneerAVR.set_user_params(%s)", params)
         self._user_params = {}
         if params is not None:
             merge(self._user_params, params)
@@ -372,39 +389,43 @@
     async def _reconnect_cancel(self):
         """Cancel any active reconnect task."""
         await cancel_task(self._reconnect_task, "reconnect")
         self._reconnect_task = None
 
     async def _connection_listener(self):
         """AVR connection listener. Parse responses and update state."""
-        _LOGGER.debug(">> PioneerAVR._connection_listener() started")
+        if self._params[PARAM_DEBUG_LISTENER]:
+            _LOGGER.debug(">> PioneerAVR._connection_listener() started")
         running = True
         while self.available:
+            debug_listener = self._params[PARAM_DEBUG_LISTENER]
+            action = " listening for responses"
             try:
                 response = await self._read_response()
                 if response is None:
                     # Connection closed or exception, exit task
                     break
 
                 # Check for empty response
-                debug_listener = self._params[PARAM_DEBUG_LISTENER]
                 self._last_updated = time.time()  # include empty responses
                 if not response:
                     # Skip processing empty responses (keepalives)
                     if debug_listener:
                         _LOGGER.debug("ignoring empty response")
                     continue
                 if debug_listener:
-                    _LOGGER.debug("AVR listener received response: %s", response)
+                    _LOGGER.debug("received AVR response: %s", response)
 
                 # Parse response, update cached properties
+                action = " parsing response " + response
                 parse_result = self._parse_response(response)
                 updated_zones = parse_result.get("updated_zones")
 
                 # Detect Main Zone power on for volume workaround
+                action = ""
                 power_on_volume_bounce = self._params[PARAM_POWER_ON_VOLUME_BOUNCE]
                 if power_on_volume_bounce and self._power_zone_1 is not None:
                     if not self._power_zone_1 and self.power.get("1"):
                         # Main zone powered on, schedule bounce task
                         _LOGGER.info("scheduling main zone volume workaround")
                         self.queue_command(
                             "volume_up", skip_if_queued=False, insert_at=0
@@ -426,79 +447,81 @@
                     await self._command_queue_schedule()
 
                 # NOTE: to avoid deadlocks, do not run any operations that
                 # depend on further responses (returned by the listener) within
                 # the listener loop.
 
                 if updated_zones:
+                    action = f" while calling zone callbacks for {updated_zones}"
                     # Call zone callbacks for updated zones
                     self._call_zone_callbacks(updated_zones)
                     # NOTE: updating zone 1 does not reset its scan interval -
                     # scan interval is set to a regular timer
 
             except asyncio.CancelledError:
-                _LOGGER.debug(">> PioneerAVR._connection_listener() cancelled")
+                if debug_listener:
+                    _LOGGER.debug(">> PioneerAVR._connection_listener() cancelled")
                 running = False
                 break
             except Exception as exc:  # pylint: disable=broad-except
-                _LOGGER.error(
-                    ">> PioneerAVR._connection_listener() exception: %s", str(exc)
-                )
+                _LOGGER.error("listener exception%s: %s", action, str(exc))
                 print(exc)
                 # continue listening on exception
 
         if running and self.available:
             # Trigger disconnection if not already disconnected
             await self.disconnect()
 
         _LOGGER.debug(">> PioneerAVR._connection_listener() completed")
 
     async def _listener_schedule(self):
         """Schedule the listener task."""
-        _LOGGER.debug(">> PioneerAVR._listener_schedule()")
+        if self._params[PARAM_DEBUG_LISTENER]:
+            _LOGGER.debug(">> PioneerAVR._listener_schedule()")
         await self._listener_cancel()
         self._listener_task = asyncio.create_task(self._connection_listener())
 
     async def _listener_cancel(self):
         """Cancel the listener task."""
-        await cancel_task(self._listener_task, "listener")
+        debug_listener = self._params[PARAM_DEBUG_LISTENER]
+        await cancel_task(self._listener_task, "listener", debug=debug_listener)
         self._listener_task = None
 
     # Reader co-routine
     async def _reader_readuntil(self):
         """Read from reader with cancel detection."""
         try:
             return await self._reader.readuntil(b"\n")
         except asyncio.CancelledError:
-            _LOGGER.debug("reader: readuntil() was cancelled")
+            if self._params[PARAM_DEBUG_RESPONDER]:
+                _LOGGER.debug("reader: readuntil() was cancelled")
             return None
 
     # Read responses from AVR
     async def _read_response(self, timeout=None):
         """Wait for a response from AVR and return to all readers."""
         debug_responder = self._params[PARAM_DEBUG_RESPONDER]
-
         if debug_responder:
             _LOGGER.debug(">> PioneerAVR._read_response(timeout=%s)", timeout)
 
         # Schedule responder task if not already created
         responder_task = self._responder_task
         if responder_task:
             if responder_task.done():
                 responder_task = None  # trigger new task creation
         if responder_task is None:
             responder_task = asyncio.create_task(self._reader_readuntil())
             # responder_task = asyncio.create_task(self._reader.readuntil(b"\n"))
             self._responder_task = responder_task
             if debug_responder:
-                _LOGGER.debug("created responder task %s", responder_task)
+                _LOGGER.debug("created responder task %s", responder_task.get_name())
         else:
             # Wait on existing responder task
             if debug_responder:
-                _LOGGER.debug("using existing responder task %s", responder_task)
+                _LOGGER.debug("using responder task %s", responder_task.get_name())
 
         # Wait for result and process
         task_name = asyncio.current_task().get_name()
         try:
             if timeout:
                 if debug_responder:
                     _LOGGER.debug(
@@ -514,29 +537,31 @@
                     return None
             else:
                 if debug_responder:
                     _LOGGER.debug("%s: waiting for data", task_name)
                 raw_response = await responder_task
         except (EOFError, TimeoutError):
             # Connection closed
-            _LOGGER.debug("%s: connection closed", task_name)
+            if debug_responder:
+                _LOGGER.debug("%s: connection closed", task_name)
             return None
         except Exception as exc:  # pylint: disable=broad-except
             _LOGGER.error("%s: exception: %s", task_name, str(exc))
             return None
         if raw_response is None:  # task cancelled
             return None
         response = raw_response.decode().strip()
         if debug_responder:
             _LOGGER.debug("%s: received response: %s", task_name, response)
         return response
 
     async def _responder_cancel(self):
         """Cancel any active responder task."""
-        await cancel_task(self._responder_task, "responder")
+        debug_responder = self._params[PARAM_DEBUG_RESPONDER]
+        await cancel_task(self._responder_task, "responder", debug=debug_responder)
         self._responder_task = None
 
     # Send commands and requests to AVR
     async def send_raw_command(self, command, rate_limit=True):
         """Send a raw command to the AVR."""
         debug_command = self._params[PARAM_DEBUG_COMMAND]
         if debug_command:
@@ -546,21 +571,24 @@
                 rate_limit,
             )
         if not self.available:
             raise RuntimeError("AVR connection not available")
 
         if rate_limit:
             # Rate limit commands
-            since_command = time.time() - self._last_command
             command_delay = self._params[PARAM_COMMAND_DELAY]
+            since_command = command_delay + 0.1
+            if self._last_command:
+                since_command = time.time() - self._last_command
             if since_command < command_delay:
                 delay = command_delay - since_command
-                _LOGGER.debug("delaying command for %.3f s", delay)
+                if debug_command:
+                    _LOGGER.debug("delaying command for %.3f s", delay)
                 await asyncio.sleep(command_delay - since_command)
-        _LOGGER.debug("sending AVR command: %s", command)
+        _LOGGER.debug("sending command: %s", command)
         self._writer.write(command.encode("ASCII") + b"\r")
         await self._writer.drain()
         self._last_command = time.time()
 
     async def send_raw_request(
         self, command, response_prefix, ignore_error=None, rate_limit=True
     ):
@@ -580,31 +608,38 @@
                 response = await self._read_response(timeout=self._timeout)
 
                 # Check response
                 if response is None:
                     _LOGGER.debug("AVR command %s timed out", command)
                     return None
                 elif response.startswith(response_prefix):
-                    _LOGGER.debug(
-                        "AVR command %s returned response: %s", command, response
-                    )
+                    if debug_command:
+                        _LOGGER.debug(
+                            "AVR command %s returned response: %s", command, response
+                        )
                     return response
                 elif response.startswith("E"):
                     err = f"AVR command {command} returned error: {response}"
                     if ignore_error is None:
                         raise RuntimeError(err)
                     elif not ignore_error:
                         _LOGGER.error(err)
                         return False
                     elif ignore_error:
                         _LOGGER.debug(err)
                         return False
 
     async def send_command(
-        self, command, zone="1", prefix="", ignore_error=None, rate_limit=True, suffix=""
+        self,
+        command,
+        zone="1",
+        prefix="",
+        ignore_error=None,
+        rate_limit=True,
+        suffix="",
     ):
         """Send a command or request to the device."""
         # pylint: disable=unidiomatic-typecheck disable=logging-not-lazy
         debug_command = self._params[PARAM_DEBUG_COMMAND]
         if debug_command:
             _LOGGER.debug(
                 '>> PioneerAVR.send_command("%s", zone="%s", prefix="%s", '
@@ -632,15 +667,17 @@
                     if debug_command:
                         _LOGGER.debug("send_command received response: %s", response)
                     return response
                 else:
                     _LOGGER.error("invalid request %s for zone %s", raw_command, zone)
                     return None
             elif type(raw_command) is str:
-                return await self.send_raw_command(prefix + raw_command + suffix, rate_limit)
+                return await self.send_raw_command(
+                    prefix + raw_command + suffix, rate_limit
+                )
             else:
                 _LOGGER.warning("invalid command %s for zone %s", command, zone)
                 return None
         except RuntimeError as exc:
             _LOGGER.error("cannot execute %s command: %s", command, exc)
             return False
 
@@ -707,22 +744,24 @@
                 self.zones.remove(zone)
                 self._call_zone_callbacks([zone])  # update availability
                 removed_zones = True
         await self.query_zones(force_update=removed_zones)
 
     def set_source_dict(self, sources):
         """Manually set source id<->name translation tables."""
+        self._set_query_sources(False)
         source_name_to_id = {}
         merge(source_name_to_id, sources)
         self._source_name_to_id = source_name_to_id
         self._source_id_to_name = {v: k for k, v in sources.items()}
 
     async def build_source_dict(self):
         """Generate source id<->name translation tables."""
         timeouts = 0
+        self._set_query_sources(True)
         self._source_name_to_id = {}
         self._source_id_to_name = {}
         _LOGGER.info("querying AVR source names")
         async with self._update_lock:
             for src_id in range(self._params[PARAM_MAX_SOURCE_ID] + 1):
                 response = await self.send_raw_request(
                     "?RGB" + str(src_id).zfill(2),
@@ -770,14 +809,23 @@
         """Return name for given source ID."""
         return (
             self._source_id_to_name.get(source_id, source_id)
             if self._source_name_to_id
             else source_id
         )
 
+    def clear_source_id(self, source_id: str) -> None:
+        """Clear name mapping for given source ID."""
+        source_name = None
+        if source_id in self._source_id_to_name:
+            source_name = self._source_id_to_name[source_id]
+            self._source_id_to_name.pop(source_id)
+        if source_name in self._source_name_to_id:
+            self._source_name_to_id.pop(source_name)
+
     def get_sound_modes(self, zone):
         """Return list of valid sound modes."""
         # Check if the zone is the main zone or not, listening modes aren't supported on other zones
         if zone == "1":
             # Now check if the current input info is multi channel or not
             if self.audio.get("input_multichannel"):
                 return list(
@@ -858,93 +906,95 @@
         #
         # https://github.com/home-assistant/architecture/blob/master/adr/0004-webscraping.md
         #
         # VSX-930 will report model and software version, but not MAC address.
         # It is unknown how iControlAV5 determines this on a routed network.
 
     # Callback functions
-    def set_zone_callback(self, zone, callback):
+    def set_zone_callback(
+        self, zone: Zones | str, callback: Callable[..., None] | None = None
+    ):
         """Register a callback for a zone."""
-        if zone in self.zones:
+        if str(zone) in self.zones:
             if callback:
-                self._zone_callback[zone] = callback
+                self._zone_callback[str(zone)] = callback
             else:
-                self._zone_callback.pop(zone)
+                self._zone_callback.pop(str(zone))
 
     def clear_zone_callbacks(self):
         """Clear all callbacks for a zone."""
         self._zone_callback = {}
 
-    def _call_zone_callbacks(self, zones=None):
+    def _call_zone_callbacks(self, zones: list[Zones | str] = None):
         """Call callbacks to signal updated zone(s)."""
         if zones is None:
             zones = self.zones
         for zone in zones:
             if str(zone) in self._zone_callback:
                 callback = self._zone_callback[str(zone)]
                 if callback:
-                    _LOGGER.debug("calling callback for zone %s", zone)
+                    # _LOGGER.debug("calling callback for zone %s", zone)
                     callback()
 
     # Update functions
-    def _parse_response(self, response):
+    def _parse_response(self, response_raw: str):
         """Parse response and update cached parameters."""
         updated_zones = set()
 
-        parsed_response: list = process_raw_response(response, self._params)
+        parsed_response: list = process_raw_response(response_raw, self._params)
         if parsed_response is not None:
             for response in parsed_response:
-                if response.base_property is not None:
+                if isfunction(response.base_property):
+                    ## Call PioneerAVR class function
+                    response.base_property(self)
+                elif response.base_property is not None:
                     current_value = getattr(self, response.base_property)
-                    if response.property_name is None and response.zone is not None:
+                    if response.property_name is None and response.zone not in [Zones.ALL, None]:
                         if current_value.get(response.zone.value) is not response.value:
                             current_value[response.zone.value] = response.value
                             setattr(self, response.base_property, current_value)
-                            if response.zone.value not in updated_zones:
-                                updated_zones.add(response.zone)
                             _LOGGER.info(
                                 "Zone %s: %s: %s (%s)",
                                 response.zone.value,
                                 response.base_property,
                                 getattr(self, response.base_property)[
                                     response.zone.value
                                 ],
                                 response.raw,
                             )
 
                     elif (
-                        response.property_name is not None and response.zone is not None
+                        response.property_name is not None and
+                        response.zone not in [Zones.ALL, None]
                     ):
                         # Set default value first otherwise we hit an exception
                         current_value.setdefault(response.zone.value, {})
                         if (
                             current_value.get(response.zone.value).get(
                                 response.property_name
                             )
                             is not response.value
                         ):
                             # Set current_value to response.value for setattr
                             current_value[response.zone.value][
                                 response.property_name
                             ] = response.value
                             setattr(self, response.base_property, current_value)
-                            if response.zone.value not in updated_zones:
-                                updated_zones.add(response.zone.value)
                             _LOGGER.info(
                                 "Zone %s: %s.%s: %s (%s)",
                                 response.zone.value,
                                 response.base_property,
                                 response.property_name,
                                 getattr(self, response.base_property)[
                                     response.zone.value
                                 ][response.property_name],
                                 response.raw,
                             )
 
-                    elif response.property_name is None and response.zone is None:
+                    elif response.property_name is None and response.zone in [Zones.ALL, None]:
                         if current_value is not response.value:
                             current_value = response.value
                             setattr(self, response.base_property, current_value)
                             _LOGGER.info(
                                 "Global: %s: %s (%s)",
                                 response.base_property,
                                 getattr(self, response.base_property),
@@ -964,14 +1014,18 @@
                                 response.property_name,
                                 getattr(self, response.base_property)[
                                     response.property_name
                                 ],
                                 response.raw,
                             )
 
+                    # Set updated_zones if response.zone is not None and not already added
+                    if response.zone is not None and response.zone not in updated_zones:
+                        updated_zones.add(response.zone)
+
                 # Add any requested extra commands to run
                 if response.command_queue is not None:
                     for command in response.command_queue:
                         self.queue_command(command)
 
                 # Some specific overrides for the command queue, these are only
                 # requested if we are not doing a full update
@@ -1036,15 +1090,16 @@
             _LOGGER.debug(">> PioneerAVR._updater_schedule()")
             await self._updater_cancel()
             self._full_update = True  # always perform full update on schedule
             self._updater_task = asyncio.create_task(self._updater())
 
     async def _updater_cancel(self):
         """Cancel the updater task."""
-        await cancel_task(self._updater_task, "updater")
+        debug_updater = self._params[PARAM_DEBUG_UPDATER]
+        await cancel_task(self._updater_task, "updater", debug=debug_updater)
         self._updater_task = None
 
     async def _update_zone(self, zone):
         """Update an AVR zone."""
         # Check for timeouts, but ignore errors (eg. ?V will
         # return E02 immediately after power on)
 
@@ -1115,22 +1170,27 @@
             _LOGGER.debug("AVR not connected, skipping update")
             return False
 
         _rc = True
         async with self._update_lock:
             # Update only if scan_interval has passed
             now = time.time()
-            since_updated = now - self._last_updated
             full_update = self._full_update
             scan_interval = self.scan_interval
+            since_updated = scan_interval + 1
+            since_updated_str = "never"
+            if self._last_updated:
+                since_updated = now - self._last_updated
+                since_updated_str = "%.3f s ago" % since_updated
+
             if full_update or not scan_interval or since_updated > scan_interval:
                 _LOGGER.info(
-                    "updating AVR status (full=%s, last updated %.3f s ago)",
+                    "updating AVR status (full=%s, last updated %s)",
                     full_update,
-                    since_updated,
+                    since_updated_str,
                 )
                 self._last_updated = now
                 self._full_update = False
                 try:
                     for zone in self.zones:
                         await self._update_zone(zone)
                     if full_update:
@@ -1151,17 +1211,15 @@
                 # within scan_interval of the response.
                 ##
                 # Keepalives may be sent by the AVR (every 30 seconds on the
                 # VSX-930) when connected to port 8102, but are not sent when
                 # connected to port 23.
                 _rc = None
                 if debug_updater:
-                    _LOGGER.debug(
-                        "skipping update: last updated %.3f s ago", since_updated
-                    )
+                    _LOGGER.debug("skipping update: last updated %s", since_updated_str)
         if _rc is False:
             # Disconnect on error
             await self.disconnect()
         if debug_updater:
             _LOGGER.debug(">> PioneerAVR._updater_update() completed")
         return _rc
 
@@ -1229,51 +1287,61 @@
     async def volume_down(self, zone="1"):
         """Volume down media player."""
         self._check_zone(zone)
         return await self.send_command("volume_down", zone, ignore_error=False)
 
     async def _execute_command_queue(self):
         """Execute commands from a queue."""
-        _LOGGER.debug(">> PioneerAVR._command_queue")
+        debug_command = self._params[PARAM_DEBUG_COMMAND]
+        if debug_command:
+            _LOGGER.debug(">> PioneerAVR._command_queue")
         while len(self._command_queue) > 0:
             # Keep command in queue until it has finished executing
             command = self._command_queue[0]
-            _LOGGER.info("Command Queue Executing: %s", command)
+            if debug_command:
+                _LOGGER.debug("command queue executing: %s", command)
             if command == "FULL_UPDATE":
                 await self.update(full=True)
             elif command == "_calculate_am_frequency_step":
                 await self._calculate_am_frequency_step()
             else:
                 await self.send_command(command, ignore_error=True)
             self._command_queue.pop(0)
 
-        _LOGGER.debug("Command Queue Finished.")
+        if debug_command:
+            _LOGGER.debug("command queue finished")
         return True
 
     async def _command_queue_cancel(self):
         """Cancel any pending commands and the task itself."""
-        await cancel_task(self._command_queue_task, "command_queue")
+        debug_command = self._params[PARAM_DEBUG_COMMAND]
+        await cancel_task(
+            self._command_queue_task, "command_queue", debug=debug_command
+        )
         self._command_queue_task = None
 
     async def _command_queue_schedule(self):
         """Schedule commands to queue."""
-        _LOGGER.debug(">> PioneerAVR._command_queue_schedule()")
+        if self._params[PARAM_DEBUG_COMMAND]:
+            _LOGGER.debug(">> PioneerAVR._command_queue_schedule()")
         await self._command_queue_cancel()
         self._command_queue_task = asyncio.create_task(self._execute_command_queue())
 
     def queue_command(self, command, skip_if_queued=True, insert_at=-1):
         """Add a new command to the queue to run."""
-        _LOGGER.debug(">> PioneerAVR.queue_command(%s)", command)
+        if self._params[PARAM_DEBUG_COMMAND]:
+            _LOGGER.debug(">> PioneerAVR.queue_command(%s)", command)
         if not skip_if_queued or command not in self._command_queue:
             if insert_at >= 0:
                 self._command_queue.insert(insert_at, command)
             else:
                 self._command_queue.append(command)
         else:
-            _LOGGER.debug("command %s already queued, skipping", command)
+            if self._params[PARAM_DEBUG_COMMAND]:
+                _LOGGER.debug("command %s already queued, skipping", command)
 
     async def _calculate_am_frequency_step(self):
         """
         Automatically calculate the AM frequency step by stepping the frequency
         up and then down.
         """
         _LOGGER.debug(">> PioneerAVR._calculate_am_frequency_step() ")
@@ -1793,26 +1861,29 @@
                 )
         else:
             raise NotImplementedError(
                 f"Current source ({self.source.get(zone)}) does not support "
                 "media_control activities."
             )
 
-    async def set_input_name(self, input_id: str, name: str = "", default: bool = False):
+    async def set_source_name(
+        self, source_id: str, source_name: str = "", default: bool = False
+    ):
         """Renames a given input, set the default parameter to true to reset to default."""
         if default:
             await self.send_command(
-                command="set_default_input_name",
-                zone="1",
-                suffix=input_id)
+                command="set_default_source_name", zone="1", suffix=source_id
+            )
         else:
-            if len(name) > 14:
-                raise ValueError(f"New input name ({name}) length too long. "
-                                 "Up to 14 characters are allowed")
-            if self._source_id_to_name.get(input_id) is not name:
+            if len(source_name) > 14:
+                raise ValueError(
+                    f"New source name ({source_name}) length too long. "
+                    "Up to 14 characters are allowed"
+                )
+            if self._source_id_to_name.get(source_id) is not source_name:
                 await self.send_command(
-                    command="set_input_name",
+                    command="set_source_name",
                     zone="1",
-                    prefix=name,
-                    suffix=input_id
+                    prefix=source_name,
+                    suffix=source_id,
                 )
         return True
```

### Comparing `aiopioneer-0.4.1/aiopioneer/util.py` & `aiopioneer-0.4.2/aiopioneer/util.py`

 * *Files 14% similar despite different names*

```diff
@@ -92,44 +92,53 @@
                 ## TODO: what if wait_for is cancelled when waiting for task to be cancelled?
                 pass
             raise asyncio.TimeoutError()
     except asyncio.CancelledError as exc:
         raise exc
 
 
-async def cancel_task(task, task_name=None):
+async def cancel_task(task, task_name=None, debug=False):
     """Cancels a task and waits for it to finish."""
     if task:
         if task_name is None:
             task_name = task.get_name()
         ## Trap exception if not called from a task
         current_task = None
         try:
             current_task = asyncio.Task.current_task()
         except AttributeError:
             pass
         if current_task is not None and task == current_task:
-            _LOGGER.debug(
-                ">> cancel_task(%s): ignoring cancellation of current task", task_name
-            )
+            if debug:
+                _LOGGER.debug(
+                    ">> cancel_task(%s): ignoring cancellation of current task",
+                    task_name,
+                )
             return
         if not task.done():
-            _LOGGER.debug(">> cancel_task(%s): requesting cancellation", task_name)
+            if debug:
+                _LOGGER.debug(">> cancel_task(%s): requesting cancellation", task_name)
             task.cancel()
-            _LOGGER.debug(">> cancel_task(%s): waiting for completion", task_name)
+            if debug:
+                _LOGGER.debug(">> cancel_task(%s): waiting for completion", task_name)
             try:
                 await task
             except asyncio.CancelledError:
-                _LOGGER.debug(">> cancel_task(%s): cancelled exception", task_name)
+                if debug:
+                    _LOGGER.debug(">> cancel_task(%s): cancelled exception", task_name)
             except Exception as exc:  # pylint: disable=broad-except
-                _LOGGER.debug(
-                    ">> cancel_task(%s): returned exception: %s", task_name, exc
-                )
+                if debug:
+                    _LOGGER.debug(
+                        ">> cancel_task(%s): returned exception: %s", task_name, exc
+                    )
             else:
-                _LOGGER.debug(">> cancel_task(%s): completed", task_name)
+                if debug:
+                    _LOGGER.debug(">> cancel_task(%s): completed", task_name)
         else:
-            _LOGGER.debug(">> cancel_task(%s): already completed", task_name)
+            if debug:
+                _LOGGER.debug(">> cancel_task(%s): already completed", task_name)
             exc = task.exception()
             if exc:
-                _LOGGER.debug(
-                    ">> cancel_task(%s): returned exception: %s", task_name, exc
-                )
+                if debug:
+                    _LOGGER.debug(
+                        ">> cancel_task(%s): returned exception: %s", task_name, exc
+                    )
```

### Comparing `aiopioneer-0.4.1/aiopioneer.egg-info/PKG-INFO` & `aiopioneer-0.4.2/aiopioneer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiopioneer
-Version: 0.4.1
+Version: 0.4.2
 Summary: Asyncio Python library for controlling a Pioneer AVR via its API
 Home-page: https://github.com/crowbarz/aiopioneer.git
 Author: Crowbar Z
 Author-email: crowbarz@outlook.com
 Keywords: pioneer avr asyncio
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
```

### Comparing `aiopioneer-0.4.1/aiopioneer.egg-info/SOURCES.txt` & `aiopioneer-0.4.2/aiopioneer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.4.1/setup.py` & `aiopioneer-0.4.2/setup.py`

 * *Files identical despite different names*

