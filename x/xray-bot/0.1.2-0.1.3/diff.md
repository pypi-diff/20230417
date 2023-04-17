# Comparing `tmp/xray_bot-0.1.2-py3-none-any.whl.zip` & `tmp/xray_bot-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 11029 bytes, number of entries: 12
+Zip file size: 11044 bytes, number of entries: 12
 -rw-r--r--  2.0 unx      164 b- defN 23-Mar-07 06:51 xraybot/__init__.py
--rw-r--r--  2.0 unx       22 b- defN 23-Apr-17 03:54 xraybot/__version__.py
+-rw-r--r--  2.0 unx       22 b- defN 23-Apr-17 06:54 xraybot/__version__.py
 -rw-r--r--  2.0 unx     4225 b- defN 23-Mar-08 02:07 xraybot/_context.py
 -rw-r--r--  2.0 unx      505 b- defN 23-Mar-03 03:43 xraybot/_data.py
 -rw-r--r--  2.0 unx      192 b- defN 23-Mar-03 03:43 xraybot/_utils.py
 -rw-r--r--  2.0 unx    17733 b- defN 23-Apr-17 03:52 xraybot/_worker.py
--rw-r--r--  2.0 unx    15181 b- defN 23-Apr-17 05:48 xraybot/_xray_bot.py
--rw-r--r--  2.0 unx     1065 b- defN 23-Apr-17 05:50 xray_bot-0.1.2.dist-info/LICENSE
--rw-r--r--  2.0 unx      483 b- defN 23-Apr-17 05:50 xray_bot-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-17 05:50 xray_bot-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Apr-17 05:50 xray_bot-0.1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      916 b- defN 23-Apr-17 05:50 xray_bot-0.1.2.dist-info/RECORD
-12 files, 40586 bytes uncompressed, 9505 bytes compressed:  76.6%
+-rw-r--r--  2.0 unx    14945 b- defN 23-Apr-17 06:10 xraybot/_xray_bot.py
+-rw-r--r--  2.0 unx     1065 b- defN 23-Apr-17 06:54 xray_bot-0.1.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx      483 b- defN 23-Apr-17 06:54 xray_bot-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-17 06:54 xray_bot-0.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Apr-17 06:54 xray_bot-0.1.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      916 b- defN 23-Apr-17 06:54 xray_bot-0.1.3.dist-info/RECORD
+12 files, 40350 bytes uncompressed, 9520 bytes compressed:  76.4%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: xraybot/_worker.py
 Comment: 
 
 Filename: xraybot/_xray_bot.py
 Comment: 
 
-Filename: xray_bot-0.1.2.dist-info/LICENSE
+Filename: xray_bot-0.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: xray_bot-0.1.2.dist-info/METADATA
+Filename: xray_bot-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: xray_bot-0.1.2.dist-info/WHEEL
+Filename: xray_bot-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: xray_bot-0.1.2.dist-info/top_level.txt
+Filename: xray_bot-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: xray_bot-0.1.2.dist-info/RECORD
+Filename: xray_bot-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xraybot/__version__.py

```diff
@@ -1 +1 @@
-__version__ = "0.1.2"
+__version__ = "0.1.3"
```

## xraybot/_xray_bot.py

```diff
@@ -185,45 +185,39 @@
                 filtered_xray_tests, internal_marked_local_tests
             )
             errors.extend(
                 self.worker_mgr.start_worker(
                     WorkerType.InternalMarkedTestUpdate, to_be_updated
                 )
             )
-        if non_marked_local_tests:
-            # non marked test -> strategy: unique identifier sync
-            # exclude internal marked local tests in xray tests
-            # do not need to proceed unique identifier sync
-            filtered_xray_tests = [
-                xray_test
-                for xray_test in xray_tests
-                if xray_test.key not in [_.key for _ in internal_marked_local_tests]
-            ]
-            (
-                to_be_deleted,
-                to_be_appended,
-                to_be_updated,
-            ) = self._get_non_marked_tests_diff(
-                filtered_xray_tests, non_marked_local_tests
-            )
-            errors.extend(
-                self.worker_mgr.start_worker(
-                    WorkerType.NonMarkedTestObsolete, to_be_deleted
-                )
-            )
-            errors.extend(
-                self.worker_mgr.start_worker(
-                    WorkerType.NonMarkedTestCreate, to_be_appended
-                )
-            )
-            errors.extend(
-                self.worker_mgr.start_worker(
-                    WorkerType.NonMarkedTestUpdate, to_be_updated
-                )
-            )
+
+        # non marked test -> strategy: unique identifier sync
+        # exclude internal marked local tests in xray tests
+        # do not need to proceed unique identifier sync
+        filtered_xray_tests = [
+            xray_test
+            for xray_test in xray_tests
+            if xray_test.key not in [_.key for _ in internal_marked_local_tests]
+        ]
+        (
+            to_be_deleted,
+            to_be_appended,
+            to_be_updated,
+        ) = self._get_non_marked_tests_diff(filtered_xray_tests, non_marked_local_tests)
+        errors.extend(
+            self.worker_mgr.start_worker(
+                WorkerType.NonMarkedTestObsolete, to_be_deleted
+            )
+        )
+        errors.extend(
+            self.worker_mgr.start_worker(WorkerType.NonMarkedTestCreate, to_be_appended)
+        )
+        errors.extend(
+            self.worker_mgr.start_worker(WorkerType.NonMarkedTestUpdate, to_be_updated)
+        )
         return errors
 
     @staticmethod
     def _get_internal_marked_tests_diff(
         filtered_xray_tests: List[TestEntity],
         internal_marked_local_tests: List[TestEntity],
     ):
```

## Comparing `xray_bot-0.1.2.dist-info/LICENSE` & `xray_bot-0.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

