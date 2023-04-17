# Comparing `tmp/OpenGeode_core.geode-1.7.8-cp39-cp39-win_amd64.whl.zip` & `tmp/OpenGeode_core.geode-1.7.9-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 598318 bytes, number of entries: 15
--rw-rw-rw-  2.0 fat    14848 b- defN 22-Jul-29 19:08 opengeode_geode/OpenGeode_geode_model.dll
--rw-rw-rw-  2.0 fat     1181 b- defN 22-Jul-29 19:08 opengeode_geode/__init__.py
+Zip file size: 598324 bytes, number of entries: 15
+-rw-rw-rw-  2.0 fat    14848 b- defN 22-Jul-30 21:17 opengeode_geode/OpenGeode_geode_model.dll
+-rw-rw-rw-  2.0 fat     1181 b- defN 22-Jul-30 21:16 opengeode_geode/__init__.py
 -rw-rw-rw-  2.0 fat   317864 b- defN 22-Jul-24 22:28 opengeode_geode/concrt140.dll
 -rw-rw-rw-  2.0 fat   566704 b- defN 22-Jul-24 22:28 opengeode_geode/msvcp140.dll
 -rw-rw-rw-  2.0 fat    23944 b- defN 22-Jul-24 22:28 opengeode_geode/msvcp140_1.dll
 -rw-rw-rw-  2.0 fat   186800 b- defN 22-Jul-24 22:28 opengeode_geode/msvcp140_2.dll
 -rw-rw-rw-  2.0 fat    57264 b- defN 22-Jul-24 22:28 opengeode_geode/msvcp140_atomic_wait.dll
 -rw-rw-rw-  2.0 fat    21424 b- defN 22-Jul-24 22:28 opengeode_geode/msvcp140_codecvt_ids.dll
--rw-rw-rw-  2.0 fat   142336 b- defN 22-Jul-29 19:08 opengeode_geode/opengeode_geode_py_model.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   142336 b- defN 22-Jul-30 21:17 opengeode_geode/opengeode_geode_py_model.cp39-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    98224 b- defN 22-Jul-24 22:28 opengeode_geode/vcruntime140.dll
 -rw-rw-rw-  2.0 fat    37256 b- defN 22-Jul-24 22:28 opengeode_geode/vcruntime140_1.dll
--rw-rw-rw-  2.0 fat     2809 b- defN 22-Jul-29 19:09 OpenGeode_core.geode-1.7.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 22-Jul-29 19:09 OpenGeode_core.geode-1.7.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       16 b- defN 22-Jul-29 19:09 OpenGeode_core.geode-1.7.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1381 b- defN 22-Jul-29 19:09 OpenGeode_core.geode-1.7.8.dist-info/RECORD
-15 files, 1472143 bytes uncompressed, 596016 bytes compressed:  59.5%
+-rw-rw-rw-  2.0 fat     2809 b- defN 22-Jul-30 21:17 OpenGeode_core.geode-1.7.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 22-Jul-30 21:17 OpenGeode_core.geode-1.7.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       16 b- defN 22-Jul-30 21:17 OpenGeode_core.geode-1.7.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1381 b- defN 22-Jul-30 21:17 OpenGeode_core.geode-1.7.9.dist-info/RECORD
+15 files, 1472143 bytes uncompressed, 596022 bytes compressed:  59.5%
```

## zipnote {}

```diff
@@ -27,20 +27,20 @@
 
 Filename: opengeode_geode/vcruntime140.dll
 Comment: 
 
 Filename: opengeode_geode/vcruntime140_1.dll
 Comment: 
 
-Filename: OpenGeode_core.geode-1.7.8.dist-info/METADATA
+Filename: OpenGeode_core.geode-1.7.9.dist-info/METADATA
 Comment: 
 
-Filename: OpenGeode_core.geode-1.7.8.dist-info/WHEEL
+Filename: OpenGeode_core.geode-1.7.9.dist-info/WHEEL
 Comment: 
 
-Filename: OpenGeode_core.geode-1.7.8.dist-info/top_level.txt
+Filename: OpenGeode_core.geode-1.7.9.dist-info/top_level.txt
 Comment: 
 
-Filename: OpenGeode_core.geode-1.7.8.dist-info/RECORD
+Filename: OpenGeode_core.geode-1.7.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## opengeode_geode/OpenGeode_geode_model.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180001b0c
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Fri Jul 29 19:08:46 2022
+Time/Date		Sat Jul 30 21:17:06 2022
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		0000000000001600
 SizeOfInitializedData	0000000000002000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000001b0c
@@ -2457,17 +2457,17 @@
    18000325a:	(bad)
    18000325b:	(bad)
    18000325c:	(bad)
    18000325d:	(bad)
    18000325e:	(bad)
    18000325f:	incl   (%rax)
    180003261:	add    %al,(%rax)
-   180003263:	add    %bh,(%rsi)
-   180003265:	xor    %ah,%ah
-   180003267:	(bad)
+   180003263:	add    %dl,%dl
+   180003265:	lahf
+   180003266:	in     $0x62,%eax
    180003268:	add    %al,(%rax)
    18000326a:	add    %al,(%rax)
    18000326c:	or     $0x58000000,%eax
    180003271:	add    (%rax),%al
    180003273:	add    %ch,(%rax)
    180003275:	xor    $0x0,%al
    180003277:	add    %ch,(%rax)
```

## Comparing `OpenGeode_core.geode-1.7.8.dist-info/METADATA` & `OpenGeode_core.geode-1.7.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenGeode-core.geode
-Version: 1.7.8
+Version: 1.7.9
 Summary: Geode module for OpenGeode
 Home-page: https://github.com/Geode-solutions/OpenGeode.geode
 Author: Geode-solutions
 Author-email: contact@geode-solutions.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: OpenGeode-core.geode Version: 1.7.8 Summary: Geode
+Metadata-Version: 2.1 Name: OpenGeode-core.geode Version: 1.7.9 Summary: Geode
 module for OpenGeode Home-page: https://github.com/Geode-solutions/
 OpenGeode.geode Author: Geode-solutions Author-email: contact@geode-
 solutions.com License: MIT Platform: UNKNOWN Classifier: License :: OSI
 Approved :: MIT License Description-Content-Type: text/markdown Requires-Dist:
 OpenGeode-core (==11.*,>=11.0.4)
                 ****** OpenGeode.geodeby Geode-solutions ******
                     **** Geode extension for OpenGeode ****
```

## Comparing `OpenGeode_core.geode-1.7.8.dist-info/RECORD` & `OpenGeode_core.geode-1.7.9.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-opengeode_geode/OpenGeode_geode_model.dll,sha256=1V3GCoPBuZp07n653KWME0NFK924632Pf2gp9sY7Uh4,14848
+opengeode_geode/OpenGeode_geode_model.dll,sha256=ezwPfocAMPdkyWGYu4CjmNSHmxp2AQH8vGXtg_q_3b4,14848
 opengeode_geode/__init__.py,sha256=VI8T5Ar95HeIf7OkCmbnNUKwkyGNc_JKwe4MxF3RGvM,1181
 opengeode_geode/concrt140.dll,sha256=VzIpoH84q50vwuGluY6SQ7mzkQAyMYDIOtfdr5ju5Go,317864
 opengeode_geode/msvcp140.dll,sha256=n-5vNlR9b26nygM4ZVVV26a7D3mLxgM00puU0VR9pNo,566704
 opengeode_geode/msvcp140_1.dll,sha256=hzGpPlGcJZXJ_UiebZrAfpZESMDaHI7p7lAKeYlIJhc,23944
 opengeode_geode/msvcp140_2.dll,sha256=Nmr44HHwBNpdlagypGsuiCGo4ClDQKk_fJXPSMRBBn4,186800
 opengeode_geode/msvcp140_atomic_wait.dll,sha256=xhoocR-Mbpv9SHnPX1OwE9ZTutrTCKvj6IfGlLIj1vA,57264
 opengeode_geode/msvcp140_codecvt_ids.dll,sha256=m0X9BpvQB22Kv-t8PDCh9cX8jnEkAXhTqT2DGjRsPSE,21424
-opengeode_geode/opengeode_geode_py_model.cp39-win_amd64.pyd,sha256=oNdPq0Iotn9QA0xcjDE8JanKhXqIp5K5mOLqDHfkPqA,142336
+opengeode_geode/opengeode_geode_py_model.cp39-win_amd64.pyd,sha256=dh1ZRtv_-fA1ZGfv2y9apZI1cs22uWYnIPR-IBBHmx8,142336
 opengeode_geode/vcruntime140.dll,sha256=nStA8DlcxdG01eoXuElwwplx1EjDcQRnbbV3WG1K0bE,98224
 opengeode_geode/vcruntime140_1.dll,sha256=NASKuqBw7ME7MYzqMUJfTKPt0TPTUDGKxlJZ5gWMizI,37256
-OpenGeode_core.geode-1.7.8.dist-info/METADATA,sha256=WOtnG-p5aF32od-wAHwjAoxWLXeqGfxv9Ei8lLcwkSc,2809
-OpenGeode_core.geode-1.7.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-OpenGeode_core.geode-1.7.8.dist-info/top_level.txt,sha256=f3YVlb1wlHTsXDNEK7sA7b93Da-XhgUJ_cQqkrD99Cg,16
-OpenGeode_core.geode-1.7.8.dist-info/RECORD,,
+OpenGeode_core.geode-1.7.9.dist-info/METADATA,sha256=xeIjfC86We9MhXrx859qCaMJ9II0XQi53DUGkCkXzW8,2809
+OpenGeode_core.geode-1.7.9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+OpenGeode_core.geode-1.7.9.dist-info/top_level.txt,sha256=f3YVlb1wlHTsXDNEK7sA7b93Da-XhgUJ_cQqkrD99Cg,16
+OpenGeode_core.geode-1.7.9.dist-info/RECORD,,
```

