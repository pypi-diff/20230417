# Comparing `tmp/redis_simple_orm-1.2.4.tar.gz` & `tmp/redis_simple_orm-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis_simple_orm-1.2.4.tar", last modified: Wed Sep 28 18:33:37 2022, max compression
+gzip compressed data, was "redis_simple_orm-1.2.5.tar", last modified: Mon Apr 17 03:49:35 2023, max compression
```

## Comparing `redis_simple_orm-1.2.4.tar` & `redis_simple_orm-1.2.5.tar`

### file list

```diff
@@ -1,26 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 18:33:37.546424 redis_simple_orm-1.2.4/
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-09-28 18:33:25.000000 redis_simple_orm-1.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-09-28 18:33:25.000000 redis_simple_orm-1.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    11345 2022-09-28 18:33:37.546424 redis_simple_orm-1.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    10538 2022-09-28 18:33:25.000000 redis_simple_orm-1.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 18:33:37.542424 redis_simple_orm-1.2.4/RSO/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-09-28 18:33:25.000000 redis_simple_orm-1.2.4/RSO/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 18:33:37.542424 redis_simple_orm-1.2.4/RSO/aioredis/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-28 18:33:25.000000 redis_simple_orm-1.2.4/RSO/aioredis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6013 2022-09-28 18:33:25.000000 redis_simple_orm-1.2.4/RSO/aioredis/index.py
--rw-r--r--   0 runner    (1001) docker     (121)     4108 2022-09-28 18:33:25.000000 redis_simple_orm-1.2.4/RSO/aioredis/model.py
--rw-r--r--   0 runner    (1001) docker     (121)     2502 2022-09-28 18:33:25.000000 redis_simple_orm-1.2.4/RSO/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     5040 2022-09-28 18:33:25.000000 redis_simple_orm-1.2.4/RSO/index.py
--rw-r--r--   0 runner    (1001) docker     (121)     1509 2022-09-28 18:33:25.000000 redis_simple_orm-1.2.4/RSO/model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 18:33:37.542424 redis_simple_orm-1.2.4/RSO/txredisapi/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-28 18:33:25.000000 redis_simple_orm-1.2.4/RSO/txredisapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6516 2022-09-28 18:33:25.000000 redis_simple_orm-1.2.4/RSO/txredisapi/index.py
--rw-r--r--   0 runner    (1001) docker     (121)     3562 2022-09-28 18:33:25.000000 redis_simple_orm-1.2.4/RSO/txredisapi/model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 18:33:37.546424 redis_simple_orm-1.2.4/redis_simple_orm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    11345 2022-09-28 18:33:37.000000 redis_simple_orm-1.2.4/redis_simple_orm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      445 2022-09-28 18:33:37.000000 redis_simple_orm-1.2.4/redis_simple_orm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-28 18:33:37.000000 redis_simple_orm-1.2.4/redis_simple_orm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-09-28 18:33:37.000000 redis_simple_orm-1.2.4/redis_simple_orm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-09-28 18:33:37.000000 redis_simple_orm-1.2.4/redis_simple_orm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-09-28 18:33:37.546424 redis_simple_orm-1.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1953 2022-09-28 18:33:25.000000 redis_simple_orm-1.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:49:35.185098 redis_simple_orm-1.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-17 03:49:21.000000 redis_simple_orm-1.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-17 03:49:21.000000 redis_simple_orm-1.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11467 2023-04-17 03:49:35.185098 redis_simple_orm-1.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10660 2023-04-17 03:49:21.000000 redis_simple_orm-1.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:49:35.177098 redis_simple_orm-1.2.5/RSO/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-17 03:49:21.000000 redis_simple_orm-1.2.5/RSO/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:49:35.181098 redis_simple_orm-1.2.5/RSO/aioredis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 03:49:21.000000 redis_simple_orm-1.2.5/RSO/aioredis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5996 2023-04-17 03:49:21.000000 redis_simple_orm-1.2.5/RSO/aioredis/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-04-17 03:49:21.000000 redis_simple_orm-1.2.5/RSO/aioredis/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-04-17 03:49:21.000000 redis_simple_orm-1.2.5/RSO/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-04-17 03:49:21.000000 redis_simple_orm-1.2.5/RSO/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-04-17 03:49:21.000000 redis_simple_orm-1.2.5/RSO/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:49:35.181098 redis_simple_orm-1.2.5/RSO/txredisapi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 03:49:21.000000 redis_simple_orm-1.2.5/RSO/txredisapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6499 2023-04-17 03:49:21.000000 redis_simple_orm-1.2.5/RSO/txredisapi/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-04-17 03:49:21.000000 redis_simple_orm-1.2.5/RSO/txredisapi/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:49:35.181098 redis_simple_orm-1.2.5/redis_simple_orm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11467 2023-04-17 03:49:35.000000 redis_simple_orm-1.2.5/redis_simple_orm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-17 03:49:35.000000 redis_simple_orm-1.2.5/redis_simple_orm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 03:49:35.000000 redis_simple_orm-1.2.5/redis_simple_orm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-17 03:49:35.000000 redis_simple_orm-1.2.5/redis_simple_orm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-17 03:49:35.000000 redis_simple_orm-1.2.5/redis_simple_orm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-17 03:49:35.185098 redis_simple_orm-1.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-04-17 03:49:21.000000 redis_simple_orm-1.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:49:35.185098 redis_simple_orm-1.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-04-17 03:49:21.000000 redis_simple_orm-1.2.5/tests/test_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-04-17 03:49:21.000000 redis_simple_orm-1.2.5/tests/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-17 03:49:21.000000 redis_simple_orm-1.2.5/tests/test_model.py
```

### Comparing `redis_simple_orm-1.2.4/LICENSE` & `redis_simple_orm-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `redis_simple_orm-1.2.4/PKG-INFO` & `redis_simple_orm-1.2.5/redis_simple_orm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: redis_simple_orm
-Version: 1.2.4
+Name: redis-simple-orm
+Version: 1.2.5
 Summary: Simple Redis ORM (Sync and Async).
 Home-page: https://github.com/jockerz/redis_simple_orm
 Author: Jockerz
 Author-email: jockerz@protonmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -18,15 +18,15 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: redis-py
 Provides-Extra: aioredis
 Provides-Extra: txredisapi
 License-File: LICENSE
 
-# WARNING: Not recommended for main data storage
+# WARNING: Old data might be replaced with new one without warning
 
 # Redis Simple ORM
 
 Redis ORM in Simple Way.
 If you find this module is too simple, please take a look on [walrus](https://walrus.readthedocs.org).
 
 > __NOTE__: Please be aware, that this module is way too simple.
@@ -46,15 +46,16 @@
 
 ```bash
 pip install redis_simple_orm[redis-py]
 ```
 
 __OR__
 
-Async with [`aioredis`](https://aioredis.readthedocs.io)
+Async with [`aioredis`](https://aioredis.readthedocs.io) 
+or [`redis.asyncio.Redis`](`https://redis-py.readthedocs.io/en/stable/examples/asyncio_examples.html`)
 
 ```bash
 pip install redis_simple_orm[aioredis]
 ```
 
 __OR__
```

### Comparing `redis_simple_orm-1.2.4/README.md` & `redis_simple_orm-1.2.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# WARNING: Not recommended for main data storage
+# WARNING: Old data might be replaced with new one without warning
 
 # Redis Simple ORM
 
 Redis ORM in Simple Way.
 If you find this module is too simple, please take a look on [walrus](https://walrus.readthedocs.org).
 
 > __NOTE__: Please be aware, that this module is way too simple.
@@ -22,15 +22,16 @@
 
 ```bash
 pip install redis_simple_orm[redis-py]
 ```
 
 __OR__
 
-Async with [`aioredis`](https://aioredis.readthedocs.io)
+Async with [`aioredis`](https://aioredis.readthedocs.io) 
+or [`redis.asyncio.Redis`](`https://redis-py.readthedocs.io/en/stable/examples/asyncio_examples.html`)
 
 ```bash
 pip install redis_simple_orm[aioredis]
 ```
 
 __OR__
```

### Comparing `redis_simple_orm-1.2.4/RSO/aioredis/index.py` & `redis_simple_orm-1.2.5/RSO/aioredis/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,14 @@
         if model_primary_value and isinstance(model_primary_value, list):
             model_primary_value = model_primary_value[0]
         return await model_class.search(redis, model_primary_value)
 
     async def remove_from_index(self, redis: Pipeline):
         index_value = getattr(self.__model__, self.__key__)
         redis.hdel(self.redis_key, index_value)
-        del self
 
 
 class ListIndex(BaseIndex):
 
     @classmethod
     def _to_redis_key(cls, value):
         model_prefix = cls.__model__.__model_name__
```

### Comparing `redis_simple_orm-1.2.4/RSO/aioredis/model.py` & `redis_simple_orm-1.2.5/RSO/aioredis/model.py`

 * *Files identical despite different names*

### Comparing `redis_simple_orm-1.2.4/RSO/base.py` & `redis_simple_orm-1.2.5/RSO/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from datetime import date, datetime
 from dataclasses import asdict, fields
-from typing import Any, List, Type, TypeVar
-
+from typing import List, Type, TypeVar
+from uuid import UUID
 
 T = TypeVar('T')
 
 
 REDIS_MODEL_PREFIX = 'simple_redis_orm'
 
 
@@ -15,15 +15,18 @@
     __index_name__: str = 'index_base'
     # Model class that using this index
     __model__: T
     __key__: str
 
     @property
     def _model_key_value(self):
-        return getattr(self.__model__, self.__model__.__key__)
+        value = getattr(self.__model__, self.__model__.__key__)
+        if isinstance(value, UUID):
+            value = str(value)
+        return value
 
     @classmethod
     def create_from_model_class(cls, model_instance: Type["BaseModel"]):
         cls.__model__ = model_instance
         return cls()
 
 
@@ -59,14 +62,16 @@
                 value = datetime.fromisoformat(f_value)
             else:
                 continue
             setattr(self, field, value)
 
     @classmethod
     def _to_redis_key(cls, value):
+        if isinstance(value, UUID):
+            value = str(value)
         return f'{cls.__prefix__}::{cls.__model_name__}:{value}'
 
     @property
     def redis_key(self):
         return self._to_redis_key(getattr(self, self.__key__))
 
     def dict(self) -> dict:
```

### Comparing `redis_simple_orm-1.2.4/RSO/index.py` & `redis_simple_orm-1.2.5/RSO/index.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,14 @@
         if isinstance(model_primary_value, list):
             model_primary_value = model_primary_value[0]
         return model_class.search(redis, model_primary_value)
 
     def remove_from_index(self, redis: Union[Pipeline, Redis]):
         index_value = getattr(self.__model__, self.__key__)
         redis.hdel(self.redis_key, index_value)
-        del self
 
 
 class ListIndex(BaseIndex):
     @classmethod
     def _to_redis_key(cls, value) -> str:
         model_prefix = cls.__model__.__model_name__
         first_part = f'{cls.__prefix__}::{model_prefix}::'\
```

### Comparing `redis_simple_orm-1.2.4/RSO/model.py` & `redis_simple_orm-1.2.5/RSO/model.py`

 * *Files identical despite different names*

### Comparing `redis_simple_orm-1.2.4/RSO/txredisapi/index.py` & `redis_simple_orm-1.2.5/RSO/txredisapi/index.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,14 @@
 
     @inlineCallbacks
     def remove_from_index(
         self, redis: Union[BaseRedisProtocol, ConnectionHandler]
     ):
         index_value = getattr(self.__model__, self.__key__)
         yield redis.hdel(self.redis_key, index_value)
-        del self
 
 
 class ListIndex(BaseIndex):
 
     @classmethod
     def _to_redis_key(cls, value):
         model_prefix = cls.__model__.__model_name__
```

### Comparing `redis_simple_orm-1.2.4/RSO/txredisapi/model.py` & `redis_simple_orm-1.2.5/RSO/txredisapi/model.py`

 * *Files identical despite different names*

### Comparing `redis_simple_orm-1.2.4/redis_simple_orm.egg-info/PKG-INFO` & `redis_simple_orm-1.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: redis-simple-orm
-Version: 1.2.4
+Name: redis_simple_orm
+Version: 1.2.5
 Summary: Simple Redis ORM (Sync and Async).
 Home-page: https://github.com/jockerz/redis_simple_orm
 Author: Jockerz
 Author-email: jockerz@protonmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -18,15 +18,15 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: redis-py
 Provides-Extra: aioredis
 Provides-Extra: txredisapi
 License-File: LICENSE
 
-# WARNING: Not recommended for main data storage
+# WARNING: Old data might be replaced with new one without warning
 
 # Redis Simple ORM
 
 Redis ORM in Simple Way.
 If you find this module is too simple, please take a look on [walrus](https://walrus.readthedocs.org).
 
 > __NOTE__: Please be aware, that this module is way too simple.
@@ -46,15 +46,16 @@
 
 ```bash
 pip install redis_simple_orm[redis-py]
 ```
 
 __OR__
 
-Async with [`aioredis`](https://aioredis.readthedocs.io)
+Async with [`aioredis`](https://aioredis.readthedocs.io) 
+or [`redis.asyncio.Redis`](`https://redis-py.readthedocs.io/en/stable/examples/asyncio_examples.html`)
 
 ```bash
 pip install redis_simple_orm[aioredis]
 ```
 
 __OR__
```

### Comparing `redis_simple_orm-1.2.4/setup.py` & `redis_simple_orm-1.2.5/setup.py`

 * *Files identical despite different names*

