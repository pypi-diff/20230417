# Comparing `tmp/uagents-0.3.2.tar.gz` & `tmp/uagents-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uagents-0.3.2.tar", max compression
+gzip compressed data, was "uagents-0.4.0.tar", max compression
```

## Comparing `uagents-0.3.2.tar` & `uagents-0.4.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    11357 2023-02-24 13:37:53.437125 uagents-0.3.2/LICENSE
--rw-r--r--   0        0        0     1397 2023-02-24 13:37:53.441125 uagents-0.3.2/README.md
--rw-r--r--   0        0        0      842 2023-03-30 12:04:07.537344 uagents-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      119 2023-03-03 10:39:04.080443 uagents-0.3.2/src/uagents/__init__.py
--rw-r--r--   0        0        0    15248 2023-03-30 09:03:26.516133 uagents-0.3.2/src/uagents/agent.py
--rw-r--r--   0        0        0     5238 2023-03-24 09:42:09.546004 uagents-0.3.2/src/uagents/asgi.py
--rw-r--r--   0        0        0     2269 2023-03-30 09:09:19.738841 uagents-0.3.2/src/uagents/config.py
--rw-r--r--   0        0        0     4979 2023-03-30 09:03:26.516133 uagents-0.3.2/src/uagents/context.py
--rw-r--r--   0        0        0        0 2023-03-02 16:19:41.886178 uagents-0.3.2/src/uagents/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-03-02 16:20:26.910313 uagents-0.3.2/src/uagents/contrib/protocols/__init__.py
--rw-r--r--   0        0        0     1312 2023-03-07 14:38:10.652721 uagents-0.3.2/src/uagents/contrib/protocols/protocol_query.py
--rw-r--r--   0        0        0     4148 2023-03-30 09:03:26.516133 uagents-0.3.2/src/uagents/crypto/__init__.py
--rw-r--r--   0        0        0     1038 2023-02-24 13:37:53.457125 uagents-0.3.2/src/uagents/dispatch.py
--rw-r--r--   0        0        0     1423 2023-02-24 13:37:53.457125 uagents-0.3.2/src/uagents/envelope.py
--rw-r--r--   0        0        0     6796 2023-03-24 09:42:09.546004 uagents-0.3.2/src/uagents/mailbox.py
--rw-r--r--   0        0        0      464 2023-03-24 09:42:09.546004 uagents-0.3.2/src/uagents/models.py
--rw-r--r--   0        0        0     1737 2023-03-30 09:03:26.516133 uagents-0.3.2/src/uagents/network.py
--rw-r--r--   0        0        0     6661 2023-03-24 09:42:09.546004 uagents-0.3.2/src/uagents/protocol.py
--rw-r--r--   0        0        0     2113 2023-03-24 09:42:09.546004 uagents-0.3.2/src/uagents/query.py
--rw-r--r--   0        0        0     1339 2023-03-24 09:42:09.546004 uagents-0.3.2/src/uagents/resolver.py
--rw-r--r--   0        0        0     1153 2023-03-24 09:42:09.546004 uagents-0.3.2/src/uagents/setup.py
--rw-r--r--   0        0        0     2256 2023-02-24 13:37:53.461125 uagents-0.3.2/src/uagents/storage/__init__.py
--rw-r--r--   0        0        0     2450 1970-01-01 00:00:00.000000 uagents-0.3.2/setup.py
--rw-r--r--   0        0        0     2328 1970-01-01 00:00:00.000000 uagents-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-02-24 13:37:53.437125 uagents-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1397 2023-02-24 13:37:53.441125 uagents-0.4.0/README.md
+-rw-r--r--   0        0        0      909 2023-04-17 14:00:08.389315 uagents-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      119 2023-03-03 10:39:04.080443 uagents-0.4.0/src/uagents/__init__.py
+-rw-r--r--   0        0        0    16085 2023-04-17 13:29:50.196085 uagents-0.4.0/src/uagents/agent.py
+-rw-r--r--   0        0        0     5651 2023-04-17 13:29:50.200085 uagents-0.4.0/src/uagents/asgi.py
+-rw-r--r--   0        0        0     2269 2023-04-17 08:26:12.076548 uagents-0.4.0/src/uagents/config.py
+-rw-r--r--   0        0        0     4979 2023-04-17 08:26:12.076548 uagents-0.4.0/src/uagents/context.py
+-rw-r--r--   0        0        0        0 2023-03-02 16:19:41.886178 uagents-0.4.0/src/uagents/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-02 16:20:26.910313 uagents-0.4.0/src/uagents/contrib/protocols/__init__.py
+-rw-r--r--   0        0        0     1312 2023-03-07 14:38:10.652721 uagents-0.4.0/src/uagents/contrib/protocols/protocol_query.py
+-rw-r--r--   0        0        0     4148 2023-04-17 08:26:12.076548 uagents-0.4.0/src/uagents/crypto/__init__.py
+-rw-r--r--   0        0        0     1038 2023-02-24 13:37:53.457125 uagents-0.4.0/src/uagents/dispatch.py
+-rw-r--r--   0        0        0     1423 2023-02-24 13:37:53.457125 uagents-0.4.0/src/uagents/envelope.py
+-rw-r--r--   0        0        0     6796 2023-03-24 09:42:09.546004 uagents-0.4.0/src/uagents/mailbox.py
+-rw-r--r--   0        0        0      464 2023-03-24 09:42:09.546004 uagents-0.4.0/src/uagents/models.py
+-rw-r--r--   0        0        0     1737 2023-04-17 08:26:12.076548 uagents-0.4.0/src/uagents/network.py
+-rw-r--r--   0        0        0     6661 2023-03-24 09:42:09.546004 uagents-0.4.0/src/uagents/protocol.py
+-rw-r--r--   0        0        0     2113 2023-03-24 09:42:09.546004 uagents-0.4.0/src/uagents/query.py
+-rw-r--r--   0        0        0     1339 2023-03-24 09:42:09.546004 uagents-0.4.0/src/uagents/resolver.py
+-rw-r--r--   0        0        0     1153 2023-03-24 09:42:09.546004 uagents-0.4.0/src/uagents/setup.py
+-rw-r--r--   0        0        0     2256 2023-02-24 13:37:53.461125 uagents-0.4.0/src/uagents/storage/__init__.py
+-rw-r--r--   0        0        0     2450 1970-01-01 00:00:00.000000 uagents-0.4.0/setup.py
+-rw-r--r--   0        0        0     2328 1970-01-01 00:00:00.000000 uagents-0.4.0/PKG-INFO
```

### Comparing `uagents-0.3.2/LICENSE` & `uagents-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `uagents-0.3.2/README.md` & `uagents-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `uagents-0.3.2/pyproject.toml` & `uagents-0.4.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "uagents"
-version = "0.3.2"
+version = "0.4.0"
 description = "Lightweight framework for rapid agent-based development"
 authors = ["Ed FitzGerald <edward.fitzgerald@fetch.ai>", "James Riehl <james.riehl@fetch.ai>", "Alejandro Morales <alejandro.madrigal@fetch.ai>"]
 license = "Apache 2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -26,10 +26,13 @@
 
 [tool.poetry.group.orm.dependencies]
 tortoise-orm = "^0.19.2"
 
 [tool.poetry.group.geo.dependencies]
 geopy = "^2.3.0"
 
+[tool.poetry.group.remote-agents.dependencies]
+pyngrok = "^5.2.3"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `uagents-0.3.2/src/uagents/agent.py` & `uagents-0.4.0/src/uagents/agent.py`

 * *Files 5% similar despite different names*

```diff
@@ -93,14 +93,17 @@
             # if mailbox is provided, override endpoints with mailbox endpoint
             self._endpoints = [
                 {
                     "url": f"{self.mailbox['http_prefix']}://{self.mailbox['base_url']}/v1/submit",
                     "weight": 1,
                 }
             ]
+        else:
+            self._mailbox = None
+            self._mailbox_client = None
 
         self._ledger = get_ledger()
         self._reg_contract = get_reg_contract()
         self._storage = KeyValueStore(self.address[0:16])
         self._interval_handlers: List[Tuple[IntervalCallback, float]] = []
         self._interval_messages: Set[str] = set()
         self._signed_message_handlers: Dict[str, MessageCallback] = {}
@@ -133,15 +136,17 @@
         # keep track of supported protocols
         self.protocols: Dict[str, Protocol] = {}
 
         # register with the dispatcher
         self._dispatcher.register(self.address, self)
 
         if not self._use_mailbox:
-            self._server = ASGIServer(self._port, self._loop, self._queries)
+            self._server = ASGIServer(
+                self._port, self._loop, self._queries, logger=self._logger
+            )
 
     @property
     def name(self) -> str:
         return self._name
 
     @property
     def address(self) -> str:
@@ -155,14 +160,18 @@
     def storage(self) -> KeyValueStore:
         return self._storage
 
     @property
     def mailbox(self) -> Dict[str, str]:
         return self._mailbox
 
+    @property
+    def mailbox_client(self) -> MailboxClient:
+        return self._mailbox_client
+
     @mailbox.setter
     def mailbox(self, config: Union[str, Dict[str, str]]):
         self._mailbox = parse_mailbox_config(config)
 
     def sign(self, data: bytes) -> str:
         return self._identity.sign(data)
 
@@ -415,18 +424,33 @@
 
 class Bureau:
     def __init__(self, port: Optional[int] = None):
         self._loop = asyncio.get_event_loop_policy().get_event_loop()
         self._agents = []
         self._port = port or 8000
         self._queries: Dict[str, asyncio.Future] = {}
-        self._server = ASGIServer(self._port, self._loop, self._queries)
+        self._logger = get_logger("bureau")
+        self._server = ASGIServer(self._port, self._loop, self._queries, self._logger)
+        self._use_mailbox = False
 
     def add(self, agent: Agent):
         agent.update_loop(self._loop)
         agent.update_queries(self._queries)
+        if agent.mailbox is not None:
+            self._use_mailbox = True
         self._agents.append(agent)
 
     def run(self):
+        tasks = []
         for agent in self._agents:
             agent.setup()
-        self._loop.run_until_complete(self._server.serve())
+            if agent.mailbox is not None:
+                tasks.append(
+                    self._loop.create_task(
+                        agent.mailbox_client.process_deletion_queue()
+                    )
+                )
+                tasks.append(self._loop.create_task(agent.mailbox_client.run()))
+        if not self._use_mailbox:
+            tasks.append(self._loop.create_task(self._server.serve()))
+
+        self._loop.run_until_complete(asyncio.gather(*tasks))
```

### Comparing `uagents-0.3.2/src/uagents/asgi.py` & `uagents-0.4.0/src/uagents/asgi.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 import asyncio
 import json
 from datetime import datetime
-from typing import Dict
+from logging import Logger
+from typing import Dict, Optional
 
 import pydantic
 import uvicorn
 
+from uagents.config import get_logger
 from uagents.crypto import is_user_address
 from uagents.dispatch import dispatcher
 from uagents.envelope import Envelope
 from uagents.models import Model, ErrorMessage
 from uagents.query import enclose_response
 
 
+HOST = "0.0.0.0"
+
+
 async def _read_asgi_body(receive):
     body = b""
     more_body = True
 
     while more_body:
         message = await receive()
         body += message.get("body", b"")
@@ -27,23 +32,33 @@
 
 class ASGIServer:
     def __init__(
         self,
         port: int,
         loop: asyncio.AbstractEventLoop,
         queries: Dict[str, asyncio.Future],
+        logger: Optional[Logger] = None,
     ):
         self._port = int(port)
         self._loop = loop
         self._queries = queries
+        self._logger = logger or get_logger("server")
+        self._server = None
+
+    @property
+    def server(self):
+        return self._server
 
     async def serve(self):
-        config = uvicorn.Config(self, host="0.0.0.0", port=self._port, log_level="info")
-        server = uvicorn.Server(config)
-        await server.serve()
+        config = uvicorn.Config(self, host=HOST, port=self._port, log_level="warning")
+        self._server = uvicorn.Server(config)
+        self._logger.info(
+            f"Starting server on http://{HOST}:{self._port} (Press CTRL+C to quit)"
+        )
+        await self._server.serve()
 
     async def __call__(self, scope, receive, send):
         if scope["type"] == "lifespan":
             return  # lifespan events not implemented
 
         assert scope["type"] == "http"
```

### Comparing `uagents-0.3.2/src/uagents/config.py` & `uagents-0.4.0/src/uagents/config.py`

 * *Files identical despite different names*

### Comparing `uagents-0.3.2/src/uagents/context.py` & `uagents-0.4.0/src/uagents/context.py`

 * *Files identical despite different names*

### Comparing `uagents-0.3.2/src/uagents/contrib/protocols/protocol_query.py` & `uagents-0.4.0/src/uagents/contrib/protocols/protocol_query.py`

 * *Files identical despite different names*

### Comparing `uagents-0.3.2/src/uagents/crypto/__init__.py` & `uagents-0.4.0/src/uagents/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `uagents-0.3.2/src/uagents/dispatch.py` & `uagents-0.4.0/src/uagents/dispatch.py`

 * *Files identical despite different names*

### Comparing `uagents-0.3.2/src/uagents/envelope.py` & `uagents-0.4.0/src/uagents/envelope.py`

 * *Files identical despite different names*

### Comparing `uagents-0.3.2/src/uagents/mailbox.py` & `uagents-0.4.0/src/uagents/mailbox.py`

 * *Files identical despite different names*

### Comparing `uagents-0.3.2/src/uagents/network.py` & `uagents-0.4.0/src/uagents/network.py`

 * *Files identical despite different names*

### Comparing `uagents-0.3.2/src/uagents/protocol.py` & `uagents-0.4.0/src/uagents/protocol.py`

 * *Files identical despite different names*

### Comparing `uagents-0.3.2/src/uagents/query.py` & `uagents-0.4.0/src/uagents/query.py`

 * *Files identical despite different names*

### Comparing `uagents-0.3.2/src/uagents/resolver.py` & `uagents-0.4.0/src/uagents/resolver.py`

 * *Files identical despite different names*

### Comparing `uagents-0.3.2/src/uagents/setup.py` & `uagents-0.4.0/src/uagents/setup.py`

 * *Files identical despite different names*

### Comparing `uagents-0.3.2/src/uagents/storage/__init__.py` & `uagents-0.4.0/src/uagents/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `uagents-0.3.2/setup.py` & `uagents-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
  'msgpack>=1.0.4,<2.0.0',
  'pydantic>=1.10.2,<2.0.0',
  'uvicorn>=0.19.0,<0.20.0',
  'websockets>=10.4,<11.0']
 
 setup_kwargs = {
     'name': 'uagents',
-    'version': '0.3.2',
+    'version': '0.4.0',
     'description': 'Lightweight framework for rapid agent-based development',
     'long_description': 'The **μAgents** (micro-Agents) project is a fast and lightweight framework that makes it easy to build agents for all kinds of decentralised use cases.\n\n## Installation\n\nInstall μAgents for Python 3.8, 3.9, or 3.10:\n\n```bash\npoetry install\npoetry shell\n```\n\n## Documentation\n\nBuild and run the docs locally with:\n\n```bash\nmkdocs serve\n```\n\nOr go to the official docs site: https://docs.fetch.ai/uAgents.\n\n## Examples\n\nThe [`examples`](https://github.com/fetchai/uAgents/tree/main/examples) folder contains several examples of how to create and run various types of agents.\n\n## Contributing\n\nAll contributions are welcome! Remember, contribution includes not only code, but any help with docs or issues raised by other developers. See our [contribution guidelines](https://github.com/fetchai/uAgents/blob/main/CONTRIBUTING.md) for more details.\n\n### Development Guidelines\n\nRead our [development guidelines](https://github.com/fetchai/uAgents/blob/main/DEVELOPING.md) to learn some useful tips related to development.\n\n### Issues, Questions and Discussions\n\nWe use [GitHub Issues](https://github.com/fetchai/uAgents/issues) for tracking requests and bugs, and [GitHub Discussions](https://github.com/fetchai/uAgents/discussions) for general questions and discussion.\n\n## License\n\nThe μAgents project is licensed under [Apache License 2.0](https://github.com/fetchai/uAgents/blob/main/LICENSE).\n\n',
     'author': 'Ed FitzGerald',
     'author_email': 'edward.fitzgerald@fetch.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `uagents-0.3.2/PKG-INFO` & `uagents-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uagents
-Version: 0.3.2
+Version: 0.4.0
 Summary: Lightweight framework for rapid agent-based development
 License: Apache 2.0
 Author: Ed FitzGerald
 Author-email: edward.fitzgerald@fetch.ai
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

