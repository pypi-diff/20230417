# Comparing `tmp/betwatch-0.9.8.tar.gz` & `tmp/betwatch-0.9.9.tar.gz`

## Comparing `betwatch-0.9.8.tar` & `betwatch-0.9.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 betwatch-0.9.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 betwatch-0.9.8/.github/dependabot.yml
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 betwatch-0.9.8/.github/workflows/test.yml
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 betwatch-0.9.8/betwatch/__about__.py
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 betwatch-0.9.8/betwatch/__init__.py
--rw-r--r--   0        0        0     7197 2020-02-02 00:00:00.000000 betwatch-0.9.8/betwatch/client.py
--rw-r--r--   0        0        0    24087 2020-02-02 00:00:00.000000 betwatch-0.9.8/betwatch/client_async.py
--rw-r--r--   0        0        0     4399 2020-02-02 00:00:00.000000 betwatch-0.9.8/betwatch/queries.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 betwatch-0.9.8/betwatch/types/__init__.py
--rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 betwatch-0.9.8/betwatch/types/bookmakers.py
--rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 betwatch-0.9.8/betwatch/types/filters.py
--rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 betwatch-0.9.8/betwatch/types/markets.py
--rw-r--r--   0        0        0    10286 2020-02-02 00:00:00.000000 betwatch-0.9.8/betwatch/types/race.py
--rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 betwatch-0.9.8/examples/get_race_prices.py
--rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 betwatch-0.9.8/examples/get_race_prices_async.py
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 betwatch-0.9.8/examples/get_races.py
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 betwatch-0.9.8/examples/get_races_async.py
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 betwatch-0.9.8/examples/subscriptions.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 betwatch-0.9.8/tests/__init__.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 betwatch-0.9.8/tests/test_check_last_updated.py
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 betwatch-0.9.8/tests/test_get_race.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 betwatch-0.9.8/tests/test_get_race_async.py
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 betwatch-0.9.8/tests/test_get_races.py
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 betwatch-0.9.8/tests/test_get_races_async.py
--rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 betwatch-0.9.8/.gitignore
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 betwatch-0.9.8/LICENSE.txt
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 betwatch-0.9.8/README.md
--rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 betwatch-0.9.8/pyproject.toml
--rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 betwatch-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 betwatch-0.9.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 betwatch-0.9.9/.github/dependabot.yml
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 betwatch-0.9.9/.github/workflows/test.yml
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 betwatch-0.9.9/betwatch/__about__.py
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 betwatch-0.9.9/betwatch/__init__.py
+-rw-r--r--   0        0        0     7197 2020-02-02 00:00:00.000000 betwatch-0.9.9/betwatch/client.py
+-rw-r--r--   0        0        0    23839 2020-02-02 00:00:00.000000 betwatch-0.9.9/betwatch/client_async.py
+-rw-r--r--   0        0        0     4399 2020-02-02 00:00:00.000000 betwatch-0.9.9/betwatch/queries.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 betwatch-0.9.9/betwatch/types/__init__.py
+-rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 betwatch-0.9.9/betwatch/types/bookmakers.py
+-rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 betwatch-0.9.9/betwatch/types/filters.py
+-rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 betwatch-0.9.9/betwatch/types/markets.py
+-rw-r--r--   0        0        0    10286 2020-02-02 00:00:00.000000 betwatch-0.9.9/betwatch/types/race.py
+-rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 betwatch-0.9.9/examples/get_race_prices.py
+-rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 betwatch-0.9.9/examples/get_race_prices_async.py
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 betwatch-0.9.9/examples/get_races.py
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 betwatch-0.9.9/examples/get_races_async.py
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 betwatch-0.9.9/examples/subscriptions.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 betwatch-0.9.9/tests/__init__.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 betwatch-0.9.9/tests/test_check_last_updated.py
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 betwatch-0.9.9/tests/test_get_race.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 betwatch-0.9.9/tests/test_get_race_async.py
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 betwatch-0.9.9/tests/test_get_races.py
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 betwatch-0.9.9/tests/test_get_races_async.py
+-rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 betwatch-0.9.9/.gitignore
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 betwatch-0.9.9/LICENSE.txt
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 betwatch-0.9.9/README.md
+-rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 betwatch-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 betwatch-0.9.9/PKG-INFO
```

### Comparing `betwatch-0.9.8/.github/workflows/test.yml` & `betwatch-0.9.9/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `betwatch-0.9.8/betwatch/__init__.py` & `betwatch-0.9.9/betwatch/__init__.py`

 * *Files identical despite different names*

### Comparing `betwatch-0.9.8/betwatch/client.py` & `betwatch-0.9.9/betwatch/client.py`

 * *Files identical despite different names*

### Comparing `betwatch-0.9.8/betwatch/client_async.py` & `betwatch-0.9.9/betwatch/client_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import typedload
 from aiohttp.client_exceptions import ClientError
 from aiohttp.web_exceptions import HTTPClientError, HTTPServerError
 from gql import Client
 from gql.client import AsyncClientSession, ReconnectingAsyncClientSession
 from gql.transport.aiohttp import AIOHTTPTransport
 from gql.transport.aiohttp import log as aiohttp_logger
-from gql.transport.exceptions import TransportQueryError
+from gql.transport.exceptions import TransportError, TransportQueryError
 from gql.transport.websockets import WebsocketsTransport
 from gql.transport.websockets import log as websockets_logger
 from graphql import DocumentNode
 from typedload.exceptions import TypedloadException
 
 from betwatch.__about__ import __version__
 from betwatch.queries import (
@@ -65,15 +65,15 @@
         self._session_lock = asyncio.Lock()
 
         self._subscription_queue: asyncio.Queue[SubscriptionUpdate] = asyncio.Queue()
         self._subscriptions_betfair: Dict[str, asyncio.Task] = {}
         self._subscriptions_prices: Dict[str, asyncio.Task] = {}
         self._subscriptions_updates: Dict[Tuple[str, str], asyncio.Task] = {}
 
-        self._monitor_task: asyncio.Task = asyncio.create_task(self._monitor())
+        self._monitor_task: asyncio.Task | None = None
         self._last_reconnect: float = monotonic()
 
     def connect(self):
         logging.debug("connecting to client sessions")
         self._gql_sub_transport = WebsocketsTransport(
             url="wss://api.betwatch.com/sub",
             headers={
@@ -350,14 +350,17 @@
             and len(self._subscriptions_updates) < 1
         ):
             raise Exception("You must subscribe to a race before listening for updates")
 
         # dont spam the user with warnings of queue size
         last_warning = datetime.now()
 
+        # start monitor
+        self._monitor_task = asyncio.create_task(self._monitor())
+
         while True:
             try:
                 logging.debug("Waiting for subscription update")
                 update = await self._subscription_queue.get()
                 self._subscription_queue.task_done()
                 yield update
                 logging.debug("Subscription update received")
@@ -450,18 +453,16 @@
                         race_id=race_id,
                         bookmaker_markets=typedload.load(
                             result["priceUpdates"], List[BookmakerMarket]
                         ),
                     )
 
                     self._subscription_queue.put_nowait(update)
-        except TransportQueryError as e:
-            logging.error(
-                f"Error subscribing to bookmaker updates: {e.errors[0].get('message') if e.errors and e.errors[0].get('message') else e}"
-            )
+        except TransportError as e:
+            logging.error(f"Error subscribing to bookmaker updates: {e}")
         except asyncio.CancelledError:
             await self.unsubscribe_bookmaker_updates(race_id)
             return
 
     async def unsubscribe_betfair_updates(self, race_id: str):
         if race_id not in self._subscriptions_betfair:
             logging.info(
@@ -520,18 +521,16 @@
                         race_id=race_id,
                         betfair_markets=typedload.load(
                             result["betfairUpdates"], List[BetfairMarket]
                         ),
                     )
                     self._subscription_queue.put_nowait(update)
 
-        except TransportQueryError as e:
-            logging.error(
-                f"Error subscribing to betfair updates: {e.errors[0].get('message') if e.errors and e.errors[0].get('message') else e}"
-            )
+        except TransportError as e:
+            logging.error(f"Error subscribing to betfair updates: {e}")
         except asyncio.CancelledError:
             await self.unsubscribe_betfair_updates(race_id)
             return
 
     async def unsubscribe_race_updates(self, date_from: str, date_to: str):
         if (date_from, date_to) not in self._subscriptions_updates:
             logging.info(f"Not subscribed to races updates for {date_from} - {date_to}")
@@ -566,18 +565,16 @@
                     ru = typedload.load(result["racesUpdates"], RaceUpdate)
                     update = SubscriptionUpdate(
                         race_id=ru.id,
                         race_update=ru,
                     )
                     self._subscription_queue.put_nowait(update)
 
-        except TransportQueryError as e:
-            logging.error(
-                f"Error subscribing to race updates: {e.errors[0].get('message') if e.errors and e.errors[0].get('message') else e}"
-            )
+        except TransportError as e:
+            logging.error(f"Error subscribing to race updates: {e}")
         except asyncio.CancelledError:
             await self.unsubscribe_race_updates(date_from, date_to)
             return
 
     @backoff.on_exception(backoff.expo, Exception, max_time=60, max_tries=5)
     async def _get_race_by_id(
         self, race_id: str, query: DocumentNode
```

### Comparing `betwatch-0.9.8/betwatch/queries.py` & `betwatch-0.9.9/betwatch/queries.py`

 * *Files identical despite different names*

### Comparing `betwatch-0.9.8/betwatch/types/bookmakers.py` & `betwatch-0.9.9/betwatch/types/bookmakers.py`

 * *Files identical despite different names*

### Comparing `betwatch-0.9.8/betwatch/types/filters.py` & `betwatch-0.9.9/betwatch/types/filters.py`

 * *Files identical despite different names*

### Comparing `betwatch-0.9.8/betwatch/types/markets.py` & `betwatch-0.9.9/betwatch/types/markets.py`

 * *Files identical despite different names*

### Comparing `betwatch-0.9.8/betwatch/types/race.py` & `betwatch-0.9.9/betwatch/types/race.py`

 * *Files identical despite different names*

### Comparing `betwatch-0.9.8/examples/get_race_prices.py` & `betwatch-0.9.9/examples/get_race_prices.py`

 * *Files identical despite different names*

### Comparing `betwatch-0.9.8/examples/get_race_prices_async.py` & `betwatch-0.9.9/examples/get_race_prices_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-0.9.8/examples/get_races.py` & `betwatch-0.9.9/examples/get_races.py`

 * *Files identical despite different names*

### Comparing `betwatch-0.9.8/examples/get_races_async.py` & `betwatch-0.9.9/examples/get_races_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-0.9.8/examples/subscriptions.py` & `betwatch-0.9.9/examples/subscriptions.py`

 * *Files identical despite different names*

### Comparing `betwatch-0.9.8/tests/test_get_race.py` & `betwatch-0.9.9/tests/test_get_race.py`

 * *Files identical despite different names*

### Comparing `betwatch-0.9.8/tests/test_get_race_async.py` & `betwatch-0.9.9/tests/test_get_race_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-0.9.8/tests/test_get_races.py` & `betwatch-0.9.9/tests/test_get_races.py`

 * *Files identical despite different names*

### Comparing `betwatch-0.9.8/tests/test_get_races_async.py` & `betwatch-0.9.9/tests/test_get_races_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-0.9.8/.gitignore` & `betwatch-0.9.9/.gitignore`

 * *Files identical despite different names*

### Comparing `betwatch-0.9.8/LICENSE.txt` & `betwatch-0.9.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `betwatch-0.9.8/README.md` & `betwatch-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `betwatch-0.9.8/pyproject.toml` & `betwatch-0.9.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
-    "gql[aiohttp,websockets,requests]==3.5.0b0",
+    "gql[aiohttp,websockets,requests]==3.5.0b3",
     "typedload==2.21",
     "aiohttp==3.8.3",
     "python-dateutil==2.8.2",
 ]
 dynamic = ["version"]
 
 [project.urls]
```

### Comparing `betwatch-0.9.8/PKG-INFO` & `betwatch-0.9.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betwatch
-Version: 0.9.8
+Version: 0.9.9
 Summary: A Python package for interacting with the Betwatch.com API
 Project-URL: Documentation, https://github.com/betwatch/betwatch-sdk-python#readme
 Project-URL: Issues, https://github.com/betwatch/betwatch-sdk-python/issues
 Project-URL: Source, https://github.com/betwatch/betwatch-sdk-python
 Project-URL: Betwatch.com, https://betwatch.com
 Author-email: Jamie Watts <jamie@betwatch.com>
 License-File: LICENSE.txt
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Requires-Dist: aiohttp==3.8.3
-Requires-Dist: gql[aiohttp,requests,websockets]==3.5.0b0
+Requires-Dist: gql[aiohttp,requests,websockets]==3.5.0b3
 Requires-Dist: python-dateutil==2.8.2
 Requires-Dist: typedload==2.21
 Description-Content-Type: text/markdown
 
 # Betwatch Python SDK
 
 [![PyPI - Version](https://img.shields.io/pypi/v/betwatch.svg)](https://pypi.org/project/betwatch)
```

