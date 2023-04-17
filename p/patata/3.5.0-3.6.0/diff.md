# Comparing `tmp/patata-3.5.0.tar.gz` & `tmp/patata-3.6.0.tar.gz`

## Comparing `patata-3.5.0.tar` & `patata-3.6.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 patata-3.5.0/Makefile
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 patata-3.5.0/requirements-tox.txt
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 patata-3.5.0/tox.ini
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 patata-3.5.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 patata-3.5.0/patata/__init__.py
--rw-r--r--   0        0        0    11971 2020-02-02 00:00:00.000000 patata-3.5.0/patata/client.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 patata-3.5.0/patata/exceptions.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 patata-3.5.0/patata/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 patata-3.5.0/tests/__init__.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 patata-3.5.0/tests/test_client.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 patata-3.5.0/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 patata-3.5.0/LICENSE
--rw-r--r--   0        0        0     8303 2020-02-02 00:00:00.000000 patata-3.5.0/README.md
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 patata-3.5.0/pyproject.toml
--rw-r--r--   0        0        0    10643 2020-02-02 00:00:00.000000 patata-3.5.0/PKG-INFO
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 patata-3.6.0/Makefile
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 patata-3.6.0/requirements-tox.txt
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 patata-3.6.0/tox.ini
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 patata-3.6.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 patata-3.6.0/patata/__init__.py
+-rw-r--r--   0        0        0    12320 2020-02-02 00:00:00.000000 patata-3.6.0/patata/client.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 patata-3.6.0/patata/exceptions.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 patata-3.6.0/patata/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 patata-3.6.0/tests/__init__.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 patata-3.6.0/tests/test_client.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 patata-3.6.0/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 patata-3.6.0/LICENSE
+-rw-r--r--   0        0        0     8303 2020-02-02 00:00:00.000000 patata-3.6.0/README.md
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 patata-3.6.0/pyproject.toml
+-rw-r--r--   0        0        0    10643 2020-02-02 00:00:00.000000 patata-3.6.0/PKG-INFO
```

### Comparing `patata-3.5.0/tox.ini` & `patata-3.6.0/tox.ini`

 * *Files identical despite different names*

### Comparing `patata-3.5.0/.github/workflows/ci.yml` & `patata-3.6.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `patata-3.5.0/patata/client.py` & `patata-3.6.0/patata/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -263,16 +263,22 @@
 
         responses = asyncio.run(
             cls._make_requests_async(method.lower(), requests, verbose_level, retries)
         )
 
         for response in responses:
             for callback in callbacks:
-                response = callback(response)
-
+                try:
+                    response = callback(response)
+                except Exception as e:
+                    response.status_code = 500
+                    response.data = e
+                    if verbose_level > VERBOSE_LEVEL_INFO:
+                        logger.exception(e)
+                    break  # if a callback fails, don't process the next ones, keep the exception
         return responses
 
     @classmethod
     async def _make_requests_async(
         cls,
         method: str,
         requests: List[Request],
```

### Comparing `patata-3.5.0/LICENSE` & `patata-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `patata-3.5.0/README.md` & `patata-3.6.0/README.md`

 * *Files identical despite different names*

### Comparing `patata-3.5.0/pyproject.toml` & `patata-3.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "patata"
-version = "3.5.0"
+version = "3.6.0"
 description = "Simple lightweight HTTP client to perform GET or POST requests in parallel with multiprocessing and in each process use aiohttp to do them concurrently and maximize the throughtput."
 requires-python = ">=3.8"
 dependencies = [
     "aiohttp>=3.8.4,<4",
     "aiohttp_retry>=2.8.3,<3",
     "pydantic>=1.9,<2",
     'importlib-metadata; python_version<"3.9"',
```

### Comparing `patata-3.5.0/PKG-INFO` & `patata-3.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: patata
-Version: 3.5.0
+Version: 3.6.0
 Summary: Simple lightweight HTTP client to perform GET or POST requests in parallel with multiprocessing and in each process use aiohttp to do them concurrently and maximize the throughtput.
 Project-URL: repository, https://github.com/oalfonso-o/patata
 Project-URL: documentation, https://github.com/oalfonso-o/patata/blob/main/README.md
 Author-email: Oriol Alfonso <oriol@oalfonso.com>
 License: MIT License
         
         Copyright (c) 2023 Oriol Alfonso Riba
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: patata Version: 3.5.0 Summary: Simple lightweight
+Metadata-Version: 2.1 Name: patata Version: 3.6.0 Summary: Simple lightweight
 HTTP client to perform GET or POST requests in parallel with multiprocessing
 and in each process use aiohttp to do them concurrently and maximize the
 throughtput. Project-URL: repository, https://github.com/oalfonso-o/patata
 Project-URL: documentation, https://github.com/oalfonso-o/patata/blob/main/
 README.md Author-email: Oriol Alfonso
 oalfonso.com> License: MIT License Copyright (c) 2023 Oriol Alfonso Riba
 Permission is hereby granted, free of charge, to any person obtaining a copy of
```

