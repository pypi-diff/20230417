# Comparing `tmp/xray_bot-0.1.1rc3-py3-none-any.whl.zip` & `tmp/xray_bot-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 10834 bytes, number of entries: 12
+Zip file size: 11029 bytes, number of entries: 12
 -rw-r--r--  2.0 unx      164 b- defN 23-Mar-07 06:51 xraybot/__init__.py
--rw-r--r--  2.0 unx       25 b- defN 23-Mar-16 08:43 xraybot/__version__.py
+-rw-r--r--  2.0 unx       22 b- defN 23-Apr-17 03:54 xraybot/__version__.py
 -rw-r--r--  2.0 unx     4225 b- defN 23-Mar-08 02:07 xraybot/_context.py
 -rw-r--r--  2.0 unx      505 b- defN 23-Mar-03 03:43 xraybot/_data.py
 -rw-r--r--  2.0 unx      192 b- defN 23-Mar-03 03:43 xraybot/_utils.py
--rw-r--r--  2.0 unx    17177 b- defN 23-Mar-08 03:54 xraybot/_worker.py
--rw-r--r--  2.0 unx    14589 b- defN 23-Mar-16 08:34 xraybot/_xray_bot.py
--rw-r--r--  2.0 unx     1065 b- defN 23-Mar-16 08:44 xray_bot-0.1.1rc3.dist-info/LICENSE
--rw-r--r--  2.0 unx      486 b- defN 23-Mar-16 08:44 xray_bot-0.1.1rc3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-16 08:44 xray_bot-0.1.1rc3.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Mar-16 08:44 xray_bot-0.1.1rc3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      931 b- defN 23-Mar-16 08:44 xray_bot-0.1.1rc3.dist-info/RECORD
-12 files, 39459 bytes uncompressed, 9280 bytes compressed:  76.5%
+-rw-r--r--  2.0 unx    17733 b- defN 23-Apr-17 03:52 xraybot/_worker.py
+-rw-r--r--  2.0 unx    15181 b- defN 23-Apr-17 05:48 xraybot/_xray_bot.py
+-rw-r--r--  2.0 unx     1065 b- defN 23-Apr-17 05:50 xray_bot-0.1.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx      483 b- defN 23-Apr-17 05:50 xray_bot-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-17 05:50 xray_bot-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Apr-17 05:50 xray_bot-0.1.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      916 b- defN 23-Apr-17 05:50 xray_bot-0.1.2.dist-info/RECORD
+12 files, 40586 bytes uncompressed, 9505 bytes compressed:  76.6%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: xraybot/_worker.py
 Comment: 
 
 Filename: xraybot/_xray_bot.py
 Comment: 
 
-Filename: xray_bot-0.1.1rc3.dist-info/LICENSE
+Filename: xray_bot-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: xray_bot-0.1.1rc3.dist-info/METADATA
+Filename: xray_bot-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: xray_bot-0.1.1rc3.dist-info/WHEEL
+Filename: xray_bot-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: xray_bot-0.1.1rc3.dist-info/top_level.txt
+Filename: xray_bot-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: xray_bot-0.1.1rc3.dist-info/RECORD
+Filename: xray_bot-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xraybot/__version__.py

```diff
@@ -1 +1 @@
-__version__ = "0.1.1rc3"
+__version__ = "0.1.2"
```

## xraybot/_worker.py

```diff
@@ -52,15 +52,17 @@
     def finalize_test(self, test_entity: TestEntity):
         logger.info(f"Start finalizing test: {test_entity.key}")
         try:
             self.context.jira.set_issue_status(test_entity.key, "Ready for Review")
             self.context.jira.set_issue_status(test_entity.key, "In Review")
             self.context.jira.set_issue_status(test_entity.key, "Finalized")
         except Exception as e:
-            logger.warning(f"Finalize test with error: {e}")
+            raise AssertionError(
+                f"Finalize test {test_entity.key} with error: {e}"
+            ) from e
 
     def link_test(self, test_entity: TestEntity):
         if test_entity.req_key:
             # support multi req keys
             req_key_list = test_entity.req_key.split(",")
             for _req_key in req_key_list:
                 logger.info(
@@ -70,25 +72,29 @@
                     "type": {"name": "Tests"},
                     "inwardIssue": {"key": test_entity.key},
                     "outwardIssue": {"key": _req_key},
                 }
                 try:
                     self.context.jira.create_issue_link(link_param)
                 except Exception as e:
-                    logger.warning(f"Link test with error: {e}")
+                    raise AssertionError(
+                        f"Link requirement {_req_key} with error: {e}"
+                    ) from e
 
     def add_test_into_folder(self, test_entity: TestEntity, folder_id: int):
         try:
             self.context.xray.put(
                 f"rest/raven/1.0/api/testrepository/"
                 f"{self.context.project_key}/folders/{folder_id}/tests",
                 data={"add": [test_entity.key]},
             )
         except Exception as e:
-            logger.warning(f"Move test to repo folder with error: {e}")
+            raise AssertionError(
+                f"Move test {test_entity.key} to repo folder with error: {e}"
+            ) from e
 
     def remove_test_from_folder(self, test_entity: TestEntity, folder_id: int):
         self.context.xray.put(
             f"rest/raven/1.0/api/testrepository/"
             f"{self.context.project_key}/folders/{folder_id}/tests",
             data={"remove": [test_entity.key]},
         )
@@ -132,15 +138,16 @@
         if status == "Finalized":
             return
 
         for status in ["Ready for Review", "In Review", "Finalized"]:
             try:
                 self.context.jira.set_issue_status(test_entity.key, status)
             except Exception as e:
-                logger.warning(f"Update test status with error: {e}")
+                # ignore errors from any status
+                logger.debug(f"Update test status with error: {e}")
 
         status = self.context.jira.get_issue_status(test_entity.key)
         assert (
             status == "Finalized"
         ), f"Marked test {test_entity.key} cannot be finalized."
 
     def renew_test_details(self, marked_test: TestEntity):
@@ -319,15 +326,15 @@
         self.api_wrapper.link_test(test_entity)
 
 
 class _ExternalMarkedTestUpdateWorker(_XrayBotWorker):
     def run(self, test_entity: TestEntity):
         logger.info(f"Start updating external marked test: {test_entity.key}")
         self.api_wrapper.renew_test_details(test_entity)
-        self.api_wrapper.finalize_test(test_entity)
+        self.api_wrapper.finalize_test_from_any_status(test_entity)
         self.api_wrapper.remove_links(test_entity)
         self.api_wrapper.link_test(test_entity)
         self.api_wrapper.add_test_into_folder(
             test_entity, self.api_wrapper.automation_folder_id
         )
 
 
@@ -414,23 +421,30 @@
     def __init__(self, context: XrayBotContext):
         self.context = context
         self.api_wrapper = _XrayAPIWrapper(self.context)
 
     @staticmethod
     def _worker_wrapper(worker_func, *iterables):
         try:
-            ret = worker_func(*iterables)
-            return ret
+            worker_func(*iterables)
+            return None
         except Exception as e:
             logger.info(
                 f"Worker [{worker_func.__qualname__.split('.')[0].lstrip('_')}] raised error: {e}"
             )
-            raise e
+            converted = []
+            for i in iterables:
+                if isinstance(i, TestEntity):
+                    converted.append(i.__str__())
+                else:
+                    converted.append(i)
+            return f"❌{e} -> 🐛{' | '.join(converted)}"
 
     def start_worker(self, worker_type: WorkerType, *iterables):
         worker: _XrayBotWorker = worker_type.value(self.api_wrapper)
         with ProcessPoolExecutor(self.context.config.worker_num) as executor:
-            executor.map(
+            results = executor.map(
                 self._worker_wrapper,
                 [worker.run for _ in range(len(iterables[0]))],
                 *iterables,
             )
+            return list(results)
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## xraybot/_xray_bot.py

```diff
@@ -146,42 +146,52 @@
                 non_marked_local_tests.append(local_test)
         return (
             non_marked_local_tests,
             internal_marked_local_tests,
             external_marked_local_tests,
         )
 
-    def sync_tests(self, local_tests: List[TestEntity]):
+    def sync_tests(self, local_tests: List[TestEntity]) -> List[str]:
+        errors = []
+        # make sure all local test keys will be considered as upper case
+        for local_test in local_tests:
+            if local_test.key is not None:
+                local_test.key = local_test.key.upper()
+
         self._check_duplicated_uniqueness(
             local_tests, "Duplicated key/unique_identifier found in local_tests"
         )
         self.worker_mgr.api_wrapper.init_automation_repo_folder()
         xray_tests = self.get_xray_tests()
         (
             non_marked_local_tests,
             internal_marked_local_tests,
             external_marked_local_tests,
         ) = self._categorize_local_tests(xray_tests, local_tests)
         if external_marked_local_tests:
             # external marked test -> strategy: update and move to automation folder
-            self.worker_mgr.start_worker(
-                WorkerType.ExternalMarkedTestUpdate, external_marked_local_tests
+            errors.extend(
+                self.worker_mgr.start_worker(
+                    WorkerType.ExternalMarkedTestUpdate, external_marked_local_tests
+                )
             )
         if internal_marked_local_tests:
             # internal marked test -> strategy: update all fields including unique identifier
             filtered_xray_tests = [
                 xray_test
                 for xray_test in xray_tests
                 if xray_test.key in [_.key for _ in internal_marked_local_tests]
             ]
             to_be_updated = self._get_internal_marked_tests_diff(
                 filtered_xray_tests, internal_marked_local_tests
             )
-            self.worker_mgr.start_worker(
-                WorkerType.InternalMarkedTestUpdate, to_be_updated
+            errors.extend(
+                self.worker_mgr.start_worker(
+                    WorkerType.InternalMarkedTestUpdate, to_be_updated
+                )
             )
         if non_marked_local_tests:
             # non marked test -> strategy: unique identifier sync
             # exclude internal marked local tests in xray tests
             # do not need to proceed unique identifier sync
             filtered_xray_tests = [
                 xray_test
@@ -191,19 +201,30 @@
             (
                 to_be_deleted,
                 to_be_appended,
                 to_be_updated,
             ) = self._get_non_marked_tests_diff(
                 filtered_xray_tests, non_marked_local_tests
             )
-            self.worker_mgr.start_worker(
-                WorkerType.NonMarkedTestObsolete, to_be_deleted
+            errors.extend(
+                self.worker_mgr.start_worker(
+                    WorkerType.NonMarkedTestObsolete, to_be_deleted
+                )
+            )
+            errors.extend(
+                self.worker_mgr.start_worker(
+                    WorkerType.NonMarkedTestCreate, to_be_appended
+                )
+            )
+            errors.extend(
+                self.worker_mgr.start_worker(
+                    WorkerType.NonMarkedTestUpdate, to_be_updated
+                )
             )
-            self.worker_mgr.start_worker(WorkerType.NonMarkedTestCreate, to_be_appended)
-            self.worker_mgr.start_worker(WorkerType.NonMarkedTestUpdate, to_be_updated)
+        return errors
 
     @staticmethod
     def _get_internal_marked_tests_diff(
         filtered_xray_tests: List[TestEntity],
         internal_marked_local_tests: List[TestEntity],
     ):
         to_be_updated = list()
```

## Comparing `xray_bot-0.1.1rc3.dist-info/LICENSE` & `xray_bot-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

