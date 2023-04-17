# Comparing `tmp/connect_extension_runner-27.8.tar.gz` & `tmp/connect_extension_runner-27.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connect_extension_runner-27.8.tar", max compression
+gzip compressed data, was "connect_extension_runner-27.9.tar", max compression
```

## Comparing `connect_extension_runner-27.8.tar` & `connect_extension_runner-27.9.tar`

### file list

```diff
@@ -1,35 +1,36 @@
--rw-r--r--   0        0        0    11357 2023-03-16 15:32:37.371013 connect_extension_runner-27.8/LICENSE
--rw-r--r--   0        0        0     1422 2023-03-16 15:32:37.371013 connect_extension_runner-27.8/README.md
--rw-r--r--   0        0        0       55 2023-03-16 15:32:37.371013 connect_extension_runner-27.8/connect/eaas/dataclasses.py
--rw-r--r--   0        0        0      405 2023-03-16 15:32:37.371013 connect_extension_runner-27.8/connect/eaas/extension.py
--rw-r--r--   0        0        0      143 2023-03-16 15:32:37.371013 connect_extension_runner-27.8/connect/eaas/runner/__init__.py
--rw-r--r--   0        0        0        0 2023-03-16 15:32:37.371013 connect_extension_runner-27.8/connect/eaas/runner/artworks/__init__.py
--rw-r--r--   0        0        0     9409 2023-03-16 15:32:37.371013 connect_extension_runner-27.8/connect/eaas/runner/artworks/ansi_regular.flf
--rw-r--r--   0        0        0      950 2023-03-16 15:32:37.371013 connect_extension_runner-27.8/connect/eaas/runner/artworks/banner.py
--rw-r--r--   0        0        0    11425 2023-03-16 15:32:37.375013 connect_extension_runner-27.8/connect/eaas/runner/artworks/bloody.flf
--rw-r--r--   0        0        0     6483 2023-03-16 15:32:37.375013 connect_extension_runner-27.8/connect/eaas/runner/config.py
--rw-r--r--   0        0        0     5575 2023-03-16 15:32:37.375013 connect_extension_runner-27.8/connect/eaas/runner/constants.py
--rw-r--r--   0        0        0      320 2023-03-16 15:32:37.375013 connect_extension_runner-27.8/connect/eaas/runner/exceptions.py
--rw-r--r--   0        0        0        0 2023-03-16 15:32:37.375013 connect_extension_runner-27.8/connect/eaas/runner/handlers/__init__.py
--rw-r--r--   0        0        0     2692 2023-03-16 15:32:37.375013 connect_extension_runner-27.8/connect/eaas/runner/handlers/anvil.py
--rw-r--r--   0        0        0     4392 2023-03-16 15:32:37.375013 connect_extension_runner-27.8/connect/eaas/runner/handlers/base.py
--rw-r--r--   0        0        0     3751 2023-03-16 15:32:37.375013 connect_extension_runner-27.8/connect/eaas/runner/handlers/events.py
--rw-r--r--   0        0        0     2444 2023-03-16 15:32:37.375013 connect_extension_runner-27.8/connect/eaas/runner/handlers/transformations.py
--rw-r--r--   0        0        0     5793 2023-03-16 15:32:37.375013 connect_extension_runner-27.8/connect/eaas/runner/handlers/web.py
--rw-r--r--   0        0        0    18704 2023-03-16 15:32:37.375013 connect_extension_runner-27.8/connect/eaas/runner/helpers.py
--rw-r--r--   0        0        0     1989 2023-03-16 15:32:37.375013 connect_extension_runner-27.8/connect/eaas/runner/main.py
--rw-r--r--   0        0        0      340 2023-03-16 15:32:37.375013 connect_extension_runner-27.8/connect/eaas/runner/managers/__init__.py
--rw-r--r--   0        0        0     3191 2023-03-16 15:32:37.375013 connect_extension_runner-27.8/connect/eaas/runner/managers/background.py
--rw-r--r--   0        0        0     8101 2023-03-16 15:32:37.375013 connect_extension_runner-27.8/connect/eaas/runner/managers/base.py
--rw-r--r--   0        0        0     2225 2023-03-16 15:32:37.375013 connect_extension_runner-27.8/connect/eaas/runner/managers/interactive.py
--rw-r--r--   0        0        0     1931 2023-03-16 15:32:37.375013 connect_extension_runner-27.8/connect/eaas/runner/managers/scheduled.py
--rw-r--r--   0        0        0    11988 2023-03-16 15:32:37.375013 connect_extension_runner-27.8/connect/eaas/runner/managers/transformation.py
--rw-r--r--   0        0        0     7917 2023-03-16 15:32:37.375013 connect_extension_runner-27.8/connect/eaas/runner/master.py
--rw-r--r--   0        0        0        0 2023-03-16 15:32:37.375013 connect_extension_runner-27.8/connect/eaas/runner/workers/__init__.py
--rw-r--r--   0        0        0     2549 2023-03-16 15:32:37.375013 connect_extension_runner-27.8/connect/eaas/runner/workers/anvil.py
--rw-r--r--   0        0        0    11320 2023-03-16 15:32:37.375013 connect_extension_runner-27.8/connect/eaas/runner/workers/base.py
--rw-r--r--   0        0        0     8834 2023-03-16 15:32:37.375013 connect_extension_runner-27.8/connect/eaas/runner/workers/events.py
--rw-r--r--   0        0        0     6545 2023-03-16 15:32:37.375013 connect_extension_runner-27.8/connect/eaas/runner/workers/transformations.py
--rw-r--r--   0        0        0     6846 2023-03-16 15:32:37.375013 connect_extension_runner-27.8/connect/eaas/runner/workers/web.py
--rw-r--r--   0        0        0     2802 2023-03-16 15:34:07.226474 connect_extension_runner-27.8/pyproject.toml
--rw-r--r--   0        0        0     3026 1970-01-01 00:00:00.000000 connect_extension_runner-27.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-03-22 15:22:15.174830 connect_extension_runner-27.9/LICENSE
+-rw-r--r--   0        0        0     1422 2023-03-22 15:22:15.174830 connect_extension_runner-27.9/README.md
+-rw-r--r--   0        0        0       55 2023-03-22 15:22:15.174830 connect_extension_runner-27.9/connect/eaas/dataclasses.py
+-rw-r--r--   0        0        0      405 2023-03-22 15:22:15.174830 connect_extension_runner-27.9/connect/eaas/extension.py
+-rw-r--r--   0        0        0      143 2023-03-22 15:22:15.174830 connect_extension_runner-27.9/connect/eaas/runner/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-22 15:22:15.174830 connect_extension_runner-27.9/connect/eaas/runner/artworks/__init__.py
+-rw-r--r--   0        0        0     9409 2023-03-22 15:22:15.174830 connect_extension_runner-27.9/connect/eaas/runner/artworks/ansi_regular.flf
+-rw-r--r--   0        0        0      950 2023-03-22 15:22:15.174830 connect_extension_runner-27.9/connect/eaas/runner/artworks/banner.py
+-rw-r--r--   0        0        0    11425 2023-03-22 15:22:15.178830 connect_extension_runner-27.9/connect/eaas/runner/artworks/bloody.flf
+-rw-r--r--   0        0        0     6483 2023-03-22 15:22:15.178830 connect_extension_runner-27.9/connect/eaas/runner/config.py
+-rw-r--r--   0        0        0     5633 2023-03-22 15:22:15.178830 connect_extension_runner-27.9/connect/eaas/runner/constants.py
+-rw-r--r--   0        0        0      320 2023-03-22 15:22:15.178830 connect_extension_runner-27.9/connect/eaas/runner/exceptions.py
+-rw-r--r--   0        0        0        0 2023-03-22 15:22:15.178830 connect_extension_runner-27.9/connect/eaas/runner/handlers/__init__.py
+-rw-r--r--   0        0        0     2692 2023-03-22 15:22:15.178830 connect_extension_runner-27.9/connect/eaas/runner/handlers/anvil.py
+-rw-r--r--   0        0        0     4392 2023-03-22 15:22:15.178830 connect_extension_runner-27.9/connect/eaas/runner/handlers/base.py
+-rw-r--r--   0        0        0     3751 2023-03-22 15:22:15.178830 connect_extension_runner-27.9/connect/eaas/runner/handlers/events.py
+-rw-r--r--   0        0        0     2444 2023-03-22 15:22:15.178830 connect_extension_runner-27.9/connect/eaas/runner/handlers/transformations.py
+-rw-r--r--   0        0        0     5793 2023-03-22 15:22:15.178830 connect_extension_runner-27.9/connect/eaas/runner/handlers/web.py
+-rw-r--r--   0        0        0    18982 2023-03-22 15:22:15.178830 connect_extension_runner-27.9/connect/eaas/runner/helpers.py
+-rw-r--r--   0        0        0     1989 2023-03-22 15:22:15.178830 connect_extension_runner-27.9/connect/eaas/runner/main.py
+-rw-r--r--   0        0        0      340 2023-03-22 15:22:15.178830 connect_extension_runner-27.9/connect/eaas/runner/managers/__init__.py
+-rw-r--r--   0        0        0     3191 2023-03-22 15:22:15.178830 connect_extension_runner-27.9/connect/eaas/runner/managers/background.py
+-rw-r--r--   0        0        0     8101 2023-03-22 15:22:15.178830 connect_extension_runner-27.9/connect/eaas/runner/managers/base.py
+-rw-r--r--   0        0        0     2225 2023-03-22 15:22:15.178830 connect_extension_runner-27.9/connect/eaas/runner/managers/interactive.py
+-rw-r--r--   0        0        0     1931 2023-03-22 15:22:15.178830 connect_extension_runner-27.9/connect/eaas/runner/managers/scheduled.py
+-rw-r--r--   0        0        0    14441 2023-03-22 15:22:15.178830 connect_extension_runner-27.9/connect/eaas/runner/managers/transformation.py
+-rw-r--r--   0        0        0      533 2023-03-22 15:22:15.178830 connect_extension_runner-27.9/connect/eaas/runner/managers/utils.py
+-rw-r--r--   0        0        0     7917 2023-03-22 15:22:15.178830 connect_extension_runner-27.9/connect/eaas/runner/master.py
+-rw-r--r--   0        0        0        0 2023-03-22 15:22:15.178830 connect_extension_runner-27.9/connect/eaas/runner/workers/__init__.py
+-rw-r--r--   0        0        0     2549 2023-03-22 15:22:15.178830 connect_extension_runner-27.9/connect/eaas/runner/workers/anvil.py
+-rw-r--r--   0        0        0    11320 2023-03-22 15:22:15.178830 connect_extension_runner-27.9/connect/eaas/runner/workers/base.py
+-rw-r--r--   0        0        0     8834 2023-03-22 15:22:15.178830 connect_extension_runner-27.9/connect/eaas/runner/workers/events.py
+-rw-r--r--   0        0        0     6545 2023-03-22 15:22:15.178830 connect_extension_runner-27.9/connect/eaas/runner/workers/transformations.py
+-rw-r--r--   0        0        0     6846 2023-03-22 15:22:15.178830 connect_extension_runner-27.9/connect/eaas/runner/workers/web.py
+-rw-r--r--   0        0        0     2802 2023-03-22 15:23:39.386584 connect_extension_runner-27.9/pyproject.toml
+-rw-r--r--   0        0        0     3026 1970-01-01 00:00:00.000000 connect_extension_runner-27.9/PKG-INFO
```

### Comparing `connect_extension_runner-27.8/LICENSE` & `connect_extension_runner-27.9/LICENSE`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-27.8/README.md` & `connect_extension_runner-27.9/README.md`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-27.8/connect/eaas/runner/artworks/ansi_regular.flf` & `connect_extension_runner-27.9/connect/eaas/runner/artworks/ansi_regular.flf`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-27.8/connect/eaas/runner/artworks/banner.py` & `connect_extension_runner-27.9/connect/eaas/runner/artworks/banner.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-27.8/connect/eaas/runner/artworks/bloody.flf` & `connect_extension_runner-27.9/connect/eaas/runner/artworks/bloody.flf`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-27.8/connect/eaas/runner/config.py` & `connect_extension_runner-27.9/connect/eaas/runner/config.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-27.8/connect/eaas/runner/constants.py` & `connect_extension_runner-27.9/connect/eaas/runner/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,19 +94,20 @@
     EventType.PRODUCT_ACTION_EXECUTION,
     EventType.PRODUCT_CUSTOM_EVENT_PROCESSING,
 )
 
 BACKGROUND_TASK_MAX_EXECUTION_TIME = 300
 INTERACTIVE_TASK_MAX_EXECUTION_TIME = 120
 SCHEDULED_TASK_MAX_EXECUTION_TIME = 60 * 60 * 12
-TRANSFORMATION_TASK_MAX_EXECUTION_TIME = 300
+TRANSFORMATION_TASK_MAX_EXECUTION_TIME = 60 * 60 * 4
+ROW_TRANSFORMATION_TASK_MAX_EXECUTION_TIME = 60
 RESULT_SENDER_MAX_RETRIES = 5
 RESULT_SENDER_WAIT_GRACE_SECONDS = 90
-TRANSFORMATION_TASK_MAX_PARALLEL_LINES = 20
-DOWNLOAD_CHUNK_SIZE = 1024
+TRANSFORMATION_TASK_MAX_PARALLEL_LINES = 200
+DOWNLOAD_CHUNK_SIZE = 65535
 UPLOAD_CHUNK_SIZE = 65535
 TRANSFORMATION_WRITE_QUEUE_TIMEOUT = 600
 
 MAX_RETRY_TIME_GENERIC_SECONDS = 15 * 60
 MAX_RETRY_TIME_MAINTENANCE_SECONDS = 3 * 60 * 60
 MAX_RETRY_DELAY_TIME_SECONDS = 5 * 60
```

### Comparing `connect_extension_runner-27.8/connect/eaas/runner/handlers/anvil.py` & `connect_extension_runner-27.9/connect/eaas/runner/handlers/anvil.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-27.8/connect/eaas/runner/handlers/base.py` & `connect_extension_runner-27.9/connect/eaas/runner/handlers/base.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-27.8/connect/eaas/runner/handlers/events.py` & `connect_extension_runner-27.9/connect/eaas/runner/handlers/events.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-27.8/connect/eaas/runner/handlers/transformations.py` & `connect_extension_runner-27.9/connect/eaas/runner/handlers/transformations.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-27.8/connect/eaas/runner/handlers/web.py` & `connect_extension_runner-27.9/connect/eaas/runner/handlers/web.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-27.8/connect/eaas/runner/helpers.py` & `connect_extension_runner-27.9/connect/eaas/runner/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 )
 from connect.eaas.runner.constants import (
     BACKGROUND_TASK_MAX_EXECUTION_TIME,
     HANDLER_CLASS_TITLE,
     INTERACTIVE_TASK_MAX_EXECUTION_TIME,
     ORDINAL_SUFFIX,
     PYPI_EXTENSION_RUNNER_URL,
+    ROW_TRANSFORMATION_TASK_MAX_EXECUTION_TIME,
     SCHEDULED_TASK_MAX_EXECUTION_TIME,
     TRANSFORMATION_TASK_MAX_EXECUTION_TIME,
     TRANSFORMATION_WRITE_QUEUE_TIMEOUT,
 )
 
 
 logger = logging.getLogger('connect.eaas')
@@ -111,14 +112,20 @@
         )),
         'scheduled_task_max_execution_time': int(os.getenv(
             'SCHEDULED_TASK_MAX_EXECUTION_TIME', SCHEDULED_TASK_MAX_EXECUTION_TIME,
         )),
         'transformation_task_max_execution_time': int(os.getenv(
             'TRANSFORMATION_TASK_MAX_EXECUTION_TIME', TRANSFORMATION_TASK_MAX_EXECUTION_TIME,
         )),
+        'row_transformation_task_max_execution_time': int(
+            os.getenv(
+                'ROW_TRANSFORMATION_TASK_MAX_EXECUTION_TIME',
+                ROW_TRANSFORMATION_TASK_MAX_EXECUTION_TIME,
+            ),
+        ),
         'transformation_write_queue_timeout': int(os.getenv(
             'TRANSFORMATION_WRITE_QUEUE_TIMEOUT', TRANSFORMATION_WRITE_QUEUE_TIMEOUT,
         )),
     }
 
 
 def get_version():
```

### Comparing `connect_extension_runner-27.8/connect/eaas/runner/main.py` & `connect_extension_runner-27.9/connect/eaas/runner/main.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-27.8/connect/eaas/runner/managers/background.py` & `connect_extension_runner-27.9/connect/eaas/runner/managers/background.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-27.8/connect/eaas/runner/managers/base.py` & `connect_extension_runner-27.9/connect/eaas/runner/managers/base.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-27.8/connect/eaas/runner/managers/interactive.py` & `connect_extension_runner-27.9/connect/eaas/runner/managers/interactive.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-27.8/connect/eaas/runner/managers/scheduled.py` & `connect_extension_runner-27.9/connect/eaas/runner/managers/scheduled.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-27.8/connect/eaas/runner/managers/transformation.py` & `connect_extension_runner-27.9/connect/eaas/runner/managers/transformation.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,14 +20,17 @@
     Workbook,
     load_workbook,
 )
 
 from connect.eaas.core.enums import (
     ResultType,
 )
+from connect.eaas.core.logging import (
+    RequestLogger,
+)
 from connect.eaas.core.proto import (
     Task,
     TaskOutput,
 )
 from connect.eaas.core.responses import (
     TransformationResponse,
 )
@@ -35,14 +38,17 @@
     DOWNLOAD_CHUNK_SIZE,
     TRANSFORMATION_TASK_MAX_PARALLEL_LINES,
     UPLOAD_CHUNK_SIZE,
 )
 from connect.eaas.runner.managers.base import (
     TasksManagerBase,
 )
+from connect.eaas.runner.managers.utils import (
+    ResultStore,
+)
 
 
 logger = logging.getLogger(__name__)
 
 
 class TransformationTasksManager(TasksManagerBase):
     """
@@ -52,14 +58,15 @@
     def get_client(self, task_data):
         if task_data.options.api_key:
             return AsyncConnectClient(
                 task_data.options.api_key,
                 endpoint=self.config.get_api_url(),
                 use_specs=False,
                 default_headers=self.config.get_user_agent(),
+                logger=RequestLogger(logger),
             )
 
         return self.client
 
     def send_skip_response(self, data, output):
         future = asyncio.Future()
         future.set_result(TransformationResponse.skip(output))
@@ -103,72 +110,93 @@
         ))
 
         logger.info(f'Enqueue result for task {task_data.options.task_id}')
         asyncio.create_task(self.enqueue_result(task_data, future))
 
     async def build_response(self, task_data, future):
         result_message = Task(**task_data.dict())
+        timeout = self.config.get_timeout('transformation')
         try:
             begin_ts = time.monotonic()
             result = await asyncio.wait_for(
                 future,
-                timeout=self.config.get_timeout('transformation'),
+                timeout=timeout,
             )
             result_message.output = TaskOutput(result=result.status)
             result_message.output.runtime = time.monotonic() - begin_ts
             logger.info(
                 f'Transformation task {task_data.options.task_id} '
                 f'result: {result.status}, '
                 f'took: {result_message.output.runtime}',
             )
             if result.status in (ResultType.SKIP, ResultType.FAIL):
                 result_message.output.message = result.output
         except Exception as e:
+            cause = (
+                str(e) if not isinstance(e, asyncio.TimeoutError)
+                else 'timed out after {timeout} s'
+            )
             self.log_exception(task_data, e)
+            await self._fail_task(task_data, cause)
             result_message.output = TaskOutput(result=ResultType.FAIL)
             result_message.output.message = traceback.format_exc()[:4000]
 
         return result_message
 
+    async def _fail_task(self, task_data, message):
+        try:
+            client = self.get_client(task_data)
+            await client('billing').requests[task_data.input.object_id]('fail').post()
+            await client.conversations[task_data.input.object_id].messages.create(
+                payload={
+                    'type': 'message',
+                    'text': f'Transformation request processing failed: {message}.',
+                },
+            )
+        except Exception:
+            logger.exception(f'Cannot fail the transformation request {task_data.input.object_id}')
+
     async def process_transformation(self, task_data, tfn_request, method):
+        semaphore = asyncio.Semaphore(TRANSFORMATION_TASK_MAX_PARALLEL_LINES)
         input_file = await asyncio.get_running_loop().run_in_executor(
             self.executor,
             self.download_excel,
             tfn_request,
             task_data.options.api_key,
         )
         output_file = NamedTemporaryFile(
             suffix=f'.{tfn_request["files"]["input"]["name"].split(".")[-1]}',
         )
 
         read_queue = asyncio.Queue(TRANSFORMATION_TASK_MAX_PARALLEL_LINES)
-        write_queue = asyncio.Queue()
+        result_store = ResultStore()
 
         loop = asyncio.get_event_loop()
 
         reader_task = loop.run_in_executor(
             self.executor,
             self.read_excel,
             input_file,
             read_queue,
             loop,
         )
         writer_task = loop.run_in_executor(
             self.executor,
             self.write_excel,
             output_file.name,
-            write_queue,
+            result_store,
             tfn_request['stats']['rows']['total'],
             tfn_request['transformation']['columns']['output'],
             task_data,
             loop,
         )
         processor_task = asyncio.create_task(self.process_rows(
+            semaphore,
             read_queue,
-            write_queue,
+            result_store,
             method,
             tfn_request['stats']['rows']['total'],
         ))
 
         tasks = [reader_task, writer_task, processor_task]
         try:
             await asyncio.gather(*tasks)
@@ -180,14 +208,20 @@
             for task in tasks:
                 if not task.done():
                     task.cancel()
             input_file.close()
             output_file.close()
             client = self.get_client(task_data)
             await client('billing').requests[task_data.input.object_id]('fail').post()
+            await client.conversations[task_data.input.object_id].messages.create(
+                payload={
+                    'type': 'message',
+                    'text': f'Transformation request processing failed: {str(e)}',
+                },
+            )
             return TransformationResponse.fail(output=str(e))
 
         await self.send_output_file(task_data, tfn_request['batch']['id'], output_file)
         input_file.close()
         output_file.close()
         return TransformationResponse.done()
 
@@ -226,102 +260,127 @@
             asyncio.run_coroutine_threadsafe(
                 queue.put((idx, row_data)),
                 loop,
             )
 
         wb.close()
 
-    async def process_rows(self, read_queue, write_queue, method, total_rows):
+    async def process_rows(self, semaphore, read_queue, result_store, method, total_rows):
         rows_processed = 0
         tasks = []
-        while rows_processed < total_rows - 1:
+        while rows_processed < total_rows:
+            await semaphore.acquire()
             row_idx, row = await read_queue.get()
-
             if inspect.iscoroutinefunction(method):
-                tasks.append(asyncio.create_task(self.async_process_row(
-                    method,
-                    row_idx,
-                    row,
-                    write_queue,
-                )))
+                tasks.append(
+                    asyncio.create_task(
+                        asyncio.wait_for(
+                            self.async_process_row(
+                                semaphore,
+                                method,
+                                row_idx,
+                                row,
+                                result_store,
+                            ),
+                            self.config.get_timeout('row_transformation'),
+                        ),
+                    ),
+                )
             else:
                 loop = asyncio.get_running_loop()
-                tasks.append(loop.run_in_executor(
-                    self.executor,
-                    self.sync_process_row,
-                    method,
-                    row_idx,
-                    row,
-                    write_queue,
-                    loop,
-                ))
+                tasks.append(
+                    asyncio.create_task(
+                        asyncio.wait_for(
+                            loop.run_in_executor(
+                                self.executor,
+                                self.sync_process_row,
+                                semaphore,
+                                method,
+                                row_idx,
+                                row,
+                                result_store,
+                                loop,
+                            ),
+                            self.config.get_timeout('row_transformation'),
+                        ),
+                    ),
+                )
 
             rows_processed += 1
 
         try:
             await asyncio.gather(*tasks)
         except Exception as e:
             logger.error('Error during applying transformation to row.')
             for task in tasks:
                 task.cancel()
             raise e
 
-    async def async_process_row(self, method, row_idx, row, write_queue):
+    async def async_process_row(self, semaphore, method, row_idx, row, result_store):
         transformed_row = await method(row)
-        await write_queue.put((row_idx, transformed_row))
+        await result_store.put(row_idx, transformed_row)
+        semaphore.release()
+
+    def sync_process_row(self, semaphore, method, row_idx, row, result_store, loop):
+        async def store_results(transformed_row):
+            await result_store.put(row_idx, transformed_row)
+            semaphore.release()
 
-    def sync_process_row(self, method, row_idx, row, write_queue, loop):
         transformed_row = method(row)
-        asyncio.run_coroutine_threadsafe(
-            write_queue.put((row_idx, transformed_row)),
-            loop,
-        )
+        asyncio.run_coroutine_threadsafe(store_results(transformed_row), loop)
 
-    def write_excel(self, filename, queue, total_rows, output_columns, task_data, loop):
-        wb = Workbook()
+    def write_excel(self, filename, result_store, total_rows, output_columns, task_data, loop):
+        wb = Workbook(write_only=True)
 
-        ws_columns = wb.active
+        ws_columns = wb.create_sheet('Columns')
         ws = wb.create_sheet('Data')
         ws_columns.title = 'Columns'
         ws_columns.append(['Name', 'Type', 'Nullable', 'Description', 'Precision'])
         column_keys = ['name', 'type', 'nullable', 'description', 'precision']
-        lookup_columns = {}
-        for col_idx, column in enumerate(output_columns, start=1):
+
+        column_names = []
+
+        for column in output_columns:
             row = [column.get(key) for key in column_keys]
             ws_columns.append(row)
-            lookup_columns[column.get('name')] = col_idx
-            ws.cell(row=1, column=col_idx, value=column.get('name'))
+            column_names.append(column.get('name'))
+
+        ws.append(column_names)
 
         rows_processed = 0
-        total_rows -= 1
         delta = 1 if total_rows <= 10 else round(total_rows / 10)
 
-        while rows_processed < total_rows:
+        for idx in range(2, total_rows + 2):
             future = asyncio.run_coroutine_threadsafe(
-                queue.get(),
+                result_store.get(idx),
                 loop,
             )
-            row_idx, row = future.result(
+            row_data = future.result(
                 timeout=self.config.env['transformation_write_queue_timeout'],
             )
-            for name, value in row.items():
-                ws.cell(row=row_idx, column=lookup_columns[name], value=value)
+            row = [row_data.get(col_name) for col_name in column_names]
+
+            ws.append(row)
             rows_processed += 1
             if rows_processed % delta == 0 or rows_processed == total_rows:
                 asyncio.run_coroutine_threadsafe(
-                    self.send_stat_update(task_data, rows_processed),
+                    self.send_stat_update(task_data, rows_processed, total_rows),
                     loop,
                 )
+                logger.debug(
+                    f'{task_data.input.object_id} processed {rows_processed}'
+                    f' of {total_rows} rows',
+                )
 
         wb.save(filename)
 
-    async def send_stat_update(self, task_data, rows_processed):
+    async def send_stat_update(self, task_data, rows_processed, total_rows):
         client = self.get_client(task_data)
         await client('billing').requests[task_data.input.object_id].update(
-            payload={'rows_processed': rows_processed},
+            payload={'stats': {'rows': {'total': total_rows, 'processed': rows_processed}}},
         )
 
     async def send_output_file(self, task_data, batch_id, output_file):
         client = self.get_client(task_data)
 
         fileobj = open(output_file.name, 'rb')
         fileobj.seek(0, os.SEEK_END)
```

### Comparing `connect_extension_runner-27.8/connect/eaas/runner/master.py` & `connect_extension_runner-27.9/connect/eaas/runner/master.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-27.8/connect/eaas/runner/workers/anvil.py` & `connect_extension_runner-27.9/connect/eaas/runner/workers/anvil.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-27.8/connect/eaas/runner/workers/base.py` & `connect_extension_runner-27.9/connect/eaas/runner/workers/base.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-27.8/connect/eaas/runner/workers/events.py` & `connect_extension_runner-27.9/connect/eaas/runner/workers/events.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-27.8/connect/eaas/runner/workers/transformations.py` & `connect_extension_runner-27.9/connect/eaas/runner/workers/transformations.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-27.8/connect/eaas/runner/workers/web.py` & `connect_extension_runner-27.9/connect/eaas/runner/workers/web.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-27.8/pyproject.toml` & `connect_extension_runner-27.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "connect-extension-runner"
-version = "27.8"
+version = "27.9"
 description = "CloudBlue Connect EaaS Extension Runner"
 authors = ["CloudBlue LLC"]
 license = "Apache-2.0"
 packages = [
     { include = "connect" },
 ]
 readme = "./README.md"
@@ -28,15 +28,15 @@
 [tool.poetry.dependencies]
 python = ">=3.8,<4"
 websockets = "10.*"
 connect-openapi-client = ">=25.16"
 logzio-python-handler = "^3.0.0"
 backoff = "^1.11.1"
 uvloop = "^0.16.0"
-connect-eaas-core = ">=27.6,<28"
+connect-eaas-core = ">=27.7,<28"
 httpx = "^0.23.0"
 rich = "^12.5.1"
 pyfiglet = "^0.8.post1"
 devtools = "^0.9.0"
 watchfiles = "^0.17.0"
 openpyxl = "^3.0.10"
```

### Comparing `connect_extension_runner-27.8/PKG-INFO` & `connect_extension_runner-27.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connect-extension-runner
-Version: 27.8
+Version: 27.9
 Summary: CloudBlue Connect EaaS Extension Runner
 Home-page: https://connect.cloudblue.com
 License: Apache-2.0
 Author: CloudBlue LLC
 Requires-Python: >=3.8,<4
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Requires-Dist: backoff (>=1.11.1,<2.0.0)
-Requires-Dist: connect-eaas-core (>=27.6,<28)
+Requires-Dist: connect-eaas-core (>=27.7,<28)
 Requires-Dist: connect-openapi-client (>=25.16)
 Requires-Dist: devtools (>=0.9.0,<0.10.0)
 Requires-Dist: httpx (>=0.23.0,<0.24.0)
 Requires-Dist: logzio-python-handler (>=3.0.0,<4.0.0)
 Requires-Dist: openpyxl (>=3.0.10,<4.0.0)
 Requires-Dist: pyfiglet (>=0.8.post1,<0.9)
 Requires-Dist: rich (>=12.5.1,<13.0.0)
```

