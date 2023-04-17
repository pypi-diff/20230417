# Comparing `tmp/ruleminer-0.1.8-py2.py3-none-any.whl.zip` & `tmp/ruleminer-0.1.9-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
 Zip file size: 16148 bytes, number of entries: 15
--rw-rw-rw-  2.0 fat      262 b- defN 22-Apr-11 07:06 ruleminer/__init__.py
+-rw-rw-rw-  2.0 fat      262 b- defN 22-Apr-11 08:02 ruleminer/__init__.py
 -rw-rw-rw-  2.0 fat      405 b- defN 21-Nov-21 10:33 ruleminer/cli.py
 -rw-rw-rw-  2.0 fat      692 b- defN 22-Feb-03 15:18 ruleminer/const.py
 -rw-rw-rw-  2.0 fat     1813 b- defN 22-Jan-03 14:44 ruleminer/encodings.py
--rw-rw-rw-  2.0 fat     7200 b- defN 22-Apr-11 07:04 ruleminer/metrics.py
+-rw-rw-rw-  2.0 fat     7195 b- defN 22-Apr-11 08:01 ruleminer/metrics.py
 -rw-rw-rw-  2.0 fat     6319 b- defN 22-Apr-06 08:33 ruleminer/parser.py
 -rw-rw-rw-  2.0 fat    22352 b- defN 22-Apr-11 07:01 ruleminer/ruleminer.py
 -rw-rw-rw-  2.0 fat     1269 b- defN 22-Feb-20 06:52 ruleminer/utils.py
--rw-rw-rw-  2.0 fat      180 b- defN 22-Apr-11 07:08 ruleminer-0.1.8.dist-info/AUTHORS.rst
--rw-rw-rw-  2.0 fat     1356 b- defN 22-Apr-11 07:08 ruleminer-0.1.8.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    11012 b- defN 22-Apr-11 07:08 ruleminer-0.1.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat      116 b- defN 22-Apr-11 07:08 ruleminer-0.1.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       50 b- defN 22-Apr-11 07:08 ruleminer-0.1.8.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       10 b- defN 22-Apr-11 07:08 ruleminer-0.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1198 b- defN 22-Apr-11 07:08 ruleminer-0.1.8.dist-info/RECORD
-15 files, 54234 bytes uncompressed, 14178 bytes compressed:  73.9%
+-rw-rw-rw-  2.0 fat      180 b- defN 22-Apr-11 08:02 ruleminer-0.1.9.dist-info/AUTHORS.rst
+-rw-rw-rw-  2.0 fat     1356 b- defN 22-Apr-11 08:02 ruleminer-0.1.9.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    11012 b- defN 22-Apr-11 08:02 ruleminer-0.1.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      116 b- defN 22-Apr-11 08:02 ruleminer-0.1.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       50 b- defN 22-Apr-11 08:02 ruleminer-0.1.9.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       10 b- defN 22-Apr-11 08:02 ruleminer-0.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1198 b- defN 22-Apr-11 08:02 ruleminer-0.1.9.dist-info/RECORD
+15 files, 54229 bytes uncompressed, 14178 bytes compressed:  73.9%
```

## zipnote {}

```diff
@@ -18,29 +18,29 @@
 
 Filename: ruleminer/ruleminer.py
 Comment: 
 
 Filename: ruleminer/utils.py
 Comment: 
 
-Filename: ruleminer-0.1.8.dist-info/AUTHORS.rst
+Filename: ruleminer-0.1.9.dist-info/AUTHORS.rst
 Comment: 
 
-Filename: ruleminer-0.1.8.dist-info/LICENSE
+Filename: ruleminer-0.1.9.dist-info/LICENSE
 Comment: 
 
-Filename: ruleminer-0.1.8.dist-info/METADATA
+Filename: ruleminer-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: ruleminer-0.1.8.dist-info/WHEEL
+Filename: ruleminer-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: ruleminer-0.1.8.dist-info/entry_points.txt
+Filename: ruleminer-0.1.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: ruleminer-0.1.8.dist-info/top_level.txt
+Filename: ruleminer-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: ruleminer-0.1.8.dist-info/RECORD
+Filename: ruleminer-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ruleminer/__init__.py

```diff
@@ -1,11 +1,11 @@
 """Top-level package for ruleminer."""
 
 __author__ = """Willem Jan Willemse"""
 __email__ = "w.j.willemse@xs4all.nl"
-__version__ = "0.1.8"
+__version__ = "0.1.9"
 
 from .ruleminer import *
 from .utils import *
 from .parser import *
 from .metrics import *
 from .const import *
```

## ruleminer/metrics.py

```diff
@@ -14,15 +14,15 @@
 import numpy as np
 
 METRICS = {
     ABSOLUTE_SUPPORT: ["X and Y"],
     ABSOLUTE_EXCEPTIONS: ["X and ~Y"],
     CONFIDENCE: ["X", "X and Y"],
     SUPPORT: ["X", "~X"],
-    ADDED_VALUE: ["X", "Y", "~Y", "X and Y"],  # conf(X⇒Y) − supp(Y)
+    ADDED_VALUE: ["X", "~X", "X and Y"],  # conf(X⇒Y) − supp(Y)
     CASUAL_CONFIDENCE: ["X", "X and Y", "~X", "~X and ~Y"],
     CONVICTION: ["X", "Y", "~Y", "X and Y"],
     LIFT: ["X", "Y", "~Y", "X and Y"],
     RULE_POWER_FACTOR: ["X", "Y", "~Y", "X and Y"],
 }
```

## Comparing `ruleminer-0.1.8.dist-info/LICENSE` & `ruleminer-0.1.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ruleminer-0.1.8.dist-info/METADATA` & `ruleminer-0.1.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ruleminer
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python package to mine association rules in datasets
 Home-page: https://github.com/wjwillemse/ruleminer
 Author: Willem Jan Willemse
 Author-email: w.j.willemse@xs4all.nl
 License: MIT license
 Keywords: ruleminer
 Platform: UNKNOWN
```

