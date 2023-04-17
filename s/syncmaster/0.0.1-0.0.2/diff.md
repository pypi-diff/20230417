# Comparing `tmp/syncmaster-0.0.1.tar.gz` & `tmp/syncmaster-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syncmaster-0.0.1.tar", last modified: Mon Apr 17 10:43:20 2023, max compression
+gzip compressed data, was "syncmaster-0.0.2.tar", last modified: Mon Apr 17 11:01:24 2023, max compression
```

## Comparing `syncmaster-0.0.1.tar` & `syncmaster-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 conor     (1000) conor     (1000)        0 2023-04-17 10:43:20.656257 syncmaster-0.0.1/
--rw-rw-r--   0 conor     (1000) conor     (1000)    11337 2023-01-20 02:50:04.000000 syncmaster-0.0.1/LICENSE
--rw-rw-r--   0 conor     (1000) conor     (1000)      111 2023-01-20 02:50:04.000000 syncmaster-0.0.1/MANIFEST.in
--rw-rw-r--   0 conor     (1000) conor     (1000)     1157 2023-04-17 10:43:20.656257 syncmaster-0.0.1/PKG-INFO
--rw-rw-r--   0 conor     (1000) conor     (1000)      305 2023-04-17 09:38:04.000000 syncmaster-0.0.1/README.md
--rw-rw-r--   0 conor     (1000) conor     (1000)     1050 2023-04-17 10:24:03.000000 syncmaster-0.0.1/settings.ini
--rw-rw-r--   0 conor     (1000) conor     (1000)       38 2023-04-17 10:43:20.656257 syncmaster-0.0.1/setup.cfg
--rw-rw-r--   0 conor     (1000) conor     (1000)     2560 2023-01-20 02:50:04.000000 syncmaster-0.0.1/setup.py
-drwxrwxr-x   0 conor     (1000) conor     (1000)        0 2023-04-17 10:43:20.656257 syncmaster-0.0.1/syncmaster/
--rw-rw-r--   0 conor     (1000) conor     (1000)      223 2023-04-17 10:34:17.000000 syncmaster-0.0.1/syncmaster/__init__.py
--rw-rw-r--   0 conor     (1000) conor     (1000)     1688 2023-04-17 10:34:17.000000 syncmaster-0.0.1/syncmaster/_modidx.py
--rw-rw-r--   0 conor     (1000) conor     (1000)     2309 2023-04-17 10:34:17.000000 syncmaster-0.0.1/syncmaster/analysis.py
--rw-rw-r--   0 conor     (1000) conor     (1000)     3232 2023-04-17 10:34:17.000000 syncmaster-0.0.1/syncmaster/device.py
-drwxrwxr-x   0 conor     (1000) conor     (1000)        0 2023-04-17 10:43:20.656257 syncmaster-0.0.1/syncmaster.egg-info/
--rw-rw-r--   0 conor     (1000) conor     (1000)     1157 2023-04-17 10:43:20.000000 syncmaster-0.0.1/syncmaster.egg-info/PKG-INFO
--rw-rw-r--   0 conor     (1000) conor     (1000)      379 2023-04-17 10:43:20.000000 syncmaster-0.0.1/syncmaster.egg-info/SOURCES.txt
--rw-rw-r--   0 conor     (1000) conor     (1000)        1 2023-04-17 10:43:20.000000 syncmaster-0.0.1/syncmaster.egg-info/dependency_links.txt
--rw-rw-r--   0 conor     (1000) conor     (1000)       42 2023-04-17 10:43:20.000000 syncmaster-0.0.1/syncmaster.egg-info/entry_points.txt
--rw-rw-r--   0 conor     (1000) conor     (1000)        1 2023-04-17 10:19:07.000000 syncmaster-0.0.1/syncmaster.egg-info/not-zip-safe
--rw-rw-r--   0 conor     (1000) conor     (1000)       41 2023-04-17 10:43:20.000000 syncmaster-0.0.1/syncmaster.egg-info/requires.txt
--rw-rw-r--   0 conor     (1000) conor     (1000)       11 2023-04-17 10:43:20.000000 syncmaster-0.0.1/syncmaster.egg-info/top_level.txt
+drwxrwxr-x   0 conor     (1000) conor     (1000)        0 2023-04-17 11:01:24.194955 syncmaster-0.0.2/
+-rw-rw-r--   0 conor     (1000) conor     (1000)    11337 2023-01-20 02:50:04.000000 syncmaster-0.0.2/LICENSE
+-rw-rw-r--   0 conor     (1000) conor     (1000)      111 2023-01-20 02:50:04.000000 syncmaster-0.0.2/MANIFEST.in
+-rw-rw-r--   0 conor     (1000) conor     (1000)     1157 2023-04-17 11:01:24.194955 syncmaster-0.0.2/PKG-INFO
+-rw-rw-r--   0 conor     (1000) conor     (1000)      305 2023-04-17 09:38:04.000000 syncmaster-0.0.2/README.md
+-rw-rw-r--   0 conor     (1000) conor     (1000)      929 2023-04-17 11:01:17.000000 syncmaster-0.0.2/settings.ini
+-rw-rw-r--   0 conor     (1000) conor     (1000)       38 2023-04-17 11:01:24.194955 syncmaster-0.0.2/setup.cfg
+-rw-rw-r--   0 conor     (1000) conor     (1000)     2560 2023-01-20 02:50:04.000000 syncmaster-0.0.2/setup.py
+drwxrwxr-x   0 conor     (1000) conor     (1000)        0 2023-04-17 11:01:24.190955 syncmaster-0.0.2/syncmaster/
+-rw-rw-r--   0 conor     (1000) conor     (1000)      223 2023-04-17 11:01:17.000000 syncmaster-0.0.2/syncmaster/__init__.py
+-rw-rw-r--   0 conor     (1000) conor     (1000)     1688 2023-04-17 11:01:17.000000 syncmaster-0.0.2/syncmaster/_modidx.py
+-rw-rw-r--   0 conor     (1000) conor     (1000)     2309 2023-04-17 11:01:17.000000 syncmaster-0.0.2/syncmaster/analysis.py
+-rw-rw-r--   0 conor     (1000) conor     (1000)     3275 2023-04-17 11:01:17.000000 syncmaster-0.0.2/syncmaster/device.py
+drwxrwxr-x   0 conor     (1000) conor     (1000)        0 2023-04-17 11:01:24.194955 syncmaster-0.0.2/syncmaster.egg-info/
+-rw-rw-r--   0 conor     (1000) conor     (1000)     1157 2023-04-17 11:01:24.000000 syncmaster-0.0.2/syncmaster.egg-info/PKG-INFO
+-rw-rw-r--   0 conor     (1000) conor     (1000)      379 2023-04-17 11:01:24.000000 syncmaster-0.0.2/syncmaster.egg-info/SOURCES.txt
+-rw-rw-r--   0 conor     (1000) conor     (1000)        1 2023-04-17 11:01:24.000000 syncmaster-0.0.2/syncmaster.egg-info/dependency_links.txt
+-rw-rw-r--   0 conor     (1000) conor     (1000)       42 2023-04-17 11:01:24.000000 syncmaster-0.0.2/syncmaster.egg-info/entry_points.txt
+-rw-rw-r--   0 conor     (1000) conor     (1000)        1 2023-04-17 10:19:07.000000 syncmaster-0.0.2/syncmaster.egg-info/not-zip-safe
+-rw-rw-r--   0 conor     (1000) conor     (1000)       41 2023-04-17 11:01:24.000000 syncmaster-0.0.2/syncmaster.egg-info/requires.txt
+-rw-rw-r--   0 conor     (1000) conor     (1000)       11 2023-04-17 11:01:24.000000 syncmaster-0.0.2/syncmaster.egg-info/top_level.txt
```

### Comparing `syncmaster-0.0.1/LICENSE` & `syncmaster-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `syncmaster-0.0.1/PKG-INFO` & `syncmaster-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncmaster
-Version: 0.0.1
+Version: 0.0.2
 Summary: Device and drivers for generating trigger signals to synchronise recorded signals with behavioural data
 Home-page: https://github.com/conorkeogh/syncmaster
 Author: Conor Keogh
 Author-email: conor.keogh@nds.ox.ac.uk
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `syncmaster-0.0.1/setup.py` & `syncmaster-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `syncmaster-0.0.1/syncmaster/_modidx.py` & `syncmaster-0.0.2/syncmaster/_modidx.py`

 * *Files identical despite different names*

### Comparing `syncmaster-0.0.1/syncmaster/analysis.py` & `syncmaster-0.0.2/syncmaster/analysis.py`

 * *Files identical despite different names*

### Comparing `syncmaster-0.0.1/syncmaster/device.py` & `syncmaster-0.0.2/syncmaster/device.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,19 +61,18 @@
         # For each port: try accessing and checking for acknowledge message
         port_found = False
         for port in ports:
             try:
                 # Connect to serial port
                 self.ser = serial.Serial(port.device, self.BAUDRATE, timeout=1)
 
-                # Send test message
-                self.sendMessage(self.HOST_MESSAGE)
-                
-                # Read response
-                response = self.ser.readline()
+                # Send test message and read response; repeat 3 times and keep third
+                for _ in range(3):
+                    self.sendMessage(self.HOST_MESSAGE)
+                    response = self.ser.readline()
 
                 # Check if response is appropriate
                 response = int(response)
                 if response == self.ACKNOWLEDGE:
                     self.target_port = port.device
                     port_found = True
```

### Comparing `syncmaster-0.0.1/syncmaster.egg-info/PKG-INFO` & `syncmaster-0.0.2/syncmaster.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncmaster
-Version: 0.0.1
+Version: 0.0.2
 Summary: Device and drivers for generating trigger signals to synchronise recorded signals with behavioural data
 Home-page: https://github.com/conorkeogh/syncmaster
 Author: Conor Keogh
 Author-email: conor.keogh@nds.ox.ac.uk
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

