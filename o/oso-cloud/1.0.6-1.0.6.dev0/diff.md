# Comparing `tmp/oso_cloud-1.0.6-py3-none-any.whl.zip` & `tmp/oso_cloud-1.0.6.dev0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 6971 bytes, number of entries: 8
--rw-r--r--  2.0 unx       57 b- defN 23-Feb-21 02:08 oso_cloud/__init__.py
--rw-r--r--  2.0 unx     9847 b- defN 23-Feb-21 02:08 oso_cloud/api.py
--rw-r--r--  2.0 unx     1619 b- defN 23-Feb-21 02:08 oso_cloud/helpers.py
--rw-r--r--  2.0 unx     6179 b- defN 23-Feb-21 02:08 oso_cloud/oso.py
--rw-r--r--  2.0 unx     3468 b- defN 23-Feb-21 02:08 oso_cloud-1.0.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-21 02:08 oso_cloud-1.0.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Feb-21 02:08 oso_cloud-1.0.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      605 b- defN 23-Feb-21 02:08 oso_cloud-1.0.6.dist-info/RECORD
-8 files, 21877 bytes uncompressed, 5923 bytes compressed:  72.9%
+Zip file size: 7027 bytes, number of entries: 8
+-rw-r--r--  2.0 unx       62 b- defN 23-Apr-17 14:00 oso_cloud/__init__.py
+-rw-r--r--  2.0 unx     9848 b- defN 23-Apr-17 14:00 oso_cloud/api.py
+-rw-r--r--  2.0 unx     1619 b- defN 23-Apr-17 14:00 oso_cloud/helpers.py
+-rw-r--r--  2.0 unx     6179 b- defN 23-Apr-17 14:00 oso_cloud/oso.py
+-rw-r--r--  2.0 unx     3473 b- defN 23-Apr-17 14:00 oso_cloud-1.0.6.dev0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-17 14:00 oso_cloud-1.0.6.dev0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Apr-17 14:00 oso_cloud-1.0.6.dev0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      625 b- defN 23-Apr-17 14:00 oso_cloud-1.0.6.dev0.dist-info/RECORD
+8 files, 21908 bytes uncompressed, 5939 bytes compressed:  72.9%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: oso_cloud/helpers.py
 Comment: 
 
 Filename: oso_cloud/oso.py
 Comment: 
 
-Filename: oso_cloud-1.0.6.dist-info/METADATA
+Filename: oso_cloud-1.0.6.dev0.dist-info/METADATA
 Comment: 
 
-Filename: oso_cloud-1.0.6.dist-info/WHEEL
+Filename: oso_cloud-1.0.6.dev0.dist-info/WHEEL
 Comment: 
 
-Filename: oso_cloud-1.0.6.dist-info/top_level.txt
+Filename: oso_cloud-1.0.6.dev0.dist-info/top_level.txt
 Comment: 
 
-Filename: oso_cloud-1.0.6.dist-info/RECORD
+Filename: oso_cloud-1.0.6.dev0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## oso_cloud/__init__.py

```diff
@@ -1,3 +1,3 @@
 from .oso import Oso, Fact, Value
 
-__version__ = "1.0.6"
+__version__ = "1.0.6.dev0"
```

## oso_cloud/api.py

```diff
@@ -7,15 +7,15 @@
 
 HTTP_ERROR_MAX_RETRIES = 10
 HTTP_ERROR_MAX_TIME = 30
 
 NETWORK_ERROR_MAX_RETRIES = 10
 NETWORK_ERROR_MAX_TIME = 30
 
-TIMEOUT_INTERVALS = (1, 5)
+TIMEOUT_INTERVALS = (1, 30)
 
 
 @dataclass
 class ApiResult:
     message: str
```

## Comparing `oso_cloud-1.0.6.dist-info/METADATA` & `oso_cloud-1.0.6.dev0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oso-cloud
-Version: 1.0.6
+Version: 1.0.6.dev0
 Summary: Oso Cloud Python client
 Home-page: https://www.osohq.com
 Author: Oso Security
 Author-email: support@osohq.com
 License: Apache-2.0
 Project-URL: Documentation, https://www.osohq.com/docs
 Keywords: authorization,rbac,oso,oso cloud,authorization as a service,microservice authorization
```

## Comparing `oso_cloud-1.0.6.dist-info/RECORD` & `oso_cloud-1.0.6.dev0.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-oso_cloud/__init__.py,sha256=OIS09k88Kyrn86eyytZliiLuowV5sK3sLUrmVzHCv4c,57
-oso_cloud/api.py,sha256=rxGwRMxdssAVr78ejo0WxuwzKBGSV4XhtTr4m1gPCV8,9847
+oso_cloud/__init__.py,sha256=0zt9jdPr41Iytmz7mUu7EmmhbpHeLIACIneR0fzq3Ho,62
+oso_cloud/api.py,sha256=b1u1XxEY0nZTs4txIRtMTWxl7hkbL6_h3NTJqYXER68,9848
 oso_cloud/helpers.py,sha256=UjUP1oCQihjnzDbXR_erulFHsOA5LmnojuNTAa7BGX4,1619
 oso_cloud/oso.py,sha256=5OWrSa3xDnPDWAloiaVOywzzDcaNSHiGayZ27mwpPxA,6179
-oso_cloud-1.0.6.dist-info/METADATA,sha256=NsLppahqqglNCqUyT_wMq9nLMAN5s7xUfYDycKI_p3E,3468
-oso_cloud-1.0.6.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-oso_cloud-1.0.6.dist-info/top_level.txt,sha256=pzOq04dOQpqHFKR4eDR1MMZ23BacelJsh7LKlSdFnmw,10
-oso_cloud-1.0.6.dist-info/RECORD,,
+oso_cloud-1.0.6.dev0.dist-info/METADATA,sha256=zlh0dA4pt6yyTy-epAnnCzc107WqkaZc2mu1dyriPnc,3473
+oso_cloud-1.0.6.dev0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+oso_cloud-1.0.6.dev0.dist-info/top_level.txt,sha256=pzOq04dOQpqHFKR4eDR1MMZ23BacelJsh7LKlSdFnmw,10
+oso_cloud-1.0.6.dev0.dist-info/RECORD,,
```

