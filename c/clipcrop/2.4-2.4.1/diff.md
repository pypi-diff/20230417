# Comparing `tmp/clipcrop-2.4.tar.gz` & `tmp/clipcrop-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clipcrop-2.4.tar", last modified: Mon Apr 17 14:31:20 2023, max compression
+gzip compressed data, was "clipcrop-2.4.1.tar", last modified: Mon Apr 17 14:43:26 2023, max compression
```

## Comparing `clipcrop-2.4.tar` & `clipcrop-2.4.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:31:20.543640 clipcrop-2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-17 14:30:57.000000 clipcrop-2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-04-17 14:31:20.543640 clipcrop-2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-04-17 14:30:57.000000 clipcrop-2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:31:20.543640 clipcrop-2.4/clipcrop/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 14:30:57.000000 clipcrop-2.4/clipcrop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-04-17 14:30:57.000000 clipcrop-2.4/clipcrop/clipcrop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:31:20.543640 clipcrop-2.4/clipcrop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-04-17 14:31:20.000000 clipcrop-2.4/clipcrop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-17 14:31:20.000000 clipcrop-2.4/clipcrop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 14:31:20.000000 clipcrop-2.4/clipcrop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 14:31:20.000000 clipcrop-2.4/clipcrop.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-17 14:31:20.000000 clipcrop-2.4/clipcrop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-17 14:31:20.000000 clipcrop-2.4/clipcrop.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-17 14:31:20.543640 clipcrop-2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-04-17 14:30:57.000000 clipcrop-2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:43:26.124187 clipcrop-2.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-17 14:43:17.000000 clipcrop-2.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-04-17 14:43:26.124187 clipcrop-2.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-04-17 14:43:17.000000 clipcrop-2.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:43:26.124187 clipcrop-2.4.1/clipcrop/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 14:43:17.000000 clipcrop-2.4.1/clipcrop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-04-17 14:43:17.000000 clipcrop-2.4.1/clipcrop/clipcrop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:43:26.124187 clipcrop-2.4.1/clipcrop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-04-17 14:43:26.000000 clipcrop-2.4.1/clipcrop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-17 14:43:26.000000 clipcrop-2.4.1/clipcrop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 14:43:26.000000 clipcrop-2.4.1/clipcrop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 14:43:26.000000 clipcrop-2.4.1/clipcrop.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-17 14:43:26.000000 clipcrop-2.4.1/clipcrop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-17 14:43:26.000000 clipcrop-2.4.1/clipcrop.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-17 14:43:26.124187 clipcrop-2.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-04-17 14:43:17.000000 clipcrop-2.4.1/setup.py
```

### Comparing `clipcrop-2.4/LICENSE` & `clipcrop-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clipcrop-2.4/PKG-INFO` & `clipcrop-2.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipcrop
-Version: 2.4
+Version: 2.4.1
 Summary: Extract sections from your image by using OpenAI CLIP and Facebooks Detr implemented on HuggingFace Transformers
 Home-page: https://github.com/Vishnunkumar/clipcrop/
 Author: Vishnu Nandakumar
 Author-email: nkumarvishnu25@gmail.com
 License: MIT license
 Keywords: clipcrop
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `clipcrop-2.4/README.md` & `clipcrop-2.4.1/README.md`

 * *Files identical despite different names*

### Comparing `clipcrop-2.4/clipcrop/clipcrop.py` & `clipcrop-2.4.1/clipcrop/clipcrop.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     self.CLIPM = CLIPM
     self.CLIPP = CLIPP
 
     image = cv2.imread(self.image_path)
     gray = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
 
     # Get the text from the image
-    ret, thresh = cv2.threshold(img, 220, 255, cv2.THRESH_BINARY)
+    ret, thresh = cv2.threshold(gray, 220, 255, cv2.THRESH_BINARY)
     kernel = cv2.getStructuringElement(cv2.MORPH_RECT, (1,1))
     close = cv2.erode(thresh, kernel, iterations=2)
     invert = cv2.bitwise_not(close)
     inf = pytesseract.image_to_string(invert)
     txt = [x for x in inf.split('\n') if len(x) > 2][1]
 
     # Process for captcha resolution
```

### Comparing `clipcrop-2.4/clipcrop.egg-info/PKG-INFO` & `clipcrop-2.4.1/clipcrop.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipcrop
-Version: 2.4
+Version: 2.4.1
 Summary: Extract sections from your image by using OpenAI CLIP and Facebooks Detr implemented on HuggingFace Transformers
 Home-page: https://github.com/Vishnunkumar/clipcrop/
 Author: Vishnu Nandakumar
 Author-email: nkumarvishnu25@gmail.com
 License: MIT license
 Keywords: clipcrop
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `clipcrop-2.4/setup.py` & `clipcrop-2.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
   'opencv-python',
   'pytesseract'
 ]
 
 
 setuptools.setup(
     name="clipcrop",
-    version="2.4",
+    version="2.4.1",
     author="Vishnu Nandakumar",
     author_email="nkumarvishnu25@gmail.com",
     description="Extract sections from your image by using OpenAI CLIP and Facebooks Detr implemented on HuggingFace Transformers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url = 'https://github.com/Vishnunkumar/clipcrop/',
     packages=[
```

