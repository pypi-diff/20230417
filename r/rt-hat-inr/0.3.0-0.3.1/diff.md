# Comparing `tmp/rt-hat-inr-0.3.0.tar.gz` & `tmp/rt-hat-inr-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/var/lib/jenkins/workspace/Publish_rpi_python/rpi_python/dist/tmp5hg_pcbk/rt-hat-inr-0.3.0.tar", last modified: Sun Jan  8 18:19:06 2023, max compression
+gzip compressed data, was "/var/lib/jenkins/workspace/Publish_rpi_python/rpi_python/dist/tmppr21nn3d/rt-hat-inr-0.3.1.tar", last modified: Mon Apr 17 20:17:52 2023, max compression
```

## Comparing `rt-hat-inr-0.3.0.tar` & `rt-hat-inr-0.3.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-01-08 18:19:06.000000 rt-hat-inr-0.3.0/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1029 2023-01-08 18:18:55.000000 rt-hat-inr-0.3.0/setup.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      984 2023-01-08 18:19:06.000000 rt-hat-inr-0.3.0/PKG-INFO
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-01-08 18:19:06.000000 rt-hat-inr-0.3.0/src/
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-01-08 18:19:06.000000 rt-hat-inr-0.3.0/src/rt_hat_inr.egg-info/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      984 2023-01-08 18:19:06.000000 rt-hat-inr-0.3.0/src/rt_hat_inr.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        1 2023-01-08 18:19:06.000000 rt-hat-inr-0.3.0/src/rt_hat_inr.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        7 2023-01-08 18:19:06.000000 rt-hat-inr-0.3.0/src/rt_hat_inr.egg-info/top_level.txt
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       40 2023-01-08 18:19:06.000000 rt-hat-inr-0.3.0/src/rt_hat_inr.egg-info/requires.txt
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      416 2023-01-08 18:19:06.000000 rt-hat-inr-0.3.0/src/rt_hat_inr.egg-info/SOURCES.txt
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-01-08 18:19:06.000000 rt-hat-inr-0.3.0/src/rt_hat/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2260 2023-01-08 18:18:55.000000 rt-hat-inr-0.3.0/src/rt_hat/SIGGEN.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2023-01-08 18:18:55.000000 rt-hat-inr-0.3.0/src/rt_hat/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2023-01-08 18:18:55.000000 rt-hat-inr-0.3.0/src/rt_hat/FLOWCACHE.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8135 2023-01-08 18:18:55.000000 rt-hat-inr-0.3.0/src/rt_hat/TAS.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5762 2023-01-08 18:18:55.000000 rt-hat-inr-0.3.0/src/rt_hat/FPGA.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       38 2023-01-08 18:19:06.000000 rt-hat-inr-0.3.0/setup.cfg
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-01-08 18:19:06.000000 rt-hat-inr-0.3.0/bin/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      297 2023-01-08 18:18:55.000000 rt-hat-inr-0.3.0/bin/INR_FPGA_status
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)     3183 2023-01-08 18:18:55.000000 rt-hat-inr-0.3.0/bin/INR_change_bitstream
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)     2176 2023-01-08 18:18:55.000000 rt-hat-inr-0.3.0/bin/INR-config
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      568 2023-01-08 18:18:55.000000 rt-hat-inr-0.3.0/bin/INR_FPGA_license
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      446 2023-01-08 18:18:55.000000 rt-hat-inr-0.3.0/README.md
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      104 2023-01-08 18:18:55.000000 rt-hat-inr-0.3.0/pyproject.toml
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    35071 2023-01-08 18:18:55.000000 rt-hat-inr-0.3.0/LICENSE
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-17 20:17:52.000000 rt-hat-inr-0.3.1/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1029 2023-04-17 20:17:32.000000 rt-hat-inr-0.3.1/setup.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      984 2023-04-17 20:17:52.000000 rt-hat-inr-0.3.1/PKG-INFO
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-17 20:17:52.000000 rt-hat-inr-0.3.1/src/
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-17 20:17:52.000000 rt-hat-inr-0.3.1/src/rt_hat_inr.egg-info/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      984 2023-04-17 20:17:52.000000 rt-hat-inr-0.3.1/src/rt_hat_inr.egg-info/PKG-INFO
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        1 2023-04-17 20:17:52.000000 rt-hat-inr-0.3.1/src/rt_hat_inr.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        7 2023-04-17 20:17:52.000000 rt-hat-inr-0.3.1/src/rt_hat_inr.egg-info/top_level.txt
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       40 2023-04-17 20:17:52.000000 rt-hat-inr-0.3.1/src/rt_hat_inr.egg-info/requires.txt
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      416 2023-04-17 20:17:52.000000 rt-hat-inr-0.3.1/src/rt_hat_inr.egg-info/SOURCES.txt
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-17 20:17:52.000000 rt-hat-inr-0.3.1/src/rt_hat/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2260 2023-04-17 20:17:32.000000 rt-hat-inr-0.3.1/src/rt_hat/SIGGEN.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2023-04-17 20:17:32.000000 rt-hat-inr-0.3.1/src/rt_hat/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2023-04-17 20:17:32.000000 rt-hat-inr-0.3.1/src/rt_hat/FLOWCACHE.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8135 2023-04-17 20:17:32.000000 rt-hat-inr-0.3.1/src/rt_hat/TAS.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5762 2023-04-17 20:17:32.000000 rt-hat-inr-0.3.1/src/rt_hat/FPGA.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       38 2023-04-17 20:17:52.000000 rt-hat-inr-0.3.1/setup.cfg
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-17 20:17:52.000000 rt-hat-inr-0.3.1/bin/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      297 2023-04-17 20:17:32.000000 rt-hat-inr-0.3.1/bin/INR_FPGA_status
+-rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)     3220 2023-04-17 20:17:32.000000 rt-hat-inr-0.3.1/bin/INR_change_bitstream
+-rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)     2176 2023-04-17 20:17:32.000000 rt-hat-inr-0.3.1/bin/INR-config
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      568 2023-04-17 20:17:32.000000 rt-hat-inr-0.3.1/bin/INR_FPGA_license
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      446 2023-04-17 20:17:32.000000 rt-hat-inr-0.3.1/README.md
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      104 2023-04-17 20:17:32.000000 rt-hat-inr-0.3.1/pyproject.toml
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    35071 2023-04-17 20:17:32.000000 rt-hat-inr-0.3.1/LICENSE
```

### Comparing `rt-hat-inr-0.3.0/setup.py` & `rt-hat-inr-0.3.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rt-hat-inr", # Replace with your own username
-    version="0.3.0",
+    version="0.3.1",
     author="Marian Ulbricht",
     author_email="ulbricht@innoroute.de",
     description="RealtimeHAT control",
     long_description=long_description,
     install_requires=[
    'npyscreen',
    'wget',
```

### Comparing `rt-hat-inr-0.3.0/PKG-INFO` & `rt-hat-inr-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rt-hat-inr
-Version: 0.3.0
+Version: 0.3.1
 Summary: RealtimeHAT control
 Home-page: https://github.com/InnoRoute/RealtimeHAT
 Author: Marian Ulbricht
 Author-email: ulbricht@innoroute.de
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/InnoRoute/RealtimeHAT/issues
 Platform: UNKNOWN
```

### Comparing `rt-hat-inr-0.3.0/src/rt_hat_inr.egg-info/PKG-INFO` & `rt-hat-inr-0.3.1/src/rt_hat_inr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rt-hat-inr
-Version: 0.3.0
+Version: 0.3.1
 Summary: RealtimeHAT control
 Home-page: https://github.com/InnoRoute/RealtimeHAT
 Author: Marian Ulbricht
 Author-email: ulbricht@innoroute.de
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/InnoRoute/RealtimeHAT/issues
 Platform: UNKNOWN
```

### Comparing `rt-hat-inr-0.3.0/src/rt_hat/SIGGEN.py` & `rt-hat-inr-0.3.1/src/rt_hat/SIGGEN.py`

 * *Files identical despite different names*

### Comparing `rt-hat-inr-0.3.0/src/rt_hat/TAS.py` & `rt-hat-inr-0.3.1/src/rt_hat/TAS.py`

 * *Files identical despite different names*

### Comparing `rt-hat-inr-0.3.0/src/rt_hat/FPGA.py` & `rt-hat-inr-0.3.1/src/rt_hat/FPGA.py`

 * *Files identical despite different names*

### Comparing `rt-hat-inr-0.3.0/bin/INR_change_bitstream` & `rt-hat-inr-0.3.1/bin/INR_change_bitstream`

 * *Files 14% similar despite different names*

```diff
@@ -7,20 +7,21 @@
 from configobj import ConfigObj
 import os
 import sys
 from rt_hat import FPGA as RT_HAT_FPGA
 
 selected=""
 modes={"Default":"_uc0",
+"EKS TSN-Analyser":"_uc1_TSN_EP",
 "Packet Generator":"_uc1",
 "Single Port TSN Endpoint":"_uc2",
 "TSN Mediaconverter":"_uc3",
 "TSN TAP 1G Analyzer Lite":"_uc4",
 "Switched TSN Endpoint":"_uc5"}
-tbi=["_uc1","_uc2""_uc3""_uc4""_uc5"]
+tbi=["_uc1","_uc2","_uc3","_uc4","_uc5"]
 
 def is_root():
     return os.geteuid() == 0
 				
 class TestApp(npyscreen.NPSApp):
     def main(self):
         global selected
```

### Comparing `rt-hat-inr-0.3.0/bin/INR-config` & `rt-hat-inr-0.3.1/bin/INR-config`

 * *Files identical despite different names*

### Comparing `rt-hat-inr-0.3.0/bin/INR_FPGA_license` & `rt-hat-inr-0.3.1/bin/INR_FPGA_license`

 * *Files identical despite different names*

### Comparing `rt-hat-inr-0.3.0/LICENSE` & `rt-hat-inr-0.3.1/LICENSE`

 * *Files identical despite different names*

