# Comparing `tmp/mfrc522-python-0.0.2.tar.gz` & `tmp/mfrc522-python-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mfrc522-python-0.0.2.tar", last modified: Sun Apr 16 16:11:43 2023, max compression
+gzip compressed data, was "mfrc522-python-0.0.3.tar", last modified: Mon Apr 17 09:26:08 2023, max compression
```

## Comparing `mfrc522-python-0.0.2.tar` & `mfrc522-python-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 16:11:43.037782 mfrc522-python-0.0.2/
--rw-rw-rw-   0        0        0    35823 2023-04-15 05:57:40.000000 mfrc522-python-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     3120 2023-04-16 16:11:43.037782 mfrc522-python-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2526 2023-04-16 16:10:38.000000 mfrc522-python-0.0.2/README.md
--rw-rw-rw-   0        0        0      674 2023-04-16 16:11:20.000000 mfrc522-python-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-16 16:11:43.038785 mfrc522-python-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-16 16:11:43.009786 mfrc522-python-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-16 16:11:43.017779 mfrc522-python-0.0.2/src/mfrc522/
--rw-rw-rw-   0        0        0    22665 2023-04-16 14:58:59.000000 mfrc522-python-0.0.2/src/mfrc522/MFRC522.py
--rw-rw-rw-   0        0        0       50 2023-04-15 05:57:40.000000 mfrc522-python-0.0.2/src/mfrc522/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-16 16:11:43.035784 mfrc522-python-0.0.2/src/mfrc522_python.egg-info/
--rw-rw-rw-   0        0        0     3120 2023-04-16 16:11:42.000000 mfrc522-python-0.0.2/src/mfrc522_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      247 2023-04-16 16:11:43.000000 mfrc522-python-0.0.2/src/mfrc522_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 16:11:42.000000 mfrc522-python-0.0.2/src/mfrc522_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-16 16:11:42.000000 mfrc522-python-0.0.2/src/mfrc522_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 09:26:08.720889 mfrc522-python-0.0.3/
+-rw-rw-rw-   0        0        0    35823 2023-04-15 05:57:40.000000 mfrc522-python-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     3015 2023-04-17 09:26:08.712890 mfrc522-python-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2435 2023-04-17 08:50:46.000000 mfrc522-python-0.0.3/README.md
+-rw-rw-rw-   0        0        0      660 2023-04-17 08:52:55.000000 mfrc522-python-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-17 09:26:08.720889 mfrc522-python-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-17 09:26:08.656889 mfrc522-python-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-17 09:26:08.672887 mfrc522-python-0.0.3/src/mfrc522/
+-rw-rw-rw-   0        0        0    22657 2023-04-17 08:36:01.000000 mfrc522-python-0.0.3/src/mfrc522/MFRC522.py
+-rw-rw-rw-   0        0        0       50 2023-04-15 05:57:40.000000 mfrc522-python-0.0.3/src/mfrc522/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 09:26:08.712890 mfrc522-python-0.0.3/src/mfrc522_python.egg-info/
+-rw-rw-rw-   0        0        0     3015 2023-04-17 09:26:08.000000 mfrc522-python-0.0.3/src/mfrc522_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      247 2023-04-17 09:26:08.000000 mfrc522-python-0.0.3/src/mfrc522_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 09:26:08.000000 mfrc522-python-0.0.3/src/mfrc522_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-17 09:26:08.000000 mfrc522-python-0.0.3/src/mfrc522_python.egg-info/top_level.txt
```

### Comparing `mfrc522-python-0.0.2/LICENSE` & `mfrc522-python-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mfrc522-python-0.0.2/PKG-INFO` & `mfrc522-python-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: mfrc522-python
-Version: 0.0.2
+Version: 0.0.3
 Summary: The mfrc522 library is used to interact with RFID readers that use the MFRC522 chip
-Author: AnonymousXsn
-Project-URL: Homepage, https://github.com/AnonymousXsn/MFRC522-python
-Project-URL: Bug Tracker, https://github.com/AnonymousXsn/MFRC522-python/issues
+Author: Aditya
+Project-URL: Homepage, https://github.com/1AdityaX/mfrc522-python
+Project-URL: Bug Tracker, https://github.com/1AdityaX/mfrc522-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -28,77 +28,75 @@
 def read(trailer_block, key, block_addrs):
     (status, TagType) = reader.Request(reader.PICC_REQIDL)
     if status != reader.MI_OK:
         return None, None
     (status, uid) = reader.Anticoll()
     if status != reader.MI_OK:
         return None, None
-    id = self.uid_to_num(uid)
+    id = uid
     reader.SelectTag(uid)
-    status = reader.Auth(
+    status = reader.Authenticate(
         reader.PICC_AUTHENT1A, trailer_block , key, uid)
     data = []
     text_read = ''
     if status == reader.MI_OK:
         for block_num in block_addrs:
             block = reader.ReadTag(block_num)
             if block:
                 data += block
         if data:
             text_read = ''.join(chr(i) for i in data)
     reader.StopAuth()
     return id, text_read
 
-trailer_block = 11
+trailer_block = 15
 key = KEY = [0xFF, 0xFF, 0xFF, 0xFF, 0xFF, 0xFF]
-block_addrs = [8, 9, 10]
+block_addrs = [12,13,14]
 id, text = read(trailer_block, key, block_addrs)
 while not id:
     id, text = read(trailer_block, key, block_addrs)
 
 print(id)
 print(text)
 ```
 
 **write.py**
 
 To write a particular sector.
 ```py
-from mfrc522.MFRC522 import MFRC522
+from mfrc522 import MFRC522
 
 reader = MFRC522()
 
 def write(trailer_block, key, block_addrs, text):
     (status, TagType) = reader.Request(reader.PICC_REQIDL)
-        if status != reader.MI_OK:
-            return None, None
-        (status, uid) = reader.Anticoll()
-        if status != reader.MI_OK:
-            return None, None
-        id = uid
-        reader.SelectTag(uid)
-        status = reader.Auth(
-            reader.PICC_AUTHENT1A, trailer_block, key, uid)
-        reader.ReadTag(trailer_block)
-        if status == reader.MI_OK:
-            data = bytearray()
-            data.extend(bytearray(text.ljust(
-                len(block_addrs) * 16).encode('ascii')))
-            i = 0
-            for block_num in block_addrs:
-                reader.WriteTag(block_num, data[(i*16):(i+1)*16])
-                i += 1
-        reader.StopAuth()
-        return id, text[0:(len(block_addrs) * 16)]
+    if status != reader.MI_OK:
+        return None, None
+    (status, uid) = reader.Anticoll()
+    if status != reader.MI_OK:
+        return None, None
+    reader.SelectTag(uid)
+    status = reader.Authenticate(
+        reader.PICC_AUTHENT1A, trailer_block, key, uid)
+    reader.ReadTag(trailer_block)
+    if status == reader.MI_OK:
+        data = bytearray()
+        data.extend(bytearray(text.ljust(
+            len(block_addrs) * 16).encode('ascii')))
+        i = 0
+        for block_num in block_addrs:
+            reader.WriteTag(block_num, data[(i*16):(i+1)*16])
+            i += 1
+    reader.StopAuth()
+    return uid, text[0:(len(block_addrs) * 16)]
 
 trailer_block = 11
 block_addrs = [8, 9, 10]
 key = [0xFF, 0xFF, 0xFF, 0xFF, 0xFF, 0xFF]
 text = "some random text"
-id, text = write(trailer_block, key, block_addrs, text)
-while not id:
-    id, text = write(trailer_block, key, block_addrs, text)
-print(id, text)
-
+uid, text_in = write(trailer_block, key, block_addrs, text)
+while not uid:
+    uid, text_in = write(trailer_block, key, block_addrs, text)
+print(uid, text_in)
 ```
```

### Comparing `mfrc522-python-0.0.2/README.md` & `mfrc522-python-0.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -14,77 +14,75 @@
 def read(trailer_block, key, block_addrs):
     (status, TagType) = reader.Request(reader.PICC_REQIDL)
     if status != reader.MI_OK:
         return None, None
     (status, uid) = reader.Anticoll()
     if status != reader.MI_OK:
         return None, None
-    id = self.uid_to_num(uid)
+    id = uid
     reader.SelectTag(uid)
-    status = reader.Auth(
+    status = reader.Authenticate(
         reader.PICC_AUTHENT1A, trailer_block , key, uid)
     data = []
     text_read = ''
     if status == reader.MI_OK:
         for block_num in block_addrs:
             block = reader.ReadTag(block_num)
             if block:
                 data += block
         if data:
             text_read = ''.join(chr(i) for i in data)
     reader.StopAuth()
     return id, text_read
 
-trailer_block = 11
+trailer_block = 15
 key = KEY = [0xFF, 0xFF, 0xFF, 0xFF, 0xFF, 0xFF]
-block_addrs = [8, 9, 10]
+block_addrs = [12,13,14]
 id, text = read(trailer_block, key, block_addrs)
 while not id:
     id, text = read(trailer_block, key, block_addrs)
 
 print(id)
 print(text)
 ```
 
 **write.py**
 
 To write a particular sector.
 ```py
-from mfrc522.MFRC522 import MFRC522
+from mfrc522 import MFRC522
 
 reader = MFRC522()
 
 def write(trailer_block, key, block_addrs, text):
     (status, TagType) = reader.Request(reader.PICC_REQIDL)
-        if status != reader.MI_OK:
-            return None, None
-        (status, uid) = reader.Anticoll()
-        if status != reader.MI_OK:
-            return None, None
-        id = uid
-        reader.SelectTag(uid)
-        status = reader.Auth(
-            reader.PICC_AUTHENT1A, trailer_block, key, uid)
-        reader.ReadTag(trailer_block)
-        if status == reader.MI_OK:
-            data = bytearray()
-            data.extend(bytearray(text.ljust(
-                len(block_addrs) * 16).encode('ascii')))
-            i = 0
-            for block_num in block_addrs:
-                reader.WriteTag(block_num, data[(i*16):(i+1)*16])
-                i += 1
-        reader.StopAuth()
-        return id, text[0:(len(block_addrs) * 16)]
+    if status != reader.MI_OK:
+        return None, None
+    (status, uid) = reader.Anticoll()
+    if status != reader.MI_OK:
+        return None, None
+    reader.SelectTag(uid)
+    status = reader.Authenticate(
+        reader.PICC_AUTHENT1A, trailer_block, key, uid)
+    reader.ReadTag(trailer_block)
+    if status == reader.MI_OK:
+        data = bytearray()
+        data.extend(bytearray(text.ljust(
+            len(block_addrs) * 16).encode('ascii')))
+        i = 0
+        for block_num in block_addrs:
+            reader.WriteTag(block_num, data[(i*16):(i+1)*16])
+            i += 1
+    reader.StopAuth()
+    return uid, text[0:(len(block_addrs) * 16)]
 
 trailer_block = 11
 block_addrs = [8, 9, 10]
 key = [0xFF, 0xFF, 0xFF, 0xFF, 0xFF, 0xFF]
 text = "some random text"
-id, text = write(trailer_block, key, block_addrs, text)
-while not id:
-    id, text = write(trailer_block, key, block_addrs, text)
-print(id, text)
-
+uid, text_in = write(trailer_block, key, block_addrs, text)
+while not uid:
+    uid, text_in = write(trailer_block, key, block_addrs, text)
+print(uid, text_in)
 ```
```

### Comparing `mfrc522-python-0.0.2/pyproject.toml` & `mfrc522-python-0.0.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mfrc522-python"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
-  { name="AnonymousXsn"},
+  { name="Aditya"},
 ]
 description = "The mfrc522 library is used to interact with RFID readers that use the MFRC522 chip"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: POSIX :: Linux",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/AnonymousXsn/MFRC522-python"
-"Bug Tracker" = "https://github.com/AnonymousXsn/MFRC522-python/issues"
+"Homepage" = "https://github.com/1AdityaX/mfrc522-python"
+"Bug Tracker" = "https://github.com/1AdityaX/mfrc522-python/issues"
```

### Comparing `mfrc522-python-0.0.2/src/mfrc522/MFRC522.py` & `mfrc522-python-0.0.3/src/mfrc522/MFRC522.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,15 +140,15 @@
         # Set reset pin based on pin_mode if not specified
         if pin_rst == -1:
             if pin_mode == 11:
                 pin_rst = 15
             else:
                 pin_rst = 22
 
-        self.MFRC522_StopAuth = self.StopCrypto1()
+        self.StopAuth = self.StopCrypto1()
         # Set up reset pin and initialize MFRC522 RFID reader
         GPIO.setup(pin_rst, GPIO.OUT)
         GPIO.output(pin_rst, 1)
         self.Init()
 
     def Reset(self):
         """
```

### Comparing `mfrc522-python-0.0.2/src/mfrc522_python.egg-info/PKG-INFO` & `mfrc522-python-0.0.3/src/mfrc522_python.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: mfrc522-python
-Version: 0.0.2
+Version: 0.0.3
 Summary: The mfrc522 library is used to interact with RFID readers that use the MFRC522 chip
-Author: AnonymousXsn
-Project-URL: Homepage, https://github.com/AnonymousXsn/MFRC522-python
-Project-URL: Bug Tracker, https://github.com/AnonymousXsn/MFRC522-python/issues
+Author: Aditya
+Project-URL: Homepage, https://github.com/1AdityaX/mfrc522-python
+Project-URL: Bug Tracker, https://github.com/1AdityaX/mfrc522-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -28,77 +28,75 @@
 def read(trailer_block, key, block_addrs):
     (status, TagType) = reader.Request(reader.PICC_REQIDL)
     if status != reader.MI_OK:
         return None, None
     (status, uid) = reader.Anticoll()
     if status != reader.MI_OK:
         return None, None
-    id = self.uid_to_num(uid)
+    id = uid
     reader.SelectTag(uid)
-    status = reader.Auth(
+    status = reader.Authenticate(
         reader.PICC_AUTHENT1A, trailer_block , key, uid)
     data = []
     text_read = ''
     if status == reader.MI_OK:
         for block_num in block_addrs:
             block = reader.ReadTag(block_num)
             if block:
                 data += block
         if data:
             text_read = ''.join(chr(i) for i in data)
     reader.StopAuth()
     return id, text_read
 
-trailer_block = 11
+trailer_block = 15
 key = KEY = [0xFF, 0xFF, 0xFF, 0xFF, 0xFF, 0xFF]
-block_addrs = [8, 9, 10]
+block_addrs = [12,13,14]
 id, text = read(trailer_block, key, block_addrs)
 while not id:
     id, text = read(trailer_block, key, block_addrs)
 
 print(id)
 print(text)
 ```
 
 **write.py**
 
 To write a particular sector.
 ```py
-from mfrc522.MFRC522 import MFRC522
+from mfrc522 import MFRC522
 
 reader = MFRC522()
 
 def write(trailer_block, key, block_addrs, text):
     (status, TagType) = reader.Request(reader.PICC_REQIDL)
-        if status != reader.MI_OK:
-            return None, None
-        (status, uid) = reader.Anticoll()
-        if status != reader.MI_OK:
-            return None, None
-        id = uid
-        reader.SelectTag(uid)
-        status = reader.Auth(
-            reader.PICC_AUTHENT1A, trailer_block, key, uid)
-        reader.ReadTag(trailer_block)
-        if status == reader.MI_OK:
-            data = bytearray()
-            data.extend(bytearray(text.ljust(
-                len(block_addrs) * 16).encode('ascii')))
-            i = 0
-            for block_num in block_addrs:
-                reader.WriteTag(block_num, data[(i*16):(i+1)*16])
-                i += 1
-        reader.StopAuth()
-        return id, text[0:(len(block_addrs) * 16)]
+    if status != reader.MI_OK:
+        return None, None
+    (status, uid) = reader.Anticoll()
+    if status != reader.MI_OK:
+        return None, None
+    reader.SelectTag(uid)
+    status = reader.Authenticate(
+        reader.PICC_AUTHENT1A, trailer_block, key, uid)
+    reader.ReadTag(trailer_block)
+    if status == reader.MI_OK:
+        data = bytearray()
+        data.extend(bytearray(text.ljust(
+            len(block_addrs) * 16).encode('ascii')))
+        i = 0
+        for block_num in block_addrs:
+            reader.WriteTag(block_num, data[(i*16):(i+1)*16])
+            i += 1
+    reader.StopAuth()
+    return uid, text[0:(len(block_addrs) * 16)]
 
 trailer_block = 11
 block_addrs = [8, 9, 10]
 key = [0xFF, 0xFF, 0xFF, 0xFF, 0xFF, 0xFF]
 text = "some random text"
-id, text = write(trailer_block, key, block_addrs, text)
-while not id:
-    id, text = write(trailer_block, key, block_addrs, text)
-print(id, text)
-
+uid, text_in = write(trailer_block, key, block_addrs, text)
+while not uid:
+    uid, text_in = write(trailer_block, key, block_addrs, text)
+print(uid, text_in)
 ```
```

