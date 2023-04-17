# Comparing `tmp/python-image-complete-0.0.4.tar.gz` & `tmp/python-image-complete-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-image-complete-0.0.4.tar", last modified: Wed Mar 29 22:55:48 2023, max compression
+gzip compressed data, was "python-image-complete-0.0.5.tar", last modified: Mon Apr 17 04:09:09 2023, max compression
```

## Comparing `python-image-complete-0.0.4.tar` & `python-image-complete-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-03-29 22:55:48.044873 python-image-complete-0.0.4/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      478 2023-03-29 22:54:06.000000 python-image-complete-0.0.4/CHANGES.rst
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      466 2023-03-29 22:52:23.000000 python-image-complete-0.0.4/DESCRIPTION.rst
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1097 2023-03-27 20:20:36.000000 python-image-complete-0.0.4/LICENSE
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       44 2021-08-14 06:44:26.000000 python-image-complete-0.0.4/MANIFEST.in
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1439 2023-03-29 22:55:48.044873 python-image-complete-0.0.4/PKG-INFO
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1637 2023-03-29 22:52:23.000000 python-image-complete-0.0.4/README.md
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       38 2023-03-29 22:55:48.044873 python-image-complete-0.0.4/setup.cfg
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      945 2023-03-29 22:54:06.000000 python-image-complete-0.0.4/setup.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-03-29 22:55:48.044873 python-image-complete-0.0.4/src/
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-03-29 22:55:48.044873 python-image-complete-0.0.4/src/image_complete/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)        0 2021-08-14 06:44:26.000000 python-image-complete-0.0.4/src/image_complete/__init__.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1771 2023-03-29 22:42:09.000000 python-image-complete-0.0.4/src/image_complete/auto.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      676 2023-03-29 22:21:18.000000 python-image-complete-0.0.4/src/image_complete/base.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1215 2023-03-29 22:36:37.000000 python-image-complete-0.0.4/src/image_complete/bmp.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1096 2023-03-29 22:36:37.000000 python-image-complete-0.0.4/src/image_complete/gif.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1169 2023-03-29 22:36:37.000000 python-image-complete-0.0.4/src/image_complete/jpg.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1359 2023-03-29 22:36:37.000000 python-image-complete-0.0.4/src/image_complete/png.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1444 2023-03-29 22:38:26.000000 python-image-complete-0.0.4/src/image_complete/webp.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-03-29 22:55:48.044873 python-image-complete-0.0.4/src/python_image_complete.egg-info/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1439 2023-03-29 22:55:48.000000 python-image-complete-0.0.4/src/python_image_complete.egg-info/PKG-INFO
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      478 2023-03-29 22:55:48.000000 python-image-complete-0.0.4/src/python_image_complete.egg-info/SOURCES.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)        1 2023-03-29 22:55:48.000000 python-image-complete-0.0.4/src/python_image_complete.egg-info/dependency_links.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       15 2023-03-29 22:55:48.000000 python-image-complete-0.0.4/src/python_image_complete.egg-info/top_level.txt
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-04-17 04:09:09.069997 python-image-complete-0.0.5/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      595 2023-04-17 04:03:14.000000 python-image-complete-0.0.5/CHANGES.rst
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      466 2023-03-29 22:52:23.000000 python-image-complete-0.0.5/DESCRIPTION.rst
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1097 2023-03-27 20:20:36.000000 python-image-complete-0.0.5/LICENSE
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       44 2021-08-14 06:44:26.000000 python-image-complete-0.0.5/MANIFEST.in
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1556 2023-04-17 04:09:09.069997 python-image-complete-0.0.5/PKG-INFO
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     2300 2023-04-17 04:07:57.000000 python-image-complete-0.0.5/README.md
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       38 2023-04-17 04:09:09.069997 python-image-complete-0.0.5/setup.cfg
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      945 2023-04-17 04:03:14.000000 python-image-complete-0.0.5/setup.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-04-17 04:09:09.069997 python-image-complete-0.0.5/src/
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-04-17 04:09:09.069997 python-image-complete-0.0.5/src/image_complete/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)        0 2021-08-14 06:44:26.000000 python-image-complete-0.0.5/src/image_complete/__init__.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     2398 2023-04-17 03:54:48.000000 python-image-complete-0.0.5/src/image_complete/auto.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      760 2023-04-17 03:35:32.000000 python-image-complete-0.0.5/src/image_complete/base.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1413 2023-04-17 03:24:35.000000 python-image-complete-0.0.5/src/image_complete/bmp.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1740 2023-04-17 04:06:07.000000 python-image-complete-0.0.5/src/image_complete/gif.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1867 2023-04-17 04:06:07.000000 python-image-complete-0.0.5/src/image_complete/jpg.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     2101 2023-04-17 04:05:08.000000 python-image-complete-0.0.5/src/image_complete/png.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1673 2023-04-17 03:24:35.000000 python-image-complete-0.0.5/src/image_complete/webp.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-04-17 04:09:09.069997 python-image-complete-0.0.5/src/python_image_complete.egg-info/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1556 2023-04-17 04:09:09.000000 python-image-complete-0.0.5/src/python_image_complete.egg-info/PKG-INFO
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      478 2023-04-17 04:09:09.000000 python-image-complete-0.0.5/src/python_image_complete.egg-info/SOURCES.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)        1 2023-04-17 04:09:09.000000 python-image-complete-0.0.5/src/python_image_complete.egg-info/dependency_links.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       15 2023-04-17 04:09:09.000000 python-image-complete-0.0.5/src/python_image_complete.egg-info/top_level.txt
```

### Comparing `python-image-complete-0.0.4/LICENSE` & `python-image-complete-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `python-image-complete-0.0.4/PKG-INFO` & `python-image-complete-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-image-complete
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python3 library for checking whether images are complete.
 Home-page: https://github.com/waikato-datamining/python-image-complete
 Author: Peter Reutemann
 Author-email: fracpete@waikato.ac.nz
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -26,14 +26,20 @@
 * PNG (extension: .png)
 * WebP (extension: .webp)
 
 
 Changelog
 =========
 
+0.0.5 (2023-04-17)
+------------------
+
+- added support for *lenient mode* via `strict` and `check_size` parameters
+
+
 0.0.4 (2023-03-30)
 ------------------
 
 - added support for determining completeness of bytes or BytesIO objects rather than just file names
 - added `is_XYZ` methods that determine whether a file/bytes/BytesIO represents file type `XYZ`
```

### Comparing `python-image-complete-0.0.4/setup.py` & `python-image-complete-0.0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,11 +28,11 @@
     license='MIT License',
     package_dir={
         '': 'src'
     },
     packages=[
         "image_complete",
     ],
-    version="0.0.4",
+    version="0.0.5",
     author='Peter Reutemann',
     author_email='fracpete@waikato.ac.nz',
 )
```

### Comparing `python-image-complete-0.0.4/src/image_complete/base.py` & `python-image-complete-0.0.5/src/image_complete/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 import os
 
 from io import BytesIO
 
 
+DEFAULT_CHECK_SIZE = 100
+""" the buffer size used to look for the EOF marker. """
+
+
 def load(img):
     """
     Loads the data and returns it as BytesIO object and the associated length.
 
     :param img: the image to load
     :type img: str or bytes or BytesIO
     :return: tuple of BytesIO wrapper and length
```

### Comparing `python-image-complete-0.0.4/src/image_complete/bmp.py` & `python-image-complete-0.0.5/src/image_complete/bmp.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,31 +20,36 @@
         data.seek(0)
         header = data.read(2)
         return header in [b"BM", b"BA", b"CI", b"CP", b"IC", b"PT"]
     except:
         return False
 
 
-def is_bmp_complete(img):
+def is_bmp_complete(img, strict=True):
     """
     Checks whether the BMP image is complete.
 
     https://en.wikipedia.org/wiki/BMP_file_format#File_structure
 
     :param img: the absolute path to the BMP image or a bytes/BytesIO object
     :type img: str or bytes or BytesIO
+    :param strict: if True then no junk data after actual data is allowed
+    :type strict: bool
     :return: True if complete
     :rtype: bool
     """
     try:
         data, data_len = load(img)
         if data is None:
             return False
         if data_len > 6:
             data.seek(2, 0)
             data = data.read(4)
             blen = struct.unpack('I', data)
-            return blen[0] == data_len
+            if strict:
+                return blen[0] == data_len
+            else:
+                return blen[0] <= data_len
         else:
             return False
     except:
         return False
```

### Comparing `python-image-complete-0.0.4/src/image_complete/gif.py` & `python-image-complete-0.0.5/src/image_complete/gif.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from io import BytesIO
-from .base import load
+from .base import load, DEFAULT_CHECK_SIZE
 
 
 def is_gif(img):
     """
     Checks whether the image represents a GIF.
 
     https://en.wikipedia.org/wiki/GIF#File_format
@@ -18,30 +18,44 @@
         data.seek(0)
         header = data.read(6)
         return header == b"GIF89a"
     except:
         return False
 
 
-def is_gif_complete(img):
+def is_gif_complete(img, strict=True, check_size=DEFAULT_CHECK_SIZE):
     """
     Checks whether the GIF image is complete.
 
     https://en.wikipedia.org/wiki/GIF#File_format
 
     :param img: the absolute path to the GIF image or a bytes/BytesIO object
     :type img: str or bytes or BytesIO
+    :param strict: if True then no junk data after actual data is allowed
+    :type strict: bool
+    :param check_size: the number of bytes from the end of the file to look for EOF marker
+    :type check_size: int
     :return: True if complete
     :rtype: bool
     """
     try:
         data, data_len = load(img)
         if data is None:
             return False
         if data_len > 1:
-            data.seek(data_len - 1, 0)
-            marker = data.read(1)
-            return marker[0] == 59
+            if strict:
+                data.seek(data_len - 1, 0)
+                marker = data.read(1)
+                return marker[0] == 59
+            else:
+                if check_size > data_len:
+                    check_size = data_len
+                data.seek(data_len - check_size, 0)
+                buffer = data.read(check_size)
+                for b in buffer:
+                    if b == 59:
+                        return True
+                return False
         else:
             return False
     except:
         return False
```

### Comparing `python-image-complete-0.0.4/src/image_complete/jpg.py` & `python-image-complete-0.0.5/src/image_complete/jpg.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from io import BytesIO
-from .base import load
+from .base import load, DEFAULT_CHECK_SIZE
 
 
 def is_jpg(img):
     """
     Checks whether the image represents a JPG.
 
     http://en.wikipedia.org/wiki/JPEG#Syntax_and_structure
@@ -18,30 +18,44 @@
         data.seek(0)
         header = data.read(2)
         return (header[0] == 0xFF) and (header[1] == 0xD8)
     except:
         return False
 
 
-def is_jpg_complete(img):
+def is_jpg_complete(img, strict=True, check_size=DEFAULT_CHECK_SIZE):
     """
     Checks whether the JPG image is complete.
 
     http://en.wikipedia.org/wiki/JPEG#Syntax_and_structure
 
     :param img: the absolute path to the JPG image or a bytes/BytesIO object
     :type img: str or bytes or BytesIO
+    :param strict: if True then no junk data after actual data is allowed
+    :type strict: bool
+    :param check_size: the number of bytes from the end of the file to look for EOF marker
+    :type check_size: int
     :return: True if complete
     :rtype: bool
     """
     try:
         data, data_len = load(img)
         if data is None:
             return False
         if data_len > 2:
-            data.seek(data_len - 2, 0)
-            marker = data.read(2)
-            return (marker[0] == 0xFF) and (marker[1] == 0xD9)
+            if strict:
+                data.seek(data_len - 2, 0)
+                marker = data.read(2)
+                return (marker[0] == 0xFF) and (marker[1] == 0xD9)
+            else:
+                if check_size > data_len:
+                    check_size = data_len
+                data.seek(data_len - check_size, 0)
+                buffer = data.read(check_size)
+                for i in range(len(buffer) - 1):
+                    if (buffer[i] == 0xFF) and (buffer[i+1] == 0xD9):
+                        return True
+                return False
         else:
             return False
     except:
         return False
```

### Comparing `python-image-complete-0.0.4/src/image_complete/png.py` & `python-image-complete-0.0.5/src/image_complete/png.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from io import BytesIO
-from .base import load
+from .base import load, DEFAULT_CHECK_SIZE
 
 
 def is_png(img):
     """
     Checks whether the image represents a PNG.
 
     https://en.wikipedia.org/wiki/Portable_Network_Graphics#Critical_chunks
@@ -18,32 +18,46 @@
         data.seek(1)
         header = data.read(3)
         return header in [b"PNG"]
     except:
         return False
 
 
-def is_png_complete(img):
+def is_png_complete(img, strict=True, check_size=DEFAULT_CHECK_SIZE):
     """
     Checks whether the PNG image is complete.
 
     https://en.wikipedia.org/wiki/Portable_Network_Graphics#Critical_chunks
     http://www.libpng.org/pub/png/spec/1.2/PNG-Structure.html#Chunk-layout
     http://www.libpng.org/pub/png/spec/1.2/PNG-Chunks.html#C.IEND
 
     :param img: the absolute path to the BMP image or a bytes/BytesIO object
     :type img: str or bytes or BytesIO
+    :param strict: if True then no junk data after actual data is allowed
+    :type strict: bool
+    :param check_size: the number of bytes from the end of the file to look for EOF marker
+    :type check_size: int
     :return: True if complete
     :rtype: bool
     """
     try:
         data, data_len = load(img)
         if data is None:
             return False
         if data_len > 8:
-            data.seek(data_len - 8, 0)
-            marker = data.read(8)
-            return (marker[0] == 73) and (marker[1] == 69) and (marker[2] == 78) and (marker[3] == 68)
+            if strict:
+                data.seek(data_len - 8, 0)
+                marker = data.read(8)
+                return (marker[0] == 73) and (marker[1] == 69) and (marker[2] == 78) and (marker[3] == 68)
+            else:
+                if check_size > data_len:
+                    check_size = data_len
+                data.seek(data_len - check_size, 0)
+                buffer = data.read(check_size)
+                for i in range(len(buffer) - 8):
+                    if (buffer[i] == 73) and (buffer[i+1] == 69) and (buffer[i+2] == 78) and (buffer[i+3] == 68):
+                        return True
+                return False
         else:
             return False
     except:
         return False
```

### Comparing `python-image-complete-0.0.4/src/image_complete/webp.py` & `python-image-complete-0.0.5/src/image_complete/webp.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,22 +20,24 @@
         data.seek(0, 0)
         data = data.read(4)
         return data.decode("utf-8") == "RIFF"
     except:
         return False
 
 
-def is_webp_complete(img):
+def is_webp_complete(img, strict=True):
     """
     Checks whether the WebP image is complete.
 
     https://developers.google.com/speed/webp/docs/riff_container
 
     :param img: the absolute path to the BMP image or a bytes/BytesIO object
     :type img: str or bytes or BytesIO
+    :param strict: if True then no junk data after actual data is allowed
+    :type strict: bool
     :return: True if complete
     :rtype: bool
     """
 
     try:
         data, data_len = load(img)
         if data is None:
@@ -46,12 +48,15 @@
             d = data.read(4)
             if d.decode("utf-8") != "RIFF":
                 return False
             # check data length against file length
             data.seek(4, 0)
             data = data.read(4)
             d_len = struct.unpack('I', data)
-            return d_len[0] == data_len - 8  # RIFF/4 + DATALEN/4 = 8
+            if strict:
+                return d_len[0] == data_len - 8  # RIFF/4 + DATALEN/4 = 8
+            else:
+                return d_len[0] <= data_len - 8  # RIFF/4 + DATALEN/4 = 8
         else:
             return False
     except:
         return False
```

### Comparing `python-image-complete-0.0.4/src/python_image_complete.egg-info/PKG-INFO` & `python-image-complete-0.0.5/src/python_image_complete.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-image-complete
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python3 library for checking whether images are complete.
 Home-page: https://github.com/waikato-datamining/python-image-complete
 Author: Peter Reutemann
 Author-email: fracpete@waikato.ac.nz
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -26,14 +26,20 @@
 * PNG (extension: .png)
 * WebP (extension: .webp)
 
 
 Changelog
 =========
 
+0.0.5 (2023-04-17)
+------------------
+
+- added support for *lenient mode* via `strict` and `check_size` parameters
+
+
 0.0.4 (2023-03-30)
 ------------------
 
 - added support for determining completeness of bytes or BytesIO objects rather than just file names
 - added `is_XYZ` methods that determine whether a file/bytes/BytesIO represents file type `XYZ`
```

