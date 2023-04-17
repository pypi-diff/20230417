# Comparing `tmp/pybeef-0.0.1-py3-none-any.whl.zip` & `tmp/pybeef-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,8 @@
-Zip file size: 8034 bytes, number of entries: 11
--rw-r--r--  2.0 unx      184 b- defN 20-Feb-02 00:00 beef/__init__.py
--rw-r--r--  2.0 unx    11888 b- defN 20-Feb-02 00:00 beef/beef.py
--rw-r--r--  2.0 unx      561 b- defN 20-Feb-02 00:00 beef/client.py
--rw-r--r--  2.0 unx     1809 b- defN 20-Feb-02 00:00 beef/pool.py
--rw-r--r--  2.0 unx      750 b- defN 20-Feb-02 00:00 beef/progress.py
--rw-r--r--  2.0 unx      203 b- defN 20-Feb-02 00:00 beef/server.py
--rw-r--r--  2.0 unx      358 b- defN 20-Feb-02 00:00 beef/worker.py
-?rw-r--r--  2.0 unx     1690 b- defN 20-Feb-02 00:00 pybeef-0.0.1.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 pybeef-0.0.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1070 b- defN 20-Feb-02 00:00 pybeef-0.0.1.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      792 b- defN 20-Feb-02 00:00 pybeef-0.0.1.dist-info/RECORD
-11 files, 19392 bytes uncompressed, 6726 bytes compressed:  65.3%
+Zip file size: 5794 bytes, number of entries: 6
+-rw-r--r--  2.0 unx      228 b- defN 20-Feb-02 00:00 beef/__init__.py
+-rw-r--r--  2.0 unx    11950 b- defN 20-Feb-02 00:00 beef/beef.py
+?rw-r--r--  2.0 unx     1721 b- defN 20-Feb-02 00:00 pybeef-0.0.2.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 pybeef-0.0.2.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1070 b- defN 20-Feb-02 00:00 pybeef-0.0.2.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      441 b- defN 20-Feb-02 00:00 pybeef-0.0.2.dist-info/RECORD
+6 files, 15497 bytes uncompressed, 5006 bytes compressed:  67.7%
```

## zipnote {}

```diff
@@ -1,34 +1,19 @@
 Filename: beef/__init__.py
 Comment: 
 
 Filename: beef/beef.py
 Comment: 
 
-Filename: beef/client.py
+Filename: pybeef-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: beef/pool.py
+Filename: pybeef-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: beef/progress.py
+Filename: pybeef-0.0.2.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: beef/server.py
-Comment: 
-
-Filename: beef/worker.py
-Comment: 
-
-Filename: pybeef-0.0.1.dist-info/METADATA
-Comment: 
-
-Filename: pybeef-0.0.1.dist-info/WHEEL
-Comment: 
-
-Filename: pybeef-0.0.1.dist-info/licenses/LICENSE
-Comment: 
-
-Filename: pybeef-0.0.1.dist-info/RECORD
+Filename: pybeef-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## beef/__init__.py

```diff
@@ -1,8 +1,9 @@
-from .beef import beef, State, Status, DEFAULT_REPLY_EXPIRATION_MILLIS, TaskID
+from .beef import beef, State, Status, DEFAULT_REPLY_EXPIRATION_MILLIS, TaskID, TaskNotFoundError
 __all__ = [
     'beef',
     'State',
     'Status',
     'DEFAULT_REPLY_EXPIRATION_MILLIS',
     'TaskID',
+    'TaskNotFoundError',
 ]
```

## beef/beef.py

```diff
@@ -8,14 +8,17 @@
 from typing import Callable, Awaitable, Any, Optional, NoReturn, Tuple, List, Dict
 import aio_pika
 import aiormq
 
 AsyncFunction = Callable[..., Awaitable[Any]]
 TaskID = str
 
+class TaskNotFoundError(RuntimeError):
+    pass
+
 class State(Enum):
     def __new__(cls, value, is_final=False):
         self = object.__new__(cls)
         self._value_ = value
         self._name_ = value
         self.is_final = is_final
         return self
@@ -122,15 +125,15 @@
             await self._set_status(channel, Status.progress(task_id=task_id, steps=0, progress=-1))
             await channel.default_exchange.publish(
                 _work_request_to_message(task_id, *av, **kw),
                 routing_key=self.name,
             )
             return task_id
 
-    async def get_status(self, task_id: Optional[TaskID] = None) -> Status:
+    async def get_status(self, *, task_id: Optional[TaskID] = None) -> Status:
         '''
         Get status of a task (fast)
         '''
         if task_id is None:
             task_id = self._get_task_id()
 
         async with self._acquire_channel() as channel, self._acquire_reply_queue(channel, task_id) as queue:
@@ -144,15 +147,15 @@
                 last = msg
                 if msg.headers.get('x-state') in FINAL_STATES:
                     break
             else:
                 raise RuntimeError('fast forward limit exceeded')
 
             if last is None:
-                raise RuntimeError(f'task {task_id} not found')
+                raise TaskNotFoundError(f'task {task_id} not found')
 
             return _message_to_status(last)
 
     async def set_progress(self, *, task_id: Optional[TaskID] = None, steps: int, progress: int = 0, message: Optional[str] = None) -> None:
         '''
         Set progress of a task.
 
@@ -261,15 +264,15 @@
     @contextlib.asynccontextmanager
     async def _acquire_reply_queue(self, channel: aio_pika.abc.AbstractRobustChannel, task_id: TaskID) -> aio_pika.abc.AbstractQueue:
         await channel.set_qos(prefetch_count=1000)
         try:
             queue = await channel.declare_queue(task_id, passive=True)
             yield queue
         except aiormq.exceptions.ChannelNotFoundEntity as e:
-            raise RuntimeError(f'Task "{task_id}" not found')
+            raise TaskNotFoundError(f'Task "{task_id}" not found')
 
     def _get_task_id(self) -> TaskID:
         task_id = self._task_id.get(None)
         if task_id is None:
             raise RuntimeError('Could not find task_id in the context. You can only omit task_id parameter when calling this method from worker function.')
         return task_id
```

## Comparing `pybeef-0.0.1.dist-info/METADATA` & `pybeef-0.0.2.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: pybeef
-Version: 0.0.1
+Version: 0.0.2
 Summary: Opinionated distributed RPC using AMQP workers
 Project-URL: Homepage, https://github.com/innodatalabs/beef
 Project-URL: Bug Tracker, https://github.com/pypa/innodatalabs/beef
 Author-email: Mike Kroutikov <mkroutikov@innodata.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
+Requires-Dist: aio-pika~=9.0.5
 Description-Content-Type: text/markdown
 
 # beef
 
 Beef is good for your health.
 
 ## Usage
```

## Comparing `pybeef-0.0.1.dist-info/licenses/LICENSE` & `pybeef-0.0.2.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

