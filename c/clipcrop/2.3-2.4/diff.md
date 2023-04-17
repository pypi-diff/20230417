# Comparing `tmp/clipcrop-2.3.tar.gz` & `tmp/clipcrop-2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clipcrop-2.3.tar", last modified: Thu Apr 13 13:37:20 2023, max compression
+gzip compressed data, was "clipcrop-2.4.tar", last modified: Mon Apr 17 14:31:20 2023, max compression
```

## Comparing `clipcrop-2.3.tar` & `clipcrop-2.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:37:20.932810 clipcrop-2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-13 13:37:10.000000 clipcrop-2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-04-13 13:37:20.932810 clipcrop-2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-13 13:37:10.000000 clipcrop-2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:37:20.932810 clipcrop-2.3/clipcrop/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 13:37:10.000000 clipcrop-2.3/clipcrop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-04-13 13:37:10.000000 clipcrop-2.3/clipcrop/clipcrop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:37:20.932810 clipcrop-2.3/clipcrop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-04-13 13:37:20.000000 clipcrop-2.3/clipcrop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-13 13:37:20.000000 clipcrop-2.3/clipcrop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 13:37:20.000000 clipcrop-2.3/clipcrop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 13:37:20.000000 clipcrop-2.3/clipcrop.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-13 13:37:20.000000 clipcrop-2.3/clipcrop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-13 13:37:20.000000 clipcrop-2.3/clipcrop.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-13 13:37:20.936810 clipcrop-2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-04-13 13:37:10.000000 clipcrop-2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:31:20.543640 clipcrop-2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-17 14:30:57.000000 clipcrop-2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-04-17 14:31:20.543640 clipcrop-2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-04-17 14:30:57.000000 clipcrop-2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:31:20.543640 clipcrop-2.4/clipcrop/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 14:30:57.000000 clipcrop-2.4/clipcrop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-04-17 14:30:57.000000 clipcrop-2.4/clipcrop/clipcrop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:31:20.543640 clipcrop-2.4/clipcrop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-04-17 14:31:20.000000 clipcrop-2.4/clipcrop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-17 14:31:20.000000 clipcrop-2.4/clipcrop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 14:31:20.000000 clipcrop-2.4/clipcrop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 14:31:20.000000 clipcrop-2.4/clipcrop.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-17 14:31:20.000000 clipcrop-2.4/clipcrop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-17 14:31:20.000000 clipcrop-2.4/clipcrop.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-17 14:31:20.543640 clipcrop-2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-04-17 14:30:57.000000 clipcrop-2.4/setup.py
```

### Comparing `clipcrop-2.3/LICENSE` & `clipcrop-2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `clipcrop-2.3/PKG-INFO` & `clipcrop-2.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipcrop
-Version: 2.3
+Version: 2.4
 Summary: Extract sections from your image by using OpenAI CLIP and Facebooks Detr implemented on HuggingFace Transformers
 Home-page: https://github.com/Vishnunkumar/clipcrop/
 Author: Vishnu Nandakumar
 Author-email: nkumarvishnu25@gmail.com
 License: MIT license
 Keywords: clipcrop
 Classifier: Development Status :: 3 - Alpha
@@ -65,23 +65,20 @@
 </p> -->
 
 ### Captcha
 Solve captacha images using CLIP and Object detection models.
 
 ```python
 from clipcrop import clipcrop
-
 # second arguement is the text prompt eg:image of cars
 clipc = clipcrop.ClipCrop(image_path, "image of cars")
-
 #loading models, processors, feature extractors
 DFE, DM, CLIPM, CLIPP = clipc.load_models()
-
 #generally keep high threshold to avoid noises
-result = clipc.captcha(DFE, DM, CLIPM, CLIPP, th=0.99)
+result = clipc.captcha(CLIPM, CLIPP, 4)
 ```
 
 ## Clip Segmentation
 
 Segment out images using Detr Panoptic segmentation pipeline and leverage CLIP models to derive at the most probable one for your query
 
 ### Implementation
```

### Comparing `clipcrop-2.3/README.md` & `clipcrop-2.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -45,23 +45,20 @@
 </p> -->
 
 ### Captcha
 Solve captacha images using CLIP and Object detection models.
 
 ```python
 from clipcrop import clipcrop
-
 # second arguement is the text prompt eg:image of cars
 clipc = clipcrop.ClipCrop(image_path, "image of cars")
-
 #loading models, processors, feature extractors
 DFE, DM, CLIPM, CLIPP = clipc.load_models()
-
 #generally keep high threshold to avoid noises
-result = clipc.captcha(DFE, DM, CLIPM, CLIPP, th=0.99)
+result = clipc.captcha(CLIPM, CLIPP, 4)
 ```
 
 ## Clip Segmentation
 
 Segment out images using Detr Panoptic segmentation pipeline and leverage CLIP models to derive at the most probable one for your query
 
 ### Implementation
```

### Comparing `clipcrop-2.3/clipcrop/clipcrop.py` & `clipcrop-2.4/clipcrop/clipcrop.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,47 @@
 import numpy as np
-from PIL import Image
-from transformers import CLIPProcessor, CLIPModel, DetrFeatureExtractor, DetrForObjectDetection, pipeline
 import torch 
 import cv2
+import pytesseract
+from PIL import Image
+from transformers import CLIPProcessor, CLIPModel, DetrFeatureExtractor, DetrForObjectDetection, pipeline
 
 class ClipCrop():
 
-  def __init__(self, image_path, text):
+  def __init__(self, image_path):
 
     self.image_path = image_path
-    self.text = text
     
-  
   def load_models(self):
 
     DFE = DetrFeatureExtractor.from_pretrained('facebook/detr-resnet-50')
     DM = DetrForObjectDetection.from_pretrained('facebook/detr-resnet-50')
     CLIPM = CLIPModel.from_pretrained("openai/clip-vit-base-patch32")
     CLIPP = CLIPProcessor.from_pretrained("openai/clip-vit-base-patch32")
 
     return DFE, DM, CLIPM, CLIPP
 
-  def captcha(self, CLIPM, CLIPP, th=3):
+  def auto_captcha(self, CLIPM, CLIPP, th=3):
     
     self.th = th
     self.CLIPM = CLIPM
     self.CLIPP = CLIPP
 
     image = cv2.imread(self.image_path)
     gray = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
+
+    # Get the text from the image
+    ret, thresh = cv2.threshold(img, 220, 255, cv2.THRESH_BINARY)
+    kernel = cv2.getStructuringElement(cv2.MORPH_RECT, (1,1))
+    close = cv2.erode(thresh, kernel, iterations=2)
+    invert = cv2.bitwise_not(close)
+    inf = pytesseract.image_to_string(invert)
+    txt = [x for x in inf.split('\n') if len(x) > 2][1]
+
+    # Process for captcha resolution
     blur = cv2.medianBlur(gray, 3)
     sharpen_kernel = np.array([[-1,-1,-1], [-1,9,-1], [-1,-1,-1]])
     sharpen = cv2.filter2D(blur, -1, sharpen_kernel)
 
     # Threshold and morph close
     thresh = cv2.threshold(sharpen, 160, 255, cv2.THRESH_BINARY_INV)[1]
     kernel = cv2.getStructuringElement(cv2.MORPH_RECT, (1,1))
@@ -49,32 +58,33 @@
         x,y,w,h = cv2.boundingRect(c)
         if w/h == 1 and (w, h) > (5, 5):
             ROI = image[y:y+h, x:x+w]
             img_list.append(Image.fromarray(ROI[:,:,::-1]))
             r_list.append([(x, y), (x + w, y + h)])
             image_number += 1
 
-    inps = self.CLIPP(text = [self.text], images=img_list , return_tensors="pt", padding=True)
+    inps = self.CLIPP(text = [txt], images=img_list , return_tensors="pt", padding=True)
     outs = self.CLIPM(**inps)
     logits_per_image = outs.logits_per_text
     probs = logits_per_image.softmax(-1)
     l_idx = list(np.argsort(probs[-1].detach().numpy())[::-1][0:self.th])
 
     for x in l_idx:
       cv2.rectangle(image, r_list[x][0], r_list[x][1], (36,255,12), 2)
 
     return Image.fromarray(image[:,:,::-1])
 
-  def extract_image(self, DFE, DM, CLIPM, CLIPP, num=3):
+  def extract_image(self, DFE, DM, CLIPM, CLIPP, text, num=3):
 
     self.DFE = DFE
     self.DM = DM
     self.CLIPM = CLIPM
     self.CLIPP = CLIPP
     self.num = num
+    self.text = text
     
     image = cv2.imread(self.image_path)
     inputs = self.DFE(images=image, return_tensors="pt")
     outputs = self.DM(**inputs)
 
     # model predicts bounding boxes and corresponding COCO classes
     logits = outputs.logits
```

### Comparing `clipcrop-2.3/clipcrop.egg-info/PKG-INFO` & `clipcrop-2.4/clipcrop.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipcrop
-Version: 2.3
+Version: 2.4
 Summary: Extract sections from your image by using OpenAI CLIP and Facebooks Detr implemented on HuggingFace Transformers
 Home-page: https://github.com/Vishnunkumar/clipcrop/
 Author: Vishnu Nandakumar
 Author-email: nkumarvishnu25@gmail.com
 License: MIT license
 Keywords: clipcrop
 Classifier: Development Status :: 3 - Alpha
@@ -65,23 +65,20 @@
 </p> -->
 
 ### Captcha
 Solve captacha images using CLIP and Object detection models.
 
 ```python
 from clipcrop import clipcrop
-
 # second arguement is the text prompt eg:image of cars
 clipc = clipcrop.ClipCrop(image_path, "image of cars")
-
 #loading models, processors, feature extractors
 DFE, DM, CLIPM, CLIPP = clipc.load_models()
-
 #generally keep high threshold to avoid noises
-result = clipc.captcha(DFE, DM, CLIPM, CLIPP, th=0.99)
+result = clipc.captcha(CLIPM, CLIPP, 4)
 ```
 
 ## Clip Segmentation
 
 Segment out images using Detr Panoptic segmentation pipeline and leverage CLIP models to derive at the most probable one for your query
 
 ### Implementation
```

### Comparing `clipcrop-2.3/setup.py` & `clipcrop-2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,21 +39,22 @@
 
 requirements = [
   'transformers',
   'torch',
   'pillow',
   'timm',
   'numpy',
-  'opencv-python'
+  'opencv-python',
+  'pytesseract'
 ]
 
 
 setuptools.setup(
     name="clipcrop",
-    version="2.3",
+    version="2.4",
     author="Vishnu Nandakumar",
     author_email="nkumarvishnu25@gmail.com",
     description="Extract sections from your image by using OpenAI CLIP and Facebooks Detr implemented on HuggingFace Transformers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url = 'https://github.com/Vishnunkumar/clipcrop/',
     packages=[
```

