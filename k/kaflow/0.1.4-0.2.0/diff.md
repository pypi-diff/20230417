# Comparing `tmp/kaflow-0.1.4.tar.gz` & `tmp/kaflow-0.2.0.tar.gz`

## Comparing `kaflow-0.1.4.tar` & `kaflow-0.2.0.tar`

### file list

```diff
@@ -1,36 +1,38 @@
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 kaflow-0.1.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 kaflow-0.1.4/Makefile
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 kaflow-0.1.4/.github/workflows/release.yaml
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 kaflow-0.1.4/.github/workflows/test.yaml
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 kaflow-0.1.4/kaflow/__init__.py
--rw-r--r--   0        0        0     8453 2020-02-02 00:00:00.000000 kaflow-0.1.4/kaflow/_consumer.py
--rw-r--r--   0        0        0    21898 2020-02-02 00:00:00.000000 kaflow-0.1.4/kaflow/applications.py
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 kaflow-0.1.4/kaflow/dependencies.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 kaflow-0.1.4/kaflow/exceptions.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 kaflow-0.1.4/kaflow/logger.py
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 kaflow-0.1.4/kaflow/message.py
--rw-r--r--   0        0        0     7648 2020-02-02 00:00:00.000000 kaflow-0.1.4/kaflow/parameters.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.1.4/kaflow/py.typed
--rw-r--r--   0        0        0     3317 2020-02-02 00:00:00.000000 kaflow-0.1.4/kaflow/serializers.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 kaflow-0.1.4/kaflow/typing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.1.4/kaflow/_utils/__init__.py
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 kaflow-0.1.4/kaflow/_utils/asyncio.py
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 kaflow-0.1.4/kaflow/_utils/inspect.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.1.4/kaflow/asyncapi/__init__.py
--rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 kaflow-0.1.4/kaflow/asyncapi/_builder.py
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 kaflow-0.1.4/kaflow/asyncapi/docs.py
--rw-r--r--   0        0        0     9688 2020-02-02 00:00:00.000000 kaflow-0.1.4/kaflow/asyncapi/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.1.4/tests/__init__.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 kaflow-0.1.4/tests/key_value.proto
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 kaflow-0.1.4/tests/key_value_pb2.py
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 kaflow-0.1.4/tests/key_value_pb2.pyi
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 kaflow-0.1.4/tests/test_application.py
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 kaflow-0.1.4/tests/test_serializers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.1.4/tests/_utils/__init__.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 kaflow-0.1.4/tests/_utils/test_asyncio.py
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 kaflow-0.1.4/tests/_utils/test_inspect.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 kaflow-0.1.4/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 kaflow-0.1.4/LICENSE
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 kaflow-0.1.4/README.md
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 kaflow-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3323 2020-02-02 00:00:00.000000 kaflow-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 kaflow-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 kaflow-0.2.0/Makefile
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 kaflow-0.2.0/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 kaflow-0.2.0/.github/workflows/test.yaml
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 kaflow-0.2.0/kaflow/__init__.py
+-rw-r--r--   0        0        0     8562 2020-02-02 00:00:00.000000 kaflow-0.2.0/kaflow/_consumer.py
+-rw-r--r--   0        0        0    22216 2020-02-02 00:00:00.000000 kaflow-0.2.0/kaflow/applications.py
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 kaflow-0.2.0/kaflow/dependencies.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 kaflow-0.2.0/kaflow/exceptions.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 kaflow-0.2.0/kaflow/logger.py
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 kaflow-0.2.0/kaflow/message.py
+-rw-r--r--   0        0        0     7648 2020-02-02 00:00:00.000000 kaflow-0.2.0/kaflow/parameters.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.2.0/kaflow/py.typed
+-rw-r--r--   0        0        0     3317 2020-02-02 00:00:00.000000 kaflow-0.2.0/kaflow/serializers.py
+-rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 kaflow-0.2.0/kaflow/testclient.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 kaflow-0.2.0/kaflow/typing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.2.0/kaflow/_utils/__init__.py
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 kaflow-0.2.0/kaflow/_utils/asyncio.py
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 kaflow-0.2.0/kaflow/_utils/inspect.py
+-rw-r--r--   0        0        0     2351 2020-02-02 00:00:00.000000 kaflow-0.2.0/kaflow/_utils/overrides.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.2.0/kaflow/asyncapi/__init__.py
+-rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 kaflow-0.2.0/kaflow/asyncapi/_builder.py
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 kaflow-0.2.0/kaflow/asyncapi/docs.py
+-rw-r--r--   0        0        0     9688 2020-02-02 00:00:00.000000 kaflow-0.2.0/kaflow/asyncapi/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 kaflow-0.2.0/tests/key_value.proto
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 kaflow-0.2.0/tests/key_value_pb2.py
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 kaflow-0.2.0/tests/key_value_pb2.pyi
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 kaflow-0.2.0/tests/test_application.py
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 kaflow-0.2.0/tests/test_serializers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.2.0/tests/_utils/__init__.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 kaflow-0.2.0/tests/_utils/test_asyncio.py
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 kaflow-0.2.0/tests/_utils/test_inspect.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 kaflow-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 kaflow-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 kaflow-0.2.0/README.md
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 kaflow-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3813 2020-02-02 00:00:00.000000 kaflow-0.2.0/PKG-INFO
```

### Comparing `kaflow-0.1.4/.github/workflows/release.yaml` & `kaflow-0.2.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.4/.github/workflows/test.yaml` & `kaflow-0.2.0/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.4/kaflow/__init__.py` & `kaflow-0.2.0/kaflow/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -31,8 +31,8 @@
     __all__.append("Avro")
 
 if has_protobuf:
     from kaflow.serializers import Protobuf  # noqa: F401
 
     __all__.append("Protobuf")
 
-__version__ = "0.1.4"
+__version__ = "0.2.0"
```

### Comparing `kaflow-0.1.4/kaflow/_consumer.py` & `kaflow-0.2.0/kaflow/_consumer.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,24 +40,24 @@
 class TopicConsumerFunc:
     __slots__ = (
         "name",
         "container",
         "publish_fn",
         "exception_handlers",
         "deserialization_error_handler",
-        "dependent",
         "func",
         "value_param_type",
         "value_deserializer",
         "key_param_type",
         "key_deserializer",
         "headers_type_deserializers",
         "sink_topics",
         "executor",
         "container_state",
+        "dependent",
     )
 
     def __init__(
         self,
         *,
         name: str,
         container: Container,
@@ -86,27 +86,28 @@
         sink_topics: Sequence[str] | None = None,
     ) -> None:
         self.name = name
         self.container = container
         self.publish_fn = publish_fn
         self.exception_handlers = exception_handlers
         self.deserialization_error_handler = deserialization_error_handler
-        self.dependent = self.container.solve(
-            Dependent(func, scope="consumer"), scopes=Scopes
-        )
+        self.func = func
         self.value_param_type = value_param_type
         self.value_deserializer = value_deserializer
         self.key_param_type = key_param_type
         self.key_deserializer = key_deserializer
         self.headers_type_deserializers = headers_type_deserializers
         self.sink_topics = sink_topics
         self.executor = AsyncExecutor()
 
     def prepare(self, state: ScopeState) -> None:
         self.container_state = state
+        self.dependent = self.container.solve(
+            Dependent(self.func, scope="consumer"), scopes=Scopes
+        )
 
     def _deserialize_value(self, value: bytes) -> TopicValueKeyHeader:
         return _deserialize(value, self.value_param_type, self.value_deserializer)
 
     def _deserialize_key(self, key: bytes) -> TopicValueKeyHeader | None:
         if self.key_param_type:
             return _deserialize(key, self.key_param_type, self.key_deserializer)
@@ -226,30 +227,32 @@
                         message.partition,
                         message.offset,
                     )
                     for topic in self.sink_topics
                 ]
             )
 
-    async def _process(self, read_message: ReadMessage) -> None:
+    async def _process(self, read_message: ReadMessage) -> Message | None:
         async with self.container.enter_scope(
             "consumer", state=self.container_state
         ) as consumer_state:
             message = await self._execute_dependent(
                 consumer_state=consumer_state, message=read_message
             )
         if message and isinstance(message, Message):
             await self._publish_messages(message)
+            return message
+        return None
 
-    async def consume(self, record: ConsumerRecord) -> None:
+    async def consume(self, record: ConsumerRecord) -> Message | None:
         value, key, headers, deserialized = await self._deserialize(record)
         if not deserialized:
-            return
+            return None
         message = ReadMessage(
             value=value,
             key=key,
             headers=headers,
             offset=record.offset,
             partition=record.partition,
             timestamp=record.timestamp,
         )
-        await self._process(read_message=message)
+        return await self._process(read_message=message)
```

### Comparing `kaflow-0.1.4/kaflow/applications.py` & `kaflow-0.2.0/kaflow/applications.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from kafka.coordinator.assignors.roundrobin import RoundRobinPartitionAssignor
 from kafka.partitioner.default import DefaultPartitioner
 
 from kaflow import parameters
 from kaflow._consumer import TopicConsumerFunc
 from kaflow._utils.asyncio import asyncify
 from kaflow._utils.inspect import is_not_coroutine_function
+from kaflow._utils.overrides import DependencyOverrideManager
 from kaflow.dependencies import Scopes
 from kaflow.exceptions import KaflowDeserializationException
 from kaflow.message import Message
 
 if TYPE_CHECKING:
     from aiokafka.abc import AbstractTokenProvider
     from kafka.coordinator.assignors.abstract import AbstractPartitionAssignor
@@ -193,14 +194,15 @@
         self.contact = contact
         self.license_info = license_info
         self.asyncapi_schema: AsyncAPI | None = None
 
         # di
         self._container = Container()
         self._container_state = ScopeState()
+        self.dependency_overrides = DependencyOverrideManager(self._container)
 
         self._loop = asyncio.get_event_loop()
         self._consumer: AIOKafkaConsumer | None = None
         self._producer: AIOKafkaProducer | None = None
 
         self._consumers: dict[str, TopicConsumerFunc] = {}
         self._producers: dict[str, list[ProducerFunc]] = defaultdict(list)
@@ -256,15 +258,15 @@
         ]
         | None = None,
         sink_topics: Sequence[str] | None = None,
     ) -> None:
         topic_processor = TopicConsumerFunc(
             name=topic,
             container=self._container,
-            publish_fn=self._publish,
+            publish_fn=lambda *args, **kwargs: self._publish(*args, **kwargs),
             exception_handlers=self._exception_handlers,
             deserialization_error_handler=self._deserialization_error_handler,
             func=func,
             value_param_type=value_param_type,
             value_deserializer=value_deserializer,
             key_param_type=key_param_type,
             key_deserializer=key_deserializer,
@@ -483,23 +485,27 @@
             value=value,
             key=key,
             partition=partition,
             timestamp_ms=timestamp,
             headers=headers_,
         )
 
+    def _get_consumer(self, topic: str) -> TopicConsumerFunc:
+        return self._consumers[topic]
+
     async def _consuming_loop(self) -> None:
         if not self._consumer:
             raise RuntimeError(
                 "The consumer has not been started yet. You're probably seeing this"
                 f" error because `{self.__class__.__name__}.start` method has not been"
                 " called yet."
             )
         async for record in self._consumer:
-            await self._consumers[record.topic].consume(record=record)
+            consumer = self._get_consumer(record.topic)
+            await consumer.consume(record=record)
 
     async def start(self) -> None:
         self._consumer = self._create_consumer()
         self._producer = self._create_producer()
 
         async with self.lifespan():
             await self._consumer.start()
```

### Comparing `kaflow-0.1.4/kaflow/message.py` & `kaflow-0.2.0/kaflow/message.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.4/kaflow/parameters.py` & `kaflow-0.2.0/kaflow/parameters.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.4/kaflow/serializers.py` & `kaflow-0.2.0/kaflow/serializers.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.4/kaflow/_utils/asyncio.py` & `kaflow-0.2.0/kaflow/_utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.4/kaflow/_utils/inspect.py` & `kaflow-0.2.0/kaflow/_utils/inspect.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.4/kaflow/asyncapi/_builder.py` & `kaflow-0.2.0/kaflow/asyncapi/_builder.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.4/kaflow/asyncapi/docs.py` & `kaflow-0.2.0/kaflow/asyncapi/docs.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.4/kaflow/asyncapi/models.py` & `kaflow-0.2.0/kaflow/asyncapi/models.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.4/tests/key_value_pb2.py` & `kaflow-0.2.0/tests/key_value_pb2.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.4/tests/test_serializers.py` & `kaflow-0.2.0/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.4/tests/_utils/test_inspect.py` & `kaflow-0.2.0/tests/_utils/test_inspect.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.4/.gitignore` & `kaflow-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.4/LICENSE` & `kaflow-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.4/pyproject.toml` & `kaflow-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.4/PKG-INFO` & `kaflow-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaflow
-Version: 0.1.4
+Version: 0.2.0
 Summary: Python Stream processing backed by Apache Kafka.
 Project-URL: Documentation, https://github.com/gabrielmbmb/kaflow#readme
 Project-URL: Issues, https://github.com/gabrielmbmb/kaflow/issues
 Project-URL: Source, https://github.com/gabrielmbmb/kaflow
 Author-email: Gabriel Martin Blazquez <gmartinbdev@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -72,28 +72,55 @@
 ```shell
 pip install kaflow
 ```
 
 ## Example
 
 ```python
-from kaflow import Json, Kaflow
+from kaflow import (
+    FromHeader,
+    FromKey,
+    FromValue,
+    Json,
+    Kaflow,
+    Message,
+    MessageOffset,
+    MessagePartition,
+    MessageTimestamp,
+    String,
+)
 from pydantic import BaseModel
 
 
 class UserClick(BaseModel):
     user_id: int
     url: str
     timestamp: int
 
 
+class Key(BaseModel):
+    environment: str
+
+
 app = Kaflow(name="AwesomeKakfaApp", brokers="localhost:9092")
 
 
-@app.consume(topic="user_clicks", sink_topics=("user_clicks_json",))
-async def consume_user_clicks(message: Json[UserClick]) -> Json[UserClick]:
-    print("user click", message)
-    return message
+@app.consume(topic="user_clicks", sink_topics=["user_clicks_json"])
+async def consume_user_clicks(
+    message: FromValue[Json[UserClick]],
+    key: FromKey[Json[Key]],
+    x_correlation_id: FromHeader[String[str]],
+    x_request_id: FromHeader[String[str]],
+    partition: MessagePartition,
+    offset: MessageOffset,
+    timestamp: MessageTimestamp,
+) -> Message:
+    # Do something with the message
+    ...
+
+    # Publish to another topic
+    return Message(value=b'{"user_clicked": "true"}')
 
 
 app.run()
+
 ```
```

