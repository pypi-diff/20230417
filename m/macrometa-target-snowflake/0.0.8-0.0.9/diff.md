# Comparing `tmp/macrometa-target-snowflake-0.0.8.tar.gz` & `tmp/macrometa-target-snowflake-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-target-snowflake-0.0.8.tar", last modified: Sat Apr  1 09:37:24 2023, max compression
+gzip compressed data, was "macrometa-target-snowflake-0.0.9.tar", last modified: Sun Apr  2 07:28:35 2023, max compression
```

## Comparing `macrometa-target-snowflake-0.0.8.tar` & `macrometa-target-snowflake-0.0.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 09:37:24.543623 macrometa-target-snowflake-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    10409 2023-04-01 09:37:07.000000 macrometa-target-snowflake-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23555 2023-04-01 09:37:24.543623 macrometa-target-snowflake-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22964 2023-04-01 09:37:07.000000 macrometa-target-snowflake-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 09:37:24.539623 macrometa-target-snowflake-0.0.8/macrometa_target_snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)    28280 2023-04-01 09:37:07.000000 macrometa-target-snowflake-0.0.8/macrometa_target_snowflake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38365 2023-04-01 09:37:07.000000 macrometa-target-snowflake-0.0.8/macrometa_target_snowflake/db_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-01 09:37:07.000000 macrometa-target-snowflake-0.0.8/macrometa_target_snowflake/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-04-01 09:37:07.000000 macrometa-target-snowflake-0.0.8/macrometa_target_snowflake/file_format.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 09:37:24.543623 macrometa-target-snowflake-0.0.8/macrometa_target_snowflake/file_formats/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 09:37:07.000000 macrometa-target-snowflake-0.0.8/macrometa_target_snowflake/file_formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-04-01 09:37:07.000000 macrometa-target-snowflake-0.0.8/macrometa_target_snowflake/file_formats/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-04-01 09:37:07.000000 macrometa-target-snowflake-0.0.8/macrometa_target_snowflake/file_formats/parquet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-04-01 09:37:07.000000 macrometa-target-snowflake-0.0.8/macrometa_target_snowflake/flattening.py
--rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-04-01 09:37:07.000000 macrometa-target-snowflake-0.0.8/macrometa_target_snowflake/stream_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 09:37:24.543623 macrometa-target-snowflake-0.0.8/macrometa_target_snowflake/upload_clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 09:37:07.000000 macrometa-target-snowflake-0.0.8/macrometa_target_snowflake/upload_clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-01 09:37:07.000000 macrometa-target-snowflake-0.0.8/macrometa_target_snowflake/upload_clients/base_upload_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-04-01 09:37:07.000000 macrometa-target-snowflake-0.0.8/macrometa_target_snowflake/upload_clients/s3_upload_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-04-01 09:37:07.000000 macrometa-target-snowflake-0.0.8/macrometa_target_snowflake/upload_clients/snowflake_upload_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 09:37:24.543623 macrometa-target-snowflake-0.0.8/macrometa_target_snowflake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23555 2023-04-01 09:37:24.000000 macrometa-target-snowflake-0.0.8/macrometa_target_snowflake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-01 09:37:24.000000 macrometa-target-snowflake-0.0.8/macrometa_target_snowflake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-01 09:37:24.000000 macrometa-target-snowflake-0.0.8/macrometa_target_snowflake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-01 09:37:24.000000 macrometa-target-snowflake-0.0.8/macrometa_target_snowflake.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-01 09:37:24.000000 macrometa-target-snowflake-0.0.8/macrometa_target_snowflake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-01 09:37:24.000000 macrometa-target-snowflake-0.0.8/macrometa_target_snowflake.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-01 09:37:24.543623 macrometa-target-snowflake-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-04-01 09:37:07.000000 macrometa-target-snowflake-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 07:28:35.115972 macrometa-target-snowflake-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    10409 2023-04-02 07:28:16.000000 macrometa-target-snowflake-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23555 2023-04-02 07:28:35.111972 macrometa-target-snowflake-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22964 2023-04-02 07:28:16.000000 macrometa-target-snowflake-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 07:28:35.111972 macrometa-target-snowflake-0.0.9/macrometa_target_snowflake/
+-rw-r--r--   0 runner    (1001) docker     (123)    29414 2023-04-02 07:28:16.000000 macrometa-target-snowflake-0.0.9/macrometa_target_snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38365 2023-04-02 07:28:16.000000 macrometa-target-snowflake-0.0.9/macrometa_target_snowflake/db_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-02 07:28:16.000000 macrometa-target-snowflake-0.0.9/macrometa_target_snowflake/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-04-02 07:28:16.000000 macrometa-target-snowflake-0.0.9/macrometa_target_snowflake/file_format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 07:28:35.111972 macrometa-target-snowflake-0.0.9/macrometa_target_snowflake/file_formats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 07:28:16.000000 macrometa-target-snowflake-0.0.9/macrometa_target_snowflake/file_formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-04-02 07:28:16.000000 macrometa-target-snowflake-0.0.9/macrometa_target_snowflake/file_formats/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-04-02 07:28:16.000000 macrometa-target-snowflake-0.0.9/macrometa_target_snowflake/file_formats/parquet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-04-02 07:28:16.000000 macrometa-target-snowflake-0.0.9/macrometa_target_snowflake/flattening.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-04-02 07:28:16.000000 macrometa-target-snowflake-0.0.9/macrometa_target_snowflake/stream_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 07:28:35.111972 macrometa-target-snowflake-0.0.9/macrometa_target_snowflake/upload_clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 07:28:16.000000 macrometa-target-snowflake-0.0.9/macrometa_target_snowflake/upload_clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-02 07:28:16.000000 macrometa-target-snowflake-0.0.9/macrometa_target_snowflake/upload_clients/base_upload_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-04-02 07:28:16.000000 macrometa-target-snowflake-0.0.9/macrometa_target_snowflake/upload_clients/s3_upload_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-04-02 07:28:16.000000 macrometa-target-snowflake-0.0.9/macrometa_target_snowflake/upload_clients/snowflake_upload_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 07:28:35.111972 macrometa-target-snowflake-0.0.9/macrometa_target_snowflake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23555 2023-04-02 07:28:35.000000 macrometa-target-snowflake-0.0.9/macrometa_target_snowflake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-02 07:28:35.000000 macrometa-target-snowflake-0.0.9/macrometa_target_snowflake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-02 07:28:35.000000 macrometa-target-snowflake-0.0.9/macrometa_target_snowflake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-02 07:28:35.000000 macrometa-target-snowflake-0.0.9/macrometa_target_snowflake.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-02 07:28:35.000000 macrometa-target-snowflake-0.0.9/macrometa_target_snowflake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-02 07:28:35.000000 macrometa-target-snowflake-0.0.9/macrometa_target_snowflake.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-02 07:28:35.115972 macrometa-target-snowflake-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-04-02 07:28:16.000000 macrometa-target-snowflake-0.0.9/setup.py
```

### Comparing `macrometa-target-snowflake-0.0.8/LICENSE` & `macrometa-target-snowflake-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-target-snowflake-0.0.8/PKG-INFO` & `macrometa-target-snowflake-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-snowflake
-Version: 0.0.8
+Version: 0.0.9
 Summary: Macrometa target for loading data to Snowflake
 Home-page: https://github.com/Macrometacorp/macrometa-target-snowflake
 Author: Macrometa
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `macrometa-target-snowflake-0.0.8/README.md` & `macrometa-target-snowflake-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `macrometa-target-snowflake-0.0.8/macrometa_target_snowflake/__init__.py` & `macrometa-target-snowflake-0.0.9/macrometa_target_snowflake/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 #!/usr/bin/env python3
 
 import argparse
+import asyncio
 import io
 import json
 import logging
 import os
 import sys
 import copy
-import threading
-import time
 
-from typing import Dict, List, Optional
+from asyncio import AbstractEventLoop
+from datetime import datetime
 from joblib import Parallel, delayed, parallel_backend
 from jsonschema import Draft7Validator, FormatChecker
 from singer import get_logger
-from datetime import datetime, timedelta
+from threading import Thread
+from typing import Dict, List, Optional
 
 import pkg_resources
 from c8connector import C8Connector, Sample, ConfigAttributeType, Schema
 from c8connector import ConfigProperty
 
 
 from macrometa_target_snowflake.file_formats import csv
 from macrometa_target_snowflake.file_formats import parquet
 from macrometa_target_snowflake import stream_utils
 
 from macrometa_target_snowflake.db_sync import DbSync
 from macrometa_target_snowflake.file_format import FileFormatTypes
 from macrometa_target_snowflake.exceptions import (
     RecordValidationException,
-    UnexpectedValueTypeException,
     InvalidValidationOperationException
 )
 
 LOGGER = get_logger('macrometa_target_snowflake')
 
 
 DEFAULT_BATCH_SIZE_ROWS = 100000
@@ -84,20 +84,14 @@
 
     # The file format is detected at DbSync init time
     file_format_type = db.file_format.file_format_type
 
     return table_cache, file_format_type
 
 
-def flush_timer(batch_wait_limit_seconds, flush_event):
-    while True:
-        time.sleep(batch_wait_limit_seconds)
-        flush_event.set()
-
-
 # pylint: disable=too-many-locals,too-many-branches,too-many-statements,invalid-name
 def persist_lines(config, lines, table_cache=None, file_format_type: FileFormatTypes = None) -> None:
     """Main loop to read and consume singer messages from stdin
 
     Params:
         config: configuration dictionary
         lines: iterable of singer messages
@@ -118,23 +112,23 @@
     key_properties = {}
     validators = {}
     records_to_load = {}
     row_count = {}
     stream_to_sync = {}
     total_row_count = {}
     batch_size_rows = config.get('batch_size_rows', DEFAULT_BATCH_SIZE_ROWS)
-    batch_wait_limit_seconds = config.get(
-        'batch_wait_limit_seconds', DEFAULT_BATCH_WAIT_TIME)
     archive_load_files = config.get('archive_load_files', False)
     archive_load_files_data = {}
 
-    flush_event = threading.Event()
-    flush_thread = threading.Thread(target=flush_timer, args=(batch_wait_limit_seconds, flush_event))
-    flush_thread.daemon = True
-    flush_thread.start()
+    time_schedule = {
+        'batch_wait_limit_seconds': config.get('batch_wait_limit_seconds', DEFAULT_BATCH_WAIT_TIME),
+        'last_executed_time': datetime.now(),
+    }
+    event_loop = setup_flush_task(time_schedule, records_to_load, row_count, stream_to_sync, config,
+                                  state, flushed_state)
 
     # Loop over lines from stdin
     for line in lines:
         try:
             o = json.loads(line)
         except json.decoder.JSONDecodeError:
             LOGGER.error('Unable to parse:\n%s', line)
@@ -204,25 +198,18 @@
 
                     if min_value is None or min_value > incremental_key_value:
                         stream_archive_load_files_values['min'] = incremental_key_value
 
                     if max_value is None or max_value < incremental_key_value:
                         stream_archive_load_files_values['max'] = incremental_key_value
 
-            flush = False
             if row_count[stream] >= batch_size_rows:
-                flush = True
                 LOGGER.info("Flush triggered by batch_size_rows (%s) reached in %s",
                             batch_size_rows, stream)
-            elif flush_event.is_set():
-                flush = True
-                LOGGER.info("Flush triggered by batch_wait_limit_seconds (%s)",
-                            batch_wait_limit_seconds)
 
-            if flush:
                 # flush all streams, delete records if needed, reset counts and then emit current state
                 if config.get('flush_all_streams'):
                     filter_streams = None
                 else:
                     filter_streams = [stream]
 
                 # Flush and return a new state dict with new positions only for the flushed streams
@@ -232,19 +219,17 @@
                     stream_to_sync,
                     config,
                     state,
                     flushed_state,
                     archive_load_files_data,
                     filter_streams=filter_streams)
 
-                # Reset the flush_event
-                flush_event.clear()
-
                 # emit last encountered state
                 emit_state(copy.deepcopy(flushed_state))
+                time_schedule['last_executed_time'] = datetime.now()
 
         elif t == 'SCHEMA':
             if 'stream' not in o:
                 raise Exception(
                     f"Line is missing required key 'stream': {line}")
 
             stream = o['stream']
@@ -353,17 +338,19 @@
 
     # if some bucket has records that need to be flushed but haven't reached batch size
     # then flush all buckets.
     if sum(row_count.values()) > 0:
         # flush all streams one last time, delete records if needed, reset counts and then emit current state
         flushed_state = flush_streams(records_to_load, row_count, stream_to_sync, config, state, flushed_state,
                                       archive_load_files_data)
+        time_schedule['last_executed_time'] = datetime.now()
 
     # emit latest state
     emit_state(copy.deepcopy(flushed_state))
+    event_loop.stop()
 
 
 # pylint: disable=too-many-arguments
 def flush_streams(
         streams,
         row_count,
         stream_to_sync,
@@ -533,14 +520,45 @@
 
         db_sync.copy_to_archive(s3_key, archive_key, archive_metadata)
 
     # Delete file from S3
     db_sync.delete_from_stage(stream, s3_key)
 
 
+def setup_flush_task(time_schedule, streams, row_count, stream_to_sync, config, state, flushed_state,
+                     filter_streams=None) -> AbstractEventLoop:
+    event_loop = asyncio.new_event_loop()
+    Thread(target=start_background_loop, args=(event_loop,), daemon=True).start()
+    asyncio.run_coroutine_threadsafe(
+        flush_task(time_schedule, streams, row_count, stream_to_sync, config, state, flushed_state, filter_streams),
+        event_loop)
+    return event_loop
+
+
+async def flush_task(time_schedule, streams, row_count, stream_to_sync, config, state, flushed_state,
+                     filter_streams=None) -> None:
+    while True:
+        timedelta = datetime.now() - time_schedule['last_executed_time']
+        if (
+            timedelta.total_seconds() >= time_schedule['batch_wait_limit_seconds']
+            and sum(row_count.values()) > 0
+        ):
+            # flush all streams one last time, delete records if needed, reset counts and then emit current state.
+            flushed_state = flush_streams(streams, row_count, stream_to_sync, config, state, flushed_state,
+                                          filter_streams)
+            # emit latest state
+            emit_state(copy.deepcopy(flushed_state))
+            time_schedule['last_executed_time'] = datetime.now()
+
+
+def start_background_loop(loop: asyncio.AbstractEventLoop) -> None:
+    asyncio.set_event_loop(loop)
+    loop.run_forever()
+
+
 class SnowflakeTargetConnector(C8Connector):
     """SnowflakeTargetConnector's C8Connector impl."""
 
     def name(self) -> str:
         """Returns the name of the connector."""
         return "Snowflake"
```

### Comparing `macrometa-target-snowflake-0.0.8/macrometa_target_snowflake/db_sync.py` & `macrometa-target-snowflake-0.0.9/macrometa_target_snowflake/db_sync.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-snowflake-0.0.8/macrometa_target_snowflake/exceptions.py` & `macrometa-target-snowflake-0.0.9/macrometa_target_snowflake/exceptions.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-snowflake-0.0.8/macrometa_target_snowflake/file_format.py` & `macrometa-target-snowflake-0.0.9/macrometa_target_snowflake/file_format.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-snowflake-0.0.8/macrometa_target_snowflake/file_formats/csv.py` & `macrometa-target-snowflake-0.0.9/macrometa_target_snowflake/file_formats/csv.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-snowflake-0.0.8/macrometa_target_snowflake/file_formats/parquet.py` & `macrometa-target-snowflake-0.0.9/macrometa_target_snowflake/file_formats/parquet.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-snowflake-0.0.8/macrometa_target_snowflake/flattening.py` & `macrometa-target-snowflake-0.0.9/macrometa_target_snowflake/flattening.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-snowflake-0.0.8/macrometa_target_snowflake/stream_utils.py` & `macrometa-target-snowflake-0.0.9/macrometa_target_snowflake/stream_utils.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-snowflake-0.0.8/macrometa_target_snowflake/upload_clients/base_upload_client.py` & `macrometa-target-snowflake-0.0.9/macrometa_target_snowflake/upload_clients/base_upload_client.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-snowflake-0.0.8/macrometa_target_snowflake/upload_clients/s3_upload_client.py` & `macrometa-target-snowflake-0.0.9/macrometa_target_snowflake/upload_clients/s3_upload_client.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-snowflake-0.0.8/macrometa_target_snowflake/upload_clients/snowflake_upload_client.py` & `macrometa-target-snowflake-0.0.9/macrometa_target_snowflake/upload_clients/snowflake_upload_client.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-snowflake-0.0.8/macrometa_target_snowflake.egg-info/PKG-INFO` & `macrometa-target-snowflake-0.0.9/macrometa_target_snowflake.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-snowflake
-Version: 0.0.8
+Version: 0.0.9
 Summary: Macrometa target for loading data to Snowflake
 Home-page: https://github.com/Macrometacorp/macrometa-target-snowflake
 Author: Macrometa
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `macrometa-target-snowflake-0.0.8/macrometa_target_snowflake.egg-info/SOURCES.txt` & `macrometa-target-snowflake-0.0.9/macrometa_target_snowflake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `macrometa-target-snowflake-0.0.8/setup.py` & `macrometa-target-snowflake-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(name="macrometa-target-snowflake",
-      version='0.0.8',
+      version='0.0.9',
       description="Macrometa target for loading data to Snowflake",
       long_description=long_description,
       long_description_content_type='text/markdown',
       author="Macrometa",
       url='https://github.com/Macrometacorp/macrometa-target-snowflake',
       classifiers=[
           'License :: OSI Approved :: Apache Software License',
```

