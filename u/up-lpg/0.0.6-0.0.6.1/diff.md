# Comparing `tmp/up_lpg-0.0.6-pp39-pypy39_pp73-win_amd64.whl.zip` & `tmp/up_lpg-0.0.6.1-pp39-pypy39_pp73-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 1190245 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat       36 b- defN 23-Mar-28 23:07 up_lpg/__init__.py
--rw-rw-rw-  2.0 fat     9595 b- defN 23-Mar-28 23:07 up_lpg/lpg_planner.py
--rw-rw-rw-  2.0 fat  3881596 b- defN 23-Mar-28 23:07 up_lpg/winlpg.exe
--rw-rw-rw-  2.0 fat    11558 b- defN 23-Mar-28 23:15 up_lpg-0.0.6.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      334 b- defN 23-Mar-28 23:15 up_lpg-0.0.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat      107 b- defN 23-Mar-28 23:15 up_lpg-0.0.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Mar-28 23:15 up_lpg-0.0.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      609 b- defN 23-Mar-28 23:15 up_lpg-0.0.6.dist-info/RECORD
-8 files, 3903842 bytes uncompressed, 1189195 bytes compressed:  69.6%
+Zip file size: 1190304 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat       36 b- defN 23-Apr-17 10:27 up_lpg/__init__.py
+-rw-rw-rw-  2.0 fat     9713 b- defN 23-Apr-17 10:27 up_lpg/lpg_planner.py
+-rw-rw-rw-  2.0 fat  3881596 b- defN 23-Apr-17 10:27 up_lpg/winlpg.exe
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-Apr-17 10:33 up_lpg-0.0.6.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      336 b- defN 23-Apr-17 10:33 up_lpg-0.0.6.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      107 b- defN 23-Apr-17 10:33 up_lpg-0.0.6.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Apr-17 10:33 up_lpg-0.0.6.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      619 b- defN 23-Apr-17 10:33 up_lpg-0.0.6.1.dist-info/RECORD
+8 files, 3903972 bytes uncompressed, 1189234 bytes compressed:  69.6%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: up_lpg/lpg_planner.py
 Comment: 
 
 Filename: up_lpg/winlpg.exe
 Comment: 
 
-Filename: up_lpg-0.0.6.dist-info/LICENSE
+Filename: up_lpg-0.0.6.1.dist-info/LICENSE
 Comment: 
 
-Filename: up_lpg-0.0.6.dist-info/METADATA
+Filename: up_lpg-0.0.6.1.dist-info/METADATA
 Comment: 
 
-Filename: up_lpg-0.0.6.dist-info/WHEEL
+Filename: up_lpg-0.0.6.1.dist-info/WHEEL
 Comment: 
 
-Filename: up_lpg-0.0.6.dist-info/top_level.txt
+Filename: up_lpg-0.0.6.1.dist-info/top_level.txt
 Comment: 
 
-Filename: up_lpg-0.0.6.dist-info/RECORD
+Filename: up_lpg-0.0.6.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## up_lpg/lpg_planner.py

```diff
@@ -33,14 +33,17 @@
     @property
     def name(self) -> str:
         return 'lpg'
 
     def _get_cmd(self, domain_filename: str, problem_filename: str, plan_filename: str) -> List[str]:
         base_command = [pkg_resources.resource_filename(__name__, lpg_os[sys.platform]), '-o', domain_filename, '-f', problem_filename, '-n', '1', '-out', plan_filename]  + self._options
         return base_command
+    
+    def  _get_engine_epsilon(self, new_epsilon:float):
+        self._options.extend(['-t', str(new_epsilon)])
 
     def _plan_from_file(self, problem: 'up.model.Problem', plan_filename: str, get_item_named: Callable[[str],
             Union[
                 'up.model.Type',
                 'up.model.Action',
                 'up.model.Fluent',
                 'up.model.Object',
```

## Comparing `up_lpg-0.0.6.dist-info/LICENSE` & `up_lpg-0.0.6.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `up_lpg-0.0.6.dist-info/RECORD` & `up_lpg-0.0.6.1.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 up_lpg/__init__.py,sha256=cD1uY16onwsxHOEI1I-lmF6WlYtDKB8YOie6BNUZji0,36
-up_lpg/lpg_planner.py,sha256=X-K9YGZF6Ore-jutxxlsaAODqczfRYMNMH6aAkeYsU0,9595
+up_lpg/lpg_planner.py,sha256=OZPI5WwqNG8mZLRyqOqwHCkJALCPyKA2o6htm3nrgAQ,9713
 up_lpg/winlpg.exe,sha256=Ut1frT86CopooTsvbc20MyQGGUrmRtWnVLObmzp4v4w,3881596
-up_lpg-0.0.6.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-up_lpg-0.0.6.dist-info/METADATA,sha256=m9d6b2asRPsty1lDYC30bQIUNhSne6b_2OY7S0y4q4A,334
-up_lpg-0.0.6.dist-info/WHEEL,sha256=kbzA5tyEuvWcVsltnhCG02Vwq0RkG0K4o74bVDVA1mQ,107
-up_lpg-0.0.6.dist-info/top_level.txt,sha256=p4RjFqpyQ96YXeEcg2Qtkfgt61fd_rOwRCePcthjdUk,7
-up_lpg-0.0.6.dist-info/RECORD,,
+up_lpg-0.0.6.1.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+up_lpg-0.0.6.1.dist-info/METADATA,sha256=yvRJjhkdGDaXUjzfCAmlgSkQwEC4KSeBnN6mJYPsyPg,336
+up_lpg-0.0.6.1.dist-info/WHEEL,sha256=kbzA5tyEuvWcVsltnhCG02Vwq0RkG0K4o74bVDVA1mQ,107
+up_lpg-0.0.6.1.dist-info/top_level.txt,sha256=p4RjFqpyQ96YXeEcg2Qtkfgt61fd_rOwRCePcthjdUk,7
+up_lpg-0.0.6.1.dist-info/RECORD,,
```

