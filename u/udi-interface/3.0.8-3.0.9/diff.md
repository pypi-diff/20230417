# Comparing `tmp/udi_interface-3.0.8.tar.gz` & `tmp/udi_interface-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/udi_interface-3.0.8.tar", last modified: Thu Jul 29 16:05:42 2021, max compression
+gzip compressed data, was "dist/udi_interface-3.0.9.tar", last modified: Sat Aug  7 16:49:34 2021, max compression
```

## Comparing `udi_interface-3.0.8.tar` & `udi_interface-3.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 bpaauwe   (1001) bpaauwe   (1001)        0 2021-07-29 16:05:42.000000 udi_interface-3.0.8/
--rw-r--r--   0 bpaauwe   (1001) bpaauwe   (1001)     2801 2021-07-29 16:05:42.000000 udi_interface-3.0.8/PKG-INFO
--rw-r--r--   0 bpaauwe   (1001) bpaauwe   (1001)     1741 2021-01-05 00:52:20.000000 udi_interface-3.0.8/README.md
--rw-r--r--   0 bpaauwe   (1001) bpaauwe   (1001)      224 2021-07-29 16:05:42.000000 udi_interface-3.0.8/setup.cfg
--rwxr-xr-x   0 bpaauwe   (1001) bpaauwe   (1001)     1415 2021-07-07 22:57:13.000000 udi_interface-3.0.8/setup.py
-drwxr-xr-x   0 bpaauwe   (1001) bpaauwe   (1001)        0 2021-07-29 16:05:42.000000 udi_interface-3.0.8/udi_interface/
--rwxr-xr-x   0 bpaauwe   (1001) bpaauwe   (1001)      543 2021-07-29 16:05:21.000000 udi_interface-3.0.8/udi_interface/__init__.py
--rw-r--r--   0 bpaauwe   (1001) bpaauwe   (1001)     4594 2021-07-26 20:10:10.000000 udi_interface-3.0.8/udi_interface/custom.py
--rw-r--r--   0 bpaauwe   (1001) bpaauwe   (1001)    38067 2021-07-26 20:07:03.000000 udi_interface-3.0.8/udi_interface/interface.py
--rw-r--r--   0 bpaauwe   (1001) bpaauwe   (1001)     2337 2021-02-03 14:43:06.000000 udi_interface-3.0.8/udi_interface/isy.py
--rw-r--r--   0 bpaauwe   (1001) bpaauwe   (1001)     5169 2021-07-29 16:04:23.000000 udi_interface-3.0.8/udi_interface/node.py
--rwxr-xr-x   0 bpaauwe   (1001) bpaauwe   (1001)     2803 2021-01-05 00:52:20.000000 udi_interface-3.0.8/udi_interface/polylogger.py
--rwxr-xr-x   0 bpaauwe   (1001) bpaauwe   (1001)     4004 2021-01-27 13:58:04.000000 udi_interface-3.0.8/udi_interface/udi_interface.py
-drwxr-xr-x   0 bpaauwe   (1001) bpaauwe   (1001)        0 2021-07-29 16:05:42.000000 udi_interface-3.0.8/udi_interface.egg-info/
--rw-r--r--   0 bpaauwe   (1001) bpaauwe   (1001)     2801 2021-07-29 16:05:42.000000 udi_interface-3.0.8/udi_interface.egg-info/PKG-INFO
--rw-r--r--   0 bpaauwe   (1001) bpaauwe   (1001)      427 2021-07-29 16:05:42.000000 udi_interface-3.0.8/udi_interface.egg-info/SOURCES.txt
--rw-r--r--   0 bpaauwe   (1001) bpaauwe   (1001)        1 2021-07-29 16:05:42.000000 udi_interface-3.0.8/udi_interface.egg-info/dependency_links.txt
--rw-r--r--   0 bpaauwe   (1001) bpaauwe   (1001)        1 2021-01-28 15:38:14.000000 udi_interface-3.0.8/udi_interface.egg-info/not-zip-safe
--rw-r--r--   0 bpaauwe   (1001) bpaauwe   (1001)       50 2021-07-29 16:05:42.000000 udi_interface-3.0.8/udi_interface.egg-info/requires.txt
--rw-r--r--   0 bpaauwe   (1001) bpaauwe   (1001)       14 2021-07-29 16:05:42.000000 udi_interface-3.0.8/udi_interface.egg-info/top_level.txt
+drwxr-xr-x   0 bpaauwe   (1001) bpaauwe   (1001)        0 2021-08-07 16:49:34.000000 udi_interface-3.0.9/
+-rw-r--r--   0 bpaauwe   (1001) bpaauwe   (1001)     2801 2021-08-07 16:49:34.000000 udi_interface-3.0.9/PKG-INFO
+-rw-r--r--   0 bpaauwe   (1001) bpaauwe   (1001)     1741 2021-01-05 00:52:20.000000 udi_interface-3.0.9/README.md
+-rw-r--r--   0 bpaauwe   (1001) bpaauwe   (1001)      224 2021-08-07 16:49:34.000000 udi_interface-3.0.9/setup.cfg
+-rwxr-xr-x   0 bpaauwe   (1001) bpaauwe   (1001)     1415 2021-07-07 22:57:13.000000 udi_interface-3.0.9/setup.py
+drwxr-xr-x   0 bpaauwe   (1001) bpaauwe   (1001)        0 2021-08-07 16:49:34.000000 udi_interface-3.0.9/udi_interface/
+-rwxr-xr-x   0 bpaauwe   (1001) bpaauwe   (1001)      543 2021-08-07 16:48:51.000000 udi_interface-3.0.9/udi_interface/__init__.py
+-rw-r--r--   0 bpaauwe   (1001) bpaauwe   (1001)     4594 2021-07-26 20:10:10.000000 udi_interface-3.0.9/udi_interface/custom.py
+-rw-r--r--   0 bpaauwe   (1001) bpaauwe   (1001)    38294 2021-08-07 16:42:53.000000 udi_interface-3.0.9/udi_interface/interface.py
+-rw-r--r--   0 bpaauwe   (1001) bpaauwe   (1001)     2337 2021-02-03 14:43:06.000000 udi_interface-3.0.9/udi_interface/isy.py
+-rw-r--r--   0 bpaauwe   (1001) bpaauwe   (1001)     5169 2021-07-29 16:04:23.000000 udi_interface-3.0.9/udi_interface/node.py
+-rwxr-xr-x   0 bpaauwe   (1001) bpaauwe   (1001)     2803 2021-01-05 00:52:20.000000 udi_interface-3.0.9/udi_interface/polylogger.py
+-rwxr-xr-x   0 bpaauwe   (1001) bpaauwe   (1001)     4004 2021-01-27 13:58:04.000000 udi_interface-3.0.9/udi_interface/udi_interface.py
+drwxr-xr-x   0 bpaauwe   (1001) bpaauwe   (1001)        0 2021-08-07 16:49:34.000000 udi_interface-3.0.9/udi_interface.egg-info/
+-rw-r--r--   0 bpaauwe   (1001) bpaauwe   (1001)     2801 2021-08-07 16:49:33.000000 udi_interface-3.0.9/udi_interface.egg-info/PKG-INFO
+-rw-r--r--   0 bpaauwe   (1001) bpaauwe   (1001)      427 2021-08-07 16:49:33.000000 udi_interface-3.0.9/udi_interface.egg-info/SOURCES.txt
+-rw-r--r--   0 bpaauwe   (1001) bpaauwe   (1001)        1 2021-08-07 16:49:33.000000 udi_interface-3.0.9/udi_interface.egg-info/dependency_links.txt
+-rw-r--r--   0 bpaauwe   (1001) bpaauwe   (1001)        1 2021-01-28 15:38:14.000000 udi_interface-3.0.9/udi_interface.egg-info/not-zip-safe
+-rw-r--r--   0 bpaauwe   (1001) bpaauwe   (1001)       50 2021-08-07 16:49:33.000000 udi_interface-3.0.9/udi_interface.egg-info/requires.txt
+-rw-r--r--   0 bpaauwe   (1001) bpaauwe   (1001)       14 2021-08-07 16:49:33.000000 udi_interface-3.0.9/udi_interface.egg-info/top_level.txt
```

### Comparing `udi_interface-3.0.8/PKG-INFO` & `udi_interface-3.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: udi_interface
-Version: 3.0.8
+Version: 3.0.9
 Summary: UDI Python Interface for Polyglot version 3
 Home-page: https://github.com/UniversalDevicesInc/udi-python-interface
 Author: Universal Devices Inc.
 Author-email: bpaauwe@yahoo.com
 License: MIT
 Description: ![Test And Publish](https://github.com/UniversalDevicesInc/udi-python-interface/workflows/Publish%20PyPI%20and%20TestPyPI/badge.svg)
```

### Comparing `udi_interface-3.0.8/README.md` & `udi_interface-3.0.9/README.md`

 * *Files identical despite different names*

### Comparing `udi_interface-3.0.8/setup.py` & `udi_interface-3.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `udi_interface-3.0.8/udi_interface/__init__.py` & `udi_interface-3.0.9/udi_interface/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from .polylogger import LOG_HANDLER, LOGGER
 from .udi_interface import unload_interface, get_network_interface
 from .node import Node
 from .interface import Interface
 from .custom import Custom
 from .isy import ISY
 
-__version__ = '3.0.8'
+__version__ = '3.0.9'
 __description__ = 'UDI Python Interface for Polyglot version 3'
 __url__ = 'https://github.com/UniversalDevicesInc/udi-python-interface'
 __author__ = 'Universal Devices Inc.'
 __authoremail__ = 'bpaauwe@yahoo.com'
 __license__ = 'MIT'
 
 LOGGER.info('{} {} Starting...'.format(__description__, __version__))
```

### Comparing `udi_interface-3.0.8/udi_interface/custom.py` & `udi_interface-3.0.9/udi_interface/custom.py`

 * *Files identical despite different names*

### Comparing `udi_interface-3.0.8/udi_interface/interface.py` & `udi_interface-3.0.9/udi_interface/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,16 @@
 LOGGER.setLevel("INFO")
 
 """
 usage:
       pub.subscribe(CONFIG, configHandler)
 
       pub.publish(CONFIG, config_data)
+
+      if pub.hasSubscriber(CONFIG):
 """
 class pub(object):
 
     # topic is index into this list
     topic_list = [
          'config',
          'start',
@@ -75,15 +77,20 @@
 
     @staticmethod
     def publish(topic, address, *argv):
         if pub.topic_list[topic] in pub.topics:
             for item in pub.topics[pub.topic_list[topic]]:
                 if item[1] == address:
                     Thread(target=item[0], args=[*argv]).start()
-        
+
+    @staticmethod
+    def hasSubscriber(topic):
+        if pub.topic_list[topic] in pub.topics:
+            return True
+        return False
 
 
 class Interface(object):
 
     CUSTOM_CONFIG_DOCS_FILE_NAME = 'POLYGLOT_CONFIG.md'
     SERVER_JSON_FILE_NAME = 'server.json'
     CONFIG            = 0
@@ -411,15 +418,14 @@
         # self._longPoll.cancel()
         # self._shortPoll.cancel()
         if self.connected:
             LOGGER.info('Disconnecting from MQTT... {}:{}'.format(
                 self._server, self._port))
             self._mqttc.loop_stop()
             self._mqttc.disconnect()
-        pub.publish(self.STOP, None)
 
     def send(self, message, type):
         """
         Formatted Message to send to Polyglot. Connection messages are sent
         automatically from this module so this method is used to send commands
         to/from Polyglot and formats it for consumption
         """
@@ -645,15 +651,17 @@
             if item['address'] in self.nodes:
                 self.nodes[item['address']].status()
             elif item['address'] == 'all':
                 # TODO: FIXME: This isn't right now
                 self.status()
         elif key == 'stop':
             LOGGER.info('Received stop from Polyglot... Shutting Down.')
-            self.stop()
+            pub.publish(self.STOP, None)
+            if not pub.hasSubscriber(self.STOP):
+                self.stop()
         elif key == 'setLogLevel':
             try:
                 self.currentLogLevel = item['level'].upper()
                 if self.currentLogLevel == 'ALL':
                     LOGGER.setLevel('DEBUG')
                     CLOGGER.setLevel('DEBUG')
                     NLOGGER.setLevel('DEBUG')
```

### Comparing `udi_interface-3.0.8/udi_interface/isy.py` & `udi_interface-3.0.9/udi_interface/isy.py`

 * *Files identical despite different names*

### Comparing `udi_interface-3.0.8/udi_interface/node.py` & `udi_interface-3.0.9/udi_interface/node.py`

 * *Files identical despite different names*

### Comparing `udi_interface-3.0.8/udi_interface/polylogger.py` & `udi_interface-3.0.9/udi_interface/polylogger.py`

 * *Files identical despite different names*

### Comparing `udi_interface-3.0.8/udi_interface/udi_interface.py` & `udi_interface-3.0.9/udi_interface/udi_interface.py`

 * *Files identical despite different names*

### Comparing `udi_interface-3.0.8/udi_interface.egg-info/PKG-INFO` & `udi_interface-3.0.9/udi_interface.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: udi-interface
-Version: 3.0.8
+Version: 3.0.9
 Summary: UDI Python Interface for Polyglot version 3
 Home-page: https://github.com/UniversalDevicesInc/udi-python-interface
 Author: Universal Devices Inc.
 Author-email: bpaauwe@yahoo.com
 License: MIT
 Description: ![Test And Publish](https://github.com/UniversalDevicesInc/udi-python-interface/workflows/Publish%20PyPI%20and%20TestPyPI/badge.svg)
```

