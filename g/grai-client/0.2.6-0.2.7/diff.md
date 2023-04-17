# Comparing `tmp/grai_client-0.2.6.tar.gz` & `tmp/grai_client-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_client-0.2.6.tar", max compression
+gzip compressed data, was "grai_client-0.2.7.tar", max compression
```

## Comparing `grai_client-0.2.6.tar` & `grai_client-0.2.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      735 2023-03-17 19:32:07.995313 grai_client-0.2.6/pyproject.toml
--rw-r--r--   0        0        0       78 2023-02-13 20:16:22.660883 grai_client-0.2.6/src/grai_client/__init__.py
--rw-r--r--   0        0        0     1344 2023-02-13 20:16:22.661185 grai_client-0.2.6/src/grai_client/authentication.py
--rw-r--r--   0        0        0      210 2023-02-13 20:16:22.661271 grai_client-0.2.6/src/grai_client/endpoints/__init__.py
--rw-r--r--   0        0        0     8317 2023-03-17 18:41:26.507354 grai_client-0.2.6/src/grai_client/endpoints/client.py
--rw-r--r--   0        0        0      274 2023-02-13 20:16:22.661431 grai_client-0.2.6/src/grai_client/endpoints/rest.py
--rw-r--r--   0        0        0     2616 2023-03-17 18:41:26.180237 grai_client-0.2.6/src/grai_client/endpoints/utilities.py
--rw-r--r--   0        0        0       82 2023-02-13 20:16:22.661588 grai_client-0.2.6/src/grai_client/endpoints/v1/__init__.py
--rw-r--r--   0        0        0     2525 2023-03-13 20:23:41.239758 grai_client-0.2.6/src/grai_client/endpoints/v1/client.py
--rw-r--r--   0        0        0      886 2023-02-13 20:16:22.661997 grai_client-0.2.6/src/grai_client/endpoints/v1/delete.py
--rw-r--r--   0        0        0     7202 2023-03-17 18:07:25.362143 grai_client-0.2.6/src/grai_client/endpoints/v1/get.py
--rw-r--r--   0        0        0     1628 2023-02-13 20:16:22.662169 grai_client-0.2.6/src/grai_client/endpoints/v1/patch.py
--rw-r--r--   0        0        0     1235 2023-02-13 20:16:22.662247 grai_client-0.2.6/src/grai_client/endpoints/v1/post.py
--rw-r--r--   0        0        0      976 2023-03-13 20:23:41.240223 grai_client-0.2.6/src/grai_client/endpoints/v1/url.py
--rw-r--r--   0        0        0      886 2023-02-13 20:16:22.662385 grai_client-0.2.6/src/grai_client/endpoints/v1/utils.py
--rw-r--r--   0        0        0        0 2023-02-13 20:16:22.662418 grai_client-0.2.6/src/grai_client/py.typed
--rw-r--r--   0        0        0       58 2023-02-13 20:16:22.662870 grai_client-0.2.6/src/grai_client/schemas/__init__.py
--rw-r--r--   0        0        0      218 2023-02-13 20:16:22.662940 grai_client-0.2.6/src/grai_client/schemas/labels.py
--rw-r--r--   0        0        0      329 2023-02-13 20:16:22.663042 grai_client-0.2.6/src/grai_client/schemas/schema.py
--rw-r--r--   0        0        0      111 2023-02-13 20:16:22.663106 grai_client-0.2.6/src/grai_client/schemas/workspace.py
--rw-r--r--   0        0        0       39 2023-02-13 20:16:22.663186 grai_client-0.2.6/src/grai_client/testing/__init__.py
--rw-r--r--   0        0        0     2907 2023-02-13 20:16:22.663262 grai_client-0.2.6/src/grai_client/testing/schema.py
--rw-r--r--   0        0        0     1375 2023-02-13 20:16:22.663339 grai_client-0.2.6/src/grai_client/update.py
--rw-r--r--   0        0        0       40 2023-02-13 20:16:22.663408 grai_client-0.2.6/src/grai_client/utilities/__init__.py
--rw-r--r--   0        0        0      529 2023-03-13 20:23:41.240448 grai_client-0.2.6/src/grai_client/utilities/tests.py
--rw-r--r--   0        0        0      906 1970-01-01 00:00:00.000000 grai_client-0.2.6/setup.py
--rw-r--r--   0        0        0      694 1970-01-01 00:00:00.000000 grai_client-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0      771 2023-04-17 19:08:37.025212 grai_client-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0       78 2023-02-13 20:16:22.660883 grai_client-0.2.7/src/grai_client/__init__.py
+-rw-r--r--   0        0        0     1344 2023-02-13 20:16:22.661185 grai_client-0.2.7/src/grai_client/authentication.py
+-rw-r--r--   0        0        0      210 2023-02-13 20:16:22.661271 grai_client-0.2.7/src/grai_client/endpoints/__init__.py
+-rw-r--r--   0        0        0     8706 2023-04-17 19:08:37.025349 grai_client-0.2.7/src/grai_client/endpoints/client.py
+-rw-r--r--   0        0        0      286 2023-04-17 19:08:37.025448 grai_client-0.2.7/src/grai_client/endpoints/rest.py
+-rw-r--r--   0        0        0     2640 2023-04-17 19:08:37.025545 grai_client-0.2.7/src/grai_client/endpoints/utilities.py
+-rw-r--r--   0        0        0       82 2023-02-13 20:16:22.661588 grai_client-0.2.7/src/grai_client/endpoints/v1/__init__.py
+-rw-r--r--   0        0        0     2514 2023-04-17 19:08:37.025648 grai_client-0.2.7/src/grai_client/endpoints/v1/client.py
+-rw-r--r--   0        0        0      931 2023-04-17 19:08:37.025740 grai_client-0.2.7/src/grai_client/endpoints/v1/delete.py
+-rw-r--r--   0        0        0     7796 2023-04-17 19:08:37.025852 grai_client-0.2.7/src/grai_client/endpoints/v1/get.py
+-rw-r--r--   0        0        0     1780 2023-04-17 19:08:37.025956 grai_client-0.2.7/src/grai_client/endpoints/v1/patch.py
+-rw-r--r--   0        0        0     1338 2023-04-17 19:08:37.026055 grai_client-0.2.7/src/grai_client/endpoints/v1/post.py
+-rw-r--r--   0        0        0      976 2023-03-13 20:23:41.240223 grai_client-0.2.7/src/grai_client/endpoints/v1/url.py
+-rw-r--r--   0        0        0      948 2023-04-17 19:08:37.026173 grai_client-0.2.7/src/grai_client/endpoints/v1/utils.py
+-rw-r--r--   0        0        0        0 2023-02-13 20:16:22.662418 grai_client-0.2.7/src/grai_client/py.typed
+-rw-r--r--   0        0        0       58 2023-02-13 20:16:22.662870 grai_client-0.2.7/src/grai_client/schemas/__init__.py
+-rw-r--r--   0        0        0      218 2023-02-13 20:16:22.662940 grai_client-0.2.7/src/grai_client/schemas/labels.py
+-rw-r--r--   0        0        0      329 2023-02-13 20:16:22.663042 grai_client-0.2.7/src/grai_client/schemas/schema.py
+-rw-r--r--   0        0        0      111 2023-02-13 20:16:22.663106 grai_client-0.2.7/src/grai_client/schemas/workspace.py
+-rw-r--r--   0        0        0       39 2023-02-13 20:16:22.663186 grai_client-0.2.7/src/grai_client/testing/__init__.py
+-rw-r--r--   0        0        0     2907 2023-02-13 20:16:22.663262 grai_client-0.2.7/src/grai_client/testing/schema.py
+-rw-r--r--   0        0        0     1375 2023-02-13 20:16:22.663339 grai_client-0.2.7/src/grai_client/update.py
+-rw-r--r--   0        0        0       40 2023-02-13 20:16:22.663408 grai_client-0.2.7/src/grai_client/utilities/__init__.py
+-rw-r--r--   0        0        0      529 2023-04-10 17:14:23.662254 grai_client-0.2.7/src/grai_client/utilities/tests.py
+-rw-r--r--   0        0        0      957 1970-01-01 00:00:00.000000 grai_client-0.2.7/setup.py
+-rw-r--r--   0        0        0      773 1970-01-01 00:00:00.000000 grai_client-0.2.7/PKG-INFO
```

### Comparing `grai_client-0.2.6/pyproject.toml` & `grai_client-0.2.7/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grai-client"
-version = "0.2.6"
+version = "0.2.7"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_client", from = "src" },
 ]
 
@@ -12,14 +12,16 @@
 python = "^3.8"
 pydantic = "^1.9.1"
 requests = "^2.28.1"
 multimethod = "1.9"
 orjson = "^3.8.3"
 pyyaml = "^6.0"
 grai-schemas = "^0.1.8"
+httpx = "^0.23.3"
+brotli = "^1.0.9"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^0.971"
 isort = "^5.10.1"
 black = "^22.6.0"
 pytest = "^7.2.0"
 types-requests = "^2.28.11.5"
```

### Comparing `grai_client-0.2.6/src/grai_client/authentication.py` & `grai_client-0.2.7/src/grai_client/authentication.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.2.6/src/grai_client/endpoints/client.py` & `grai_client-0.2.7/src/grai_client/endpoints/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import abc
+import asyncio
 import sys
 from typing import Any, Dict, List, Literal, Optional, Sequence, TypeVar, Union
-from uuid import UUID
 
-import requests
+import httpx
+from httpx import BasicAuth, Request, Response
 from multimethod import multimethod
 from pydantic import BaseModel
 
-from grai_client.authentication import APIKeyHeader, UserTokenHeader
+from grai_client.authentication import APIKeyHeader
 from grai_client.endpoints.rest import delete, get, patch, post
 from grai_client.endpoints.utilities import (
     add_query_params,
     response_status_check,
     serialize_obj,
 )
 from grai_client.schemas.schema import GraiType
@@ -40,23 +41,30 @@
 
 PROTOCOL = Optional[Union[Literal["http"], Literal["https"]]]
 
 
 class BaseClient(abc.ABC):
     id: str = "base"
 
-    def __init__(self, host: str, port: str = "443", protocol: PROTOCOL = None, insecure: bool = False):
+    def __init__(
+        self,
+        host: str,
+        port: str = "443",
+        protocol: PROTOCOL = None,
+        insecure: bool = False,
+        httpx_async_client: Optional[httpx.AsyncClient] = None,
+    ):
         self.host = host
         self.port = port
         self.insecure = insecure
 
         self.default_payload: Dict = dict()
         self.default_headers: Dict = dict()
         self.default_request_args: Dict = dict()
-        self.session = requests.Session()
+        self.session = httpx.AsyncClient(timeout=120) if httpx_async_client is None else httpx_async_client
 
         if protocol is None:
             protocol = "http" if insecure else "https"
         self.protocol = protocol
 
         self.url = f"{self.protocol}://{self.host}:{self.port}"
         self.api = f"{self.url}"
@@ -72,26 +80,24 @@
             **{
                 "payload": self.default_payload,
                 "headers": self.default_headers,
                 "request_args": self.default_request_args,
             }
         )
 
-    def server_health_status(self) -> requests.Response:
-        return self.session.get(self.health_endpoint)
+    def server_health_status(self) -> Response:
+        return httpx.get(self.health_endpoint)
 
     def build_url(self, endpoint: str) -> str:
         return f"{self.api}{endpoint}"
 
     @property
     def auth_headers(self) -> Dict:
         if self._auth_headers is None:
-            raise Exception(
-                "Client not authenticated. Please call `set_authentication_headers` with your credentials first"
-            )
+            raise Exception("Client not authenticated. Please call `authenticate` with your credentials first")
         return self._auth_headers
 
     def set_authentication_headers(
         self,
         username: Optional[str] = None,
         password: Optional[str] = None,
         api_key: Optional[str] = None,
@@ -105,27 +111,30 @@
         password: Optional[str] = None,
         api_key: Optional[str] = None,
     ) -> None:
         if api_key is not None:
             self._auth_headers = APIKeyHeader(api_key).headers
             self.session.auth = None
         elif username and password:
-            self.session.auth = (username, password)
+            self.session.auth = BasicAuth(username, password)
             self._auth_headers = {}
         else:
             raise Exception("Authentication requires either an api key, or username/password combination.")
 
         resp = self.check_authentication()
         if resp.status_code != 200:
-            raise Exception(
-                f"Unable to authenticate connection to the server with the provided credentials. Received status_code: {resp.status_code}"
+            message = (
+                f"Unable to authenticate connection to the server with the provided credentials. ",
+                f"Received status_code: {resp.status_code}",
             )
 
+            raise Exception(message)
+
     @abc.abstractmethod
-    def check_authentication(self) -> requests.Response:
+    def check_authentication(self) -> Response:
         raise NotImplementedError(f"No authentication implemented for {type(self)}")
 
     @multimethod
     def get_url(self, grai_type: Any) -> str:
         raise NotImplementedError(f"No url method implemented for type {type(grai_type)}")
 
     def prep_options(self, options: OptionType = None) -> ClientOptions:
@@ -143,123 +152,124 @@
         else:
             raise NotImplementedError(f"Unrecognized options type: {type(options)}")
 
         return default_options
 
     def get(self, *args, options: OptionType = None, **kwargs):
         options = self.prep_options(options)
-        return get(self, *args, options=options, **kwargs)
+        return asyncio.run(get(self, *args, options=options, **kwargs))
 
     def post(self, *args, options: OptionType = None, **kwargs):
         options = self.prep_options(options)
-        return post(self, *args, options=options, **kwargs)
+        return asyncio.run(post(self, *args, options=options, **kwargs))
 
     def patch(self, *args, options: OptionType = None, **kwargs):
         options = self.prep_options(options)
-        return patch(self, *args, options=options, **kwargs)
+        return asyncio.run(patch(self, *args, options=options, **kwargs))
 
     def delete(self, *args, options: OptionType = None, **kwargs):
         options = self.prep_options(options)
-        return delete(self, *args, options=options, **kwargs)
+        return asyncio.run(delete(self, *args, options=options, **kwargs))
 
 
 @get.register
-def get_sequence(
+async def get_sequence(
     client: BaseClient,
     objs: Sequence,
     options: ClientOptions = ClientOptions(),
 ) -> Sequence[T]:
-    result = [client.get(obj, options=options) for obj in objs]
+    result = await asyncio.gather(*[get(client, obj, options=options) for obj in objs])
     return result
 
 
 @delete.register
-def delete_sequence(
+async def delete_sequence(
     client: BaseClient,
     objs: Sequence,
     options: ClientOptions = ClientOptions(),
 ) -> None:
-    for obj in objs:
-        client.delete(obj, options=options)
+    await asyncio.gather(*[delete(client, obj, options=options) for obj in objs])
 
 
 @post.register
-def post_sequence(
+async def post_sequence(
     client: BaseClient,
     objs: Sequence,
     options: ClientOptions = ClientOptions(),
 ) -> List[T]:
-    result = [client.post(obj, options=options) for obj in objs]
+    result = await asyncio.gather(*[post(client, obj, options=options) for obj in objs])
     return result
 
 
 @patch.register
-def patch_sequence(
+async def patch_sequence(
     client: BaseClient,
     objs: Sequence,
     options: ClientOptions = ClientOptions(),
 ) -> List[T]:
-    result = [client.patch(obj, options=options) for obj in objs]
+    result = await asyncio.gather(*[patch(client, obj, options=options) for obj in objs])
     return result
 
 
 # -------------------------------------------- #
 
 
 @get.register
-def client_get_url(client: BaseClient, url: str, options: ClientOptions = ClientOptions()) -> requests.Response:
+async def client_get_url(client: BaseClient, url: str, options: ClientOptions = ClientOptions()) -> Response:
     headers = {**client.auth_headers, **options.headers}
 
     if "workspace" in options.payload:
         url = add_query_params(url, {"workspace": options.payload["workspace"]})
 
-    response = client.session.get(url, headers=headers, **options.request_args)
+    response = await client.session.get(url, headers=headers, **options.request_args)
     response_status_check(response)
     return response
 
 
 @delete.register
-def client_delete_url(client: BaseClient, url: str, options: ClientOptions = ClientOptions()) -> requests.Response:
+async def client_delete_url(client: BaseClient, url: str, options: ClientOptions = ClientOptions()) -> Response:
     headers = {**client.auth_headers, **options.headers}
 
-    response = client.session.delete(url, headers=headers, **options.request_args)
+    response = await client.session.delete(url, headers=headers, **options.request_args)
     response_status_check(response)
     return response
 
 
 @post.register
-def client_post_url(
+async def client_post_url(
     client: BaseClient,
     url: str,
     payload: Dict,
     options: ClientOptions = ClientOptions(),
-) -> requests.Response:
+) -> Response:
     headers = {
         **client.auth_headers,
         "Content-Type": "application/json",
         **options.headers,
     }
     payload = {**payload, **options.payload}
-    response = client.session.post(url, data=serialize_obj(payload), headers=headers)  # , **options.request_args
+    response = await client.session.post(
+        url, content=serialize_obj(payload), headers=headers
+    )  # , **options.request_args
 
     response_status_check(response)
     return response
 
 
 @patch.register
-def client_patch_url(
+async def client_patch_url(
     client: BaseClient,
     url: str,
     payload: Dict,
     options: ClientOptions = ClientOptions(),
-) -> requests.Response:
+) -> Response:
     headers = {
         **client.auth_headers,
         "Content-Type": "application/json",
         **options.headers,
     }
     payload = {**payload, **options.payload}
 
-    response = client.session.patch(url, data=serialize_obj(payload), headers=headers, **options.request_args)
+    response = await client.session.patch(url, content=serialize_obj(payload), headers=headers, **options.request_args)
 
     response_status_check(response)
     return response
```

### Comparing `grai_client-0.2.6/src/grai_client/endpoints/utilities.py` & `grai_client-0.2.7/src/grai_client/endpoints/utilities.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 import urllib
 import uuid
 from typing import Any, Dict, TypeVar, Union
 from uuid import UUID
 
 import orjson
 from grai_schemas.generics import GraiBaseModel
+from httpx import Response
 from pydantic import BaseModel
-from requests import RequestException, Response
+from requests import RequestException
 
 if sys.version_info < (3, 10):
     from typing_extensions import ParamSpec
 else:
     from typing import ParamSpec
 
 
@@ -33,15 +34,15 @@
         return False
 
 
 def response_status_check(resp: Response) -> Response:
     if resp.status_code in {200, 201, 204}:
         return resp
 
-    message = f"Error: {resp.status_code}. {resp.reason}. {resp.content.decode()}"
+    message = f"Error: {resp.status_code}. {resp.reason_phrase}. {resp.content.decode()}"
     if resp.status_code == 500:
         message = (
             f"{message}"
             "If you think this should not be the case it might be a bug, you can "
             "submit a bug report at https://github.com/grai-io/grai-core/issues"
         )
```

### Comparing `grai_client-0.2.6/src/grai_client/endpoints/v1/client.py` & `grai_client-0.2.7/src/grai_client/endpoints/v1/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+import asyncio
 from typing import Optional, Union
 from uuid import UUID, uuid4
 
-import requests
+from httpx import Response
 
 from grai_client.endpoints.client import BaseClient
 from grai_client.endpoints.utilities import is_valid_uuid
 
 
 class ClientV1(BaseClient):
     id = "v1"
@@ -21,31 +22,30 @@
         self.node_endpoint = f"{self.api}{self._node_endpoint}"
         self.edge_endpoint = f"{self.api}{self._edge_endpoint}"
         self.workspace_endpoint = f"{self.api}{self._workspace_endpoint}"
         self.is_authenticated_endpoint = f"{self.api}{self._is_authenticated_endpoint}"
 
         self._workspace = str(workspace) if workspace is not None else None
 
-    def check_authentication(self) -> requests.Response:
-        result = self.session.get(self.is_authenticated_endpoint, headers=self.auth_headers)
-        return result
+    def check_authentication(self) -> Response:
+        return asyncio.run(self.session.get(self.is_authenticated_endpoint, headers=self.auth_headers))
 
     @property
     def workspace(self) -> Optional[str]:
         return self._workspace
 
     @workspace.setter
     def workspace(self, workspace: Optional[Union[str, UUID]]):
         if workspace is None:
             self._workspace = workspace
             self.default_payload.pop("workspace", None)
             return
 
         if is_valid_uuid(workspace):
-            workspace = workspace
+            pass
         elif isinstance(workspace, str):
             result = self.get("workspace", workspace)
 
             if result is None:
                 raise Exception(f"No workspace matching `name={workspace}`")
             else:
                 workspace = result.id
```

### Comparing `grai_client-0.2.6/src/grai_client/endpoints/v1/get.py` & `grai_client-0.2.7/src/grai_client/endpoints/v1/get.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import asyncio
 from typing import Dict, List, Literal, Optional, TypeVar, Union
 
 from grai_schemas.v1 import EdgeV1, NodeV1
 from grai_schemas.v1.node import NodeIdTypes, NodeNamedID, NodeUuidID
 
 from grai_client.endpoints.client import ClientOptions
 from grai_client.endpoints.rest import get
@@ -10,40 +11,43 @@
 from grai_client.schemas.labels import EdgeLabels, NodeLabels, WorkspaceLabels
 from grai_client.schemas.workspace import Workspace
 
 T = TypeVar("T", NodeV1, EdgeV1)
 X = TypeVar("X")
 
 
-def query_obj_from_param_string(
+async def query_obj_from_param_string(
     client: ClientV1, base_url: str, options=ClientOptions(), **kwargs
 ) -> Optional[List[Dict]]:
     supported_params = ["name", "namespace"]
     query = "&".join([f"{param}={kwargs[param]}" for param in supported_params if param in kwargs])
 
     url = f"{base_url}?{query}"
-    resp = client.get(url, options=options).json()
+    resp = await get(client, url, options=options)
+    resp = resp.json()
+
     num_results = len(resp)
     if num_results == 0:
         return None
     else:
         return resp
 
 
-def get_node_from_id(
+async def get_node_from_id(
     client: ClientV1,
     grai_type: NodeIdTypes,
     options: Optional[ClientOptions] = ClientOptions(),
 ) -> Optional[Dict]:
     base_url = client.get_url(grai_type)
     if grai_type.id is not None:
-        url = f"{base_url}{grai_type.id}"
-        resp = client.get(url, options=options).json()
+        url = f"{base_url}{grai_type.id}/"
+        resp = await get(client, url, options=options)
+        resp = resp.json()
     else:
-        resp = query_obj_from_param_string(
+        resp = await query_obj_from_param_string(
             client, base_url, options=options, name=grai_type.name, namespace=grai_type.namespace
         )
 
         if resp is None:
             return None
         elif len(resp) == 1:
             return resp[0]
@@ -54,165 +58,180 @@
             )
             raise Exception(message)
 
     return resp
 
 
 @get.register
-def get_from_node_id(
+async def get_from_node_id(
     client: ClientV1, grai_type: NodeIdTypes, options: ClientOptions = ClientOptions()
 ) -> Optional[NodeV1]:
-    spec = get_node_from_id(client, grai_type, options=options)
+    spec = await get_node_from_id(client, grai_type, options=options)
     return NodeV1.from_spec(spec) if isinstance(spec, dict) else spec
 
 
 @get.register
-def get_node_v1(client: ClientV1, grai_type: NodeV1, options: ClientOptions = ClientOptions()) -> Optional[NodeV1]:
-    spec = get_node_from_id(client, grai_type.spec, options)
+async def get_node_v1(
+    client: ClientV1, grai_type: NodeV1, options: ClientOptions = ClientOptions()
+) -> Optional[NodeV1]:
+    spec = await get_node_from_id(client, grai_type.spec, options)
     return NodeV1.from_spec(spec) if isinstance(spec, dict) else spec
 
 
-def _get_nodes_by_name(
+async def _get_nodes_by_name(
     client: ClientV1,
     grai_type: NodeLabels,
     name: str,
     options: ClientOptions = ClientOptions(),
 ) -> Optional[List[NodeV1]]:
     url = f"{client.get_url(grai_type)}?name={name}"
-    resp = client.get(url, options=options).json()
+    resp = await get(client, url, options=options)
+    resp = resp.json()
     num_results = len(resp)
     if num_results == 0:
         return None
     else:
         return [NodeV1.from_spec(obj) for obj in resp]
 
 
-def _get_nodes_by_uuid(
+async def _get_nodes_by_uuid(
     client: ClientV1,
     grai_type: NodeLabels,
     name: str,
     options: ClientOptions = ClientOptions(),
 ) -> Optional[NodeV1]:
-    url = f"{client.get_url(grai_type)}{name}"
+    url = f"{client.get_url(grai_type)}{name}/"
 
-    resp = client.get(url, options=options).json()
+    resp = await get(client, url, options=options)
+    resp = resp.json()
     return NodeV1.from_spec(resp)
 
 
 @get.register
-def get_nodes_by_str(
+async def get_nodes_by_str(
     client: ClientV1,
     grai_type: NodeLabels,
     name: str,
     options: ClientOptions = ClientOptions(),
 ) -> Optional[Union[List[NodeV1], NodeV1]]:
     if is_valid_uuid(name):
-        return _get_nodes_by_uuid(client, grai_type, name, options=options)
+        return await _get_nodes_by_uuid(client, grai_type, name, options=options)
     else:
-        return _get_nodes_by_name(client, grai_type, name, options=options)
+        return await _get_nodes_by_name(client, grai_type, name, options=options)
 
 
 @get.register
-def get_nodes_by_namespace(
+async def get_nodes_by_namespace(
     client: ClientV1,
     grai_type: NodeLabels,
     name: Literal["*"],
     namespace: str,
     options: ClientOptions = ClientOptions(),
 ) -> Optional[List[NodeV1]]:
     base_url = client.get_url(grai_type)
-    results = query_obj_from_param_string(client, base_url, options=options, namespace=namespace)
+    results = await query_obj_from_param_string(client, base_url, options=options, namespace=namespace)
     if results is None:
         return results
 
     return [NodeV1.from_spec(result) for result in results]
 
 
 @get.register
-def get_nodes_by_name_and_namespace(
+async def get_nodes_by_name_and_namespace(
     client: ClientV1,
     grai_type: NodeLabels,
     name: str,
     namespace: str,
     options: ClientOptions = ClientOptions(),
 ) -> Optional[NodeV1]:
     node_id = NodeNamedID(name=name, namespace=namespace)
-    return client.get(node_id, options=options)
+    return await get(client, node_id, options=options)
 
 
 @get.register
-def get_node_by_label_v1(
+async def get_node_by_label_v1(
     client: ClientV1, grai_type: NodeLabels, options: ClientOptions = ClientOptions()
 ) -> List[NodeV1]:
     url = client.get_url(grai_type)
-    resp = client.get(url, options=options).json()
+    resp = await get(client, url, options=options)
+    resp = resp.json()
     return [NodeV1.from_spec(obj) for obj in resp]
 
 
 @get.register
-def get_edge_v1(client: ClientV1, grai_type: EdgeV1, options: ClientOptions = ClientOptions()) -> Optional[EdgeV1]:
+async def get_edge_v1(
+    client: ClientV1, grai_type: EdgeV1, options: ClientOptions = ClientOptions()
+) -> Optional[EdgeV1]:
     base_url = client.get_url(grai_type)
     if grai_type.spec.id is not None:
-        url = f"{base_url}{grai_type.spec.id}"
-        resp = client.get(url, options=options).json()
+        url = f"{base_url}{grai_type.spec.id}/"
+        resp = await get(client, url, options=options)
+        resp = resp.json()
     else:
         url = f"{base_url}?name={grai_type.spec.name}&namespace={grai_type.spec.namespace}"
-        resp = client.get(url, options=options).json()
+        resp = await get(client, url, options=options)
+        resp = resp.json()
         if len(resp) == 0:
             return None
         resp = resp[0]
 
-    resp["source"] = client.get("node", resp["source"]).spec
-    resp["destination"] = client.get("node", resp["destination"]).spec
+    nodes = await asyncio.gather(get(client, "node", resp["source"]), get(client, "node", resp["destination"]))
+    resp["source"] = nodes[0].spec
+    resp["destination"] = nodes[1].spec
     return EdgeV1.from_spec(resp)
 
 
 @get.register
-def get_edge_by_label_v1(
+async def get_edge_by_label_v1(
     client: ClientV1, grai_type: EdgeLabels, options: ClientOptions = ClientOptions()
 ) -> List[EdgeV1]:
     url = client.get_url(grai_type)
-    resp = client.get(url, options=options).json()
+    resp = await get(client, url, options=options)
+    resp = resp.json()
 
-    for r in resp:
-        r["source"] = client.get("node", r["source"]).spec
-        r["destination"] = client.get("node", r["destination"]).spec
+    groups = [asyncio.gather(get(client, "node", r["source"]), get(client, "node", r["destination"])) for r in resp]
+    nodes_groups = await asyncio.gather(*groups)
+    for r, node in zip(resp, nodes_groups):
+        r["source"] = node[0].spec
+        r["destination"] = node[1].spec
 
     return [EdgeV1.from_spec(obj) for obj in resp]
 
 
 @get.register
-def get_all_workspaces(
+async def get_all_workspaces(
     client: ClientV1,
     grai_type: WorkspaceLabels,
     options: ClientOptions = ClientOptions(),
 ) -> Optional[List[Workspace]]:
-    resp = client.get(client.get_url(grai_type), options=options).json()
+    resp = await get(client, client.get_url(grai_type), options=options)
+    resp = resp.json()
 
     if len(resp) == 0:
         return None
     else:
         return [Workspace(**item) for item in resp]
 
 
 @get.register
-def get_workspace_by_name_v1(
+async def get_workspace_by_name_v1(
     client: ClientV1,
     grai_type: WorkspaceLabels,
     name: str,
     options: ClientOptions = ClientOptions(),
 ) -> Optional[Workspace]:
     if is_valid_uuid(name):
-        url = f"{client.get_url(grai_type)}{name}"
+        url = f"{client.get_url(grai_type)}{name}/"
     elif len(name.split("/")) == 2:
         # this is a ref string i.e. org-name/workspace-name
         url = f"{client.get_url(grai_type)}?ref={name}"
     else:
         url = f"{client.get_url(grai_type)}?name={name}"
-    resp = client.get(url, options=options).json()
+    resp = await get(client, url, options=options)
+    resp = resp.json()
 
     num_resp = len(resp)
     if num_resp == 0:
         return None
     elif num_resp == 1:
         return Workspace(**resp[0])
     else:
```

### Comparing `grai_client-0.2.6/src/grai_client/endpoints/v1/patch.py` & `grai_client-0.2.7/src/grai_client/endpoints/v1/patch.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,55 @@
+import asyncio
 from typing import Optional, TypeVar
 
 from grai_schemas.v1 import EdgeV1, NodeV1
 
 from grai_client.endpoints.client import ClientOptions
-from grai_client.endpoints.rest import patch
+from grai_client.endpoints.rest import get, patch
 from grai_client.endpoints.v1.client import ClientV1
 from grai_client.endpoints.v1.utils import process_node_id
 
 T = TypeVar("T", NodeV1, EdgeV1)
 
 
 @patch.register
-def patch_node_v1(client: ClientV1, grai_type: NodeV1, options: ClientOptions = ClientOptions()) -> Optional[NodeV1]:
+async def patch_node_v1(
+    client: ClientV1, grai_type: NodeV1, options: ClientOptions = ClientOptions()
+) -> Optional[NodeV1]:
     if grai_type.spec.id is None:
-        current = client.get(grai_type)
+        current = await get(client, grai_type)
         grai_type.spec.id = current.spec.id
 
     url = f"{client.get_url(grai_type)}{grai_type.spec.id}/"
-    response = client.patch(url, grai_type.spec.dict(exclude_none=True), options=options).json()
+    response = await patch(client, url, grai_type.spec.dict(exclude_none=True), options=options)
+    response = response.json()
     if response is None:
         return None
     return NodeV1.from_spec(response)
 
 
 @patch.register
-def patch_edge_v1(client: ClientV1, grai_type: EdgeV1, options: ClientOptions = ClientOptions()) -> Optional[EdgeV1]:
+async def patch_edge_v1(
+    client: ClientV1, grai_type: EdgeV1, options: ClientOptions = ClientOptions()
+) -> Optional[EdgeV1]:
     if grai_type.spec.id is None:
-        current = client.get(grai_type)
+        current = await get(client, grai_type)
         grai_type.spec.id = current.spec.id
 
     url = f"{client.get_url(grai_type)}{grai_type.spec.id}/"
 
-    source = process_node_id(client, grai_type.spec.source)
-    destination = process_node_id(client, grai_type.spec.destination)
+    source, destination = await asyncio.gather(
+        process_node_id(client, grai_type.spec.source), process_node_id(client, grai_type.spec.destination)
+    )
 
     payload = grai_type.spec.dict(exclude_none=True)
     payload["source"] = source.id
     payload["destination"] = destination.id
 
-    response = client.patch(url, payload, options=options).json()
+    response = await patch(client, url, payload, options=options)
+    response = response.json()
     if response is None:
         return None
 
     response["source"] = source
     response["destination"] = destination
     return EdgeV1.from_spec(response)
```

### Comparing `grai_client-0.2.6/src/grai_client/endpoints/v1/post.py` & `grai_client-0.2.7/src/grai_client/endpoints/v1/post.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,40 @@
+import asyncio
 from typing import Optional
 
 from grai_schemas.v1 import EdgeV1, NodeV1
 
 from grai_client.endpoints.client import ClientOptions
 from grai_client.endpoints.rest import post
 from grai_client.endpoints.v1.client import ClientV1
 from grai_client.endpoints.v1.utils import process_node_id
 
 
 @post.register
-def post_node_v1(client: ClientV1, grai_type: NodeV1, options: ClientOptions = ClientOptions()) -> NodeV1:
+async def post_node_v1(client: ClientV1, grai_type: NodeV1, options: ClientOptions = ClientOptions()) -> NodeV1:
     url = client.get_url(grai_type)
-    response = client.post(url, grai_type.spec.dict(exclude_none=True), options=options)
+    response = await post(client, url, grai_type.spec.dict(exclude_none=True), options=options)
     return NodeV1.from_spec(response.json())
 
 
 @post.register
-def post_edge_v1(client: ClientV1, grai_type: EdgeV1, options: ClientOptions = ClientOptions()) -> Optional[EdgeV1]:
+async def post_edge_v1(
+    client: ClientV1, grai_type: EdgeV1, options: ClientOptions = ClientOptions()
+) -> Optional[EdgeV1]:
     url = client.get_url(grai_type)
 
-    source = process_node_id(client, grai_type.spec.source)
-    destination = process_node_id(client, grai_type.spec.destination)
+    source, destination = await asyncio.gather(
+        process_node_id(client, grai_type.spec.source), process_node_id(client, grai_type.spec.destination)
+    )
 
     payload = grai_type.spec.dict(exclude_none=True)
     payload["source"] = source.id
     payload["destination"] = destination.id
-    response = client.post(url, payload, options=options).json()
+    response = await post(client, url, payload, options=options)
+    response = response.json()
 
     if response is None:
         return None
 
     response["source"] = source
     response["destination"] = destination
     return EdgeV1.from_spec(response)
```

### Comparing `grai_client-0.2.6/src/grai_client/endpoints/v1/url.py` & `grai_client-0.2.7/src/grai_client/endpoints/v1/url.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.2.6/src/grai_client/endpoints/v1/utils.py` & `grai_client-0.2.7/src/grai_client/endpoints/v1/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 from grai_schemas.v1.node import NodeIdTypes
 
 from grai_client.endpoints.client import ClientOptions
+from grai_client.endpoints.rest import get
 from grai_client.endpoints.v1.client import ClientV1
 
 
-def process_node_id(client: ClientV1, grai_type: NodeIdTypes, options: ClientOptions = ClientOptions()) -> NodeIdTypes:
+async def process_node_id(
+    client: ClientV1, grai_type: NodeIdTypes, options: ClientOptions = ClientOptions()
+) -> NodeIdTypes:
     """
     Process a NodeID object, either by returning if it has a known id, or by getting
     the id from the server.
     """
     if grai_type.id is not None:
         return grai_type
 
-    server_node = client.get(grai_type, options=options)
+    server_node = await get(client, grai_type, options=options)
     if server_node is None:
         if grai_type.id is None:
             message = (
                 f"Could not find node with namespace=`{grai_type.namespace} " f"and name=`{grai_type.name}` on server"
             )
         else:
             message = f"Could not find node with id=`{grai_type.id}`"
```

### Comparing `grai_client-0.2.6/src/grai_client/testing/schema.py` & `grai_client-0.2.7/src/grai_client/testing/schema.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.2.6/src/grai_client/update.py` & `grai_client-0.2.7/src/grai_client/update.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.2.6/src/grai_client/utilities/tests.py` & `grai_client-0.2.7/src/grai_client/utilities/tests.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.2.6/setup.py` & `grai_client-0.2.7/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,24 +12,26 @@
  'grai_client.testing',
  'grai_client.utilities']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['grai-schemas>=0.1.8,<0.2.0',
+['brotli>=1.0.9,<2.0.0',
+ 'grai-schemas>=0.1.8,<0.2.0',
+ 'httpx>=0.23.3,<0.24.0',
  'multimethod==1.9',
  'orjson>=3.8.3,<4.0.0',
  'pydantic>=1.9.1,<2.0.0',
  'pyyaml>=6.0,<7.0',
  'requests>=2.28.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'grai-client',
-    'version': '0.2.6',
+    'version': '0.2.7',
     'description': '',
     'long_description': 'None',
     'author': 'Ian Eaves',
     'author_email': 'ian@grai.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `grai_client-0.2.6/PKG-INFO` & `grai_client-0.2.7/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: grai-client
-Version: 0.2.6
+Version: 0.2.7
 Summary: 
 License: Elastic-2.0
 Author: Ian Eaves
 Author-email: ian@grai.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: brotli (>=1.0.9,<2.0.0)
 Requires-Dist: grai-schemas (>=0.1.8,<0.2.0)
+Requires-Dist: httpx (>=0.23.3,<0.24.0)
 Requires-Dist: multimethod (==1.9)
 Requires-Dist: orjson (>=3.8.3,<4.0.0)
 Requires-Dist: pydantic (>=1.9.1,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
```

