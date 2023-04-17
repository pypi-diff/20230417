# Comparing `tmp/upathlib-0.7.7b1.tar.gz` & `tmp/upathlib-0.7.8b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upathlib-0.7.7b1.tar", last modified: Mon Apr 10 09:15:46 2023, max compression
+gzip compressed data, was "upathlib-0.7.8b1.tar", last modified: Mon Apr 17 07:08:38 2023, max compression
```

## Comparing `upathlib-0.7.7b1.tar` & `upathlib-0.7.8b1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1067 2022-12-13 07:44:37.384893 upathlib-0.7.7b1/LICENSE
--rw-r--r--   0        0        0      993 2023-03-30 16:49:23.794031 upathlib-0.7.7b1/README.rst
--rw-r--r--   0        0        0     1696 2023-04-10 08:06:32.336660 upathlib-0.7.7b1/pyproject.toml
--rw-r--r--   0        0        0     2305 2023-04-10 09:02:39.215528 upathlib-0.7.7b1/src/upathlib/__init__.py
--rw-r--r--   0        0        0     4438 2023-04-10 08:06:32.336660 upathlib-0.7.7b1/src/upathlib/_blob.py
--rw-r--r--   0        0        0    11176 2023-04-10 09:03:09.436670 upathlib-0.7.7b1/src/upathlib/_local.py
--rw-r--r--   0        0        0     7852 2023-03-07 05:27:40.006650 upathlib-0.7.7b1/src/upathlib/_tests.py
--rw-r--r--   0        0        0    34266 2023-04-10 09:03:09.506671 upathlib-0.7.7b1/src/upathlib/_upath.py
--rw-r--r--   0        0        0    12562 2023-04-10 08:06:32.346660 upathlib-0.7.7b1/src/upathlib/azure.py
--rw-r--r--   0        0        0    25298 2023-04-10 08:06:32.346660 upathlib-0.7.7b1/src/upathlib/gcs.py
--rw-r--r--   0        0        0        0 2022-12-13 07:44:37.384893 upathlib-0.7.7b1/src/upathlib/py.typed
--rw-r--r--   0        0        0     3763 2023-04-10 08:06:32.346660 upathlib-0.7.7b1/src/upathlib/serializer.py
--rw-r--r--   0        0        0     2383 1970-01-01 00:00:00.000000 upathlib-0.7.7b1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2022-12-13 07:44:37.384893 upathlib-0.7.8b1/LICENSE
+-rw-r--r--   0        0        0      993 2023-03-30 16:49:23.794031 upathlib-0.7.8b1/README.rst
+-rw-r--r--   0        0        0     1726 2023-04-15 03:57:22.660027 upathlib-0.7.8b1/pyproject.toml
+-rw-r--r--   0        0        0     2305 2023-04-17 06:17:49.758743 upathlib-0.7.8b1/src/upathlib/__init__.py
+-rw-r--r--   0        0        0     4438 2023-04-10 08:06:32.336660 upathlib-0.7.8b1/src/upathlib/_blob.py
+-rw-r--r--   0        0        0    11176 2023-04-15 03:57:22.660027 upathlib-0.7.8b1/src/upathlib/_local.py
+-rw-r--r--   0        0        0     7852 2023-03-07 05:27:40.006650 upathlib-0.7.8b1/src/upathlib/_tests.py
+-rw-r--r--   0        0        0    34436 2023-04-15 03:57:22.660027 upathlib-0.7.8b1/src/upathlib/_upath.py
+-rw-r--r--   0        0        0    12562 2023-04-10 08:06:32.346660 upathlib-0.7.8b1/src/upathlib/azure.py
+-rw-r--r--   0        0        0    25885 2023-04-17 06:40:21.797618 upathlib-0.7.8b1/src/upathlib/gcs.py
+-rw-r--r--   0        0        0        0 2022-12-13 07:44:37.384893 upathlib-0.7.8b1/src/upathlib/py.typed
+-rw-r--r--   0        0        0     3763 2023-04-10 08:06:32.346660 upathlib-0.7.8b1/src/upathlib/serializer.py
+-rw-r--r--   0        0        0     2383 1970-01-01 00:00:00.000000 upathlib-0.7.8b1/PKG-INFO
```

### Comparing `upathlib-0.7.7b1/LICENSE` & `upathlib-0.7.8b1/LICENSE`

 * *Files identical despite different names*

### Comparing `upathlib-0.7.7b1/README.rst` & `upathlib-0.7.8b1/README.rst`

 * *Files identical despite different names*

### Comparing `upathlib-0.7.7b1/pyproject.toml` & `upathlib-0.7.8b1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -58,17 +58,18 @@
 
 [tool.flit.module]
 name = "upathlib"
 
 
 # See https://beta.ruff.rs/docs/rules/
 [tool.ruff]
-target-version = "py310"
+target-version = "py38"
 select = ["E", "F", "S", "I001"]  # isort
 ignore = ["E501", "S101", "S102", "S103", "S104", "S108", "S301", "S311", "S608"]
+exclude = ["tests/benchmarks"]
 
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["E402", "F401"]
 
 
 [tool.pytest.ini_options]
```

### Comparing `upathlib-0.7.7b1/src/upathlib/__init__.py` & `upathlib-0.7.8b1/src/upathlib/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 One use case is the package `biglist <https://biglist.readthedocs.io/en/latest/>`__,
 where the class `Biglist <https://biglist.readthedocs.io/en/latest/#biglist.Biglist>`__ takes a Upath object to indicate its location of storage.
 It does not care whether the storage is local or in a cloud blob store---it
 simply uses the common API to operate the storage.
 """
 
-__version__ = "0.7.7b1"
+__version__ = "0.7.8b1"
 
 from pathlib import Path
 from typing import Union
 
 from ._blob import BlobUpath
 from ._local import LocalUpath
 from ._upath import FileInfo, LockAcquireError, LockReleaseError, Upath
```

### Comparing `upathlib-0.7.7b1/src/upathlib/_blob.py` & `upathlib-0.7.8b1/src/upathlib/_blob.py`

 * *Files identical despite different names*

### Comparing `upathlib-0.7.7b1/src/upathlib/_local.py` & `upathlib-0.7.8b1/src/upathlib/_local.py`

 * *Files identical despite different names*

### Comparing `upathlib-0.7.7b1/src/upathlib/_tests.py` & `upathlib-0.7.8b1/src/upathlib/_tests.py`

 * *Files identical despite different names*

### Comparing `upathlib-0.7.7b1/src/upathlib/_upath.py` & `upathlib-0.7.8b1/src/upathlib/_upath.py`

 * *Files 1% similar despite different names*

```diff
@@ -894,28 +894,31 @@
         Similar to :meth:`iterdir`, if ``self`` is not a dir or does not exist,
         then nothing is yielded, and no exception is raised either.
 
         There is no guarantee on the order of the returned elements.
         """
         raise NotImplementedError
 
-    def rmrf(self, *, quiet: bool = True, concurrent: bool = True) -> int:
+    def rmrf(self, *, quiet: bool = True, concurrent: bool = False) -> int:
         """Remove the current file or dir (i.e. ``self``) recursively.
 
         Analogous to the Linux command ``rm -rf``, hence the name of this method.
 
         Return the number of files removed.
 
         For example, if these blobs are present::
 
             /a/b/c/d/e.txt
             /a/b/c/kk.data
             /a/b/c
 
         then ``Upath('/a/b/c').rmrf()`` would remove all of them.
+
+        ``concurrent`` is ``False`` by default because this method is often used in
+        ``__del__`` of user classes, and thread pool is problematic in ``__del__``.
         """
         if self._path == "/":
             raise UnsupportedOperation("`rmrf` not allowed on root directory")
         try:
             self.remove_file()
         except (FileNotFoundError, IsADirectoryError):
             n = 0
```

### Comparing `upathlib-0.7.7b1/src/upathlib/azure.py` & `upathlib-0.7.8b1/src/upathlib/azure.py`

 * *Files identical despite different names*

### Comparing `upathlib-0.7.7b1/src/upathlib/gcs.py` & `upathlib-0.7.8b1/src/upathlib/gcs.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,22 +10,30 @@
 import time
 from collections.abc import Iterator
 from datetime import datetime, timezone
 from io import BufferedReader, BytesIO, UnsupportedOperation
 from typing import Optional
 
 import google.auth
-import requests
-import requests.exceptions
 from google import resumable_media
 from google.api_core import exceptions
-from google.api_core.retry import if_exception_type
-from google.auth import exceptions as auth_exceptions
 from google.cloud import storage
-from google.cloud.storage.retry import DEFAULT_RETRY
+
+# 60 seconds; this is the "connection timeout" to server.
+# From my reading, it's the `timeout` parameter to `google.cloud.storage.client._connection.api_request`,
+# that is, the `timeout` parameter to `google.cloud._http.JSONConnection.api_request`.
+# `google.cloud` is repo python-cloud-core.
+from google.cloud.storage.retry import (
+    DEFAULT_RETRY,
+    DEFAULT_RETRY_IF_GENERATION_SPECIFIED,
+    ConditionalRetryPolicy,
+    is_generation_specified,
+)
+
+# The default timeout in `DEFAULT_RETRY` is 120 seconds.
 from mpservice.util import MAX_THREADS, get_shared_thread_pool
 from typing_extensions import Self
 
 from ._blob import BlobUpath, LocalPathType, _resolve_local_path
 from ._upath import FileInfo, LockAcquireError, LockReleaseError, Upath
 
 logger = logging.getLogger(__name__)
@@ -35,25 +43,25 @@
 
 
 # 67108864 = 256 * 1024 * 256 = 64 MB
 MEGABYTES32 = 33554432
 MEGABYTES64 = 67108864
 LARGE_FILE_SIZE = MEGABYTES64
 
+# DEFAULT_RETRY has default timeout 120 seconds.
+
 
-RETRY_WRITE_ON_EXCEPTIONS = [
-    exceptions.InternalServerError,
-    exceptions.TooManyRequests,
-    exceptions.ServiceUnavailable,
-    exceptions.GatewayTimeout,
-    requests.exceptions.ReadTimeout,
-    requests.exceptions.ConnectionError,
-    requests.exceptions.ChunkedEncodingError,
-    auth_exceptions.TransportError,
-]
+def retry_if_generation_specified(retry_timeout=None):
+    if retry_timeout is None:
+        return DEFAULT_RETRY_IF_GENERATION_SPECIFIED
+    return ConditionalRetryPolicy(
+        DEFAULT_RETRY.with_timeout(retry_timeout),
+        is_generation_specified,
+        ["query_params"],
+    )
 
 
 def get_google_auth(
     project_id=None,
     credentials=None,
     *,
     scopes: list[str] = None,
@@ -261,22 +269,30 @@
             prefix=prefix,
             max_results=1,
             page_size=1,
             fields="items(name),nextPageToken",
         )
         return len(list(blobs)) > 0
 
-    def file_info(self) -> Optional[FileInfo]:
+    def file_info(self, *, request_timeout=60) -> Optional[FileInfo]:
         """
         Return file info if the current path is a file;
         otherwise return ``None``.
+
+        ``request_timeout`` is the http request timeout, not "retry" timeout.
+        The default is 60 (``google.cloud.storage.constants._DEFAULT_TIMEOUT``).
         """
         b = self._blob()
         try:
-            b.reload(client=self._client())
+            print('type(b)', type(b))
+            b.reload(
+                client=self._client(),
+                timeout=request_timeout,
+                retry=DEFAULT_RETRY.with_timeout(max(120, request_timeout * 2)),
+            )
         except exceptions.NotFound:
             return None
         return FileInfo(
             ctime=b.time_created.timestamp(),
             mtime=b.updated.timestamp(),
             time_created=b.time_created,
             time_modified=b.updated,
@@ -295,26 +311,33 @@
         obj = self.__class__(
             bucket_name=self.bucket_name,
         )
         obj._bucket_ = self._bucket()
         return obj
 
     def _write_from_buffer(
-        self, file_obj, *, overwrite=False, content_type=None, size=None
+        self,
+        file_obj,
+        *,
+        overwrite=False,
+        content_type=None,
+        size=None,
+        retry_timeout=None,
     ):
         if self._path == "/":
             raise UnsupportedOperation("can not write to root as a blob", self)
 
         try:
             self._blob().upload_from_file(
                 file_obj,
                 content_type=content_type,
                 size=size,
                 client=self._client(),
                 if_generation_match=None if overwrite else 0,
+                retry=retry_if_generation_specified(retry_timeout=retry_timeout),
             )
             # TODO: set "create_time", 'update_time" to be the same
             # as the source local file?
             # Blob objects has methods `_set_properties`, `_patch_property`,
             # `patch`.
         except exceptions.PreconditionFailed:
             raise FileExistsError(self)
@@ -335,31 +358,37 @@
         try:
             memoryview(data)
         except TypeError:  # file-like data
             self._write_from_buffer(
                 data, content_type="text/plain", overwrite=overwrite
             )
         else:  # bytes-like data
-            self._blob_rate_limit(self._write_bytes, data, overwrite=overwrite)
+            self._write_bytes(data, overwrite=overwrite)
 
     def _multipart_download(self, blob_size, file_obj):
         client = self._client()
         blob = self._blob()
 
         def _download(start, end):
             # Both `start` and `end` are inclusive.
             # The very first `start` should be 0.
             buffer = BytesIO()
             target_size = end - start + 1
             current_size = 0
             while True:
                 try:
                     blob.download_to_file(
-                        buffer, client=client, start=start + current_size, end=end
+                        buffer,
+                        client=client,
+                        start=start + current_size,
+                        end=end,
+                        raw_download=True,
                     )
+                    # "checksum mismatch" errors were encountered when downloading Parquet files.
+                    # `raw_download=True` seems to prevent that error.
                 except exceptions.NotFound:
                     raise FileNotFoundError(blob.name)
                 current_size = buffer.tell()
                 if current_size >= target_size:
                     break
                 # When a large number (say 10) of workers independently download
                 # the same large blob, practice showed the number of bytes downloaded
@@ -392,47 +421,43 @@
             for tt in tasks[it:]:
                 if not tt.done():
                     tt.cancel()
                     # This may not succeed, but there isn't a good way to
                     # guarantee cancellation here.
             raise
 
-    def _read_into_buffer(self, file_obj):
-        file_info = self.file_info()
+    def _read_into_buffer(self, file_obj, *, request_timeout=120):
+        file_info = self.file_info(request_timeout=request_timeout)
         if not file_info:
             raise FileNotFoundError(self)
         file_size = file_info.size  # bytes
         if file_size <= LARGE_FILE_SIZE:
             try:
-                self._blob().download_to_file(file_obj, client=self._client())
+                self._blob().download_to_file(
+                    file_obj, client=self._client(), raw_download=True
+                )
+                # "checksum mismatch" errors were encountered when downloading Parquet files.
+                # `raw_download=True` seems to prevent that error.
                 return
             except exceptions.NotFound:
                 raise FileNotFoundError(self)
         else:
             self._multipart_download(file_size, file_obj)
 
     def read_bytes(self) -> bytes:
         """
         Return the content of the current blob as bytes.
         """
         buffer = BytesIO()
         self._read_into_buffer(buffer)
         return buffer.getvalue()
 
-    def _blob_rate_limit(self, func, *args, **kwargs):
-        # `func_name` is a create/update/delete function.
-        # Google imposes rate limiting on such requests.
-        # According to Google doc, https://cloud.google.com/storage/quotas,
-        #   There is a write limit to the same object name. This limit is once per second.
-        f = DEFAULT_RETRY.with_predicate(if_exception_type(*RETRY_WRITE_ON_EXCEPTIONS))(
-            func
-        )
-        # Apply this inside the function so that user could add elements
-        # to ``RETRY_WRITE_ON_EXCEPTIONS``.
-        return f(*args, **kwargs)
+    # Google imposes rate limiting on create/update/delete requests.
+    # According to Google doc, https://cloud.google.com/storage/quotas,
+    #   There is a limit on writes to the same object name. This limit is once per second.
 
     def _copy_file(self, target: Upath, *, overwrite=False) -> None:
         if isinstance(target, GcsBlobUpath):
             # https://cloud.google.com/storage/docs/copying-renaming-moving-objects
             try:
                 self._bucket().copy_blob(
                     self._blob(),
@@ -483,25 +508,22 @@
         content_type = self._blob()._get_content_type(None, filename=filename)
 
         if self.is_file():
             if not overwrite:
                 raise FileExistsError(self)
             self.remove_file()
 
-        def _upload():
-            with open(filename, "rb") as file_obj:
-                total_bytes = os.fstat(file_obj.fileno()).st_size
-                self._write_from_buffer(
-                    file_obj,
-                    size=total_bytes,
-                    content_type=content_type,
-                    overwrite=overwrite,
-                )
-
-        self._blob_rate_limit(_upload)
+        with open(filename, "rb") as file_obj:
+            total_bytes = os.fstat(file_obj.fileno()).st_size
+            self._write_from_buffer(
+                file_obj,
+                size=total_bytes,
+                content_type=content_type,
+                overwrite=overwrite,
+            )
 
     def iterdir(self) -> Iterator[Self]:
         """
         Yield immediate children under the current dir.
         """
         # From Google doc:
         #
@@ -567,15 +589,15 @@
         return z
 
     def remove_file(self) -> None:
         """
         Remove the current blob.
         """
         try:
-            self._blob_rate_limit(self._blob().delete, client=self._client())
+            self._blob().delete(client=self._client())
         except exceptions.NotFound:
             raise FileNotFoundError(self)
 
     def riterdir(self) -> Iterator[Self]:
         """
         Yield all blobs recursively under the current dir.
         """
@@ -596,47 +618,33 @@
         # `timeout = None` with infinite wait, the default wait
         # is a long period.
         if self._path == "/":
             raise UnsupportedOperation("can not write to root as a blob", self)
         if timeout is None:
             timeout = 120  # seconds
 
-        retry = DEFAULT_RETRY.with_timeout(timeout).with_predicate(
-            if_exception_type(
-                *RETRY_WRITE_ON_EXCEPTIONS,
-                exceptions.PreconditionFailed,
-                FileExistsError,
-            )
-        )
-
-        @retry
-        def _acquire_():
-            self._write_bytes(b"0")
-            self._generation = self._blob().generation
-
         t0 = time.perf_counter()
         try:
-            _acquire_()
+            self._write_bytes(b"0", retry_timeout=timeout)
+            self._generation = self._blob().generation
         except FileExistsError as e:
-            finfo = self.file_info()
+            finfo = self.file_info(request_timeout=timeout)
             now = datetime.utcnow().replace(tzinfo=timezone.utc)
             file_age = (now - finfo.time_created).total_seconds()
             if file_age - timeout > self._LOCK_EXPIRE_IN_SECONDS:
                 # If the file is old,
                 # assume it is a dead file, that is, the last lock operation
                 # somehow failed and did not delete the file.
                 logger.warning(
                     "the locker file '%s' was created %d seconds ago; assuming it is dead and deleting it",
                     self,
                     int(file_age),
                 )
-                self._blob_rate_limit(
-                    self._blob().delete,
-                    client=self._client(),
-                )  # If this fails, the exception will propagate, which is not LockAcquireError.
+                self._blob().delete(client=self._client())
+                # If this fails, the exception will propagate, which is not LockAcquireError.
                 # After deleting the file, try it again:
                 self._acquire_lease(timeout=timeout)
             else:
                 raise LockAcquireError(
                     f"waited on '{self}' for {time.perf_counter() - t0:.2f} seconds"
                 ) from e
         except Exception as e:
@@ -666,19 +674,20 @@
         self._lock_count += 1
         try:
             yield
         finally:
             self._lock_count -= 1
             if self._lock_count == 0:
                 try:
-                    self._blob_rate_limit(
-                        self._blob().delete,
-                        client=self._client(),
+                    self._blob().delete(
                         if_generation_match=self._generation,  # TODO: should we remove this condition?
+                        timeout=150,
+                        retry=retry_if_generation_specified(retry_timeout=300),
                     )
+
                 except Exception as e:
                     raise LockReleaseError(f"failed to delete lock file {self}") from e
 
     def open(self, mode="r", **kwargs):
         """
         Use this on a blob (not a "directory") as a context manager.
         See Google documentation.
```

### Comparing `upathlib-0.7.7b1/src/upathlib/serializer.py` & `upathlib-0.7.8b1/src/upathlib/serializer.py`

 * *Files identical despite different names*

### Comparing `upathlib-0.7.7b1/PKG-INFO` & `upathlib-0.7.8b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upathlib
-Version: 0.7.7b1
+Version: 0.7.8b1
 Summary: The package *upathlib*
 Author-email: Zepu Zhang <zepu.zhang@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

