# Comparing `tmp/i3dFeatureExtraction-0.1-py3-none-any.whl.zip` & `tmp/i3dFeatureExtraction-0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 16835 bytes, number of entries: 15
+Zip file size: 16798 bytes, number of entries: 15
 -rw-rw-rw-  2.0 fat     4087 b- defN 23-Apr-17 09:23 i3dFeatureExtraction/__init__.py
 -rw-rw-rw-  2.0 fat    10423 b- defN 23-Apr-17 01:43 i3dFeatureExtraction/extract_features.py
 -rw-rw-rw-  2.0 fat     2294 b- defN 23-Mar-27 11:20 i3dFeatureExtraction/extract_features_org.py
 -rw-rw-rw-  2.0 fat     2136 b- defN 23-Mar-27 11:20 i3dFeatureExtraction/extract_main.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-27 11:20 i3dFeatureExtraction/models/__init__.py
 -rw-rw-rw-  2.0 fat     2235 b- defN 23-Mar-27 11:20 i3dFeatureExtraction/models/model_builder_video.py
 -rw-rw-rw-  2.0 fat     3803 b- defN 23-Mar-27 11:20 i3dFeatureExtraction/models/nonlocal_helper.py
 -rw-rw-rw-  2.0 fat     7644 b- defN 23-Mar-27 13:19 i3dFeatureExtraction/models/resnet.py
 -rw-rw-rw-  2.0 fat     3998 b- defN 23-Mar-27 11:20 i3dFeatureExtraction/models/resnet_helper.py
 -rw-rw-rw-  2.0 fat     3220 b- defN 23-Mar-27 11:20 i3dFeatureExtraction/models/resnet_video_org.py
--rw-rw-rw-  2.0 fat     1355 b- defN 23-Apr-17 09:40 i3dFeatureExtraction-0.1.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     2120 b- defN 23-Apr-17 09:40 i3dFeatureExtraction-0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-17 09:40 i3dFeatureExtraction-0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       21 b- defN 23-Apr-17 09:40 i3dFeatureExtraction-0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1428 b- defN 23-Apr-17 09:40 i3dFeatureExtraction-0.1.dist-info/RECORD
-15 files, 44856 bytes uncompressed, 14407 bytes compressed:  67.9%
+-rw-rw-rw-  2.0 fat     1355 b- defN 23-Apr-17 09:57 i3dFeatureExtraction-0.2.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     1932 b- defN 23-Apr-17 09:57 i3dFeatureExtraction-0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-17 09:57 i3dFeatureExtraction-0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       21 b- defN 23-Apr-17 09:57 i3dFeatureExtraction-0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1428 b- defN 23-Apr-17 09:57 i3dFeatureExtraction-0.2.dist-info/RECORD
+15 files, 44668 bytes uncompressed, 14370 bytes compressed:  67.8%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: i3dFeatureExtraction/models/resnet_helper.py
 Comment: 
 
 Filename: i3dFeatureExtraction/models/resnet_video_org.py
 Comment: 
 
-Filename: i3dFeatureExtraction-0.1.dist-info/LICENSE.txt
+Filename: i3dFeatureExtraction-0.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: i3dFeatureExtraction-0.1.dist-info/METADATA
+Filename: i3dFeatureExtraction-0.2.dist-info/METADATA
 Comment: 
 
-Filename: i3dFeatureExtraction-0.1.dist-info/WHEEL
+Filename: i3dFeatureExtraction-0.2.dist-info/WHEEL
 Comment: 
 
-Filename: i3dFeatureExtraction-0.1.dist-info/top_level.txt
+Filename: i3dFeatureExtraction-0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: i3dFeatureExtraction-0.1.dist-info/RECORD
+Filename: i3dFeatureExtraction-0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `i3dFeatureExtraction-0.1.dist-info/LICENSE.txt` & `i3dFeatureExtraction-0.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `i3dFeatureExtraction-0.1.dist-info/METADATA` & `i3dFeatureExtraction-0.2.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i3dFeatureExtraction
-Version: 0.1
+Version: 0.2
 Summary: This package helps extract i3D features with ResNet-50 backbone given a folder of videos
 Author: Hao Vy Phan
 Author-email: vyhao03@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Freely Distributable
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.8
@@ -41,17 +41,14 @@
 Requires-Dist: python-dateutil (==2.8.2)
 Requires-Dist: pytz (==2023.3)
 Requires-Dist: PyYAML (==6.0)
 Requires-Dist: requests (==2.28.1)
 Requires-Dist: six (==1.16.0)
 Requires-Dist: SQLAlchemy (==2.0.9)
 Requires-Dist: textwrap3
-Requires-Dist: torch-1.10.1-cu113-cp38-cp38-win-amd64.whl
-Requires-Dist: torchaudio-0.10.1-cu113-cp38-cp38-win-amd64.whl
-Requires-Dist: torchvision-0.11.2-cu113-cp38-cp38-win-amd64.whl
 Requires-Dist: tqdm (==4.34.0)
 Requires-Dist: typing-extensions (==4.5.0)
 Requires-Dist: tzdata (==2023.3)
 Requires-Dist: urllib3 (==1.26.15)
 Requires-Dist: Werkzeug (==2.2.2)
 Requires-Dist: zipp (==3.15.0)
```

## Comparing `i3dFeatureExtraction-0.1.dist-info/RECORD` & `i3dFeatureExtraction-0.2.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -4,12 +4,12 @@
 i3dFeatureExtraction/extract_main.py,sha256=m7b8y-wBc0gzhKtBImAh-pUXWz4Ch5w2e1ySyCDiclk,2136
 i3dFeatureExtraction/models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 i3dFeatureExtraction/models/model_builder_video.py,sha256=Rhq75giPwKqyqgsHXFQaEEKi_KEdT2nIy_RmLHYO7OU,2235
 i3dFeatureExtraction/models/nonlocal_helper.py,sha256=bP3x2hRSY58t2neeAhHOi-bivJohBUPNPyhZJBTcZ6k,3803
 i3dFeatureExtraction/models/resnet.py,sha256=MmQoaa0Z0dOFVnMe-Rb-qnjeTDnXvExx9zjE92OIGMc,7644
 i3dFeatureExtraction/models/resnet_helper.py,sha256=7LRnIYmbaQVqrdNgyKlwvWR7_9ad41RDEDpgSeehSk8,3998
 i3dFeatureExtraction/models/resnet_video_org.py,sha256=EUNucgPLxwerOV2QPWPrNqD6YfHahn_N4E0zXbtDRN0,3220
-i3dFeatureExtraction-0.1.dist-info/LICENSE.txt,sha256=ncWu_RGjXBnqZDrVVTs4ZSKposYA5lAiRiUJbdMWQO0,1355
-i3dFeatureExtraction-0.1.dist-info/METADATA,sha256=lnNcQUJ5eBCG6j3vxnYeIfRsu90g9BqYzLN6kFcnzq4,2120
-i3dFeatureExtraction-0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-i3dFeatureExtraction-0.1.dist-info/top_level.txt,sha256=yxjkhX408DHF75Tq1cxynym3i0_cdZNOnuxa8aMvK2s,21
-i3dFeatureExtraction-0.1.dist-info/RECORD,,
+i3dFeatureExtraction-0.2.dist-info/LICENSE.txt,sha256=ncWu_RGjXBnqZDrVVTs4ZSKposYA5lAiRiUJbdMWQO0,1355
+i3dFeatureExtraction-0.2.dist-info/METADATA,sha256=sI_R8aZL76gOI8RTHGkezhB4yRibYVezH9shy8p9QtU,1932
+i3dFeatureExtraction-0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+i3dFeatureExtraction-0.2.dist-info/top_level.txt,sha256=yxjkhX408DHF75Tq1cxynym3i0_cdZNOnuxa8aMvK2s,21
+i3dFeatureExtraction-0.2.dist-info/RECORD,,
```

