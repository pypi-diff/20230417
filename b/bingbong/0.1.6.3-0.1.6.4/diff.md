# Comparing `tmp/bingbong-0.1.6.3-py3-none-any.whl.zip` & `tmp/bingbong-0.1.6.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 11035 bytes, number of entries: 15
--rw-rw-rw-  2.0 unx       55 b- defN 23-Apr-17 12:43 pingpong/__init__.py
+Zip file size: 11054 bytes, number of entries: 15
+-rw-rw-rw-  2.0 unx       55 b- defN 23-Apr-17 13:04 pingpong/__init__.py
 -rw-rw-rw-  2.0 unx     1446 b- defN 23-Apr-17 12:46 pingpong/alpaca.py
 -rw-rw-rw-  2.0 unx     1215 b- defN 23-Apr-14 12:55 pingpong/dolly.py
 -rw-rw-rw-  2.0 unx      987 b- defN 23-Apr-14 05:26 pingpong/gradio.py
 -rw-rw-rw-  2.0 unx     1192 b- defN 23-Apr-14 12:50 pingpong/pingpong.py
 -rw-rw-rw-  2.0 unx      173 b- defN 23-Apr-12 04:36 pingpong/context/__init__.py
 -rw-rw-rw-  2.0 unx      589 b- defN 23-Apr-12 00:59 pingpong/context/auto_summary_strategy.py
--rw-rw-rw-  2.0 unx      711 b- defN 23-Apr-13 23:18 pingpong/context/last_window_strategy.py
+-rw-rw-rw-  2.0 unx      773 b- defN 23-Apr-17 13:04 pingpong/context/last_window_strategy.py
 -rw-rw-rw-  2.0 unx      840 b- defN 23-Apr-12 04:54 pingpong/context/search_window_strategy.py
 -rw-rw-rw-  2.0 unx      119 b- defN 23-Apr-11 14:54 pingpong/context/strategy.py
--rw-rw-rw-  2.0 unx    11357 b- defN 23-Apr-17 12:46 bingbong-0.1.6.3.dist-info/LICENSE
--rw-rw-rw-  2.0 unx     3348 b- defN 23-Apr-17 12:46 bingbong-0.1.6.3.dist-info/METADATA
--rw-rw-rw-  2.0 unx       92 b- defN 23-Apr-17 12:46 bingbong-0.1.6.3.dist-info/WHEEL
--rw-rw-rw-  2.0 unx        9 b- defN 23-Apr-17 12:46 bingbong-0.1.6.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1235 b- defN 23-Apr-17 12:46 bingbong-0.1.6.3.dist-info/RECORD
-15 files, 23368 bytes uncompressed, 8981 bytes compressed:  61.6%
+-rw-rw-rw-  2.0 unx    11357 b- defN 23-Apr-17 13:04 bingbong-0.1.6.4.dist-info/LICENSE
+-rw-rw-rw-  2.0 unx     3348 b- defN 23-Apr-17 13:04 bingbong-0.1.6.4.dist-info/METADATA
+-rw-rw-rw-  2.0 unx       92 b- defN 23-Apr-17 13:04 bingbong-0.1.6.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 unx        9 b- defN 23-Apr-17 13:04 bingbong-0.1.6.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1235 b- defN 23-Apr-17 13:04 bingbong-0.1.6.4.dist-info/RECORD
+15 files, 23430 bytes uncompressed, 9000 bytes compressed:  61.6%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: pingpong/context/search_window_strategy.py
 Comment: 
 
 Filename: pingpong/context/strategy.py
 Comment: 
 
-Filename: bingbong-0.1.6.3.dist-info/LICENSE
+Filename: bingbong-0.1.6.4.dist-info/LICENSE
 Comment: 
 
-Filename: bingbong-0.1.6.3.dist-info/METADATA
+Filename: bingbong-0.1.6.4.dist-info/METADATA
 Comment: 
 
-Filename: bingbong-0.1.6.3.dist-info/WHEEL
+Filename: bingbong-0.1.6.4.dist-info/WHEEL
 Comment: 
 
-Filename: bingbong-0.1.6.3.dist-info/top_level.txt
+Filename: bingbong-0.1.6.4.dist-info/top_level.txt
 Comment: 
 
-Filename: bingbong-0.1.6.3.dist-info/RECORD
+Filename: bingbong-0.1.6.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pingpong/__init__.py

```diff
@@ -1,3 +1,3 @@
-__version__ = '0.1.6.3'
+__version__ = '0.1.6.4'
 
 from .pingpong import PingPong
```

## pingpong/context/last_window_strategy.py

```diff
@@ -1,21 +1,22 @@
 from pingpong.pingpong import PPManager
 from pingpong.context.strategy import CtxStrategy
 
 class CtxLastWindowStrategy(CtxStrategy):
     def __init__(self, max_pingpongs: int):
         self.max_pingpongs = max_pingpongs
     
-    def __call__(self, ppmanager: PPManager, build_uis=False):
+    def __call__(self, ppmanager: PPManager, build_uis=False, remove_last=False):
         pps = ppmanager.pingpongs
 
         if len(pps) <= self.max_pingpongs:
             start_idx = 0
         else:
             start_idx = len(pps) - self.max_pingpongs
+            if remove_last: start_idx -= 1
 
         if build_uis:
             return (
                 ppmanager.build_prompts(from_idx=start_idx),
                 ppmanager.build_uis(from_idx=start_idx)
             )
         else:
```

## Comparing `bingbong-0.1.6.3.dist-info/LICENSE` & `bingbong-0.1.6.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `bingbong-0.1.6.3.dist-info/METADATA` & `bingbong-0.1.6.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bingbong
-Version: 0.1.6.3
+Version: 0.1.6.4
 Summary: Ping pong management library for LLM applied application
 Home-page: https://github.com/deep-diver/PingPong
 Author: chansung park
 Author-email: deep.diver.csp@gmail.com
 Keywords: LLM,pingpong,prompt,context,management
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

