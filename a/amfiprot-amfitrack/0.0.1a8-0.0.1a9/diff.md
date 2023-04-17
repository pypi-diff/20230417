# Comparing `tmp/amfiprot_amfitrack-0.0.1a8.tar.gz` & `tmp/amfiprot_amfitrack-0.0.1a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amfiprot_amfitrack-0.0.1a8.tar", last modified: Thu Apr 13 12:27:24 2023, max compression
+gzip compressed data, was "amfiprot_amfitrack-0.0.1a9.tar", last modified: Mon Apr 17 13:34:05 2023, max compression
```

## Comparing `amfiprot_amfitrack-0.0.1a8.tar` & `amfiprot_amfitrack-0.0.1a9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 12:27:24.005969 amfiprot_amfitrack-0.0.1a8/
--rw-rw-rw-   0        0        0     1057 2023-04-05 08:30:15.000000 amfiprot_amfitrack-0.0.1a8/LICENSE
--rw-rw-rw-   0        0        0     1552 2023-04-13 12:27:24.005969 amfiprot_amfitrack-0.0.1a8/PKG-INFO
--rw-rw-rw-   0        0        0     1119 2023-04-05 08:30:15.000000 amfiprot_amfitrack-0.0.1a8/README.md
--rw-rw-rw-   0        0        0      110 2023-04-05 08:30:15.000000 amfiprot_amfitrack-0.0.1a8/pyproject.toml
--rw-rw-rw-   0        0        0      671 2023-04-13 12:27:24.015981 amfiprot_amfitrack-0.0.1a8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-13 12:27:23.970065 amfiprot_amfitrack-0.0.1a8/src/
-drwxrwxrwx   0        0        0        0 2023-04-13 12:27:23.980040 amfiprot_amfitrack-0.0.1a8/src/amfiprot_amfitrack/
--rw-rw-rw-   0        0        0      124 2023-04-13 12:26:08.000000 amfiprot_amfitrack-0.0.1a8/src/amfiprot_amfitrack/__init__.py
--rw-rw-rw-   0        0        0      761 2023-04-05 08:30:15.000000 amfiprot_amfitrack-0.0.1a8/src/amfiprot_amfitrack/device.py
--rw-rw-rw-   0        0        0    19358 2023-04-05 09:16:31.000000 amfiprot_amfitrack-0.0.1a8/src/amfiprot_amfitrack/payload.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:27:24.004012 amfiprot_amfitrack-0.0.1a8/src/amfiprot_amfitrack.egg-info/
--rw-rw-rw-   0        0        0     1552 2023-04-13 12:27:23.000000 amfiprot_amfitrack-0.0.1a8/src/amfiprot_amfitrack.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      373 2023-04-13 12:27:23.000000 amfiprot_amfitrack-0.0.1a8/src/amfiprot_amfitrack.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 12:27:23.000000 amfiprot_amfitrack-0.0.1a8/src/amfiprot_amfitrack.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-13 12:27:23.000000 amfiprot_amfitrack-0.0.1a8/src/amfiprot_amfitrack.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-13 12:27:23.000000 amfiprot_amfitrack-0.0.1a8/src/amfiprot_amfitrack.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 13:34:05.656022 amfiprot_amfitrack-0.0.1a9/
+-rw-rw-rw-   0        0        0     1057 2023-04-13 12:00:53.000000 amfiprot_amfitrack-0.0.1a9/LICENSE
+-rw-rw-rw-   0        0        0     1552 2023-04-17 13:34:05.657507 amfiprot_amfitrack-0.0.1a9/PKG-INFO
+-rw-rw-rw-   0        0        0     1119 2023-04-13 12:00:53.000000 amfiprot_amfitrack-0.0.1a9/README.md
+-rw-rw-rw-   0        0        0      110 2023-04-13 12:00:53.000000 amfiprot_amfitrack-0.0.1a9/pyproject.toml
+-rw-rw-rw-   0        0        0      671 2023-04-17 13:34:05.660539 amfiprot_amfitrack-0.0.1a9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-17 13:34:05.603651 amfiprot_amfitrack-0.0.1a9/src/
+drwxrwxrwx   0        0        0        0 2023-04-17 13:34:05.633613 amfiprot_amfitrack-0.0.1a9/src/amfiprot_amfitrack/
+-rw-rw-rw-   0        0        0      124 2023-04-17 13:32:51.000000 amfiprot_amfitrack-0.0.1a9/src/amfiprot_amfitrack/__init__.py
+-rw-rw-rw-   0        0        0      761 2023-04-13 12:00:53.000000 amfiprot_amfitrack-0.0.1a9/src/amfiprot_amfitrack/device.py
+-rw-rw-rw-   0        0        0    21025 2023-04-17 13:10:16.000000 amfiprot_amfitrack-0.0.1a9/src/amfiprot_amfitrack/payload.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:34:05.653424 amfiprot_amfitrack-0.0.1a9/src/amfiprot_amfitrack.egg-info/
+-rw-rw-rw-   0        0        0     1552 2023-04-17 13:34:05.000000 amfiprot_amfitrack-0.0.1a9/src/amfiprot_amfitrack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      373 2023-04-17 13:34:05.000000 amfiprot_amfitrack-0.0.1a9/src/amfiprot_amfitrack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 13:34:05.000000 amfiprot_amfitrack-0.0.1a9/src/amfiprot_amfitrack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-17 13:34:05.000000 amfiprot_amfitrack-0.0.1a9/src/amfiprot_amfitrack.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-17 13:34:05.000000 amfiprot_amfitrack-0.0.1a9/src/amfiprot_amfitrack.egg-info/top_level.txt
```

### Comparing `amfiprot_amfitrack-0.0.1a8/LICENSE` & `amfiprot_amfitrack-0.0.1a9/LICENSE`

 * *Files identical despite different names*

### Comparing `amfiprot_amfitrack-0.0.1a8/PKG-INFO` & `amfiprot_amfitrack-0.0.1a9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amfiprot_amfitrack
-Version: 0.0.1a8
+Version: 0.0.1a9
 Summary: AmfiTrack extension for Amfiprot
 Author: Kristian Klein-Wengel
 Author-email: kkw@amfitech.dk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Requires-Python: >=3.6
```

### Comparing `amfiprot_amfitrack-0.0.1a8/README.md` & `amfiprot_amfitrack-0.0.1a9/README.md`

 * *Files identical despite different names*

### Comparing `amfiprot_amfitrack-0.0.1a8/setup.cfg` & `amfiprot_amfitrack-0.0.1a9/setup.cfg`

 * *Files identical despite different names*

### Comparing `amfiprot_amfitrack-0.0.1a8/src/amfiprot_amfitrack/device.py` & `amfiprot_amfitrack-0.0.1a9/src/amfiprot_amfitrack/device.py`

 * *Files identical despite different names*

### Comparing `amfiprot_amfitrack-0.0.1a8/src/amfiprot_amfitrack/payload.py` & `amfiprot_amfitrack-0.0.1a9/src/amfiprot_amfitrack/payload.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     RAW_B_FIELD_X = 0xA0  # DEPRECATED
     RAW_B_FIELD_Y = 0xA1  # DEPRECATED
     RAW_B_FIELD_Z = 0xA2  # DEPRECATED
     RAW_B_FIELD_REF = 0xA3  # DEPRECATED
     RAW_B_FIELD = 0xA4
     NORM_B_FIELD = 0xA5
     B_FIELD_PHASE = 0xA6
+    NORM_B_FIELD_IMU = 0xA7
 
     CALIBRATED_B_FIELD_X = 0xB3  # DEPRECATED
     CALIBRATED_B_FIELD_Y = 0xB4  # DEPRECATED
     CALIBRATED_B_FIELD_Z = 0xB5  # DEPRECATED
     SOURCE_CROSS_TALK = 0xC0
     RAW_ADC_SAMPLES = 0xE0
 
@@ -324,15 +325,59 @@
         return {
             'b_field': self.b_field,
             'current': self.current,
             'sensor_status': self.sensor_status,
             'source_coil_id': self.source_coil_id,
             'frame_id': self.frame_id
         }
+    
+class NormBFieldImuPayload(amfiprot.payload.Payload):
+    """
+    B-field given as a two-dimensional array (source_on_sensor):
+    ((x_on_x, x_on_y, x_on_z),
+     (y_on_x, y_on_y, y_on_z),
+     (z_on_x, z_on_y, z_on_z))
+    """
+    payload_type = PayloadType.NORM_B_FIELD_IMU
+
+    def __init__(self, data):
+        self.data = data
+        b_field_data = struct.unpack("<9f", self.data[0:36])
+        self.b_field = ((b_field_data[0], b_field_data[1], b_field_data[2]),
+                        (b_field_data[3], b_field_data[4], b_field_data[5]),
+                        (b_field_data[6], b_field_data[7], b_field_data[8]))
+        self.sensor_status = self.data[36]
+        self.source_coil_id = self.data[37]
+        self.imu = ImuData(self.data[38.50])
+        self.metal_distortion = self.data[50]
+        self.frame_id = int.from_bytes(self.data[51:54], byteorder='little', signed=False)
+
+    def __len__(self) -> int:
+        return len(self.data)
+
+    def __str__(self) -> str:
+        return "<Norm B-Field IMU> " + str(self.to_dict())
 
+    @property
+    def type(self) -> PayloadType:
+        return self.payload_type
+
+    def to_bytes(self) -> array.array:
+        return array.array('B', self.data)
+
+    def to_dict(self) -> dict:
+        return {
+            'b_field': self.b_field,
+            'sensor_status': self.sensor_status,
+            'source_coil_id': self.source_coil_id,
+            'imu': self.imu,
+            'metal_distortion': self.metal_distortion,
+            'frame_id': self.frame_id
+        }
+    
 
 class SourceCoilCalDataPayload(amfiprot.payload.Payload):
     payload_type = PayloadType.SOURCE_COIL_CAL_DATA
 
     def __init__(self, data):
         self.data = data
         self.current = struct.unpack("<3f", data[0:12])
@@ -502,14 +547,15 @@
     PayloadType.SET_PHASE_MODULATION: SetPhaseModulationPayload,
     PayloadType.EMF: EmfPayload,
     PayloadType.EMF_TIMESTAMP: EmfTimestampPayload,
     PayloadType.EMF_IMU: EmfImuPayload,
     PayloadType.EMF_IMU_TIMESTAMP: EmfImuTimestampPayload,
     PayloadType.EMF_IMU_FRAME_ID: EmfImuFrameIdPayload,
     PayloadType.RAW_B_FIELD: RawBFieldPayload,
+    PayloadType.NORM_B_FIELD_IMU: NormBFieldImuPayload,
     PayloadType.SIGN_DATA: SignDataPayload,
     PayloadType.PLL: PllPayload
 }
 
 
 def interpret_amfitrack_payload(payload: amfiprot.Payload, payload_type) -> amfiprot.Payload:
     if payload_type in amfitrack_payload_mappings:
```

### Comparing `amfiprot_amfitrack-0.0.1a8/src/amfiprot_amfitrack.egg-info/PKG-INFO` & `amfiprot_amfitrack-0.0.1a9/src/amfiprot_amfitrack.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amfiprot-amfitrack
-Version: 0.0.1a8
+Version: 0.0.1a9
 Summary: AmfiTrack extension for Amfiprot
 Author: Kristian Klein-Wengel
 Author-email: kkw@amfitech.dk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Requires-Python: >=3.6
```

