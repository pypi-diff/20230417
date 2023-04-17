# Comparing `tmp/xia_engine_terraform-0.0.5-cp39-none-win_amd64.whl.zip` & `tmp/xia_engine_terraform-0.0.6-cp39-none-macosx_11_0_x86_64.whl.zip`

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
+Zip file size: 134877 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      394 b- defN 23-Apr-17 09:10 xia_engine_terraform/__init__.py
+-rw-r--r--  2.0 unx   372552 b- defN 23-Apr-17 09:11 xia_engine_terraform/engine.cpython-310-darwin.so
+-rw-r--r--  2.0 unx      152 b- defN 23-Apr-17 09:11 xia_engine_terraform-0.0.6.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      699 b- defN 23-Apr-17 09:11 xia_engine_terraform-0.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-Apr-17 09:11 xia_engine_terraform-0.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       21 b- defN 23-Apr-17 09:11 xia_engine_terraform-0.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      650 b- defN 23-Apr-17 09:11 xia_engine_terraform-0.0.6.dist-info/RECORD
+7 files, 374576 bytes uncompressed, 133705 bytes compressed:  64.3%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_engine_terraform/__init__.py
 Comment: 
 
-Filename: xia_engine_terraform/engine.cp39-win_amd64.pyd
+Filename: xia_engine_terraform/engine.cpython-310-darwin.so
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

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: xia-engine-terraform
-Version: 0.0.5
+Version: 0.0.6
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-engine-terraform/0.0.5/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-engine-terraform/0.0.6/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
-License: UNKNOWN
-Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 Requires-Dist: jinja2
 Requires-Dist: google-cloud-storage
 Requires-Dist: xia-engine
 
@@ -28,9 +26,7 @@
 =============================
 
 Install the package::
 
     pip install
 
 
-
-
```

