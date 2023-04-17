# Comparing `tmp/anyon-3.1.15-cp311-cp311-win_amd64.whl.zip` & `tmp/anyon-3.1.16-cp311-cp311-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 366268 bytes, number of entries: 14
--rw-rw-rw-  2.0 fat     1080 b- defN 23-Apr-08 08:14 anyon-3.1.15.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1193 b- defN 23-Apr-08 08:14 anyon-3.1.15.dist-info/METADATA
--rw-rw-rw-  2.0 fat      102 b- defN 23-Apr-08 08:14 anyon-3.1.15.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        1 b- defN 23-Apr-08 08:14 anyon-3.1.15.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      381 b- defN 23-Apr-08 08:14 anyon-3.1.15.dist-info/RECORD
--rw-rw-rw-  2.0 fat    20480 b- defN 23-Apr-08 08:13 anyon/__init__.pyd
--rw-rw-rw-  2.0 fat    75264 b- defN 23-Apr-08 08:13 anyon/loader.pyd
--rw-rw-rw-  2.0 fat   100352 b- defN 23-Apr-08 08:13 anyon/remote.pyd
--rw-rw-rw-  2.0 fat   182784 b- defN 23-Apr-08 08:13 anyon/server.pyd
--rw-rw-rw-  2.0 fat    20992 b- defN 23-Apr-08 08:14 anyon/stage/__init__.pyd
--rw-rw-rw-  2.0 fat    94208 b- defN 23-Apr-08 08:14 anyon/stage/calculator.pyd
--rw-rw-rw-  2.0 fat   133632 b- defN 23-Apr-08 08:14 anyon/stage/compiler.pyd
--rw-rw-rw-  2.0 fat    62976 b- defN 23-Apr-08 08:14 anyon/stage/demodulator.pyd
--rw-rw-rw-  2.0 fat   114176 b- defN 23-Apr-08 08:14 anyon/stage/device.pyd
-14 files, 807621 bytes uncompressed, 364496 bytes compressed:  54.9%
+Zip file size: 364766 bytes, number of entries: 14
+-rw-rw-rw-  2.0 fat     1080 b- defN 23-Apr-16 13:39 anyon-3.1.16.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1193 b- defN 23-Apr-16 13:39 anyon-3.1.16.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      102 b- defN 23-Apr-16 13:39 anyon-3.1.16.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        1 b- defN 23-Apr-16 13:39 anyon-3.1.16.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      381 b- defN 23-Apr-16 13:39 anyon-3.1.16.dist-info/RECORD
+-rw-rw-rw-  2.0 fat    20480 b- defN 23-Apr-16 13:39 anyon/__init__.pyd
+-rw-rw-rw-  2.0 fat    74752 b- defN 23-Apr-16 13:39 anyon/loader.pyd
+-rw-rw-rw-  2.0 fat    99328 b- defN 23-Apr-16 13:39 anyon/remote.pyd
+-rw-rw-rw-  2.0 fat   181760 b- defN 23-Apr-16 13:39 anyon/server.pyd
+-rw-rw-rw-  2.0 fat    20992 b- defN 23-Apr-16 13:39 anyon/stage/__init__.pyd
+-rw-rw-rw-  2.0 fat    94208 b- defN 23-Apr-16 13:39 anyon/stage/calculator.pyd
+-rw-rw-rw-  2.0 fat   133632 b- defN 23-Apr-16 13:39 anyon/stage/compiler.pyd
+-rw-rw-rw-  2.0 fat    62976 b- defN 23-Apr-16 13:39 anyon/stage/demodulator.pyd
+-rw-rw-rw-  2.0 fat   114176 b- defN 23-Apr-16 13:39 anyon/stage/device.pyd
+14 files, 805061 bytes uncompressed, 362994 bytes compressed:  54.9%
```

## zipnote {}

```diff
@@ -1,20 +1,20 @@
-Filename: anyon-3.1.15.dist-info/LICENSE
+Filename: anyon-3.1.16.dist-info/LICENSE
 Comment: 
 
-Filename: anyon-3.1.15.dist-info/METADATA
+Filename: anyon-3.1.16.dist-info/METADATA
 Comment: 
 
-Filename: anyon-3.1.15.dist-info/WHEEL
+Filename: anyon-3.1.16.dist-info/WHEEL
 Comment: 
 
-Filename: anyon-3.1.15.dist-info/top_level.txt
+Filename: anyon-3.1.16.dist-info/top_level.txt
 Comment: 
 
-Filename: anyon-3.1.15.dist-info/RECORD
+Filename: anyon-3.1.16.dist-info/RECORD
 Comment: 
 
 Filename: anyon/__init__.pyd
 Comment: 
 
 Filename: anyon/loader.pyd
 Comment:
```

## Comparing `anyon-3.1.15.dist-info/LICENSE` & `anyon-3.1.16.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `anyon-3.1.15.dist-info/METADATA` & `anyon-3.1.16.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anyon
-Version: 3.1.15
+Version: 3.1.16
 Summary: Dream It Possible!
 Home-page: https://gitee.com/
 Author: YL Feng
 Author-email: fengyulong@pku.edu.cn
 License: MIT
 Project-URL: source, https://gitee.com
 Keywords: Hello,World!
@@ -19,16 +19,16 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy (>=1.20.0)
-Requires-Dist: axion (>=3.2.17)
-Requires-Dist: srpc (>=4.2.4)
+Requires-Dist: axion (>=3.2.20)
+Requires-Dist: srpc (>=4.2.7)
 Requires-Dist: zee (>=0.0.2)
 Requires-Dist: requests (>=2.28.0)
 
 #### 介绍
 
 
 #### 软件架构
```

