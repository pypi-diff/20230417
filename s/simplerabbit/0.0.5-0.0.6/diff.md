# Comparing `tmp/simplerabbit-0.0.5.tar.gz` & `tmp/simplerabbit-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplerabbit-0.0.5.tar", last modified: Tue Apr 11 12:41:00 2023, max compression
+gzip compressed data, was "simplerabbit-0.0.6.tar", last modified: Mon Apr 17 09:33:53 2023, max compression
```

## Comparing `simplerabbit-0.0.5.tar` & `simplerabbit-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-04-11 12:41:00.125262 simplerabbit-0.0.5/
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     1595 2023-04-11 12:41:00.125262 simplerabbit-0.0.5/PKG-INFO
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     1100 2023-04-11 11:23:43.000000 simplerabbit-0.0.5/README.md
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)      638 2023-04-11 12:40:27.000000 simplerabbit-0.0.5/pyproject.toml
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)       38 2023-04-11 12:41:00.125262 simplerabbit-0.0.5/setup.cfg
-drwxrwxr-x   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-04-11 12:41:00.125262 simplerabbit-0.0.5/src/
-drwxrwxr-x   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-04-11 12:41:00.125262 simplerabbit-0.0.5/src/simplerabbit/
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        1 2023-04-11 11:39:32.000000 simplerabbit-0.0.5/src/simplerabbit/__init__.py
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     3067 2023-04-11 12:11:18.000000 simplerabbit-0.0.5/src/simplerabbit/receiver.py
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     2553 2023-04-11 12:40:10.000000 simplerabbit-0.0.5/src/simplerabbit/sender.py
-drwxrwxr-x   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-04-11 12:41:00.125262 simplerabbit-0.0.5/src/simplerabbit.egg-info/
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     1595 2023-04-11 12:41:00.000000 simplerabbit-0.0.5/src/simplerabbit.egg-info/PKG-INFO
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)      283 2023-04-11 12:41:00.000000 simplerabbit-0.0.5/src/simplerabbit.egg-info/SOURCES.txt
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        1 2023-04-11 12:41:00.000000 simplerabbit-0.0.5/src/simplerabbit.egg-info/dependency_links.txt
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)       13 2023-04-11 12:41:00.000000 simplerabbit-0.0.5/src/simplerabbit.egg-info/top_level.txt
-drwxrwxr-x   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-04-11 12:41:00.125262 simplerabbit-0.0.5/tests/
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)      107 2023-04-11 12:29:32.000000 simplerabbit-0.0.5/tests/test.py
+drwxrwxr-x   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-04-17 09:33:53.221900 simplerabbit-0.0.6/
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     1595 2023-04-17 09:33:53.221900 simplerabbit-0.0.6/PKG-INFO
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     1100 2023-04-11 11:23:43.000000 simplerabbit-0.0.6/README.md
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)      638 2023-04-17 09:33:09.000000 simplerabbit-0.0.6/pyproject.toml
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)       38 2023-04-17 09:33:53.221900 simplerabbit-0.0.6/setup.cfg
+drwxrwxr-x   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-04-17 09:33:53.217900 simplerabbit-0.0.6/src/
+drwxrwxr-x   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-04-17 09:33:53.221900 simplerabbit-0.0.6/src/simplerabbit/
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        1 2023-04-11 11:39:32.000000 simplerabbit-0.0.6/src/simplerabbit/__init__.py
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     3111 2023-04-17 09:32:39.000000 simplerabbit-0.0.6/src/simplerabbit/receiver.py
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     2553 2023-04-11 12:40:10.000000 simplerabbit-0.0.6/src/simplerabbit/sender.py
+drwxrwxr-x   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-04-17 09:33:53.221900 simplerabbit-0.0.6/src/simplerabbit.egg-info/
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     1595 2023-04-17 09:33:53.000000 simplerabbit-0.0.6/src/simplerabbit.egg-info/PKG-INFO
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)      283 2023-04-17 09:33:53.000000 simplerabbit-0.0.6/src/simplerabbit.egg-info/SOURCES.txt
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        1 2023-04-17 09:33:53.000000 simplerabbit-0.0.6/src/simplerabbit.egg-info/dependency_links.txt
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)       13 2023-04-17 09:33:53.000000 simplerabbit-0.0.6/src/simplerabbit.egg-info/top_level.txt
+drwxrwxr-x   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-04-17 09:33:53.221900 simplerabbit-0.0.6/tests/
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)      107 2023-04-11 12:29:32.000000 simplerabbit-0.0.6/tests/test.py
```

### Comparing `simplerabbit-0.0.5/PKG-INFO` & `simplerabbit-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplerabbit
-Version: 0.0.5
+Version: 0.0.6
 Summary: Simple RabbitMQ library
 Author-email: Phuong Do <phdo@energidanmark.dk>
 Project-URL: Homepage, https://github.com/Energidanmark/simplerabbit
 Project-URL: Bug Tracker, https://github.com/Energidanmark/simplerabbit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `simplerabbit-0.0.5/README.md` & `simplerabbit-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `simplerabbit-0.0.5/pyproject.toml` & `simplerabbit-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "simplerabbit"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Phuong Do", email="phdo@energidanmark.dk" },
 ]
 description = "Simple RabbitMQ library"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `simplerabbit-0.0.5/src/simplerabbit/receiver.py` & `simplerabbit-0.0.6/src/simplerabbit/receiver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import pika
 import threading
+import time
 
 class RabbitReceiver:
     def __init__(self, host='localhost', port='5672', username=None, password=None, virtual_host='/'):
         self.host = host
         self.queues = []
         self.username = username
         self.password = password
@@ -48,14 +49,15 @@
     def _consume_messages(self):
         for queue in self.queues:
             self.channel.basic_consume(queue=queue, on_message_callback=self._callback, auto_ack=True)
         print("Waiting for messages...")
         while not self.stop_event.is_set():
             try:
                 self.channel.connection.process_data_events()
+                time.sleep(0.2)
             except Exception as e:
                 if self.on_connection_closed:
                     self.on_connection_closed()
 
     def _callback(self, ch, method, properties, body):
         if self.on_message:
             self.on_message(int(properties.correlation_id), body)
```

### Comparing `simplerabbit-0.0.5/src/simplerabbit/sender.py` & `simplerabbit-0.0.6/src/simplerabbit/sender.py`

 * *Files identical despite different names*

### Comparing `simplerabbit-0.0.5/src/simplerabbit.egg-info/PKG-INFO` & `simplerabbit-0.0.6/src/simplerabbit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplerabbit
-Version: 0.0.5
+Version: 0.0.6
 Summary: Simple RabbitMQ library
 Author-email: Phuong Do <phdo@energidanmark.dk>
 Project-URL: Homepage, https://github.com/Energidanmark/simplerabbit
 Project-URL: Bug Tracker, https://github.com/Energidanmark/simplerabbit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

