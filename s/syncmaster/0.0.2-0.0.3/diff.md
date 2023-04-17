# Comparing `tmp/syncmaster-0.0.2.tar.gz` & `tmp/syncmaster-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syncmaster-0.0.2.tar", last modified: Mon Apr 17 11:01:24 2023, max compression
+gzip compressed data, was "syncmaster-0.0.3.tar", last modified: Mon Apr 17 15:29:53 2023, max compression
```

## Comparing `syncmaster-0.0.2.tar` & `syncmaster-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 conor     (1000) conor     (1000)        0 2023-04-17 11:01:24.194955 syncmaster-0.0.2/
--rw-rw-r--   0 conor     (1000) conor     (1000)    11337 2023-01-20 02:50:04.000000 syncmaster-0.0.2/LICENSE
--rw-rw-r--   0 conor     (1000) conor     (1000)      111 2023-01-20 02:50:04.000000 syncmaster-0.0.2/MANIFEST.in
--rw-rw-r--   0 conor     (1000) conor     (1000)     1157 2023-04-17 11:01:24.194955 syncmaster-0.0.2/PKG-INFO
--rw-rw-r--   0 conor     (1000) conor     (1000)      305 2023-04-17 09:38:04.000000 syncmaster-0.0.2/README.md
--rw-rw-r--   0 conor     (1000) conor     (1000)      929 2023-04-17 11:01:17.000000 syncmaster-0.0.2/settings.ini
--rw-rw-r--   0 conor     (1000) conor     (1000)       38 2023-04-17 11:01:24.194955 syncmaster-0.0.2/setup.cfg
--rw-rw-r--   0 conor     (1000) conor     (1000)     2560 2023-01-20 02:50:04.000000 syncmaster-0.0.2/setup.py
-drwxrwxr-x   0 conor     (1000) conor     (1000)        0 2023-04-17 11:01:24.190955 syncmaster-0.0.2/syncmaster/
--rw-rw-r--   0 conor     (1000) conor     (1000)      223 2023-04-17 11:01:17.000000 syncmaster-0.0.2/syncmaster/__init__.py
--rw-rw-r--   0 conor     (1000) conor     (1000)     1688 2023-04-17 11:01:17.000000 syncmaster-0.0.2/syncmaster/_modidx.py
--rw-rw-r--   0 conor     (1000) conor     (1000)     2309 2023-04-17 11:01:17.000000 syncmaster-0.0.2/syncmaster/analysis.py
--rw-rw-r--   0 conor     (1000) conor     (1000)     3275 2023-04-17 11:01:17.000000 syncmaster-0.0.2/syncmaster/device.py
-drwxrwxr-x   0 conor     (1000) conor     (1000)        0 2023-04-17 11:01:24.194955 syncmaster-0.0.2/syncmaster.egg-info/
--rw-rw-r--   0 conor     (1000) conor     (1000)     1157 2023-04-17 11:01:24.000000 syncmaster-0.0.2/syncmaster.egg-info/PKG-INFO
--rw-rw-r--   0 conor     (1000) conor     (1000)      379 2023-04-17 11:01:24.000000 syncmaster-0.0.2/syncmaster.egg-info/SOURCES.txt
--rw-rw-r--   0 conor     (1000) conor     (1000)        1 2023-04-17 11:01:24.000000 syncmaster-0.0.2/syncmaster.egg-info/dependency_links.txt
--rw-rw-r--   0 conor     (1000) conor     (1000)       42 2023-04-17 11:01:24.000000 syncmaster-0.0.2/syncmaster.egg-info/entry_points.txt
--rw-rw-r--   0 conor     (1000) conor     (1000)        1 2023-04-17 10:19:07.000000 syncmaster-0.0.2/syncmaster.egg-info/not-zip-safe
--rw-rw-r--   0 conor     (1000) conor     (1000)       41 2023-04-17 11:01:24.000000 syncmaster-0.0.2/syncmaster.egg-info/requires.txt
--rw-rw-r--   0 conor     (1000) conor     (1000)       11 2023-04-17 11:01:24.000000 syncmaster-0.0.2/syncmaster.egg-info/top_level.txt
+drwxrwxr-x   0 conor     (1000) conor     (1000)        0 2023-04-17 15:29:53.704179 syncmaster-0.0.3/
+-rw-rw-r--   0 conor     (1000) conor     (1000)    11337 2023-01-20 02:50:04.000000 syncmaster-0.0.3/LICENSE
+-rw-rw-r--   0 conor     (1000) conor     (1000)      111 2023-01-20 02:50:04.000000 syncmaster-0.0.3/MANIFEST.in
+-rw-rw-r--   0 conor     (1000) conor     (1000)     3262 2023-04-17 15:29:53.704179 syncmaster-0.0.3/PKG-INFO
+-rw-rw-r--   0 conor     (1000) conor     (1000)     2410 2023-04-17 14:44:42.000000 syncmaster-0.0.3/README.md
+-rw-rw-r--   0 conor     (1000) conor     (1000)      934 2023-04-17 15:29:41.000000 syncmaster-0.0.3/settings.ini
+-rw-rw-r--   0 conor     (1000) conor     (1000)       38 2023-04-17 15:29:53.704179 syncmaster-0.0.3/setup.cfg
+-rw-rw-r--   0 conor     (1000) conor     (1000)     2560 2023-01-20 02:50:04.000000 syncmaster-0.0.3/setup.py
+drwxrwxr-x   0 conor     (1000) conor     (1000)        0 2023-04-17 15:29:53.704179 syncmaster-0.0.3/syncmaster/
+-rw-rw-r--   0 conor     (1000) conor     (1000)      235 2023-04-17 15:29:41.000000 syncmaster-0.0.3/syncmaster/__init__.py
+-rw-rw-r--   0 conor     (1000) conor     (1000)     1918 2023-04-17 15:29:41.000000 syncmaster-0.0.3/syncmaster/_modidx.py
+-rw-rw-r--   0 conor     (1000) conor     (1000)     2418 2023-04-17 15:29:41.000000 syncmaster-0.0.3/syncmaster/analysis.py
+-rw-rw-r--   0 conor     (1000) conor     (1000)     3523 2023-04-17 15:29:41.000000 syncmaster-0.0.3/syncmaster/device.py
+drwxrwxr-x   0 conor     (1000) conor     (1000)        0 2023-04-17 15:29:53.704179 syncmaster-0.0.3/syncmaster.egg-info/
+-rw-rw-r--   0 conor     (1000) conor     (1000)     3262 2023-04-17 15:29:53.000000 syncmaster-0.0.3/syncmaster.egg-info/PKG-INFO
+-rw-rw-r--   0 conor     (1000) conor     (1000)      379 2023-04-17 15:29:53.000000 syncmaster-0.0.3/syncmaster.egg-info/SOURCES.txt
+-rw-rw-r--   0 conor     (1000) conor     (1000)        1 2023-04-17 15:29:53.000000 syncmaster-0.0.3/syncmaster.egg-info/dependency_links.txt
+-rw-rw-r--   0 conor     (1000) conor     (1000)       42 2023-04-17 15:29:53.000000 syncmaster-0.0.3/syncmaster.egg-info/entry_points.txt
+-rw-rw-r--   0 conor     (1000) conor     (1000)        1 2023-04-17 10:19:07.000000 syncmaster-0.0.3/syncmaster.egg-info/not-zip-safe
+-rw-rw-r--   0 conor     (1000) conor     (1000)       46 2023-04-17 15:29:53.000000 syncmaster-0.0.3/syncmaster.egg-info/requires.txt
+-rw-rw-r--   0 conor     (1000) conor     (1000)       11 2023-04-17 15:29:53.000000 syncmaster-0.0.3/syncmaster.egg-info/top_level.txt
```

### Comparing `syncmaster-0.0.2/LICENSE` & `syncmaster-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `syncmaster-0.0.2/settings.ini` & `syncmaster-0.0.3/settings.ini`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = syncmaster
 lib_name = syncmaster
-version = 0.0.2
+version = 0.0.3
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = syncmaster
 nbs_path = nbs
 recursive = True
@@ -22,15 +22,15 @@
 author_email = conor.keogh@nds.ox.ac.uk
 copyright = 2023 onwards, Conor Keogh
 description = Device and drivers for generating trigger signals to synchronise recorded signals with behavioural data
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
 user = conorkeogh
-requirements = numpy pyserial matplotlib seaborn
+requirements = numpy pyserial matplotlib seaborn time
 readme_nb = index.ipynb
 allowed_metadata_keys = 
 allowed_cell_metadata_keys = 
 jupyter_hooks = True
 clean_ids = True
 clear_all = False
```

### Comparing `syncmaster-0.0.2/setup.py` & `syncmaster-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `syncmaster-0.0.2/syncmaster/_modidx.py` & `syncmaster-0.0.3/syncmaster/_modidx.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,8 +11,10 @@
                                                                               'syncmaster/device.py'),
                                    'syncmaster.device.SyncMaster.close': ('initialisation.html#syncmaster.close', 'syncmaster/device.py'),
                                    'syncmaster.device.SyncMaster.end': ('initialisation.html#syncmaster.end', 'syncmaster/device.py'),
                                    'syncmaster.device.SyncMaster.event1': ('initialisation.html#syncmaster.event1', 'syncmaster/device.py'),
                                    'syncmaster.device.SyncMaster.event2': ('initialisation.html#syncmaster.event2', 'syncmaster/device.py'),
                                    'syncmaster.device.SyncMaster.sendMessage': ( 'initialisation.html#syncmaster.sendmessage',
                                                                                  'syncmaster/device.py'),
-                                   'syncmaster.device.SyncMaster.start': ('initialisation.html#syncmaster.start', 'syncmaster/device.py')}}}
+                                   'syncmaster.device.SyncMaster.start': ('initialisation.html#syncmaster.start', 'syncmaster/device.py'),
+                                   'syncmaster.device.SyncMaster.testSignal': ( 'initialisation.html#syncmaster.testsignal',
+                                                                                'syncmaster/device.py')}}}
```

### Comparing `syncmaster-0.0.2/syncmaster/analysis.py` & `syncmaster-0.0.3/syncmaster/analysis.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/04_events.ipynb.
 
 # %% auto 0
 __all__ = ['getEvents']
 
 # %% ../nbs/04_events.ipynb 3
+import numpy as np
+from matplotlib import pyplot as plt
+import seaborn as sns
+
+# %% ../nbs/04_events.ipynb 5
 # Process data
 def getEvents(data, samplerate):
     '''
     Recover event timings
     Args:
         data: 1d array containing event signals recorded at each timepoint
         samplerate: samplerate of recording (Hz)
```

### Comparing `syncmaster-0.0.2/syncmaster/device.py` & `syncmaster-0.0.3/syncmaster/device.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 SyncMaster device class
 Provide functions to interact with device
 Finds device and confirms presence
 Sends messages to trigger device
 '''
 import serial
 import serial.tools.list_ports
+import time
 
 class SyncMaster:
 
     def __init__(self):
         '''
         Find device and check acknowledge message
         Finds device on USB port automatically
@@ -117,7 +118,16 @@
     # Close channel
     def close(self):
         '''
         Closes serial connection
         Should be run before shutting off device
         '''
         self.ser.close()
+        
+    # Send test signal
+    def testSignal(self):
+        '''
+        Sends test pulses over output port once per second for five seconds
+        '''
+        for _ in range(5):
+            self.start()
+            time.sleep(1)
```

