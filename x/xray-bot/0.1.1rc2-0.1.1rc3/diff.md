# Comparing `tmp/xray_bot-0.1.1rc2-py3-none-any.whl.zip` & `tmp/xray_bot-0.1.1rc3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 10818 bytes, number of entries: 12
+Zip file size: 10834 bytes, number of entries: 12
 -rw-r--r--  2.0 unx      164 b- defN 23-Mar-07 06:51 xraybot/__init__.py
--rw-r--r--  2.0 unx       25 b- defN 23-Mar-08 04:03 xraybot/__version__.py
+-rw-r--r--  2.0 unx       25 b- defN 23-Mar-16 08:43 xraybot/__version__.py
 -rw-r--r--  2.0 unx     4225 b- defN 23-Mar-08 02:07 xraybot/_context.py
 -rw-r--r--  2.0 unx      505 b- defN 23-Mar-03 03:43 xraybot/_data.py
 -rw-r--r--  2.0 unx      192 b- defN 23-Mar-03 03:43 xraybot/_utils.py
 -rw-r--r--  2.0 unx    17177 b- defN 23-Mar-08 03:54 xraybot/_worker.py
--rw-r--r--  2.0 unx    14520 b- defN 23-Mar-08 03:54 xraybot/_xray_bot.py
--rw-r--r--  2.0 unx     1065 b- defN 23-Mar-08 04:03 xray_bot-0.1.1rc2.dist-info/LICENSE
--rw-r--r--  2.0 unx      486 b- defN 23-Mar-08 04:03 xray_bot-0.1.1rc2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-08 04:03 xray_bot-0.1.1rc2.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Mar-08 04:03 xray_bot-0.1.1rc2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      931 b- defN 23-Mar-08 04:03 xray_bot-0.1.1rc2.dist-info/RECORD
-12 files, 39390 bytes uncompressed, 9264 bytes compressed:  76.5%
+-rw-r--r--  2.0 unx    14589 b- defN 23-Mar-16 08:34 xraybot/_xray_bot.py
+-rw-r--r--  2.0 unx     1065 b- defN 23-Mar-16 08:44 xray_bot-0.1.1rc3.dist-info/LICENSE
+-rw-r--r--  2.0 unx      486 b- defN 23-Mar-16 08:44 xray_bot-0.1.1rc3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Mar-16 08:44 xray_bot-0.1.1rc3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Mar-16 08:44 xray_bot-0.1.1rc3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      931 b- defN 23-Mar-16 08:44 xray_bot-0.1.1rc3.dist-info/RECORD
+12 files, 39459 bytes uncompressed, 9280 bytes compressed:  76.5%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: xraybot/_worker.py
 Comment: 
 
 Filename: xraybot/_xray_bot.py
 Comment: 
 
-Filename: xray_bot-0.1.1rc2.dist-info/LICENSE
+Filename: xray_bot-0.1.1rc3.dist-info/LICENSE
 Comment: 
 
-Filename: xray_bot-0.1.1rc2.dist-info/METADATA
+Filename: xray_bot-0.1.1rc3.dist-info/METADATA
 Comment: 
 
-Filename: xray_bot-0.1.1rc2.dist-info/WHEEL
+Filename: xray_bot-0.1.1rc3.dist-info/WHEEL
 Comment: 
 
-Filename: xray_bot-0.1.1rc2.dist-info/top_level.txt
+Filename: xray_bot-0.1.1rc3.dist-info/top_level.txt
 Comment: 
 
-Filename: xray_bot-0.1.1rc2.dist-info/RECORD
+Filename: xray_bot-0.1.1rc3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xraybot/__version__.py

```diff
@@ -1 +1 @@
-__version__ = "0.1.1rc2"
+__version__ = "0.1.1rc3"
```

## xraybot/_xray_bot.py

```diff
@@ -321,26 +321,26 @@
         clean_test_plan_and_execution: bool = False,
     ):
         test_plan_key = self.worker_mgr.api_wrapper.create_test_plan(test_plan_name)
         test_execution_key = self.worker_mgr.api_wrapper.create_test_execution(
             test_execution_name
         )
         tests = self.get_xray_tests()
-        # add tests to test plan
+        # add tests to test plan based on all xray tests
         self.worker_mgr.start_worker(
             WorkerType.AddTestsToPlan,
             [test_plan_key for _ in range(len(tests))],
             [_.key for _ in tests],
         )
 
-        # add tests to test execution
+        # add tests to test execution based on local tests execution
         self.worker_mgr.start_worker(
             WorkerType.AddTestsToExecution,
-            [test_execution_key for _ in range(len(tests))],
-            [_.key for _ in tests],
+            [test_execution_key for _ in range(len(test_results))],
+            [_.key for _ in test_results],
         )
 
         logger.info(
             f"Start adding test execution {test_execution_key} to test plan {test_plan_key}"
         )
         self.context.xray.update_test_plan_test_executions(
             test_plan_key, add=[test_execution_key]
```

## Comparing `xray_bot-0.1.1rc2.dist-info/LICENSE` & `xray_bot-0.1.1rc3.dist-info/LICENSE`

 * *Files identical despite different names*

