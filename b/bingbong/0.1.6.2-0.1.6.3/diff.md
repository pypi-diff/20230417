# Comparing `tmp/bingbong-0.1.6.2-py3-none-any.whl.zip` & `tmp/bingbong-0.1.6.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 10978 bytes, number of entries: 15
--rw-rw-rw-  2.0 unx       55 b- defN 23-Apr-14 12:55 pingpong/__init__.py
--rw-rw-rw-  2.0 unx     1199 b- defN 23-Apr-14 12:44 pingpong/alpaca.py
+Zip file size: 11035 bytes, number of entries: 15
+-rw-rw-rw-  2.0 unx       55 b- defN 23-Apr-17 12:43 pingpong/__init__.py
+-rw-rw-rw-  2.0 unx     1446 b- defN 23-Apr-17 12:46 pingpong/alpaca.py
 -rw-rw-rw-  2.0 unx     1215 b- defN 23-Apr-14 12:55 pingpong/dolly.py
 -rw-rw-rw-  2.0 unx      987 b- defN 23-Apr-14 05:26 pingpong/gradio.py
 -rw-rw-rw-  2.0 unx     1192 b- defN 23-Apr-14 12:50 pingpong/pingpong.py
 -rw-rw-rw-  2.0 unx      173 b- defN 23-Apr-12 04:36 pingpong/context/__init__.py
 -rw-rw-rw-  2.0 unx      589 b- defN 23-Apr-12 00:59 pingpong/context/auto_summary_strategy.py
 -rw-rw-rw-  2.0 unx      711 b- defN 23-Apr-13 23:18 pingpong/context/last_window_strategy.py
 -rw-rw-rw-  2.0 unx      840 b- defN 23-Apr-12 04:54 pingpong/context/search_window_strategy.py
 -rw-rw-rw-  2.0 unx      119 b- defN 23-Apr-11 14:54 pingpong/context/strategy.py
--rw-rw-rw-  2.0 unx    11357 b- defN 23-Apr-14 12:55 bingbong-0.1.6.2.dist-info/LICENSE
--rw-rw-rw-  2.0 unx     3348 b- defN 23-Apr-14 12:55 bingbong-0.1.6.2.dist-info/METADATA
--rw-rw-rw-  2.0 unx       92 b- defN 23-Apr-14 12:55 bingbong-0.1.6.2.dist-info/WHEEL
--rw-rw-rw-  2.0 unx        9 b- defN 23-Apr-14 12:55 bingbong-0.1.6.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1235 b- defN 23-Apr-14 12:55 bingbong-0.1.6.2.dist-info/RECORD
-15 files, 23121 bytes uncompressed, 8924 bytes compressed:  61.4%
+-rw-rw-rw-  2.0 unx    11357 b- defN 23-Apr-17 12:46 bingbong-0.1.6.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 unx     3348 b- defN 23-Apr-17 12:46 bingbong-0.1.6.3.dist-info/METADATA
+-rw-rw-rw-  2.0 unx       92 b- defN 23-Apr-17 12:46 bingbong-0.1.6.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 unx        9 b- defN 23-Apr-17 12:46 bingbong-0.1.6.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1235 b- defN 23-Apr-17 12:46 bingbong-0.1.6.3.dist-info/RECORD
+15 files, 23368 bytes uncompressed, 8981 bytes compressed:  61.6%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: pingpong/context/search_window_strategy.py
 Comment: 
 
 Filename: pingpong/context/strategy.py
 Comment: 
 
-Filename: bingbong-0.1.6.2.dist-info/LICENSE
+Filename: bingbong-0.1.6.3.dist-info/LICENSE
 Comment: 
 
-Filename: bingbong-0.1.6.2.dist-info/METADATA
+Filename: bingbong-0.1.6.3.dist-info/METADATA
 Comment: 
 
-Filename: bingbong-0.1.6.2.dist-info/WHEEL
+Filename: bingbong-0.1.6.3.dist-info/WHEEL
 Comment: 
 
-Filename: bingbong-0.1.6.2.dist-info/top_level.txt
+Filename: bingbong-0.1.6.3.dist-info/top_level.txt
 Comment: 
 
-Filename: bingbong-0.1.6.2.dist-info/RECORD
+Filename: bingbong-0.1.6.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pingpong/__init__.py

```diff
@@ -1,3 +1,3 @@
-__version__ = '0.1.6.2'
+__version__ = '0.1.6.3'
 
 from .pingpong import PingPong
```

## pingpong/alpaca.py

```diff
@@ -3,34 +3,42 @@
 
 class AlpacaPromptFmt(PromptFmt):
   @classmethod
   def ctx(cls, context):
     if context is None or context == "":
       return ""
     else:
-      return f"""### Input:{context}
+      return f"""### Input:
+{context}
 
 """
 
   @classmethod
   def prompt(cls, pingpong):
     return f"""### Instruction: {pingpong.ping}
 
 ### Response: {"" if pingpong.pong is None else pingpong.pong}"""
 
 class AlpacaChatPPManager(PPManager):
   def add_ping(self, ping, fmt: PromptFmt=AlpacaPromptFmt):
     allowed = super().add_ping(ping, fmt)
 
     if allowed:
-      prompts = f"""Below is an instruction that describes a task. Write a response that appropriately completes the request.
-
-### Instruction:{ping}
+      if self.ctx == "":
+        prompts = "Below is an instruction that describes a task. Write a response that appropriately completes the request."
+      else:
+        prompts = "Below is an instruction that describes a task, paired with an input that provides further context. Write a response that appropriately completes the request."
+
+      prompts += f"""
+      
+### Instruction:
+{ping}
 {fmt.ctx(self.ctx)}
-### Response:"""
+### Response:
+"""
       return prompts
 
     return None
 
 
   def build_prompts(self, from_idx: int=0, to_idx: int=-1, fmt: PromptFmt=AlpacaPromptFmt):
     if to_idx == -1 or to_idx >= len(self.pingpongs):
```

## Comparing `bingbong-0.1.6.2.dist-info/LICENSE` & `bingbong-0.1.6.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `bingbong-0.1.6.2.dist-info/METADATA` & `bingbong-0.1.6.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bingbong
-Version: 0.1.6.2
+Version: 0.1.6.3
 Summary: Ping pong management library for LLM applied application
 Home-page: https://github.com/deep-diver/PingPong
 Author: chansung park
 Author-email: deep.diver.csp@gmail.com
 Keywords: LLM,pingpong,prompt,context,management
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

## Comparing `bingbong-0.1.6.2.dist-info/RECORD` & `bingbong-0.1.6.3.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-pingpong/__init__.py,sha256=urOQF36qoe_DAoPImWQlUpY1lrQG0QiKV1yALpkTFlY,55
-pingpong/alpaca.py,sha256=3z9EnziOat6P9DzuBlDXPh8wU47IaAUrLz8Z27zrb3s,1199
+pingpong/__init__.py,sha256=nbVCJWeMGyvXyYLVD97Nj9RaVxYXQPPHP8wS7ktHbAA,55
+pingpong/alpaca.py,sha256=WIo2FX8PAUDmLdq2FeN4_8fuuxmEnWStRpmNG1dTxUM,1446
 pingpong/dolly.py,sha256=jAWnieNLTPFzGNBI5hBaSIhx7XW0c7xGyO1PVGaBy9g,1215
 pingpong/gradio.py,sha256=IchvS_gOuPk3TCATVKDWMaLEaIRqjPpi3MFnYwa0JwU,987
 pingpong/pingpong.py,sha256=yQcXkdWc9aWem0vdbqtwMMvJXsqmLnwlSuGBkM4ZHk8,1192
 pingpong/context/__init__.py,sha256=ksYP7nq8inYK7SHDwpd7Hs_h87gPKdP9Ac6E5w0X6zM,173
 pingpong/context/auto_summary_strategy.py,sha256=s2lrlGKzLFNBGdLMAkaC6d2VY8aJSdgtrwa_Rvmt3Fc,589
 pingpong/context/last_window_strategy.py,sha256=37Gu94VVIMlj-pK3r7NMrOPp_XufMYsSthf5-ZJNw00,711
 pingpong/context/search_window_strategy.py,sha256=OPd2xxiI9FrzU4w2R5luaDEKiNEj4KYr_EF53Qi6l_Q,840
 pingpong/context/strategy.py,sha256=xGoy7T92gYubrwekz0Kz2Vxv10njgXG44K48bC9BqAU,119
-bingbong-0.1.6.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-bingbong-0.1.6.2.dist-info/METADATA,sha256=8O1yonxpEFHXis5NUuXPYhy2aV7x6FpQrE4p7Iaddu0,3348
-bingbong-0.1.6.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-bingbong-0.1.6.2.dist-info/top_level.txt,sha256=gEn53k5ARNLZodzDYx4bPsQ-F69t7ln5s4vJGgc3dgo,9
-bingbong-0.1.6.2.dist-info/RECORD,,
+bingbong-0.1.6.3.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+bingbong-0.1.6.3.dist-info/METADATA,sha256=7BH1k7OSrAcKYtYVhdGYjdUg0oaqk8hboI_ZXasNvY4,3348
+bingbong-0.1.6.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+bingbong-0.1.6.3.dist-info/top_level.txt,sha256=gEn53k5ARNLZodzDYx4bPsQ-F69t7ln5s4vJGgc3dgo,9
+bingbong-0.1.6.3.dist-info/RECORD,,
```

