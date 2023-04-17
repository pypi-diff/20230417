# Comparing `tmp/neuroio-0.1.1.tar.gz` & `tmp/neuroio-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuroio-0.1.1.tar", max compression
+gzip compressed data, was "neuroio-0.1.2.tar", max compression
```

## Comparing `neuroio-0.1.1.tar` & `neuroio-0.1.2.tar`

### file list

```diff
@@ -1,45 +1,44 @@
--rw-r--r--   0        0        0     1095 2021-06-02 15:37:20.312100 neuroio-0.1.1/LICENSE
--rw-r--r--   0        0        0     7147 2022-04-08 10:47:51.486817 neuroio-0.1.1/README.md
--rw-r--r--   0        0        0      256 2022-04-08 10:47:51.489028 neuroio-0.1.1/neuroio/__init__.py
--rw-r--r--   0        0        0        0 2021-09-23 14:58:52.803004 neuroio-0.1.1/neuroio/auth/__init__.py
--rw-r--r--   0        0        0     1689 2021-09-23 14:58:52.803367 neuroio-0.1.1/neuroio/auth/v1.py
--rw-r--r--   0        0        0      644 2021-09-23 14:58:52.803633 neuroio-0.1.1/neuroio/auth_token.py
--rw-r--r--   0        0        0      804 2021-09-23 14:58:52.803955 neuroio-0.1.1/neuroio/base.py
--rw-r--r--   0        0        0        0 2021-09-23 14:58:52.804157 neuroio-0.1.1/neuroio/billing/__init__.py
--rw-r--r--   0        0        0     3077 2021-09-24 14:03:39.860944 neuroio-0.1.1/neuroio/billing/v1.py
--rw-r--r--   0        0        0     3206 2021-09-23 14:58:52.805870 neuroio-0.1.1/neuroio/clients.py
--rw-r--r--   0        0        0      934 2022-04-08 10:47:51.489873 neuroio-0.1.1/neuroio/constants.py
--rw-r--r--   0        0        0        0 2021-09-23 14:58:52.806609 neuroio-0.1.1/neuroio/entries/__init__.py
--rw-r--r--   0        0        0     2945 2021-09-23 14:58:52.807012 neuroio-0.1.1/neuroio/entries/v1.py
--rw-r--r--   0        0        0        0 2021-09-23 14:58:52.807244 neuroio-0.1.1/neuroio/groups/__init__.py
--rw-r--r--   0        0        0     4842 2021-09-23 14:58:52.807577 neuroio-0.1.1/neuroio/groups/v1.py
--rw-r--r--   0        0        0        0 2021-09-23 14:58:52.807806 neuroio-0.1.1/neuroio/licenses/__init__.py
--rw-r--r--   0        0        0        0 2021-09-23 14:58:52.807992 neuroio-0.1.1/neuroio/licenses/sources/__init__.py
--rw-r--r--   0        0        0     2959 2021-09-24 14:03:39.862469 neuroio-0.1.1/neuroio/licenses/sources/v1.py
--rw-r--r--   0        0        0     1804 2022-04-08 10:47:51.490501 neuroio-0.1.1/neuroio/listeners.py
--rw-r--r--   0        0        0        0 2021-09-23 14:58:52.808564 neuroio-0.1.1/neuroio/lists/__init__.py
--rw-r--r--   0        0        0        0 2021-09-23 14:58:52.808741 neuroio-0.1.1/neuroio/lists/spaces/__init__.py
--rw-r--r--   0        0        0      561 2021-09-23 14:58:52.809063 neuroio-0.1.1/neuroio/lists/spaces/v1.py
--rw-r--r--   0        0        0        0 2021-09-23 14:58:52.809301 neuroio-0.1.1/neuroio/notifications/__init__.py
--rw-r--r--   0        0        0     5193 2021-09-23 14:58:52.809725 neuroio-0.1.1/neuroio/notifications/v1.py
--rw-r--r--   0        0        0        0 2021-09-23 14:58:52.809961 neuroio-0.1.1/neuroio/persons/__init__.py
--rw-r--r--   0        0        0     4843 2021-09-23 14:58:52.810323 neuroio-0.1.1/neuroio/persons/v1.py
--rw-r--r--   0        0        0        0 2021-09-23 14:58:52.810569 neuroio-0.1.1/neuroio/settings/__init__.py
--rw-r--r--   0        0        0     1852 2021-09-23 14:58:52.810836 neuroio-0.1.1/neuroio/settings/v1.py
--rw-r--r--   0        0        0        0 2021-09-23 14:58:52.810993 neuroio-0.1.1/neuroio/sources/__init__.py
--rw-r--r--   0        0        0     7017 2021-10-28 13:08:32.669626 neuroio-0.1.1/neuroio/sources/v1.py
--rw-r--r--   0        0        0        0 2021-09-23 14:58:52.811581 neuroio-0.1.1/neuroio/spaces/__init__.py
--rw-r--r--   0        0        0     2822 2021-09-23 14:58:52.811789 neuroio-0.1.1/neuroio/spaces/v1.py
--rw-r--r--   0        0        0        0 2021-09-23 14:58:52.811945 neuroio-0.1.1/neuroio/streams/__init__.py
--rw-r--r--   0        0        0        0 2021-09-23 14:58:52.812099 neuroio-0.1.1/neuroio/streams/tokens/__init__.py
--rw-r--r--   0        0        0     3333 2021-09-23 14:58:52.812647 neuroio-0.1.1/neuroio/streams/tokens/v1.py
--rw-r--r--   0        0        0        0 2021-09-23 14:58:52.812869 neuroio-0.1.1/neuroio/tokens/__init__.py
--rw-r--r--   0        0        0     3299 2021-09-23 14:58:52.813230 neuroio-0.1.1/neuroio/tokens/v1.py
--rw-r--r--   0        0        0        0 2021-09-23 14:58:52.813464 neuroio-0.1.1/neuroio/utility/__init__.py
--rw-r--r--   0        0        0     1513 2021-09-23 14:58:52.813818 neuroio-0.1.1/neuroio/utility/v1.py
--rw-r--r--   0        0        0     2759 2022-04-08 10:47:51.491261 neuroio-0.1.1/neuroio/utils.py
--rw-r--r--   0        0        0        0 2021-09-23 14:58:52.814554 neuroio-0.1.1/neuroio/whoami/__init__.py
--rw-r--r--   0        0        0      538 2021-09-23 14:58:52.814988 neuroio-0.1.1/neuroio/whoami/v1.py
--rw-r--r--   0        0        0      728 2022-04-08 10:49:52.483186 neuroio-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     8414 2022-04-08 10:52:08.063823 neuroio-0.1.1/setup.py
--rw-r--r--   0        0        0     7712 2022-04-08 10:52:08.064399 neuroio-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1095 2023-01-15 07:01:23.996141 neuroio-0.1.2/LICENSE
+-rw-r--r--   0        0        0     7147 2023-01-15 07:01:23.996254 neuroio-0.1.2/README.md
+-rw-r--r--   0        0        0      256 2023-04-17 14:13:59.045019 neuroio-0.1.2/neuroio/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-15 07:01:23.998212 neuroio-0.1.2/neuroio/auth/__init__.py
+-rw-r--r--   0        0        0     1689 2023-01-15 07:01:23.998293 neuroio-0.1.2/neuroio/auth/v1.py
+-rw-r--r--   0        0        0      644 2023-01-15 07:01:23.998363 neuroio-0.1.2/neuroio/auth_token.py
+-rw-r--r--   0        0        0      804 2023-01-15 07:01:23.998429 neuroio-0.1.2/neuroio/base.py
+-rw-r--r--   0        0        0        0 2023-01-15 07:01:23.998493 neuroio-0.1.2/neuroio/billing/__init__.py
+-rw-r--r--   0        0        0     3077 2023-01-15 07:01:23.998575 neuroio-0.1.2/neuroio/billing/v1.py
+-rw-r--r--   0        0        0     3206 2023-01-15 07:01:23.998679 neuroio-0.1.2/neuroio/clients.py
+-rw-r--r--   0        0        0      934 2023-01-15 07:01:23.998756 neuroio-0.1.2/neuroio/constants.py
+-rw-r--r--   0        0        0        0 2023-01-15 07:01:23.998825 neuroio-0.1.2/neuroio/entries/__init__.py
+-rw-r--r--   0        0        0     2945 2023-01-15 07:01:23.998926 neuroio-0.1.2/neuroio/entries/v1.py
+-rw-r--r--   0        0        0        0 2023-01-15 07:01:23.998989 neuroio-0.1.2/neuroio/groups/__init__.py
+-rw-r--r--   0        0        0     4842 2023-01-15 07:01:23.999070 neuroio-0.1.2/neuroio/groups/v1.py
+-rw-r--r--   0        0        0        0 2023-01-15 07:01:23.999132 neuroio-0.1.2/neuroio/licenses/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-15 07:01:23.999203 neuroio-0.1.2/neuroio/licenses/sources/__init__.py
+-rw-r--r--   0        0        0     2959 2023-01-15 07:01:23.999275 neuroio-0.1.2/neuroio/licenses/sources/v1.py
+-rw-r--r--   0        0        0     1804 2023-01-15 07:01:23.999347 neuroio-0.1.2/neuroio/listeners.py
+-rw-r--r--   0        0        0        0 2023-01-15 07:01:23.999410 neuroio-0.1.2/neuroio/lists/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-15 07:01:23.999482 neuroio-0.1.2/neuroio/lists/spaces/__init__.py
+-rw-r--r--   0        0        0      561 2023-01-15 07:01:23.999561 neuroio-0.1.2/neuroio/lists/spaces/v1.py
+-rw-r--r--   0        0        0        0 2023-01-15 07:01:23.999624 neuroio-0.1.2/neuroio/notifications/__init__.py
+-rw-r--r--   0        0        0     5193 2023-01-15 07:01:23.999689 neuroio-0.1.2/neuroio/notifications/v1.py
+-rw-r--r--   0        0        0        0 2023-01-15 07:01:23.999749 neuroio-0.1.2/neuroio/persons/__init__.py
+-rw-r--r--   0        0        0     4843 2023-01-15 07:01:23.999859 neuroio-0.1.2/neuroio/persons/v1.py
+-rw-r--r--   0        0        0        0 2023-01-15 07:01:23.999920 neuroio-0.1.2/neuroio/settings/__init__.py
+-rw-r--r--   0        0        0     1852 2023-01-15 07:01:24.000003 neuroio-0.1.2/neuroio/settings/v1.py
+-rw-r--r--   0        0        0        0 2023-01-15 07:01:24.000070 neuroio-0.1.2/neuroio/sources/__init__.py
+-rw-r--r--   0        0        0     7017 2023-01-15 07:01:24.000185 neuroio-0.1.2/neuroio/sources/v1.py
+-rw-r--r--   0        0        0        0 2023-01-15 07:01:24.000247 neuroio-0.1.2/neuroio/spaces/__init__.py
+-rw-r--r--   0        0        0     2822 2023-01-15 07:01:24.000324 neuroio-0.1.2/neuroio/spaces/v1.py
+-rw-r--r--   0        0        0        0 2023-01-15 07:01:24.000387 neuroio-0.1.2/neuroio/streams/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-15 07:01:24.000460 neuroio-0.1.2/neuroio/streams/tokens/__init__.py
+-rw-r--r--   0        0        0     3437 2023-04-17 14:13:01.524238 neuroio-0.1.2/neuroio/streams/tokens/v1.py
+-rw-r--r--   0        0        0        0 2023-01-15 07:01:24.000601 neuroio-0.1.2/neuroio/tokens/__init__.py
+-rw-r--r--   0        0        0     3403 2023-04-17 14:12:40.875819 neuroio-0.1.2/neuroio/tokens/v1.py
+-rw-r--r--   0        0        0        0 2023-01-15 07:01:24.000746 neuroio-0.1.2/neuroio/utility/__init__.py
+-rw-r--r--   0        0        0     1513 2023-01-15 07:01:24.000826 neuroio-0.1.2/neuroio/utility/v1.py
+-rw-r--r--   0        0        0     2759 2023-01-15 07:01:24.000923 neuroio-0.1.2/neuroio/utils.py
+-rw-r--r--   0        0        0        0 2023-01-15 07:01:24.000984 neuroio-0.1.2/neuroio/whoami/__init__.py
+-rw-r--r--   0        0        0      538 2023-01-15 07:01:24.001051 neuroio-0.1.2/neuroio/whoami/v1.py
+-rw-r--r--   0        0        0      728 2023-04-17 14:13:17.416849 neuroio-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     7814 1970-01-01 00:00:00.000000 neuroio-0.1.2/PKG-INFO
```

### Comparing `neuroio-0.1.1/LICENSE` & `neuroio-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `neuroio-0.1.1/README.md` & `neuroio-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `neuroio-0.1.1/neuroio/auth/v1.py` & `neuroio-0.1.2/neuroio/auth/v1.py`

 * *Files identical despite different names*

### Comparing `neuroio-0.1.1/neuroio/auth_token.py` & `neuroio-0.1.2/neuroio/auth_token.py`

 * *Files identical despite different names*

### Comparing `neuroio-0.1.1/neuroio/base.py` & `neuroio-0.1.2/neuroio/base.py`

 * *Files identical despite different names*

### Comparing `neuroio-0.1.1/neuroio/billing/v1.py` & `neuroio-0.1.2/neuroio/billing/v1.py`

 * *Files identical despite different names*

### Comparing `neuroio-0.1.1/neuroio/clients.py` & `neuroio-0.1.2/neuroio/clients.py`

 * *Files identical despite different names*

### Comparing `neuroio-0.1.1/neuroio/constants.py` & `neuroio-0.1.2/neuroio/constants.py`

 * *Files identical despite different names*

### Comparing `neuroio-0.1.1/neuroio/entries/v1.py` & `neuroio-0.1.2/neuroio/entries/v1.py`

 * *Files identical despite different names*

### Comparing `neuroio-0.1.1/neuroio/groups/v1.py` & `neuroio-0.1.2/neuroio/groups/v1.py`

 * *Files identical despite different names*

### Comparing `neuroio-0.1.1/neuroio/licenses/sources/v1.py` & `neuroio-0.1.2/neuroio/licenses/sources/v1.py`

 * *Files identical despite different names*

### Comparing `neuroio-0.1.1/neuroio/listeners.py` & `neuroio-0.1.2/neuroio/listeners.py`

 * *Files identical despite different names*

### Comparing `neuroio-0.1.1/neuroio/lists/spaces/v1.py` & `neuroio-0.1.2/neuroio/lists/spaces/v1.py`

 * *Files identical despite different names*

### Comparing `neuroio-0.1.1/neuroio/notifications/v1.py` & `neuroio-0.1.2/neuroio/notifications/v1.py`

 * *Files identical despite different names*

### Comparing `neuroio-0.1.1/neuroio/persons/v1.py` & `neuroio-0.1.2/neuroio/persons/v1.py`

 * *Files identical despite different names*

### Comparing `neuroio-0.1.1/neuroio/settings/v1.py` & `neuroio-0.1.2/neuroio/settings/v1.py`

 * *Files identical despite different names*

### Comparing `neuroio-0.1.1/neuroio/sources/v1.py` & `neuroio-0.1.2/neuroio/sources/v1.py`

 * *Files identical despite different names*

### Comparing `neuroio-0.1.1/neuroio/spaces/v1.py` & `neuroio-0.1.2/neuroio/spaces/v1.py`

 * *Files identical despite different names*

### Comparing `neuroio-0.1.1/neuroio/streams/tokens/v1.py` & `neuroio-0.1.2/neuroio/tokens/v1.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 from typing import Union
 
 from httpx import Response
 
-from neuroio.base import APIBase, APIBaseAsync, APIBaseBase
+from neuroio.base import IAMBase, IAMBaseAsync, IAMBaseBase
 
 
-class StreamTokensBase(APIBaseBase):
+class TokensBase(IAMBaseBase):
     def get_url(self, key: str = None) -> str:
         if key:
-            return self.base_url + f"/v1/streams/tokens/{key}/"
+            return self.base_url + f"/v1/tokens/{key}/"
         else:
-            return self.base_url + "/v1/streams/tokens/"
+            return self.base_url + "/v1/tokens/"
 
 
-class Impl(APIBase, StreamTokensBase):
+class Impl(IAMBase, TokensBase):
     def create(self, permanent: bool = False) -> Response:
         data = {"permanent": permanent}
 
         with self.get_client() as client:
             return client.post(url=self.get_url(), json=data)
 
     def list(
         self, permanent: bool = None, limit: int = 20, offset: int = 0
     ) -> Response:
-        data = {"permanent": permanent, "limit": limit, "offset": offset}
+        data = {"limit": limit, "offset": offset}
+        if permanent is not None:
+            data["permanent"] = permanent
 
         with self.get_client() as client:
             return client.get(url=self.get_url(), params=data)
 
     def get(self, token_id_or_key: Union[int, str]) -> Response:
         with self.get_client() as client:
             return client.get(url=self.get_url(f"{token_id_or_key}"))
@@ -48,25 +50,27 @@
             return client.delete(url=self.get_url(), params=data)
 
     def delete(self, token_id_or_key: Union[int, str]) -> Response:
         with self.get_client() as client:
             return client.delete(url=self.get_url(f"{token_id_or_key}"))
 
 
-class ImplAsync(APIBaseAsync, StreamTokensBase):
+class ImplAsync(IAMBaseAsync, TokensBase):
     async def create(self, permanent: bool = False) -> Response:
         data = {"permanent": permanent}
 
         async with self.get_client() as client:
             return await client.post(url=self.get_url(), json=data)
 
     async def list(
         self, permanent: bool = None, limit: int = 20, offset: int = 0
     ) -> Response:
-        data = {"permanent": permanent, "limit": limit, "offset": offset}
+        data = {"limit": limit, "offset": offset}
+        if permanent is not None:
+            data["permanent"] = permanent
 
         async with self.get_client() as client:
             return await client.get(url=self.get_url(), params=data)
 
     async def get(self, token_id_or_key: Union[int, str]) -> Response:
         async with self.get_client() as client:
             return await client.get(url=self.get_url(f"{token_id_or_key}"))
```

### Comparing `neuroio-0.1.1/neuroio/tokens/v1.py` & `neuroio-0.1.2/neuroio/streams/tokens/v1.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 from typing import Union
 
 from httpx import Response
 
-from neuroio.base import IAMBase, IAMBaseAsync, IAMBaseBase
+from neuroio.base import APIBase, APIBaseAsync, APIBaseBase
 
 
-class TokensBase(IAMBaseBase):
+class StreamTokensBase(APIBaseBase):
     def get_url(self, key: str = None) -> str:
         if key:
-            return self.base_url + f"/v1/tokens/{key}/"
+            return self.base_url + f"/v1/streams/tokens/{key}/"
         else:
-            return self.base_url + "/v1/tokens/"
+            return self.base_url + "/v1/streams/tokens/"
 
 
-class Impl(IAMBase, TokensBase):
+class Impl(APIBase, StreamTokensBase):
     def create(self, permanent: bool = False) -> Response:
         data = {"permanent": permanent}
 
         with self.get_client() as client:
             return client.post(url=self.get_url(), json=data)
 
     def list(
         self, permanent: bool = None, limit: int = 20, offset: int = 0
     ) -> Response:
-        data = {"permanent": permanent, "limit": limit, "offset": offset}
+        data = {"limit": limit, "offset": offset}
+        if permanent is not None:
+            data["permanent"] = permanent
 
         with self.get_client() as client:
             return client.get(url=self.get_url(), params=data)
 
     def get(self, token_id_or_key: Union[int, str]) -> Response:
         with self.get_client() as client:
             return client.get(url=self.get_url(f"{token_id_or_key}"))
@@ -48,25 +50,27 @@
             return client.delete(url=self.get_url(), params=data)
 
     def delete(self, token_id_or_key: Union[int, str]) -> Response:
         with self.get_client() as client:
             return client.delete(url=self.get_url(f"{token_id_or_key}"))
 
 
-class ImplAsync(IAMBaseAsync, TokensBase):
+class ImplAsync(APIBaseAsync, StreamTokensBase):
     async def create(self, permanent: bool = False) -> Response:
         data = {"permanent": permanent}
 
         async with self.get_client() as client:
             return await client.post(url=self.get_url(), json=data)
 
     async def list(
         self, permanent: bool = None, limit: int = 20, offset: int = 0
     ) -> Response:
-        data = {"permanent": permanent, "limit": limit, "offset": offset}
+        data = {"limit": limit, "offset": offset}
+        if permanent is not None:
+            data["permanent"] = permanent
 
         async with self.get_client() as client:
             return await client.get(url=self.get_url(), params=data)
 
     async def get(self, token_id_or_key: Union[int, str]) -> Response:
         async with self.get_client() as client:
             return await client.get(url=self.get_url(f"{token_id_or_key}"))
```

### Comparing `neuroio-0.1.1/neuroio/utility/v1.py` & `neuroio-0.1.2/neuroio/utility/v1.py`

 * *Files identical despite different names*

### Comparing `neuroio-0.1.1/neuroio/utils.py` & `neuroio-0.1.2/neuroio/utils.py`

 * *Files identical despite different names*

### Comparing `neuroio-0.1.1/neuroio/whoami/v1.py` & `neuroio-0.1.2/neuroio/whoami/v1.py`

 * *Files identical despite different names*

### Comparing `neuroio-0.1.1/pyproject.toml` & `neuroio-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neuroio"
-version = "0.1.1"
+version = "0.1.2"
 description = "A Python package for interacting with NeuroIO API"
 authors = ["Lev Rubel <l@datacorp.ee>", "Roman Lyalin <rly@datacorp.ee>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7.0"
```

### Comparing `neuroio-0.1.1/setup.py` & `neuroio-0.1.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,251 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: neuroio
+Version: 0.1.2
+Summary: A Python package for interacting with NeuroIO API
+License: MIT
+Author: Lev Rubel
+Author-email: l@datacorp.ee
+Requires-Python: >=3.7.0,<4.0.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: httpx (>=0.19.0)
+Requires-Dist: websockets (>=10.0,<11.0)
+Description-Content-Type: text/markdown
+
+# Python API client for NeuroIO
+
+
+[![PyPI version](https://badge.fury.io/py/neuroio.svg)](http://badge.fury.io/py/neuroio)
+[![codecov](https://codecov.io/gh/neuroio/neuroio-python/branch/master/graph/badge.svg)](https://codecov.io/gh/neuroio/neuroio-python)
+[![License](https://img.shields.io/github/license/mashape/apistatus.svg)](https://pypi.python.org/pypi/neuroio/)
+[![Downloads](https://pepy.tech/badge/neuroio)](https://pepy.tech/project/neuroio)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://timothycrosley.github.io/isort/)
+
+_________________
+
+[Read Latest Documentation](https://neuroio.github.io/neuroio-python/) - [Browse GitHub Code Repository](https://github.com/neuroio/neuroio-python/)
+_________________
+
+This library strives to be a complete mirror of official NeuroIO API in terms of methods and interfaces.
+
+Official latest API documentation can be found [here](https://kb.neuroio.com/).
+
+For your convenience, you can make API calls using sync or async (asyncio) interface.
+
+## Installation
+
+```sh
+pip install neuroio
+```
+
+Note that it is always recommended pinning version of your installed packages.
+
+## Usage example (sync)
+
+An example of how to create a source:
+
+```python
+from neuroio import Client
+
+
+if __name__ == '__main__':
+    # api_token is just str with your API token from NeuroIO
+    api_token = "abcd012345"
+    # Now create instance of Client. There should be only one per process.
+    client = Client(api_token=api_token)
+    # Issue API request to create source
+    client.sources.create(name="test_name")
+
+```
+
+Now that we have our source created, we can create person inside that source:
+
+```python
+from neuroio import Client
+
+
+def create_persons_example(client: Client):
+    source_name = "test_name"
+    with open("image.png", "rb") as f:
+        response = client.persons.create(
+            image=f,
+            source=source_name,
+            facesize=1000,
+            create_on_ha=True,
+            create_on_junk=True,
+            identify_asm=True
+        )
+    print("Persons Create Response:\n", response.json(), flush=True)
+
+
+if __name__ == '__main__':
+    # api_token is just str with your API token from NeuroIO
+    api_token = "abcd012345"
+    # Now create instance of Client. There should be only one per process.
+    client = Client(api_token=api_token)
+    # Issue API request to create a person
+    create_persons_example(client)
+
+```
+
+Now that we have our source & person created, we can search for persons:
+
+```python
+from neuroio import Client
+
+
+def search_persons_example(client: Client):
+    with open("image.png", "rb") as f:
+        response = client.persons.search(
+            image=f,
+            identify_asm=True
+        )
+    print("Persons Search Response:\n", response.json(), flush=True)
+
+
+if __name__ == '__main__':
+    # api_token is just str with your API token from NeuroIO
+    api_token = "abcd012345"
+    # Now create instance of Client. There should be only one per process.
+    client = Client(api_token=api_token)
+    # Issue API request to search persons
+    search_persons_example(client)
+
+```
+
+An example of how to listen for events:
+
+```python
+import asyncio
+import json
+import logging
+import signal
+
+from neuroio import EventListener
+
+
+async def event_handler_func(event_message: str):
+    # NOTE: this must be awaitable and accept single param Union[str, bytes]
+    json_message = json.loads(event_message)
+    is_ping_response = "PING" in json_message.keys()
+    is_auth_response = "auth" in json_message.keys()
+    is_error_response = "error" in json_message.keys()
+    if is_ping_response:
+        if json_message["PING"] != "PONG":
+            # something is wrong with socket connection
+            raise RuntimeError()
+        else:
+            # this is correct pong response on our periodic pings
+            logging.info("Connection is alive")
+    elif is_auth_response:
+        logging.info("Authorized successfully")
+    elif is_error_response:
+        # something is wrong with provided token
+        logging.info(json_message["error"], flush=True)
+    else:
+        # this must be event about entry itself
+        # now you can inspect json_message for information about that
+        logging.info(json_message["data"]["face_image"])
+
+
+async def shutdown(signal, loop):
+    """Cleanup tasks tied to the service's shutdown."""
+    logging.info(f"Received exit signal {signal.name}...")
+    tasks = [t for t in asyncio.all_tasks() if t is not asyncio.current_task()]
+
+    [task.cancel() for task in tasks]
+
+    logging.info(f"Cancelling {len(tasks)} outstanding tasks")
+    await asyncio.gather(*tasks, return_exceptions=True)
+    loop.stop()
+
+
+if __name__ == "__main__":
+    logging.getLogger().setLevel(logging.INFO)
+    
+    # NOTE: You are advised to hook-up uvloop here for improved performance
+    
+    api_token = "1234567890"
+    events_listener = EventListener(
+        api_token=api_token, event_handler_func=event_handler_func
+    )
+
+    loop = asyncio.get_event_loop()
+    # May want to catch other signals too
+    signals = (signal.SIGHUP, signal.SIGTERM, signal.SIGINT)
+    for s in signals:
+        loop.add_signal_handler(
+            s, lambda _s=s: asyncio.create_task(shutdown(_s, loop))
+        )
+
+    try:
+        loop.create_task(events_listener.listen())
+        loop.run_forever()
+    finally:
+        loop.close()
+        logging.info("Successfully shutdown")
+
+
+```
+
+_For more examples and usage, please refer to the [docs](https://neuroio.github.io/neuroio-python/)._
+
+## Development setup
+
+To install all the development requirements:
+
+```sh
+pip install --upgrade pip
+pip install poetry
+poetry install --no-root
+```
+
+To run linters & test suite:
+
+```sh
+./scripts/test.sh
+```
+
+## Release History
+* 0.1.0
+    * Support for WebSocket Events
+    * Drop Python 3.6 support
+* 0.0.9
+    * Fixes to the sources API in terms of required fields
+* 0.0.8
+    * Updated library to latest API version (at the time of this release - 1.3.1)
+    * Updated README & docs
+* 0.0.7
+    * Updated library to latest API version (at the time of this release - 1.3.0)
+    * Updated requirements
+    * Updated README & docs
+* 0.0.6
+    * Updated library to latest API version (at the time of this release - 1.2.1)
+    * Updated README & docs
+* 0.0.5
+    * Fixed persistent connection problems
+    * Updated requirements
+    * Codebase cleanup
+* 0.0.4
+    * Changed the way how we treat httpx connection - now we don't close it after every request (which was supposedly right way in httpx docs)
+* 0.0.3
+    * Updated httpx version, disabled cruft check since it just messes up project files
+
+## License
+
+Distributed under the MIT license. See ``LICENSE`` for more information.
+
+## Contributing
+
+1. Fork it (<https://github.com/yourname/yourproject/fork>)
+2. Create your feature branch (`git checkout -b feature/fooBar`)
+3. Commit your changes (`git commit -am 'Add some fooBar'`)
+4. Push to the branch (`git push origin feature/fooBar`)
+5. Create a new Pull Request
 
-packages = \
-['neuroio',
- 'neuroio.auth',
- 'neuroio.billing',
- 'neuroio.entries',
- 'neuroio.groups',
- 'neuroio.licenses',
- 'neuroio.licenses.sources',
- 'neuroio.lists',
- 'neuroio.lists.spaces',
- 'neuroio.notifications',
- 'neuroio.persons',
- 'neuroio.settings',
- 'neuroio.sources',
- 'neuroio.spaces',
- 'neuroio.streams',
- 'neuroio.streams.tokens',
- 'neuroio.tokens',
- 'neuroio.utility',
- 'neuroio.whoami']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['httpx>=0.19.0', 'websockets>=10.0,<11.0']
-
-setup_kwargs = {
-    'name': 'neuroio',
-    'version': '0.1.1',
-    'description': 'A Python package for interacting with NeuroIO API',
-    'long_description': '# Python API client for NeuroIO\n\n\n[![PyPI version](https://badge.fury.io/py/neuroio.svg)](http://badge.fury.io/py/neuroio)\n[![codecov](https://codecov.io/gh/neuroio/neuroio-python/branch/master/graph/badge.svg)](https://codecov.io/gh/neuroio/neuroio-python)\n[![License](https://img.shields.io/github/license/mashape/apistatus.svg)](https://pypi.python.org/pypi/neuroio/)\n[![Downloads](https://pepy.tech/badge/neuroio)](https://pepy.tech/project/neuroio)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://timothycrosley.github.io/isort/)\n\n_________________\n\n[Read Latest Documentation](https://neuroio.github.io/neuroio-python/) - [Browse GitHub Code Repository](https://github.com/neuroio/neuroio-python/)\n_________________\n\nThis library strives to be a complete mirror of official NeuroIO API in terms of methods and interfaces.\n\nOfficial latest API documentation can be found [here](https://kb.neuroio.com/).\n\nFor your convenience, you can make API calls using sync or async (asyncio) interface.\n\n## Installation\n\n```sh\npip install neuroio\n```\n\nNote that it is always recommended pinning version of your installed packages.\n\n## Usage example (sync)\n\nAn example of how to create a source:\n\n```python\nfrom neuroio import Client\n\n\nif __name__ == \'__main__\':\n    # api_token is just str with your API token from NeuroIO\n    api_token = "abcd012345"\n    # Now create instance of Client. There should be only one per process.\n    client = Client(api_token=api_token)\n    # Issue API request to create source\n    client.sources.create(name="test_name")\n\n```\n\nNow that we have our source created, we can create person inside that source:\n\n```python\nfrom neuroio import Client\n\n\ndef create_persons_example(client: Client):\n    source_name = "test_name"\n    with open("image.png", "rb") as f:\n        response = client.persons.create(\n            image=f,\n            source=source_name,\n            facesize=1000,\n            create_on_ha=True,\n            create_on_junk=True,\n            identify_asm=True\n        )\n    print("Persons Create Response:\\n", response.json(), flush=True)\n\n\nif __name__ == \'__main__\':\n    # api_token is just str with your API token from NeuroIO\n    api_token = "abcd012345"\n    # Now create instance of Client. There should be only one per process.\n    client = Client(api_token=api_token)\n    # Issue API request to create a person\n    create_persons_example(client)\n\n```\n\nNow that we have our source & person created, we can search for persons:\n\n```python\nfrom neuroio import Client\n\n\ndef search_persons_example(client: Client):\n    with open("image.png", "rb") as f:\n        response = client.persons.search(\n            image=f,\n            identify_asm=True\n        )\n    print("Persons Search Response:\\n", response.json(), flush=True)\n\n\nif __name__ == \'__main__\':\n    # api_token is just str with your API token from NeuroIO\n    api_token = "abcd012345"\n    # Now create instance of Client. There should be only one per process.\n    client = Client(api_token=api_token)\n    # Issue API request to search persons\n    search_persons_example(client)\n\n```\n\nAn example of how to listen for events:\n\n```python\nimport asyncio\nimport json\nimport logging\nimport signal\n\nfrom neuroio import EventListener\n\n\nasync def event_handler_func(event_message: str):\n    # NOTE: this must be awaitable and accept single param Union[str, bytes]\n    json_message = json.loads(event_message)\n    is_ping_response = "PING" in json_message.keys()\n    is_auth_response = "auth" in json_message.keys()\n    is_error_response = "error" in json_message.keys()\n    if is_ping_response:\n        if json_message["PING"] != "PONG":\n            # something is wrong with socket connection\n            raise RuntimeError()\n        else:\n            # this is correct pong response on our periodic pings\n            logging.info("Connection is alive")\n    elif is_auth_response:\n        logging.info("Authorized successfully")\n    elif is_error_response:\n        # something is wrong with provided token\n        logging.info(json_message["error"], flush=True)\n    else:\n        # this must be event about entry itself\n        # now you can inspect json_message for information about that\n        logging.info(json_message["data"]["face_image"])\n\n\nasync def shutdown(signal, loop):\n    """Cleanup tasks tied to the service\'s shutdown."""\n    logging.info(f"Received exit signal {signal.name}...")\n    tasks = [t for t in asyncio.all_tasks() if t is not asyncio.current_task()]\n\n    [task.cancel() for task in tasks]\n\n    logging.info(f"Cancelling {len(tasks)} outstanding tasks")\n    await asyncio.gather(*tasks, return_exceptions=True)\n    loop.stop()\n\n\nif __name__ == "__main__":\n    logging.getLogger().setLevel(logging.INFO)\n    \n    # NOTE: You are advised to hook-up uvloop here for improved performance\n    \n    api_token = "1234567890"\n    events_listener = EventListener(\n        api_token=api_token, event_handler_func=event_handler_func\n    )\n\n    loop = asyncio.get_event_loop()\n    # May want to catch other signals too\n    signals = (signal.SIGHUP, signal.SIGTERM, signal.SIGINT)\n    for s in signals:\n        loop.add_signal_handler(\n            s, lambda _s=s: asyncio.create_task(shutdown(_s, loop))\n        )\n\n    try:\n        loop.create_task(events_listener.listen())\n        loop.run_forever()\n    finally:\n        loop.close()\n        logging.info("Successfully shutdown")\n\n\n```\n\n_For more examples and usage, please refer to the [docs](https://neuroio.github.io/neuroio-python/)._\n\n## Development setup\n\nTo install all the development requirements:\n\n```sh\npip install --upgrade pip\npip install poetry\npoetry install --no-root\n```\n\nTo run linters & test suite:\n\n```sh\n./scripts/test.sh\n```\n\n## Release History\n* 0.1.0\n    * Support for WebSocket Events\n    * Drop Python 3.6 support\n* 0.0.9\n    * Fixes to the sources API in terms of required fields\n* 0.0.8\n    * Updated library to latest API version (at the time of this release - 1.3.1)\n    * Updated README & docs\n* 0.0.7\n    * Updated library to latest API version (at the time of this release - 1.3.0)\n    * Updated requirements\n    * Updated README & docs\n* 0.0.6\n    * Updated library to latest API version (at the time of this release - 1.2.1)\n    * Updated README & docs\n* 0.0.5\n    * Fixed persistent connection problems\n    * Updated requirements\n    * Codebase cleanup\n* 0.0.4\n    * Changed the way how we treat httpx connection - now we don\'t close it after every request (which was supposedly right way in httpx docs)\n* 0.0.3\n    * Updated httpx version, disabled cruft check since it just messes up project files\n\n## License\n\nDistributed under the MIT license. See ``LICENSE`` for more information.\n\n## Contributing\n\n1. Fork it (<https://github.com/yourname/yourproject/fork>)\n2. Create your feature branch (`git checkout -b feature/fooBar`)\n3. Commit your changes (`git commit -am \'Add some fooBar\'`)\n4. Push to the branch (`git push origin feature/fooBar`)\n5. Create a new Pull Request\n',
-    'author': 'Lev Rubel',
-    'author_email': 'l@datacorp.ee',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7.0,<4.0.0',
-}
-
-
-setup(**setup_kwargs)
```

