# Comparing `tmp/lazylinop-1.0.8-py3-none-any.whl.zip` & `tmp/lazylinop-1.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 23368 bytes, number of entries: 8
--rw-r--r--  2.0 unx       71 b- defN 23-Apr-09 13:53 lazylinop/__init__.py
--rw-r--r--  2.0 unx    63971 b- defN 23-Apr-09 13:53 lazylinop/lazylinop.py
--rw-r--r--  2.0 unx    28887 b- defN 23-Apr-09 13:53 lazylinop/wip/lsignal.py
--rw-rw-rw-  2.0 unx     1434 b- defN 23-Apr-09 13:53 lazylinop-1.0.8.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     4769 b- defN 23-Apr-09 13:53 lazylinop-1.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-09 13:53 lazylinop-1.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Apr-09 13:53 lazylinop-1.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      638 b- defN 23-Apr-09 13:53 lazylinop-1.0.8.dist-info/RECORD
-8 files, 99872 bytes uncompressed, 22258 bytes compressed:  77.7%
+Zip file size: 23367 bytes, number of entries: 8
+-rw-r--r--  2.0 unx       71 b- defN 23-Apr-09 14:52 lazylinop/__init__.py
+-rw-r--r--  2.0 unx    63971 b- defN 23-Apr-09 14:52 lazylinop/lazylinop.py
+-rw-r--r--  2.0 unx    28887 b- defN 23-Apr-09 14:52 lazylinop/wip/lsignal.py
+-rw-rw-rw-  2.0 unx     1434 b- defN 23-Apr-09 14:53 lazylinop-1.0.9.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     4769 b- defN 23-Apr-09 14:53 lazylinop-1.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-09 14:53 lazylinop-1.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Apr-09 14:53 lazylinop-1.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      638 b- defN 23-Apr-09 14:53 lazylinop-1.0.9.dist-info/RECORD
+8 files, 99872 bytes uncompressed, 22257 bytes compressed:  77.7%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: lazylinop/lazylinop.py
 Comment: 
 
 Filename: lazylinop/wip/lsignal.py
 Comment: 
 
-Filename: lazylinop-1.0.8.dist-info/LICENSE.txt
+Filename: lazylinop-1.0.9.dist-info/LICENSE.txt
 Comment: 
 
-Filename: lazylinop-1.0.8.dist-info/METADATA
+Filename: lazylinop-1.0.9.dist-info/METADATA
 Comment: 
 
-Filename: lazylinop-1.0.8.dist-info/WHEEL
+Filename: lazylinop-1.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: lazylinop-1.0.8.dist-info/top_level.txt
+Filename: lazylinop-1.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: lazylinop-1.0.8.dist-info/RECORD
+Filename: lazylinop-1.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## lazylinop/__init__.py

```diff
@@ -1,3 +1,3 @@
 from . import lazylinop
 from .lazylinop import *
-__version__ = '1.0.8'
+__version__ = '1.0.9'
```

## Comparing `lazylinop-1.0.8.dist-info/LICENSE.txt` & `lazylinop-1.0.9.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `lazylinop-1.0.8.dist-info/METADATA` & `lazylinop-1.0.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazylinop
-Version: 1.0.8
+Version: 1.0.9
 Summary: A package dedicated to lazy linear operators based on diverse backends/libraries.
 Author-email: Inria <remi.gribonval@inria.fr>, Pascal Carrivain <pascal.carrivain@inria.fr>, Simon Delamare <simon.delamare@ens-lyon.fr>, Hakim Hadj-Djilani <hakim.hadj-djilani@inria.fr>, Rémi Gribonval <remi.gribonval@inria.fr>
 License: Copyright 2023, Inria
         
         BSD License 2.0
         
         Redistribution and use in source and binary forms, with or without
```

