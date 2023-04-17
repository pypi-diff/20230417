# Comparing `tmp/home_assistant_chip_clusters-2023.2.2-py3-none-any.whl.zip` & `tmp/home_assistant_chip_clusters-2023.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 91375 bytes, number of entries: 12
--rw-r--r--  2.0 unx     2175 b- defN 23-Feb-21 16:37 chip/ChipUtility.py
--rw-r--r--  2.0 unx   283478 b- defN 23-Feb-21 16:37 chip/clusters/CHIPClusters.py
--rw-r--r--  2.0 unx    12959 b- defN 23-Feb-21 16:37 chip/clusters/ClusterObjects.py
--rw-r--r--  2.0 unx  1183596 b- defN 23-Feb-21 16:37 chip/clusters/Objects.py
--rw-r--r--  2.0 unx     1945 b- defN 23-Feb-21 16:37 chip/clusters/TestObjects.py
--rw-r--r--  2.0 unx      972 b- defN 23-Feb-21 16:37 chip/clusters/Types.py
--rw-r--r--  2.0 unx    28824 b- defN 23-Feb-21 16:37 chip/tlv/__init__.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Feb-21 16:37 home_assistant_chip_clusters-2023.2.2.dist-info/LICENSE
--rw-r--r--  2.0 unx      527 b- defN 23-Feb-21 16:37 home_assistant_chip_clusters-2023.2.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-21 16:37 home_assistant_chip_clusters-2023.2.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Feb-21 16:37 home_assistant_chip_clusters-2023.2.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1083 b- defN 23-Feb-21 16:37 home_assistant_chip_clusters-2023.2.2.dist-info/RECORD
-12 files, 1527013 bytes uncompressed, 89537 bytes compressed:  94.1%
+Zip file size: 91374 bytes, number of entries: 12
+-rw-r--r--  2.0 unx     2175 b- defN 23-Apr-17 10:32 chip/ChipUtility.py
+-rw-r--r--  2.0 unx   283478 b- defN 23-Apr-17 10:32 chip/clusters/CHIPClusters.py
+-rw-r--r--  2.0 unx    12959 b- defN 23-Apr-17 10:32 chip/clusters/ClusterObjects.py
+-rw-r--r--  2.0 unx  1183596 b- defN 23-Apr-17 10:32 chip/clusters/Objects.py
+-rw-r--r--  2.0 unx     1945 b- defN 23-Apr-17 10:32 chip/clusters/TestObjects.py
+-rw-r--r--  2.0 unx      972 b- defN 23-Apr-17 10:32 chip/clusters/Types.py
+-rw-r--r--  2.0 unx    28824 b- defN 23-Apr-17 10:32 chip/tlv/__init__.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Apr-17 10:32 home_assistant_chip_clusters-2023.4.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      527 b- defN 23-Apr-17 10:32 home_assistant_chip_clusters-2023.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-17 10:32 home_assistant_chip_clusters-2023.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Apr-17 10:32 home_assistant_chip_clusters-2023.4.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1083 b- defN 23-Apr-17 10:32 home_assistant_chip_clusters-2023.4.0.dist-info/RECORD
+12 files, 1527013 bytes uncompressed, 89536 bytes compressed:  94.1%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: chip/clusters/Types.py
 Comment: 
 
 Filename: chip/tlv/__init__.py
 Comment: 
 
-Filename: home_assistant_chip_clusters-2023.2.2.dist-info/LICENSE
+Filename: home_assistant_chip_clusters-2023.4.0.dist-info/LICENSE
 Comment: 
 
-Filename: home_assistant_chip_clusters-2023.2.2.dist-info/METADATA
+Filename: home_assistant_chip_clusters-2023.4.0.dist-info/METADATA
 Comment: 
 
-Filename: home_assistant_chip_clusters-2023.2.2.dist-info/WHEEL
+Filename: home_assistant_chip_clusters-2023.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: home_assistant_chip_clusters-2023.2.2.dist-info/top_level.txt
+Filename: home_assistant_chip_clusters-2023.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: home_assistant_chip_clusters-2023.2.2.dist-info/RECORD
+Filename: home_assistant_chip_clusters-2023.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `home_assistant_chip_clusters-2023.2.2.dist-info/LICENSE` & `home_assistant_chip_clusters-2023.4.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `home_assistant_chip_clusters-2023.2.2.dist-info/METADATA` & `home_assistant_chip_clusters-2023.4.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: home-assistant-chip-clusters
-Version: 2023.2.2
+Version: 2023.4.0
 Summary: Python-base APIs and tools for CHIP.
 Home-page: https://github.com/project-chip/connectedhomeip
 License: Apache
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
```

## Comparing `home_assistant_chip_clusters-2023.2.2.dist-info/RECORD` & `home_assistant_chip_clusters-2023.4.0.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 chip/ChipUtility.py,sha256=jhHl2Jxf3XxNEqYqsahS_yVnMLM1_pUxEYn-bqsR6oE,2175
 chip/clusters/CHIPClusters.py,sha256=xwOn-5qJo7N9rAVdzhC60wiMPLklPSpfDedV0wzIXGg,283478
 chip/clusters/ClusterObjects.py,sha256=die71TG9uKINaWtYWEVWxMOeP6-r9o-jEL6BLMC5Dys,12959
 chip/clusters/Objects.py,sha256=7Bq-9PXKhOeZ8I7azmF2lTEeSElRZVVUFwldoF1p2Lw,1183596
 chip/clusters/TestObjects.py,sha256=88W9PAc1iV_gTHGLY4MMxhPzXPKvU4CiQ4jzrrHSH2A,1945
 chip/clusters/Types.py,sha256=4pEp46uHkg8_F8KQ0DNcsIE6bGwvnDRCk9RrI3iHtaQ,972
 chip/tlv/__init__.py,sha256=erjEmevCuma4xMHsJ-VPMYmHhCQHtiwy23nU1Qg3j4I,28824
-home_assistant_chip_clusters-2023.2.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-home_assistant_chip_clusters-2023.2.2.dist-info/METADATA,sha256=FbDN0HOt2y3Jg9JApDpBLBqAVgnBEID6N_Gk9jcS4N0,527
-home_assistant_chip_clusters-2023.2.2.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-home_assistant_chip_clusters-2023.2.2.dist-info/top_level.txt,sha256=5pBsfKK6BMqu66YKYb0-uQqOgrqirLFfcBFAxXDNme0,5
-home_assistant_chip_clusters-2023.2.2.dist-info/RECORD,,
+home_assistant_chip_clusters-2023.4.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+home_assistant_chip_clusters-2023.4.0.dist-info/METADATA,sha256=JhIM_N3SFXxgpPuuvXlNQHgFESNuWxRfvo__hXJ4Bag,527
+home_assistant_chip_clusters-2023.4.0.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+home_assistant_chip_clusters-2023.4.0.dist-info/top_level.txt,sha256=5pBsfKK6BMqu66YKYb0-uQqOgrqirLFfcBFAxXDNme0,5
+home_assistant_chip_clusters-2023.4.0.dist-info/RECORD,,
```

