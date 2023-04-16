# Comparing `tmp/tinytuya-1.9.0-py2.py3-none-any.whl.zip` & `tmp/tinytuya-1.9.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,24 @@
-Zip file size: 92229 bytes, number of entries: 22
+Zip file size: 92230 bytes, number of entries: 22
 -rw-r--r--  2.0 unx    24084 b- defN 22-Oct-31 23:49 tinytuya/BulbDevice.py
--rw-r--r--  2.0 unx    20805 b- defN 22-Dec-03 04:11 tinytuya/Cloud.py
+-rw-r--r--  2.0 unx    20829 b- defN 22-Dec-03 05:26 tinytuya/Cloud.py
 -rw-r--r--  2.0 unx     2845 b- defN 22-Oct-05 04:48 tinytuya/CoverDevice.py
 -rw-r--r--  2.0 unx     3716 b- defN 22-Oct-05 04:48 tinytuya/OutletDevice.py
 -rw-r--r--  2.0 unx     4669 b- defN 22-Oct-05 04:48 tinytuya/__init__.py
 -rw-r--r--  2.0 unx     2699 b- defN 22-Jun-15 03:25 tinytuya/__main__.py
--rw-r--r--  2.0 unx    65557 b- defN 22-Dec-03 04:30 tinytuya/core.py
+-rw-r--r--  2.0 unx    65557 b- defN 22-Dec-03 05:34 tinytuya/core.py
 -rw-r--r--  2.0 unx    27029 b- defN 22-Aug-13 15:26 tinytuya/scanner.py
 -rw-r--r--  2.0 unx     8943 b- defN 22-Jun-16 05:14 tinytuya/ui.py
--rw-r--r--  2.0 unx    13545 b- defN 22-Dec-03 04:11 tinytuya/wizard.py
+-rw-r--r--  2.0 unx    13545 b- defN 22-Dec-03 05:09 tinytuya/wizard.py
 -rw-r--r--  2.0 unx     4958 b- defN 22-Nov-22 17:42 tinytuya/Contrib/AtorchTemperatureControllerDevice.py
 -rw-r--r--  2.0 unx     5438 b- defN 22-Oct-31 23:49 tinytuya/Contrib/ClimateDevice.py
 -rw-r--r--  2.0 unx     5479 b- defN 22-Oct-05 04:48 tinytuya/Contrib/DoorbellDevice.py
 -rw-r--r--  2.0 unx    54567 b- defN 22-Dec-03 04:11 tinytuya/Contrib/IRRemoteControlDevice.py
 -rw-r--r--  2.0 unx     3362 b- defN 22-Oct-05 04:48 tinytuya/Contrib/SocketDevice.py
 -rw-r--r--  2.0 unx    48837 b- defN 22-Dec-03 04:11 tinytuya/Contrib/ThermostatDevice.py
 -rw-r--r--  2.0 unx      458 b- defN 22-Nov-22 17:42 tinytuya/Contrib/__init__.py
--rw-r--r--  2.0 unx     1066 b- defN 22-Dec-03 04:52 tinytuya-1.9.0.dist-info/LICENSE
--rw-r--r--  2.0 unx    40368 b- defN 22-Dec-03 04:52 tinytuya-1.9.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 22-Dec-03 04:52 tinytuya-1.9.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 22-Dec-03 04:52 tinytuya-1.9.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1817 b- defN 22-Dec-03 04:52 tinytuya-1.9.0.dist-info/RECORD
-22 files, 340361 bytes uncompressed, 89307 bytes compressed:  73.8%
+-rw-r--r--  2.0 unx     1066 b- defN 22-Dec-03 05:47 tinytuya-1.9.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx    40368 b- defN 22-Dec-03 05:47 tinytuya-1.9.1.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 22-Dec-03 05:47 tinytuya-1.9.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 22-Dec-03 05:47 tinytuya-1.9.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1817 b- defN 22-Dec-03 05:47 tinytuya-1.9.1.dist-info/RECORD
+22 files, 340385 bytes uncompressed, 89308 bytes compressed:  73.8%
```

## zipnote {}

```diff
@@ -45,23 +45,23 @@
 
 Filename: tinytuya/Contrib/ThermostatDevice.py
 Comment: 
 
 Filename: tinytuya/Contrib/__init__.py
 Comment: 
 
-Filename: tinytuya-1.9.0.dist-info/LICENSE
+Filename: tinytuya-1.9.1.dist-info/LICENSE
 Comment: 
 
-Filename: tinytuya-1.9.0.dist-info/METADATA
+Filename: tinytuya-1.9.1.dist-info/METADATA
 Comment: 
 
-Filename: tinytuya-1.9.0.dist-info/WHEEL
+Filename: tinytuya-1.9.1.dist-info/WHEEL
 Comment: 
 
-Filename: tinytuya-1.9.0.dist-info/top_level.txt
+Filename: tinytuya-1.9.1.dist-info/top_level.txt
 Comment: 
 
-Filename: tinytuya-1.9.0.dist-info/RECORD
+Filename: tinytuya-1.9.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tinytuya/Cloud.py

```diff
@@ -248,15 +248,15 @@
             )
             return self.error
 
         if 't' in response_dict:
             # round it to 2 minutes to try and factor out any processing delays
             self.server_time_offset = round( ((response_dict['t'] / 1000.0) - time.time()) / 120 )
             self.server_time_offset *= 120
-            log.warning(self.server_time_offset)
+            log.debug("server_time_offset: %r", self.server_time_offset)
 
         self.token = response_dict['result']['access_token']
         return self.token
 
     def _getuid(self, deviceid=None):
         # Get user ID (UID) for deviceid
         if not self.token:
```

## tinytuya/core.py

```diff
@@ -79,15 +79,15 @@
 except ImportError:
     Crypto = AES = None
     import pyaes  # https://github.com/ricmoo/pyaes
 
 # Colorama terminal color capability for all platforms
 init()
 
-version_tuple = (1, 9, 0)
+version_tuple = (1, 9, 1)
 version = __version__ = "%d.%d.%d" % version_tuple
 __author__ = "jasonacox"
 
 log = logging.getLogger(__name__)
 # Uncomment the following to set debug mode or call set_debug()
 # logging.basicConfig(level=logging.DEBUG)
```

## Comparing `tinytuya-1.9.0.dist-info/LICENSE` & `tinytuya-1.9.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tinytuya-1.9.0.dist-info/METADATA` & `tinytuya-1.9.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinytuya
-Version: 1.9.0
+Version: 1.9.1
 Summary: Python module to interface with Tuya WiFi smart devices
 Home-page: https://github.com/jasonacox/tinytuya
 Author: Jason Cox
 Author-email: jason@jasonacox.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2
```

## Comparing `tinytuya-1.9.0.dist-info/RECORD` & `tinytuya-1.9.1.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 tinytuya/BulbDevice.py,sha256=RI0eV9NaiTh5Ep-1GGnUiCOgNN2SaXa_cwmo1F5kIjw,24084
-tinytuya/Cloud.py,sha256=IPu_T4A5aiTLorDyENT9sxYqUN4B3fF7-kIpAYZc1sU,20805
+tinytuya/Cloud.py,sha256=d7w4cw1ArAfiv81TQqUeuj3PtPKIlnhGuf1GcGD3Jdk,20829
 tinytuya/CoverDevice.py,sha256=-Yu7eCcu3Bcqpsyh1MmXzhfnjxG2WcDjw3FtbBes5DQ,2845
 tinytuya/OutletDevice.py,sha256=sJZsuNmCRxFj1j_8O1S9yJ_CdaTKwxWQ2icBDTIgs90,3716
 tinytuya/__init__.py,sha256=XIzq4o7qW0G23N57uJFJeyh3rEc0qFtul6ZbfDRSZ5g,4669
 tinytuya/__main__.py,sha256=5nZbadiw9Xf4mIrlGoToAmsXyqeC4FR1Qlw23gL13KA,2699
-tinytuya/core.py,sha256=ZbS_zA--O8q2YZXzXFq-pFTClLQjXO_lV9xNkcRE5Rc,65557
+tinytuya/core.py,sha256=WqWYe1RMXtC6IdL_7MvT0Q-tW8zIgr1URjnGtPudpLc,65557
 tinytuya/scanner.py,sha256=JQE0INEqkrtUGDb_K1fwa8n-LApO22Rg71a9JxXLus0,27029
 tinytuya/ui.py,sha256=vGQDplI2cAXtwcBj9XkMJ1kY-0TV3Zf6E94c97KVyUY,8943
 tinytuya/wizard.py,sha256=xDpN_2HabCW3TZy-tu30nC5X1qdy_wOkxEVOcD9V-xI,13545
 tinytuya/Contrib/AtorchTemperatureControllerDevice.py,sha256=v5Jrkfm0hepIGYwOWfXPZaniflQrbZjokokMc7HuGFg,4958
 tinytuya/Contrib/ClimateDevice.py,sha256=eppLANTv6DrSp3B8YM28kGIWE5SN5AoZVqcldgyx6is,5438
 tinytuya/Contrib/DoorbellDevice.py,sha256=aJP4LflgZxqaS9P9PWRdHT2GH1-3_ZxDIRH0PHrCr9Q,5479
 tinytuya/Contrib/IRRemoteControlDevice.py,sha256=t0rS5a9sASvqx8yer933HMIiiV8y_AeJDnD_nApZtWU,54567
 tinytuya/Contrib/SocketDevice.py,sha256=YluDRFC2BZmOjE6Rhai1cUrmJ3HzJJYi4BpPDFX1fgE,3362
 tinytuya/Contrib/ThermostatDevice.py,sha256=5EE5atA_n56TD3j3-raLspeXJfWl4NFgeKASALC7pUw,48837
 tinytuya/Contrib/__init__.py,sha256=tBo_yn9cW0wVC7fwxCZb6eOczhH9FUuzRHlY1LJr068,458
-tinytuya-1.9.0.dist-info/LICENSE,sha256=R8Su4NDXT7jqnIWgOSEyVBcFwgA60f-usg6zmv6Fp24,1066
-tinytuya-1.9.0.dist-info/METADATA,sha256=epYAA033iotIs-E4zVuy0yfpO0pV2AFO7HOofPOkD5s,40368
-tinytuya-1.9.0.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
-tinytuya-1.9.0.dist-info/top_level.txt,sha256=y8SLa0YK1csUy1uxMQGryQFyjIW5V9egIGu6stWM67U,9
-tinytuya-1.9.0.dist-info/RECORD,,
+tinytuya-1.9.1.dist-info/LICENSE,sha256=R8Su4NDXT7jqnIWgOSEyVBcFwgA60f-usg6zmv6Fp24,1066
+tinytuya-1.9.1.dist-info/METADATA,sha256=E8kfab7lCfOhAdWLAc_uJfK7MfZUCoSQK3t7vnoiPhg,40368
+tinytuya-1.9.1.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
+tinytuya-1.9.1.dist-info/top_level.txt,sha256=y8SLa0YK1csUy1uxMQGryQFyjIW5V9egIGu6stWM67U,9
+tinytuya-1.9.1.dist-info/RECORD,,
```

