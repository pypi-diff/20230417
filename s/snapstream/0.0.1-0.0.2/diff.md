# Comparing `tmp/snapstream-0.0.1.tar.gz` & `tmp/snapstream-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snapstream-0.0.1.tar", max compression
+gzip compressed data, was "snapstream-0.0.2.tar", max compression
```

## Comparing `snapstream-0.0.1.tar` & `snapstream-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1065 2023-04-13 20:05:46.184868 snapstream-0.0.1/LICENSE
--rw-r--r--   0        0        0     2064 2023-04-13 20:05:46.184868 snapstream-0.0.1/README.md
--rw-r--r--   0        0        0     1265 2023-04-13 20:06:00.020870 snapstream-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1673 2023-04-13 20:05:46.188869 snapstream-0.0.1/snapstream/__init__.py
--rw-r--r--   0        0        0     9660 2023-04-13 20:05:46.188869 snapstream-0.0.1/snapstream/caching.py
--rw-r--r--   0        0        0     2538 2023-04-13 20:05:46.188869 snapstream-0.0.1/snapstream/codecs.py
--rw-r--r--   0        0        0     8396 2023-04-13 20:05:46.188869 snapstream-0.0.1/snapstream/core.py
--rw-r--r--   0        0        0     1033 2023-04-13 20:05:46.188869 snapstream-0.0.1/snapstream/utils.py
--rw-r--r--   0        0        0     3214 1970-01-01 00:00:00.000000 snapstream-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-17 13:31:07.558570 snapstream-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2064 2023-04-17 13:31:07.558570 snapstream-0.0.2/README.md
+-rw-r--r--   0        0        0     1265 2023-04-17 13:31:20.466662 snapstream-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1673 2023-04-17 13:31:07.562570 snapstream-0.0.2/snapstream/__init__.py
+-rw-r--r--   0        0        0     9660 2023-04-17 13:31:07.562570 snapstream-0.0.2/snapstream/caching.py
+-rw-r--r--   0        0        0     2538 2023-04-17 13:31:07.562570 snapstream-0.0.2/snapstream/codecs.py
+-rw-r--r--   0        0        0     8531 2023-04-17 13:31:07.562570 snapstream-0.0.2/snapstream/core.py
+-rw-r--r--   0        0        0     1033 2023-04-17 13:31:07.562570 snapstream-0.0.2/snapstream/utils.py
+-rw-r--r--   0        0        0     3214 1970-01-01 00:00:00.000000 snapstream-0.0.2/PKG-INFO
```

### Comparing `snapstream-0.0.1/LICENSE` & `snapstream-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `snapstream-0.0.1/README.md` & `snapstream-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `snapstream-0.0.1/pyproject.toml` & `snapstream-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "snapstream"
-version = "0.0.1"
+version = "0.0.2"
 description = "Streamline your Kafka data processing, this tool aims to standardize streaming data from multiple Kafka clusters. With a pub-sub approach, multiple functions can easily subscribe to incoming messages, serialization can be specified per topic, and data is automatically processed by data sink functions."
 authors = ["Menziess <stefan_schenk@hotmail.com>"]
 readme = "README.md"
 repository = "https://github.com/Menziess/snapstream"
 license = "MIT"
 keywords = ["kafka", "pubsub"]
```

### Comparing `snapstream-0.0.1/snapstream/__init__.py` & `snapstream-0.0.2/snapstream/__init__.py`

 * *Files identical despite different names*

### Comparing `snapstream-0.0.1/snapstream/caching.py` & `snapstream-0.0.2/snapstream/caching.py`

 * *Files identical despite different names*

### Comparing `snapstream-0.0.1/snapstream/codecs.py` & `snapstream-0.0.2/snapstream/codecs.py`

 * *Files identical despite different names*

### Comparing `snapstream-0.0.1/snapstream/core.py` & `snapstream-0.0.2/snapstream/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -236,24 +236,28 @@
         self,
         name: str,
         conf: dict = {},
         offset: Optional[int] = None,
         codec: Optional[ICodec] = None,
         flush_timeout: float = -1.0,
         poll_timeout: float = 1.0,
+        callback=_producer_handler,
+        poller=_consumer_handler,
         dry: bool = False
     ) -> None:
         """Pass topic related configuration."""
         c = Conf()
         self.name = name
         self.conf = {**c.conf, **conf}
         self.starting_offset = offset
         self.flush_timeout = flush_timeout
         self.poll_timeout = poll_timeout
         self.producer = None
+        self.callback = callback
+        self.poller = poller
         self.codec = codec
         self.dry = dry
 
     def create_topic(self, *args, **kwargs) -> None:
         """Create topic."""
         admin = AdminClient(self.conf)
         for t, f in admin.create_topics([NewTopic(self.name, *args, **kwargs)]).items():
@@ -265,22 +269,21 @@
                     logger.warning(e)
                 else:
                     logger.error(e)
                     raise
 
     def __iter__(self) -> Iterator[Any]:
         """Consume from topic."""
-        c = get_consumer(self.name, self.conf, self.starting_offset,
-                         self.codec, self.poll_timeout)
+        c = get_consumer(self.name, self.conf, self.starting_offset, self.codec, self.poll_timeout, self.poller)
         with c as consumer:
             for msg in consumer:
                 yield msg
 
     def __call__(self, val, key=None, *args, **kwargs) -> None:
         """Produce to topic."""
         if not (key or val):
             return
         self.producer = (
             self.producer or
-            get_producer(self.name, self.conf, self.dry, self.codec, self.flush_timeout).__enter__()
+            get_producer(self.name, self.conf, self.dry, self.codec, self.flush_timeout, self.callback).__enter__()
         )
         self.producer(key, val, *args, **kwargs)
```

### Comparing `snapstream-0.0.1/snapstream/utils.py` & `snapstream-0.0.2/snapstream/utils.py`

 * *Files identical despite different names*

### Comparing `snapstream-0.0.1/PKG-INFO` & `snapstream-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snapstream
-Version: 0.0.1
+Version: 0.0.2
 Summary: Streamline your Kafka data processing, this tool aims to standardize streaming data from multiple Kafka clusters. With a pub-sub approach, multiple functions can easily subscribe to incoming messages, serialization can be specified per topic, and data is automatically processed by data sink functions.
 Home-page: https://github.com/Menziess/snapstream
 License: MIT
 Keywords: kafka,pubsub
 Author: Menziess
 Author-email: stefan_schenk@hotmail.com
 Requires-Python: >=3.8.1,<4.0.0
```

