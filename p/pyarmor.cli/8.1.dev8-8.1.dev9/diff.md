# Comparing `tmp/pyarmor.cli-8.1.dev8-py2.py3-none-any.whl.zip` & `tmp/pyarmor.cli-8.1.dev9-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 33127 bytes, number of entries: 18
+Zip file size: 33129 bytes, number of entries: 18
 -rw-r--r--  2.0 unx     1292 b- defN 23-Apr-05 16:02 pyarmor/cli/__init__.py
--rw-r--r--  2.0 unx    20090 b- defN 23-Apr-08 22:48 pyarmor/cli/__main__.py
+-rw-r--r--  2.0 unx    20090 b- defN 23-Apr-08 23:41 pyarmor/cli/__main__.py
 -rw-r--r--  2.0 unx     8608 b- defN 23-Apr-02 14:49 pyarmor/cli/config.py
 -rw-r--r--  2.0 unx    15562 b- defN 23-Apr-08 00:25 pyarmor/cli/context.py
 -rw-r--r--  2.0 unx     7736 b- defN 23-Apr-08 04:34 pyarmor/cli/default.cfg
 -rw-r--r--  2.0 unx      880 b- defN 23-Jan-12 09:29 pyarmor/cli/errors.py
 -rw-r--r--  2.0 unx     5603 b- defN 23-Apr-05 01:07 pyarmor/cli/generate.py
 -rw-r--r--  2.0 unx     4008 b- defN 23-Feb-11 01:53 pyarmor/cli/mixer.py
 -rw-r--r--  2.0 unx     2487 b- defN 23-Mar-25 22:51 pyarmor/cli/public_capsule.zip
 -rw-r--r--  2.0 unx    10980 b- defN 23-Apr-06 22:19 pyarmor/cli/register.py
 -rw-r--r--  2.0 unx    11386 b- defN 23-Mar-29 13:18 pyarmor/cli/repack.py
 -rw-r--r--  2.0 unx     6366 b- defN 23-Apr-06 11:59 pyarmor/cli/resource.py
 -rw-r--r--  2.0 unx     2193 b- defN 23-Feb-22 14:43 pyarmor/cli/shell.py
--rw-r--r--  2.0 unx     2405 b- defN 23-Apr-08 23:32 pyarmor.cli-8.1.dev8.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Apr-08 23:32 pyarmor.cli-8.1.dev8.dist-info/WHEEL
--rw-r--r--  2.0 unx       41 b- defN 23-Apr-08 23:32 pyarmor.cli-8.1.dev8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 23-Apr-08 23:32 pyarmor.cli-8.1.dev8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1465 b- defN 23-Apr-08 23:32 pyarmor.cli-8.1.dev8.dist-info/RECORD
-18 files, 101220 bytes uncompressed, 30745 bytes compressed:  69.6%
+-rw-r--r--  2.0 unx     2405 b- defN 23-Apr-08 23:42 pyarmor.cli-8.1.dev9.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Apr-08 23:42 pyarmor.cli-8.1.dev9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       41 b- defN 23-Apr-08 23:42 pyarmor.cli-8.1.dev9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-Apr-08 23:42 pyarmor.cli-8.1.dev9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1465 b- defN 23-Apr-08 23:42 pyarmor.cli-8.1.dev9.dist-info/RECORD
+18 files, 101220 bytes uncompressed, 30747 bytes compressed:  69.6%
```

## zipnote {}

```diff
@@ -33,23 +33,23 @@
 
 Filename: pyarmor/cli/resource.py
 Comment: 
 
 Filename: pyarmor/cli/shell.py
 Comment: 
 
-Filename: pyarmor.cli-8.1.dev8.dist-info/METADATA
+Filename: pyarmor.cli-8.1.dev9.dist-info/METADATA
 Comment: 
 
-Filename: pyarmor.cli-8.1.dev8.dist-info/WHEEL
+Filename: pyarmor.cli-8.1.dev9.dist-info/WHEEL
 Comment: 
 
-Filename: pyarmor.cli-8.1.dev8.dist-info/entry_points.txt
+Filename: pyarmor.cli-8.1.dev9.dist-info/entry_points.txt
 Comment: 
 
-Filename: pyarmor.cli-8.1.dev8.dist-info/top_level.txt
+Filename: pyarmor.cli-8.1.dev9.dist-info/top_level.txt
 Comment: 
 
-Filename: pyarmor.cli-8.1.dev8.dist-info/RECORD
+Filename: pyarmor.cli-8.1.dev9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyarmor/cli/__main__.py

```diff
@@ -112,15 +112,15 @@
 
 
 def check_cross_platform(ctx, platforms):
     try:
         from pyarmor.cli import runtime
     except ModuleNotFoundError:
         raise CliError('cross platform need pyarmor.cli.runtime, please '
-                       'run "pip install pyarmor.cli.runtime==2.1.dev8" first')
+                       'run "pip install pyarmor.cli.runtime==2.1.dev9" first')
 
     platnames = []
     for path in runtime.__path__:
         platnames.extend(os.listdir(os.path.join(path, 'libs')))
 
     map_platform = runtime.map_platform
     unknown = set([map_platform(x) for x in platforms]) - set(platnames)
```

## Comparing `pyarmor.cli-8.1.dev8.dist-info/METADATA` & `pyarmor.cli-8.1.dev9.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyarmor.cli
-Version: 8.1.dev8
+Version: 8.1.dev9
 Summary: A comand line tool to obfuscate python scripts
 Home-page: https://github.com/dashingsoft/pyarmor
 Author: Jondy Zhao
 Author-email: pyarmor@163.com
 License: Free To Use But Restricted
 Keywords: protect obfuscate encrypt obfuscation distribute
 Platform: UNKNOWN
```

## Comparing `pyarmor.cli-8.1.dev8.dist-info/RECORD` & `pyarmor.cli-8.1.dev9.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 pyarmor/cli/__init__.py,sha256=ewQIh0wc49TeewnGYkGsG_ALFMA_g314F4Ad7fRlktM,1292
-pyarmor/cli/__main__.py,sha256=DTREFo3uiOxKLmsPxecxZa0HuiWXDOZnslbbHu1CvDg,20090
+pyarmor/cli/__main__.py,sha256=uyTndUm2mpiTcjCP5XO4SeCqD2LskS00MtOF_OBguBg,20090
 pyarmor/cli/config.py,sha256=HbCIOkJ2Zd7aGeanB1tUpBhWTj1LhyMiSwWGdmFgN0A,8608
 pyarmor/cli/context.py,sha256=Onjz-5zEsdumN0GkpEJGH0ld24W5m6SjqZRpGRnm-KE,15562
 pyarmor/cli/default.cfg,sha256=i-EM_E4Ee1rU6yBq8a00eZEKI8moRow9ZFKr_i6Gd7s,7736
 pyarmor/cli/errors.py,sha256=gNlPhcqgCS4OVdU9H8V23YxThyvHKtFI3LKAu-sxH60,880
 pyarmor/cli/generate.py,sha256=7GnIcVG2G8MlaH60-7a2UcCsyedu5Cr0OH_IoOix_GQ,5603
 pyarmor/cli/mixer.py,sha256=CQOttISF-h55lWEbRUaywsNZybxe8KsXC7axO1ISxUE,4008
 pyarmor/cli/public_capsule.zip,sha256=1r4u42ixfocGPMQc0OklpoHF3nvVW6GA1f4SwcEJWVI,2487
 pyarmor/cli/register.py,sha256=fNtET8fjd1KxypZ34E9sy9zIA3wkmy2kI57bkDe7saA,10980
 pyarmor/cli/repack.py,sha256=JTmb-KAzPLNu_VttJTym53uJg5GJlPkmNZQ-LjM8gS8,11386
 pyarmor/cli/resource.py,sha256=ef-2nvRhlyYOlSub6LbYywnmABFmtCAADRcK6j89Udg,6366
 pyarmor/cli/shell.py,sha256=S1yJ5RQZhTIysQgXk3H4E_cJsV2Lymh-w-_GdnHFngU,2193
-pyarmor.cli-8.1.dev8.dist-info/METADATA,sha256=deri40CjPElEtE78NMEnEfe3iqN2AQMz4gE41baSN-Q,2405
-pyarmor.cli-8.1.dev8.dist-info/WHEEL,sha256=kGT74LWyRUZrL4VgLh6_g12IeVl_9u9ZVhadrgXZUEY,110
-pyarmor.cli-8.1.dev8.dist-info/entry_points.txt,sha256=MODwyeC-iHX4KItYshzQRa5kWWQnMhIuT64w5bqKFR0,41
-pyarmor.cli-8.1.dev8.dist-info/top_level.txt,sha256=UE1ovZ_90YzwF_lZ3LV7o8HKLe-RgzUaUUvdH5UTUus,8
-pyarmor.cli-8.1.dev8.dist-info/RECORD,,
+pyarmor.cli-8.1.dev9.dist-info/METADATA,sha256=tglg14h4D3Cn-LG0HvYdQfGCHz7dXaiw2Dvf4ZtHFMQ,2405
+pyarmor.cli-8.1.dev9.dist-info/WHEEL,sha256=kGT74LWyRUZrL4VgLh6_g12IeVl_9u9ZVhadrgXZUEY,110
+pyarmor.cli-8.1.dev9.dist-info/entry_points.txt,sha256=MODwyeC-iHX4KItYshzQRa5kWWQnMhIuT64w5bqKFR0,41
+pyarmor.cli-8.1.dev9.dist-info/top_level.txt,sha256=UE1ovZ_90YzwF_lZ3LV7o8HKLe-RgzUaUUvdH5UTUus,8
+pyarmor.cli-8.1.dev9.dist-info/RECORD,,
```

