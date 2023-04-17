# Comparing `tmp/socketscpi-2022.8.0.tar.gz` & `tmp/socketscpi-2023.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socketscpi-2022.8.0.tar", last modified: Thu Aug 11 20:42:34 2022, max compression
+gzip compressed data, was "socketscpi-2023.4.0.tar", last modified: Mon Apr 17 20:25:38 2023, max compression
```

## Comparing `socketscpi-2022.8.0.tar` & `socketscpi-2023.4.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2022-08-11 20:42:34.888574 socketscpi-2022.8.0/
--rw-rw-rw-   0        0        0      179 2021-05-06 23:00:54.000000 socketscpi-2022.8.0/AUTHORS.rst
--rw-rw-rw-   0        0        0     3718 2021-05-06 23:00:54.000000 socketscpi-2022.8.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     1080 2021-05-06 23:00:54.000000 socketscpi-2022.8.0/LICENSE
--rw-rw-rw-   0        0        0      273 2021-05-06 23:00:54.000000 socketscpi-2022.8.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2020 2022-08-11 20:42:34.888574 socketscpi-2022.8.0/PKG-INFO
--rw-rw-rw-   0        0        0     1171 2022-08-11 20:38:31.000000 socketscpi-2022.8.0/README.rst
-drwxrwxrwx   0        0        0        0 2022-08-11 20:42:34.841574 socketscpi-2022.8.0/docs/
--rw-rw-rw-   0        0        0      631 2021-05-06 23:00:54.000000 socketscpi-2022.8.0/docs/Makefile
-drwxrwxrwx   0        0        0        0 2022-08-11 20:42:34.698590 socketscpi-2022.8.0/docs/_build/
-drwxrwxrwx   0        0        0        0 2022-08-11 20:42:34.701581 socketscpi-2022.8.0/docs/_build/html/
-drwxrwxrwx   0        0        0        0 2022-08-11 20:42:34.852575 socketscpi-2022.8.0/docs/_build/html/_static/
--rw-rw-rw-   0        0        0      286 2022-08-11 20:34:12.000000 socketscpi-2022.8.0/docs/_build/html/_static/file.png
--rw-rw-rw-   0        0        0       90 2022-08-11 20:34:12.000000 socketscpi-2022.8.0/docs/_build/html/_static/minus.png
--rw-rw-rw-   0        0        0       90 2022-08-11 20:34:12.000000 socketscpi-2022.8.0/docs/_build/html/_static/plus.png
--rw-rw-rw-   0        0        0       29 2021-05-06 23:00:54.000000 socketscpi-2022.8.0/docs/authors.rst
--rw-rw-rw-   0        0        0     5020 2021-05-06 23:00:54.000000 socketscpi-2022.8.0/docs/conf.py
--rw-rw-rw-   0        0        0       34 2021-05-06 23:00:54.000000 socketscpi-2022.8.0/docs/contributing.rst
--rw-rw-rw-   0        0        0      837 2022-08-11 20:35:34.000000 socketscpi-2022.8.0/docs/history.rst
--rw-rw-rw-   0        0        0      315 2021-05-06 23:00:54.000000 socketscpi-2022.8.0/docs/index.rst
--rw-rw-rw-   0        0        0     1229 2021-05-06 23:00:54.000000 socketscpi-2022.8.0/docs/installation.rst
--rwxrwxrwx   0        0        0      808 2021-05-06 23:00:54.000000 socketscpi-2022.8.0/docs/make.bat
--rw-rw-rw-   0        0        0       28 2021-05-06 23:00:54.000000 socketscpi-2022.8.0/docs/readme.rst
--rw-rw-rw-   0        0        0     4345 2022-08-11 20:34:55.000000 socketscpi-2022.8.0/docs/usage.rst
--rw-rw-rw-   0        0        0       95 2021-07-09 19:46:58.000000 socketscpi-2022.8.0/pyproject.toml
--rw-rw-rw-   0        0        0     1297 2022-08-11 20:42:34.892576 socketscpi-2022.8.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-08-11 20:42:34.860579 socketscpi-2022.8.0/socketscpi/
--rw-rw-rw-   0        0        0      163 2022-08-11 20:38:44.000000 socketscpi-2022.8.0/socketscpi/__init__.py
--rw-rw-rw-   0        0        0    13109 2022-08-11 19:24:28.000000 socketscpi-2022.8.0/socketscpi/socketscpi.py
-drwxrwxrwx   0        0        0        0 2022-08-11 20:42:34.878586 socketscpi-2022.8.0/socketscpi.egg-info/
--rw-rw-rw-   0        0        0     2020 2022-08-11 20:42:34.000000 socketscpi-2022.8.0/socketscpi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      612 2022-08-11 20:42:34.000000 socketscpi-2022.8.0/socketscpi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-11 20:42:34.000000 socketscpi-2022.8.0/socketscpi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2022-08-11 20:42:34.000000 socketscpi-2022.8.0/socketscpi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2022-08-11 20:42:34.000000 socketscpi-2022.8.0/socketscpi.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-08-11 20:42:34.885576 socketscpi-2022.8.0/tests/
--rw-rw-rw-   0        0        0       68 2021-05-06 23:00:54.000000 socketscpi-2022.8.0/tests/__init__.py
--rw-rw-rw-   0        0        0      887 2021-05-06 23:00:54.000000 socketscpi-2022.8.0/tests/test_socketscpi.py
+drwxrwxrwx   0        0        0        0 2023-04-17 20:25:38.463078 socketscpi-2023.4.0/
+-rw-rw-rw-   0        0        0      179 2021-05-06 23:00:54.000000 socketscpi-2023.4.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3718 2021-05-06 23:00:54.000000 socketscpi-2023.4.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     1080 2021-05-06 23:00:54.000000 socketscpi-2023.4.0/LICENSE
+-rw-rw-rw-   0        0        0      273 2021-05-06 23:00:54.000000 socketscpi-2023.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2020 2023-04-17 20:25:38.464077 socketscpi-2023.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1171 2023-04-17 20:14:12.000000 socketscpi-2023.4.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-17 20:25:38.415079 socketscpi-2023.4.0/docs/
+-rw-rw-rw-   0        0        0      631 2021-05-06 23:00:54.000000 socketscpi-2023.4.0/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-04-17 20:25:38.352080 socketscpi-2023.4.0/docs/_build/
+drwxrwxrwx   0        0        0        0 2023-04-17 20:25:38.353077 socketscpi-2023.4.0/docs/_build/html/
+drwxrwxrwx   0        0        0        0 2023-04-17 20:25:38.426083 socketscpi-2023.4.0/docs/_build/html/_static/
+-rw-rw-rw-   0        0        0      286 2022-08-11 20:34:12.000000 socketscpi-2023.4.0/docs/_build/html/_static/file.png
+-rw-rw-rw-   0        0        0       90 2022-08-11 20:34:12.000000 socketscpi-2023.4.0/docs/_build/html/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2022-08-11 20:34:12.000000 socketscpi-2023.4.0/docs/_build/html/_static/plus.png
+-rw-rw-rw-   0        0        0       29 2021-05-06 23:00:54.000000 socketscpi-2023.4.0/docs/authors.rst
+-rw-rw-rw-   0        0        0     5020 2021-05-06 23:00:54.000000 socketscpi-2023.4.0/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2021-05-06 23:00:54.000000 socketscpi-2023.4.0/docs/contributing.rst
+-rw-rw-rw-   0        0        0     1063 2023-04-17 20:11:11.000000 socketscpi-2023.4.0/docs/history.rst
+-rw-rw-rw-   0        0        0      315 2021-05-06 23:00:54.000000 socketscpi-2023.4.0/docs/index.rst
+-rw-rw-rw-   0        0        0     1229 2021-05-06 23:00:54.000000 socketscpi-2023.4.0/docs/installation.rst
+-rwxrwxrwx   0        0        0      808 2021-05-06 23:00:54.000000 socketscpi-2023.4.0/docs/make.bat
+-rw-rw-rw-   0        0        0       28 2021-05-06 23:00:54.000000 socketscpi-2023.4.0/docs/readme.rst
+-rw-rw-rw-   0        0        0     4599 2023-04-17 20:12:40.000000 socketscpi-2023.4.0/docs/usage.rst
+-rw-rw-rw-   0        0        0       95 2021-07-09 19:46:58.000000 socketscpi-2023.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1297 2023-04-17 20:25:38.466079 socketscpi-2023.4.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-17 20:25:38.434079 socketscpi-2023.4.0/socketscpi/
+-rw-rw-rw-   0        0        0      163 2023-04-17 20:13:17.000000 socketscpi-2023.4.0/socketscpi/__init__.py
+-rw-rw-rw-   0        0        0    13293 2023-04-17 19:18:11.000000 socketscpi-2023.4.0/socketscpi/socketscpi.py
+drwxrwxrwx   0        0        0        0 2023-04-17 20:25:38.452091 socketscpi-2023.4.0/socketscpi.egg-info/
+-rw-rw-rw-   0        0        0     2020 2023-04-17 20:25:38.000000 socketscpi-2023.4.0/socketscpi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      612 2023-04-17 20:25:38.000000 socketscpi-2023.4.0/socketscpi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 20:25:38.000000 socketscpi-2023.4.0/socketscpi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-17 20:25:38.000000 socketscpi-2023.4.0/socketscpi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-04-17 20:25:38.000000 socketscpi-2023.4.0/socketscpi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 20:25:38.460079 socketscpi-2023.4.0/tests/
+-rw-rw-rw-   0        0        0       68 2021-05-06 23:00:54.000000 socketscpi-2023.4.0/tests/__init__.py
+-rw-rw-rw-   0        0        0      887 2021-05-06 23:00:54.000000 socketscpi-2023.4.0/tests/test_socketscpi.py
```

### Comparing `socketscpi-2022.8.0/CONTRIBUTING.rst` & `socketscpi-2023.4.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `socketscpi-2022.8.0/LICENSE` & `socketscpi-2023.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `socketscpi-2022.8.0/PKG-INFO` & `socketscpi-2023.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketscpi
-Version: 2022.8.0
+Version: 2023.4.0
 Summary: socketscpi provides a robust SCPI interface to electronic test and measurement equipment via raw socket protocol, removing the requirement for VISA and improving data transfer speed over VXI-11.
 Home-page: https://github.com/morgan-at-keysight/socketscpi
 Author: Morgan Allison
 Author-email: morgan.allison@keysight.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `socketscpi-2022.8.0/README.rst` & `socketscpi-2023.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `socketscpi-2022.8.0/docs/Makefile` & `socketscpi-2023.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `socketscpi-2022.8.0/docs/conf.py` & `socketscpi-2023.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `socketscpi-2022.8.0/docs/history.rst` & `socketscpi-2023.4.0/docs/history.rst`

 * *Files 16% similar despite different names*

```diff
@@ -21,8 +21,13 @@
 ----------------------
 
 * Adjusted the error checking for the ``.query()`` method to account for SCPI queries that require additional arguments.
 
 2022.08.0 (2022-08-11)
 ----------------------
 
-* Renamed ``binblockwrite()``, ``binblockread()``, and ``disconnect()`` to ``write_binary_values()``, ``read_binary_values()``, and ``close()``, respectively, to match the function calls in PyVISA.
+* Renamed ``binblockwrite()``, ``binblockread()``, and ``disconnect()`` to ``write_binary_values()``, ``read_binary_values()``, and ``close()``, respectively, to match the function calls in PyVISA.
+
+2023.04.0 (2023-04-17)
+----------------------
+
+* Added error checking syntax for UXR scopes. Added an argument in the ``SocketInstrument`` constructor to allow user to decide if verbose error checking will be attempted.
```

### Comparing `socketscpi-2022.8.0/docs/installation.rst` & `socketscpi-2023.4.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `socketscpi-2022.8.0/docs/make.bat` & `socketscpi-2023.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `socketscpi-2022.8.0/docs/usage.rst` & `socketscpi-2023.4.0/docs/usage.rst`

 * *Files 4% similar despite different names*

```diff
@@ -29,24 +29,26 @@
     instrument.close()
 
 ====================
 **SocketInstrument**
 ====================
 ::
 
-    socketscpi.SocketInstrument(host, port=5025, timeout=10, noDelay=True)
+    socketscpi.SocketInstrument(host, port=5025, timeout=10, noDelay=True, globalErrCheck=False, verboseErrCheck=True)
 
 Class constructor that connects to the test equipment and returns a SocketInstrument object that can be used to communicate with the equipment.
 
 **Arguments**
 
 * ``host`` ``(string)``: Instrument host IP address. Argument is a string containing a valid IP address.
 * ``port`` ``(int)``:  Port used by the instrument to facilitate socket communication (Keysight equipment uses port 5025 by default).
 * ``timeout`` ``(int)``: Timeout in seconds. This is how long the instrument will wait before sending a timeout error in response to a command or query. Argument is an int. Default is ``10``.
 * ``noDelay`` ``(bool)``: True turns on the TCP_NODELAY flag, which sends data immediately without concatenating multiple packets together. Just leave this alone.
+* ``globalErrCheck`` ``(bool)``: Determines if error checking will be done automatically after calling class methods.
+* ``verboseErrCheck`` ``(bool)``: Determines if verbose error checking will be attempted.
 
 **Returns**
 
 * ``socketscpi.SocketInstrument``: Instrument object to be used for communication and control.
 
 
 **close**
```

### Comparing `socketscpi-2022.8.0/socketscpi/socketscpi.py` & `socketscpi-2023.4.0/socketscpi/socketscpi.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,24 +9,25 @@
 import warnings
 import socket
 import numpy as np
 import ipaddress
 
 
 class SocketInstrument:
-    def __init__(self, ipAddress, port=5025, timeout=10, noDelay=True, globalErrCheck=False):
+    def __init__(self, ipAddress, port=5025, timeout=10, noDelay=True, globalErrCheck=False, verboseErrCheck=True):
         """
         Open socket connection with settings for instrument control.
 
         Args:
             ipAddress (string): Instrument host IP address. Argument is a string containing a valid IP address.
             port (int): Port used by the instrument to facilitate socket communication (Keysight equipment uses port 5025 by default).
             timeout (int): Timeout in seconds.
             noDelay (bool): True sends data immediately without concatenating multiple packets together. Just leave this alone.
             globalErrCheck (bool): Determines if error checking will be done automatically after calling class methods.
+            verboseErrCheck (bool): Determines if verbose error checking will be attempted.
         """
         # Validate IP address (will raise an error if given an invalid address).
         ipaddress.ip_address(ipAddress)
 
         self.globalErrCheck = globalErrCheck
         self.timeout = timeout
 
@@ -41,20 +42,21 @@
         self.socket.settimeout(timeout)
         # Connect to socket
         self.socket.connect((ipAddress, port))
 
         # Get the instrument ID
         self.instId = self.query('*idn?', errCheck=False)
 
-        # Enable verbose error checking of instrument supports this
-        try:
-            self.write('syst:err:verbose 1', errCheck=False)
-            self.err_check()
-        except SockInstError:
-            pass
+        # Enable verbose error checking of instrument supports this and if user desires
+        if verboseErrCheck:
+            try:
+                self.write('syst:err:verbose 1', errCheck=False)
+                self.err_check()
+            except SockInstError:
+                pass
 
     def disconnect(self):
         """DEPRECATED. THIS IS A PASS-THROUGH FUNCTION ONLY."""
 
         warnings.warn("socketscpi.binblockread() is deprecated. Use socketscpi.query_binary_values() instead.")
 
         return self.close()
```

### Comparing `socketscpi-2022.8.0/socketscpi.egg-info/PKG-INFO` & `socketscpi-2023.4.0/socketscpi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketscpi
-Version: 2022.8.0
+Version: 2023.4.0
 Summary: socketscpi provides a robust SCPI interface to electronic test and measurement equipment via raw socket protocol, removing the requirement for VISA and improving data transfer speed over VXI-11.
 Home-page: https://github.com/morgan-at-keysight/socketscpi
 Author: Morgan Allison
 Author-email: morgan.allison@keysight.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `socketscpi-2022.8.0/socketscpi.egg-info/SOURCES.txt` & `socketscpi-2023.4.0/socketscpi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `socketscpi-2022.8.0/tests/test_socketscpi.py` & `socketscpi-2023.4.0/tests/test_socketscpi.py`

 * *Files identical despite different names*

