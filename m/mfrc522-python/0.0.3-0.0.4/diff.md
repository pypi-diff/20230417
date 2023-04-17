# Comparing `tmp/mfrc522-python-0.0.3.tar.gz` & `tmp/mfrc522-python-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mfrc522-python-0.0.3.tar", last modified: Mon Apr 17 09:26:08 2023, max compression
+gzip compressed data, was "mfrc522-python-0.0.4.tar", last modified: Mon Apr 17 09:47:47 2023, max compression
```

## Comparing `mfrc522-python-0.0.3.tar` & `mfrc522-python-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 09:26:08.720889 mfrc522-python-0.0.3/
--rw-rw-rw-   0        0        0    35823 2023-04-15 05:57:40.000000 mfrc522-python-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     3015 2023-04-17 09:26:08.712890 mfrc522-python-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2435 2023-04-17 08:50:46.000000 mfrc522-python-0.0.3/README.md
--rw-rw-rw-   0        0        0      660 2023-04-17 08:52:55.000000 mfrc522-python-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-17 09:26:08.720889 mfrc522-python-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-17 09:26:08.656889 mfrc522-python-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-17 09:26:08.672887 mfrc522-python-0.0.3/src/mfrc522/
--rw-rw-rw-   0        0        0    22657 2023-04-17 08:36:01.000000 mfrc522-python-0.0.3/src/mfrc522/MFRC522.py
--rw-rw-rw-   0        0        0       50 2023-04-15 05:57:40.000000 mfrc522-python-0.0.3/src/mfrc522/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 09:26:08.712890 mfrc522-python-0.0.3/src/mfrc522_python.egg-info/
--rw-rw-rw-   0        0        0     3015 2023-04-17 09:26:08.000000 mfrc522-python-0.0.3/src/mfrc522_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      247 2023-04-17 09:26:08.000000 mfrc522-python-0.0.3/src/mfrc522_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 09:26:08.000000 mfrc522-python-0.0.3/src/mfrc522_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-17 09:26:08.000000 mfrc522-python-0.0.3/src/mfrc522_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 09:47:47.744548 mfrc522-python-0.0.4/
+-rw-rw-rw-   0        0        0    35823 2023-04-15 05:57:40.000000 mfrc522-python-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     3013 2023-04-17 09:47:47.744548 mfrc522-python-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2433 2023-04-17 09:44:23.000000 mfrc522-python-0.0.4/README.md
+-rw-rw-rw-   0        0        0      660 2023-04-17 09:46:51.000000 mfrc522-python-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-17 09:47:47.744548 mfrc522-python-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-17 09:47:47.712512 mfrc522-python-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-04-17 09:47:47.720509 mfrc522-python-0.0.4/src/mfrc522/
+-rw-rw-rw-   0        0        0    22655 2023-04-17 09:42:23.000000 mfrc522-python-0.0.4/src/mfrc522/MFRC522.py
+-rw-rw-rw-   0        0        0       50 2023-04-15 05:57:40.000000 mfrc522-python-0.0.4/src/mfrc522/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 09:47:47.744548 mfrc522-python-0.0.4/src/mfrc522_python.egg-info/
+-rw-rw-rw-   0        0        0     3013 2023-04-17 09:47:47.000000 mfrc522-python-0.0.4/src/mfrc522_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      247 2023-04-17 09:47:47.000000 mfrc522-python-0.0.4/src/mfrc522_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 09:47:47.000000 mfrc522-python-0.0.4/src/mfrc522_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-17 09:47:47.000000 mfrc522-python-0.0.4/src/mfrc522_python.egg-info/top_level.txt
```

### Comparing `mfrc522-python-0.0.3/LICENSE` & `mfrc522-python-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mfrc522-python-0.0.3/PKG-INFO` & `mfrc522-python-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mfrc522-python
-Version: 0.0.3
+Version: 0.0.4
 Summary: The mfrc522 library is used to interact with RFID readers that use the MFRC522 chip
 Author: Aditya
 Project-URL: Homepage, https://github.com/1AdityaX/mfrc522-python
 Project-URL: Bug Tracker, https://github.com/1AdityaX/mfrc522-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
@@ -44,17 +44,17 @@
             if block:
                 data += block
         if data:
             text_read = ''.join(chr(i) for i in data)
     reader.StopAuth()
     return id, text_read
 
-trailer_block = 15
+trailer_block = 11
 key = KEY = [0xFF, 0xFF, 0xFF, 0xFF, 0xFF, 0xFF]
-block_addrs = [12,13,14]
+block_addrs = [8,9,10]
 id, text = read(trailer_block, key, block_addrs)
 while not id:
     id, text = read(trailer_block, key, block_addrs)
 
 print(id)
 print(text)
 ```
```

### Comparing `mfrc522-python-0.0.3/README.md` & `mfrc522-python-0.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -30,17 +30,17 @@
             if block:
                 data += block
         if data:
             text_read = ''.join(chr(i) for i in data)
     reader.StopAuth()
     return id, text_read
 
-trailer_block = 15
+trailer_block = 11
 key = KEY = [0xFF, 0xFF, 0xFF, 0xFF, 0xFF, 0xFF]
-block_addrs = [12,13,14]
+block_addrs = [8,9,10]
 id, text = read(trailer_block, key, block_addrs)
 while not id:
     id, text = read(trailer_block, key, block_addrs)
 
 print(id)
 print(text)
 ```
```

### Comparing `mfrc522-python-0.0.3/pyproject.toml` & `mfrc522-python-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mfrc522-python"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Aditya"},
 ]
 description = "The mfrc522 library is used to interact with RFID readers that use the MFRC522 chip"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `mfrc522-python-0.0.3/src/mfrc522/MFRC522.py` & `mfrc522-python-0.0.4/src/mfrc522/MFRC522.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,15 +140,15 @@
         # Set reset pin based on pin_mode if not specified
         if pin_rst == -1:
             if pin_mode == 11:
                 pin_rst = 15
             else:
                 pin_rst = 22
 
-        self.StopAuth = self.StopCrypto1()
+        self.StopAuth = self.StopCrypto1
         # Set up reset pin and initialize MFRC522 RFID reader
         GPIO.setup(pin_rst, GPIO.OUT)
         GPIO.output(pin_rst, 1)
         self.Init()
 
     def Reset(self):
         """
```

### Comparing `mfrc522-python-0.0.3/src/mfrc522_python.egg-info/PKG-INFO` & `mfrc522-python-0.0.4/src/mfrc522_python.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mfrc522-python
-Version: 0.0.3
+Version: 0.0.4
 Summary: The mfrc522 library is used to interact with RFID readers that use the MFRC522 chip
 Author: Aditya
 Project-URL: Homepage, https://github.com/1AdityaX/mfrc522-python
 Project-URL: Bug Tracker, https://github.com/1AdityaX/mfrc522-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
@@ -44,17 +44,17 @@
             if block:
                 data += block
         if data:
             text_read = ''.join(chr(i) for i in data)
     reader.StopAuth()
     return id, text_read
 
-trailer_block = 15
+trailer_block = 11
 key = KEY = [0xFF, 0xFF, 0xFF, 0xFF, 0xFF, 0xFF]
-block_addrs = [12,13,14]
+block_addrs = [8,9,10]
 id, text = read(trailer_block, key, block_addrs)
 while not id:
     id, text = read(trailer_block, key, block_addrs)
 
 print(id)
 print(text)
 ```
```

