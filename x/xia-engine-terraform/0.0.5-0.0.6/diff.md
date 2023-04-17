# Comparing `tmp/xia_engine_terraform-0.0.5-cp39-none-win_amd64.whl.zip` & `tmp/xia_engine_terraform-0.0.6-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 158682 bytes, number of entries: 7
--rw-r--r--  2.0 unx      394 b- defN 23-Apr-16 20:41 xia_engine_terraform/__init__.py
--rw-r--r--  2.0 unx   405504 b- defN 23-Apr-16 20:44 xia_engine_terraform/engine.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-16 20:44 xia_engine_terraform-0.0.5.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      736 b- defN 23-Apr-16 20:44 xia_engine_terraform-0.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Apr-16 20:44 xia_engine_terraform-0.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       21 b- defN 23-Apr-16 20:44 xia_engine_terraform-0.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      646 b- defN 23-Apr-16 20:44 xia_engine_terraform-0.0.5.dist-info/RECORD
-7 files, 407552 bytes uncompressed, 157516 bytes compressed:  61.4%
+Zip file size: 165335 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      394 b- defN 23-Apr-17 09:09 xia_engine_terraform/__init__.py
+-rw-r--r--  2.0 unx   423936 b- defN 23-Apr-17 09:12 xia_engine_terraform/engine.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-17 09:12 xia_engine_terraform-0.0.6.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      736 b- defN 23-Apr-17 09:12 xia_engine_terraform-0.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Apr-17 09:12 xia_engine_terraform-0.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       21 b- defN 23-Apr-17 09:12 xia_engine_terraform-0.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      646 b- defN 23-Apr-17 09:12 xia_engine_terraform-0.0.6.dist-info/RECORD
+7 files, 425984 bytes uncompressed, 164169 bytes compressed:  61.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_engine_terraform/__init__.py
 Comment: 
 
 Filename: xia_engine_terraform/engine.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_engine_terraform-0.0.5.dist-info/LICENSE.txt
+Filename: xia_engine_terraform-0.0.6.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_engine_terraform-0.0.5.dist-info/METADATA
+Filename: xia_engine_terraform-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: xia_engine_terraform-0.0.5.dist-info/WHEEL
+Filename: xia_engine_terraform-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: xia_engine_terraform-0.0.5.dist-info/top_level.txt
+Filename: xia_engine_terraform-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_engine_terraform-0.0.5.dist-info/RECORD
+Filename: xia_engine_terraform-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_engine_terraform/__init__.py

```diff
@@ -3,8 +3,8 @@
 
 
 __all__ = [
     "TerraformEngine", "TerraformConnectParam", "TerraformClient",
     "TerraformLocalEngine", "TerraformLocalConnectParam", "TerraformLocalClient"
 ]
 
-__version__ = "0.0.5"
+__version__ = "0.0.6"
```

## Comparing `xia_engine_terraform-0.0.5.dist-info/METADATA` & `xia_engine_terraform-0.0.6.dist-info/METADATA`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-engine-terraform
-Version: 0.0.5
+Version: 0.0.6
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-engine-terraform/0.0.5/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-engine-terraform/0.0.6/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

