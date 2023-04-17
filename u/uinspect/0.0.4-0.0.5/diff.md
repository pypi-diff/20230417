# Comparing `tmp/uinspect-0.0.4-cp39-cp39-win_amd64.whl.zip` & `tmp/uinspect-0.0.5-cp311-cp311-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 78434 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat   169472 b- defN 23-Jan-18 18:55 uinspect.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     2692 b- defN 23-Jan-18 18:55 uinspect-0.0.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Jan-18 18:55 uinspect-0.0.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Jan-18 18:55 uinspect-0.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      388 b- defN 23-Jan-18 18:55 uinspect-0.0.4.dist-info/RECORD
-5 files, 172661 bytes uncompressed, 77714 bytes compressed:  55.0%
+Zip file size: 78505 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat   169984 b- defN 23-Apr-17 20:43 uinspect.cp311-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     2826 b- defN 23-Apr-17 20:43 uinspect-0.0.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      102 b- defN 23-Apr-17 20:43 uinspect-0.0.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-17 20:43 uinspect-0.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      389 b- defN 23-Apr-17 20:43 uinspect-0.0.5.dist-info/RECORD
+5 files, 173310 bytes uncompressed, 77783 bytes compressed:  55.1%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: uinspect.cp39-win_amd64.pyd
+Filename: uinspect.cp311-win_amd64.pyd
 Comment: 
 
-Filename: uinspect-0.0.4.dist-info/METADATA
+Filename: uinspect-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: uinspect-0.0.4.dist-info/WHEEL
+Filename: uinspect-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: uinspect-0.0.4.dist-info/top_level.txt
+Filename: uinspect-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: uinspect-0.0.4.dist-info/RECORD
+Filename: uinspect-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `uinspect-0.0.4.dist-info/METADATA` & `uinspect-0.0.5.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: uinspect
-Version: 0.0.4
+Version: 0.0.5
 Summary: Ultra-fast inspect functions for Python
 Home-page: https://github.com/Kuree/uinspect
 Author: Keyi Zhang
 Author-email: keyi@cs.stanford.edu
-License: UNKNOWN
-Platform: UNKNOWN
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: test
 Requires-Dist: pytest (>=6.0) ; extra == 'test'
 
 uinspect
 ========
 
-This is a small Python package that offers :sub:`fast` runtime inspection similar to that of ``inspect`` module in Python. To install, simply do
+This is a small Python package that offers fast runtime inspection similar to that of ``inspect`` module in Python. To install, simply do
 
 ::
 
    pip install uinspect
 
 benchmark
 =========
@@ -37,7 +35,16 @@
 | Frame walking   | ``uinspect.FrameWalker({}).get_location()`` - 1.45s | N/A                          | 52.27s  | 35.9x   | 1.46 us/op   |
 +-----------------+-----------------------------------------------------+------------------------------+---------+---------+--------------+
 
 It turns out that the ``uinspect`` does not speed up the local variable calculation. This is because we have to run an expensive Python C API call regardless of whether itâ€™s ``uinspect`` or ``inspect``. As a result, the overhead is caused by the fact that ``uinspect`` needs to convert Python object to C++ object.
 
 The lesson is to use ``inspect`` module for any local variables related manipulation since itâ€™s faster, but use ``uinspect`` to obtain source location.
 
+install from source
+===================
+
+::
+
+   git clone https://github.com/Kuree/uinspect.git
+   cd uinspect
+   git submodule update --init
+   python setup.py install
```

