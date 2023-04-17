# Comparing `tmp/meilisearch_python_async-1.1.1.tar.gz` & `tmp/meilisearch_python_async-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meilisearch_python_async-1.1.1.tar", max compression
+gzip compressed data, was "meilisearch_python_async-1.2.0.tar", max compression
```

## Comparing `meilisearch_python_async-1.1.1.tar` & `meilisearch_python_async-1.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1069 2023-04-07 22:06:54.234997 meilisearch_python_async-1.1.1/LICENSE
--rw-r--r--   0        0        0     4641 2023-04-07 22:06:54.234997 meilisearch_python_async-1.1.1/README.md
--rw-r--r--   0        0        0       73 2023-04-07 22:06:54.238996 meilisearch_python_async-1.1.1/meilisearch_python_async/__init__.py
--rw-r--r--   0        0        0     2538 2023-04-07 22:06:54.238996 meilisearch_python_async-1.1.1/meilisearch_python_async/_http_requests.py
--rw-r--r--   0        0        0    22123 2023-04-07 22:06:54.238996 meilisearch_python_async-1.1.1/meilisearch_python_async/client.py
--rw-r--r--   0        0        0     1886 2023-04-07 22:06:54.238996 meilisearch_python_async-1.1.1/meilisearch_python_async/errors.py
--rw-r--r--   0        0        0    86427 2023-04-07 22:06:54.238996 meilisearch_python_async-1.1.1/meilisearch_python_async/index.py
--rw-r--r--   0        0        0        0 2023-04-07 22:06:54.238996 meilisearch_python_async-1.1.1/meilisearch_python_async/models/__init__.py
--rw-r--r--   0        0        0     1576 2023-04-07 22:06:54.238996 meilisearch_python_async-1.1.1/meilisearch_python_async/models/client.py
--rw-r--r--   0        0        0      202 2023-04-07 22:06:54.238996 meilisearch_python_async-1.1.1/meilisearch_python_async/models/documents.py
--rw-r--r--   0        0        0       95 2023-04-07 22:06:54.238996 meilisearch_python_async-1.1.1/meilisearch_python_async/models/health.py
--rw-r--r--   0        0        0      392 2023-04-07 22:06:54.238996 meilisearch_python_async-1.1.1/meilisearch_python_async/models/index.py
--rw-r--r--   0        0        0     1285 2023-04-07 22:06:54.238996 meilisearch_python_async-1.1.1/meilisearch_python_async/models/search.py
--rw-r--r--   0        0        0     1119 2023-04-07 22:06:54.238996 meilisearch_python_async-1.1.1/meilisearch_python_async/models/settings.py
--rw-r--r--   0        0        0      769 2023-04-07 22:06:54.238996 meilisearch_python_async-1.1.1/meilisearch_python_async/models/task.py
--rw-r--r--   0        0        0      215 2023-04-07 22:06:54.238996 meilisearch_python_async-1.1.1/meilisearch_python_async/models/version.py
--rw-r--r--   0        0        0        0 2023-04-07 22:06:54.238996 meilisearch_python_async-1.1.1/meilisearch_python_async/py.typed
--rw-r--r--   0        0        0    10993 2023-04-07 22:06:54.238996 meilisearch_python_async-1.1.1/meilisearch_python_async/task.py
--rw-r--r--   0        0        0     2138 2023-04-07 22:06:54.238996 meilisearch_python_async-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     6102 1970-01-01 00:00:00.000000 meilisearch_python_async-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-17 14:11:57.547336 meilisearch_python_async-1.2.0/LICENSE
+-rw-r--r--   0        0        0     4641 2023-04-17 14:11:57.547336 meilisearch_python_async-1.2.0/README.md
+-rw-r--r--   0        0        0       73 2023-04-17 14:11:57.547336 meilisearch_python_async-1.2.0/meilisearch_python_async/__init__.py
+-rw-r--r--   0        0        0     2538 2023-04-17 14:11:57.547336 meilisearch_python_async-1.2.0/meilisearch_python_async/_http_requests.py
+-rw-r--r--   0        0        0    22123 2023-04-17 14:11:57.547336 meilisearch_python_async-1.2.0/meilisearch_python_async/client.py
+-rw-r--r--   0        0        0     1886 2023-04-17 14:11:57.547336 meilisearch_python_async-1.2.0/meilisearch_python_async/errors.py
+-rw-r--r--   0        0        0    86427 2023-04-17 14:11:57.547336 meilisearch_python_async-1.2.0/meilisearch_python_async/index.py
+-rw-r--r--   0        0        0        0 2023-04-17 14:11:57.547336 meilisearch_python_async-1.2.0/meilisearch_python_async/models/__init__.py
+-rw-r--r--   0        0        0     1576 2023-04-17 14:11:57.547336 meilisearch_python_async-1.2.0/meilisearch_python_async/models/client.py
+-rw-r--r--   0        0        0      202 2023-04-17 14:11:57.547336 meilisearch_python_async-1.2.0/meilisearch_python_async/models/documents.py
+-rw-r--r--   0        0        0       95 2023-04-17 14:11:57.547336 meilisearch_python_async-1.2.0/meilisearch_python_async/models/health.py
+-rw-r--r--   0        0        0      392 2023-04-17 14:11:57.547336 meilisearch_python_async-1.2.0/meilisearch_python_async/models/index.py
+-rw-r--r--   0        0        0     1285 2023-04-17 14:11:57.547336 meilisearch_python_async-1.2.0/meilisearch_python_async/models/search.py
+-rw-r--r--   0        0        0     1119 2023-04-17 14:11:57.547336 meilisearch_python_async-1.2.0/meilisearch_python_async/models/settings.py
+-rw-r--r--   0        0        0      769 2023-04-17 14:11:57.547336 meilisearch_python_async-1.2.0/meilisearch_python_async/models/task.py
+-rw-r--r--   0        0        0      215 2023-04-17 14:11:57.547336 meilisearch_python_async-1.2.0/meilisearch_python_async/models/version.py
+-rw-r--r--   0        0        0        0 2023-04-17 14:11:57.547336 meilisearch_python_async-1.2.0/meilisearch_python_async/py.typed
+-rw-r--r--   0        0        0    11610 2023-04-17 14:11:57.547336 meilisearch_python_async-1.2.0/meilisearch_python_async/task.py
+-rw-r--r--   0        0        0     2138 2023-04-17 14:11:57.551337 meilisearch_python_async-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6102 1970-01-01 00:00:00.000000 meilisearch_python_async-1.2.0/PKG-INFO
```

### Comparing `meilisearch_python_async-1.1.1/LICENSE` & `meilisearch_python_async-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.1.1/README.md` & `meilisearch_python_async-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.1.1/meilisearch_python_async/_http_requests.py` & `meilisearch_python_async-1.2.0/meilisearch_python_async/_http_requests.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.1.1/meilisearch_python_async/client.py` & `meilisearch_python_async-1.2.0/meilisearch_python_async/client.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.1.1/meilisearch_python_async/errors.py` & `meilisearch_python_async-1.2.0/meilisearch_python_async/errors.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.1.1/meilisearch_python_async/index.py` & `meilisearch_python_async-1.2.0/meilisearch_python_async/index.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.1.1/meilisearch_python_async/models/client.py` & `meilisearch_python_async-1.2.0/meilisearch_python_async/models/client.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.1.1/meilisearch_python_async/models/search.py` & `meilisearch_python_async-1.2.0/meilisearch_python_async/models/search.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.1.1/meilisearch_python_async/models/settings.py` & `meilisearch_python_async-1.2.0/meilisearch_python_async/models/settings.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.1.1/meilisearch_python_async/models/task.py` & `meilisearch_python_async-1.2.0/meilisearch_python_async/models/task.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.1.1/meilisearch_python_async/task.py` & `meilisearch_python_async-1.2.0/meilisearch_python_async/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,25 +226,26 @@
     return TaskStatus(**response.json())
 
 
 async def wait_for_task(
     client: AsyncClient | Client,
     task_id: int,
     *,
-    timeout_in_ms: int = 5000,
+    timeout_in_ms: int | None = 5000,
     interval_in_ms: int = 50,
 ) -> TaskStatus:
     """Wait until Meilisearch processes a task, and get its status.
 
     Args:
 
         client: An httpx AsyncClient or meilisearch_python_async Client instance.
         task_id: Identifier of the task to retrieve.
         timeout_in_ms: Amount of time in milliseconds to wait before raising a
-            MeilisearchTimeoutError. Defaults to 5000.
+            MeilisearchTimeoutError. `None` can also be passed to wait indefinitely. Be aware that
+            if the `None` option is used the wait time could be very long. Defaults to 5000.
         interval_in_ms: Time interval in miliseconds to sleep between requests. Defaults to 50.
 
     Returns:
 
         Details of the processed update status.
 
     Raises:
@@ -267,25 +268,36 @@
         >>>     await wait_for_pending_task(client, response.update_id)
     """
     client_ = _get_client(client)
     url = f"tasks/{task_id}"
     http_requests = HttpRequests(client_)
     start_time = datetime.now()
     elapsed_time = 0.0
-    while elapsed_time < timeout_in_ms:
-        response = await http_requests.get(url)
-        status = TaskStatus(**response.json())
-        if status.status in ("succeeded", "failed"):
-            return status
-        await sleep(interval_in_ms / 1000)
-        time_delta = datetime.now() - start_time
-        elapsed_time = time_delta.seconds * 1000 + time_delta.microseconds / 1000
-    raise MeilisearchTimeoutError(
-        f"timeout of {timeout_in_ms}ms has exceeded on process {task_id} when waiting for pending update to resolve."
-    )
+
+    if timeout_in_ms:
+        while elapsed_time < timeout_in_ms:
+            response = await http_requests.get(url)
+            status = TaskStatus(**response.json())
+            if status.status in ("succeeded", "failed"):
+                return status
+            await sleep(interval_in_ms / 1000)
+            time_delta = datetime.now() - start_time
+            elapsed_time = time_delta.seconds * 1000 + time_delta.microseconds / 1000
+        raise MeilisearchTimeoutError(
+            f"timeout of {timeout_in_ms}ms has exceeded on process {task_id} when waiting for pending update to resolve."
+        )
+    else:
+        while True:
+            response = await http_requests.get(url)
+            status = TaskStatus(**response.json())
+            if status.status in ("succeeded", "failed"):
+                return status
+            await sleep(interval_in_ms / 1000)
+            time_delta = datetime.now() - start_time
+            elapsed_time = time_delta.seconds * 1000 + time_delta.microseconds / 1000
 
 
 def _get_client(client: AsyncClient | Client) -> AsyncClient:
     if isinstance(client, AsyncClient):
         return client
 
     return client.http_client
```

### Comparing `meilisearch_python_async-1.1.1/pyproject.toml` & `meilisearch_python_async-1.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "meilisearch-python-async"
-version = "1.1.1"
+version = "1.2.0"
 description = "A Python async client for the Meilisearch API"
 authors = ["Paul Sanders <psanders1@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/sanders41/meilisearch-python-async"
 homepage = "https://github.com/sanders41/meilisearch-python-async"
 documentation = "https://meilisearch-python-async.paulsanders.dev"
```

### Comparing `meilisearch_python_async-1.1.1/PKG-INFO` & `meilisearch_python_async-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meilisearch-python-async
-Version: 1.1.1
+Version: 1.2.0
 Summary: A Python async client for the Meilisearch API
 Home-page: https://github.com/sanders41/meilisearch-python-async
 License: MIT
 Keywords: meilisearch,async,python
 Author: Paul Sanders
 Author-email: psanders1@gmail.com
 Requires-Python: >=3.7,<4.0
```

