# Comparing `tmp/flask_pydantic_spec-0.4.3.tar.gz` & `tmp/flask_pydantic_spec-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_pydantic_spec-0.4.3.tar", last modified: Tue Mar 14 09:28:23 2023, max compression
+gzip compressed data, was "flask_pydantic_spec-0.4.4.tar", last modified: Mon Apr 17 10:03:22 2023, max compression
```

## Comparing `flask_pydantic_spec-0.4.3.tar` & `flask_pydantic_spec-0.4.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 09:28:23.144933 flask_pydantic_spec-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11436 2023-03-14 09:28:15.000000 flask_pydantic_spec-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7265 2023-03-14 09:28:23.144933 flask_pydantic_spec-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-03-14 09:28:15.000000 flask_pydantic_spec-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 09:28:23.144933 flask_pydantic_spec-0.4.3/flask_pydantic_spec/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-03-14 09:28:15.000000 flask_pydantic_spec-0.4.3/flask_pydantic_spec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-03-14 09:28:15.000000 flask_pydantic_spec-0.4.3/flask_pydantic_spec/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7317 2023-03-14 09:28:15.000000 flask_pydantic_spec-0.4.3/flask_pydantic_spec/flask_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-03-14 09:28:15.000000 flask_pydantic_spec-0.4.3/flask_pydantic_spec/page.py
--rw-r--r--   0 runner    (1001) docker     (123)    11906 2023-03-14 09:28:15.000000 flask_pydantic_spec-0.4.3/flask_pydantic_spec/spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-03-14 09:28:15.000000 flask_pydantic_spec-0.4.3/flask_pydantic_spec/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7984 2023-03-14 09:28:15.000000 flask_pydantic_spec-0.4.3/flask_pydantic_spec/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 09:28:23.144933 flask_pydantic_spec-0.4.3/flask_pydantic_spec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7265 2023-03-14 09:28:23.000000 flask_pydantic_spec-0.4.3/flask_pydantic_spec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-03-14 09:28:23.000000 flask_pydantic_spec-0.4.3/flask_pydantic_spec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 09:28:23.000000 flask_pydantic_spec-0.4.3/flask_pydantic_spec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-14 09:28:23.000000 flask_pydantic_spec-0.4.3/flask_pydantic_spec.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 09:28:23.000000 flask_pydantic_spec-0.4.3/flask_pydantic_spec.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-14 09:28:23.000000 flask_pydantic_spec-0.4.3/flask_pydantic_spec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-14 09:28:23.000000 flask_pydantic_spec-0.4.3/flask_pydantic_spec.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-03-14 09:28:15.000000 flask_pydantic_spec-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-03-14 09:28:23.144933 flask_pydantic_spec-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-03-14 09:28:15.000000 flask_pydantic_spec-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:03:22.387046 flask_pydantic_spec-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11436 2023-04-17 10:03:13.000000 flask_pydantic_spec-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7265 2023-04-17 10:03:22.387046 flask_pydantic_spec-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-04-17 10:03:13.000000 flask_pydantic_spec-0.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:03:22.383046 flask_pydantic_spec-0.4.4/flask_pydantic_spec/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-17 10:03:13.000000 flask_pydantic_spec-0.4.4/flask_pydantic_spec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-04-17 10:03:13.000000 flask_pydantic_spec-0.4.4/flask_pydantic_spec/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-04-17 10:03:13.000000 flask_pydantic_spec-0.4.4/flask_pydantic_spec/flask_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-04-17 10:03:13.000000 flask_pydantic_spec-0.4.4/flask_pydantic_spec/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11966 2023-04-17 10:03:13.000000 flask_pydantic_spec-0.4.4/flask_pydantic_spec/spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-04-17 10:03:13.000000 flask_pydantic_spec-0.4.4/flask_pydantic_spec/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7984 2023-04-17 10:03:13.000000 flask_pydantic_spec-0.4.4/flask_pydantic_spec/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:03:22.387046 flask_pydantic_spec-0.4.4/flask_pydantic_spec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7265 2023-04-17 10:03:22.000000 flask_pydantic_spec-0.4.4/flask_pydantic_spec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-17 10:03:22.000000 flask_pydantic_spec-0.4.4/flask_pydantic_spec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 10:03:22.000000 flask_pydantic_spec-0.4.4/flask_pydantic_spec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-17 10:03:22.000000 flask_pydantic_spec-0.4.4/flask_pydantic_spec.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 10:03:22.000000 flask_pydantic_spec-0.4.4/flask_pydantic_spec.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-17 10:03:22.000000 flask_pydantic_spec-0.4.4/flask_pydantic_spec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-17 10:03:22.000000 flask_pydantic_spec-0.4.4/flask_pydantic_spec.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-17 10:03:13.000000 flask_pydantic_spec-0.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-17 10:03:22.387046 flask_pydantic_spec-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-04-17 10:03:13.000000 flask_pydantic_spec-0.4.4/setup.py
```

### Comparing `flask_pydantic_spec-0.4.3/LICENSE` & `flask_pydantic_spec-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_pydantic_spec-0.4.3/PKG-INFO` & `flask_pydantic_spec-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask_pydantic_spec
-Version: 0.4.3
+Version: 0.4.4
 Summary: generate OpenAPI document and validate request & response with Python annotations.
 Home-page: https://github.com/turner-townsend/flask-pydantic-spec
 Author: Chris Gearing, Simon Hayward, Rob Young, Donald Fleming, Saurabh Jha
 Author-email: chris.gearing@turntown.digital
 License: UNKNOWN
 Description: # Flask Pydantic Spec
```

### Comparing `flask_pydantic_spec-0.4.3/README.md` & `flask_pydantic_spec-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `flask_pydantic_spec-0.4.3/flask_pydantic_spec/config.py` & `flask_pydantic_spec-0.4.4/flask_pydantic_spec/config.py`

 * *Files identical despite different names*

### Comparing `flask_pydantic_spec-0.4.3/flask_pydantic_spec/flask_backend.py` & `flask_pydantic_spec-0.4.4/flask_pydantic_spec/flask_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,15 @@
         else:
             req_query = {}
         if request.content_type and "application/json" in request.content_type:
             if request.content_encoding and "gzip" in request.content_encoding:
                 raw_body = gzip.decompress(request.stream.read()).decode(encoding="utf-8")
                 parsed_body = json.loads(raw_body)
             else:
-                parsed_body = request.get_json() or {}
+                parsed_body = request.get_json(silent=True) or {}
         elif request.content_type and "multipart/form-data" in request.content_type:
             parsed_body = parse_multi_dict(request.form) if request.form else {}
         else:
             parsed_body = request.get_data() or {}
         req_headers: Optional[Headers] = request.headers or None
         req_cookies: Optional[Mapping[str, str]] = request.cookies or None
         setattr(
```

### Comparing `flask_pydantic_spec-0.4.3/flask_pydantic_spec/page.py` & `flask_pydantic_spec-0.4.4/flask_pydantic_spec/page.py`

 * *Files identical despite different names*

### Comparing `flask_pydantic_spec-0.4.3/flask_pydantic_spec/spec.py` & `flask_pydantic_spec-0.4.4/flask_pydantic_spec/spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -311,15 +311,16 @@
             if model not in definitions.keys():
                 definitions[model] = deepcopy(schema)
 
             if "definitions" in schema:
                 for key, value in schema["definitions"].items():
                     definitions[key] = self._get_open_api_schema(value)
                 del schema["definitions"]
-                del definitions[model]["definitions"]
+                if "definitions" in definitions[model]:
+                    del definitions[model]["definitions"]
 
         return definitions
 
     def _parse_request_body(self, request_body: Mapping[str, Any]) -> Mapping[str, Any]:
         content_types = list(request_body["content"].keys())
         if len(content_types) != 1:
             raise RuntimeError(
```

### Comparing `flask_pydantic_spec-0.4.3/flask_pydantic_spec/types.py` & `flask_pydantic_spec-0.4.4/flask_pydantic_spec/types.py`

 * *Files identical despite different names*

### Comparing `flask_pydantic_spec-0.4.3/flask_pydantic_spec/utils.py` & `flask_pydantic_spec-0.4.4/flask_pydantic_spec/utils.py`

 * *Files identical despite different names*

### Comparing `flask_pydantic_spec-0.4.3/flask_pydantic_spec.egg-info/PKG-INFO` & `flask_pydantic_spec-0.4.4/flask_pydantic_spec.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-pydantic-spec
-Version: 0.4.3
+Version: 0.4.4
 Summary: generate OpenAPI document and validate request & response with Python annotations.
 Home-page: https://github.com/turner-townsend/flask-pydantic-spec
 Author: Chris Gearing, Simon Hayward, Rob Young, Donald Fleming, Saurabh Jha
 Author-email: chris.gearing@turntown.digital
 License: UNKNOWN
 Description: # Flask Pydantic Spec
```

### Comparing `flask_pydantic_spec-0.4.3/flask_pydantic_spec.egg-info/SOURCES.txt` & `flask_pydantic_spec-0.4.4/flask_pydantic_spec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flask_pydantic_spec-0.4.3/setup.py` & `flask_pydantic_spec-0.4.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 with open(path.join(here, "requirements/production.txt"), encoding="utf-8") as f:
     requires = [req.strip() for req in f if req]
 
 
 setup(
     name="flask_pydantic_spec",
-    version="0.4.3",
+    version="0.4.4",
     author="Chris Gearing, Simon Hayward, Rob Young, Donald Fleming, Saurabh Jha",
     author_email="chris.gearing@turntown.digital",
     description=(
         "generate OpenAPI document and validate request & response "
         "with Python annotations."
     ),
     long_description=readme,
```

