# Comparing `tmp/autoplugin-0.1.1.tar.gz` & `tmp/autoplugin-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoplugin-0.1.1.tar", last modified: Mon Apr 17 20:00:41 2023, max compression
+gzip compressed data, was "autoplugin-0.1.2.tar", last modified: Mon Apr 17 21:10:46 2023, max compression
```

## Comparing `autoplugin-0.1.1.tar` & `autoplugin-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 suvansh    (501) staff       (20)        0 2023-04-17 20:00:41.777325 autoplugin-0.1.1/
--rw-r--r--   0 suvansh    (501) staff       (20)     1492 2023-04-17 18:30:44.000000 autoplugin-0.1.1/LICENSE
--rw-r--r--   0 suvansh    (501) staff       (20)     5337 2023-04-17 20:00:41.776998 autoplugin-0.1.1/PKG-INFO
--rw-r--r--   0 suvansh    (501) staff       (20)     4484 2023-04-17 19:57:23.000000 autoplugin-0.1.1/README.md
-drwxr-xr-x   0 suvansh    (501) staff       (20)        0 2023-04-17 20:00:41.775644 autoplugin-0.1.1/autoplugin/
--rw-r--r--   0 suvansh    (501) staff       (20)       50 2023-04-17 18:44:53.000000 autoplugin-0.1.1/autoplugin/__init__.py
--rw-r--r--   0 suvansh    (501) staff       (20)     8439 2023-04-17 19:33:25.000000 autoplugin-0.1.1/autoplugin/autoplugin.py
--rw-r--r--   0 suvansh    (501) staff       (20)     1179 2023-04-14 20:36:12.000000 autoplugin-0.1.1/autoplugin/testing.py
-drwxr-xr-x   0 suvansh    (501) staff       (20)        0 2023-04-17 20:00:41.776704 autoplugin-0.1.1/autoplugin.egg-info/
--rw-r--r--   0 suvansh    (501) staff       (20)     5337 2023-04-17 20:00:41.000000 autoplugin-0.1.1/autoplugin.egg-info/PKG-INFO
--rw-r--r--   0 suvansh    (501) staff       (20)      265 2023-04-17 20:00:41.000000 autoplugin-0.1.1/autoplugin.egg-info/SOURCES.txt
--rw-r--r--   0 suvansh    (501) staff       (20)        1 2023-04-17 20:00:41.000000 autoplugin-0.1.1/autoplugin.egg-info/dependency_links.txt
--rw-r--r--   0 suvansh    (501) staff       (20)       51 2023-04-17 20:00:41.000000 autoplugin-0.1.1/autoplugin.egg-info/requires.txt
--rw-r--r--   0 suvansh    (501) staff       (20)       11 2023-04-17 20:00:41.000000 autoplugin-0.1.1/autoplugin.egg-info/top_level.txt
--rw-r--r--   0 suvansh    (501) staff       (20)       38 2023-04-17 20:00:41.777439 autoplugin-0.1.1/setup.cfg
--rw-r--r--   0 suvansh    (501) staff       (20)     1181 2023-04-17 19:58:32.000000 autoplugin-0.1.1/setup.py
+drwxr-xr-x   0 suvansh    (501) staff       (20)        0 2023-04-17 21:10:46.201649 autoplugin-0.1.2/
+-rw-r--r--   0 suvansh    (501) staff       (20)     1492 2023-04-17 18:30:44.000000 autoplugin-0.1.2/LICENSE
+-rw-r--r--   0 suvansh    (501) staff       (20)     5405 2023-04-17 21:10:46.201474 autoplugin-0.1.2/PKG-INFO
+-rw-r--r--   0 suvansh    (501) staff       (20)     4552 2023-04-17 21:07:05.000000 autoplugin-0.1.2/README.md
+drwxr-xr-x   0 suvansh    (501) staff       (20)        0 2023-04-17 21:10:46.200250 autoplugin-0.1.2/autoplugin/
+-rw-r--r--   0 suvansh    (501) staff       (20)       50 2023-04-17 18:44:53.000000 autoplugin-0.1.2/autoplugin/__init__.py
+-rw-r--r--   0 suvansh    (501) staff       (20)     8789 2023-04-17 20:59:08.000000 autoplugin-0.1.2/autoplugin/autoplugin.py
+-rw-r--r--   0 suvansh    (501) staff       (20)     1179 2023-04-14 20:36:12.000000 autoplugin-0.1.2/autoplugin/testing.py
+drwxr-xr-x   0 suvansh    (501) staff       (20)        0 2023-04-17 21:10:46.201199 autoplugin-0.1.2/autoplugin.egg-info/
+-rw-r--r--   0 suvansh    (501) staff       (20)     5405 2023-04-17 21:10:46.000000 autoplugin-0.1.2/autoplugin.egg-info/PKG-INFO
+-rw-r--r--   0 suvansh    (501) staff       (20)      265 2023-04-17 21:10:46.000000 autoplugin-0.1.2/autoplugin.egg-info/SOURCES.txt
+-rw-r--r--   0 suvansh    (501) staff       (20)        1 2023-04-17 21:10:46.000000 autoplugin-0.1.2/autoplugin.egg-info/dependency_links.txt
+-rw-r--r--   0 suvansh    (501) staff       (20)       58 2023-04-17 21:10:46.000000 autoplugin-0.1.2/autoplugin.egg-info/requires.txt
+-rw-r--r--   0 suvansh    (501) staff       (20)       11 2023-04-17 21:10:46.000000 autoplugin-0.1.2/autoplugin.egg-info/top_level.txt
+-rw-r--r--   0 suvansh    (501) staff       (20)       38 2023-04-17 21:10:46.201703 autoplugin-0.1.2/setup.cfg
+-rw-r--r--   0 suvansh    (501) staff       (20)     1200 2023-04-17 21:10:25.000000 autoplugin-0.1.2/setup.py
```

### Comparing `autoplugin-0.1.1/LICENSE` & `autoplugin-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `autoplugin-0.1.1/PKG-INFO` & `autoplugin-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoplugin
-Version: 0.1.1
+Version: 0.1.2
 Summary: Create ChatGPT plugins from Python code
 Home-page: https://github.com/suvansh/autoplugin
 Author: Suvansh Sanjeev
 Author-email: suvansh@brilliantly.ai
 Project-URL: Tracker, https://github.com/suvansh/autoplugin/issues
 Project-URL: Source, https://github.com/suvansh/autoplugin/
 Project-URL: Documentation, https://github.com/suvansh/AutoPlugin/blob/main/README.md
@@ -41,31 +41,33 @@
 ```
 
 ## Basic Usage
 To get started with AutoPlugin, follow these steps:
 
 1. Import the necessary functions from AutoPlugin and FastAPI:
 ```python
-from autoplugin.autoplugin import register, generate, launch
+from autoplugin import register, generate, launch
 from fastapi import FastAPI
 ```
 
 2. Create a FastAPI app instance:
 ```python
 app = FastAPI()
 ```
 
 3. Use the register decorator to register your functions as API endpoints.
 AutoPlugin generates function descriptions in the OpenAPI spec so that ChatGPT knows how to use your endpoints.
 By default, the description is fetched from the docstring. If there's no docstring, or if you specify `generate_description=True`, AutoPlugin will generate one automatically from OpenAI's API (requires setting the `OPENAI_API_KEY` environment variable).
-Finally, you can specify a description (e.g. if the docstring contains extra information not needed in the OpenAPI description) by passing the `description` keyword argument:
+Finally, you can specify a description (e.g. if the docstring contains extra information not needed in the OpenAPI description) by passing the `description` keyword argument.
 ```python
-@register(app, methods=["GET", "POST"], generate_description=True)
-async def hello(name: str, age: int = 5) -> str:
-    return f"Hello, {name}! Age {age}."
+@register(app, methods=["GET"])
+async def get_order(name: str) -> str:
+    order = await get_order_from_db(name)
+    return f"Order for {name}: {order}"
+# Generated description: "Retrieves an order from the database for a given name."
 ```
 
 4. Generate the necessary files (`openapi.yaml` and `ai-plugin.json`) for your ChatGPT plugin.
 Optionally, specify `out_dir` to change where they're saved to:
 ```python
 generate(app)  # generated files saved to `.well-known/` directory
 ```
```

### Comparing `autoplugin-0.1.1/README.md` & `autoplugin-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -20,31 +20,33 @@
 ```
 
 ## Basic Usage
 To get started with AutoPlugin, follow these steps:
 
 1. Import the necessary functions from AutoPlugin and FastAPI:
 ```python
-from autoplugin.autoplugin import register, generate, launch
+from autoplugin import register, generate, launch
 from fastapi import FastAPI
 ```
 
 2. Create a FastAPI app instance:
 ```python
 app = FastAPI()
 ```
 
 3. Use the register decorator to register your functions as API endpoints.
 AutoPlugin generates function descriptions in the OpenAPI spec so that ChatGPT knows how to use your endpoints.
 By default, the description is fetched from the docstring. If there's no docstring, or if you specify `generate_description=True`, AutoPlugin will generate one automatically from OpenAI's API (requires setting the `OPENAI_API_KEY` environment variable).
-Finally, you can specify a description (e.g. if the docstring contains extra information not needed in the OpenAPI description) by passing the `description` keyword argument:
+Finally, you can specify a description (e.g. if the docstring contains extra information not needed in the OpenAPI description) by passing the `description` keyword argument.
 ```python
-@register(app, methods=["GET", "POST"], generate_description=True)
-async def hello(name: str, age: int = 5) -> str:
-    return f"Hello, {name}! Age {age}."
+@register(app, methods=["GET"])
+async def get_order(name: str) -> str:
+    order = await get_order_from_db(name)
+    return f"Order for {name}: {order}"
+# Generated description: "Retrieves an order from the database for a given name."
 ```
 
 4. Generate the necessary files (`openapi.yaml` and `ai-plugin.json`) for your ChatGPT plugin.
 Optionally, specify `out_dir` to change where they're saved to:
 ```python
 generate(app)  # generated files saved to `.well-known/` directory
 ```
```

### Comparing `autoplugin-0.1.1/autoplugin/autoplugin.py` & `autoplugin-0.1.2/autoplugin/autoplugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,22 +69,27 @@
 
 
 def register(app: FastAPI,
              func: Callable = None,
              *,
              methods: List[str] = None,
              description: Optional[str] = None,
-             generate_description: bool = True,
+             generate_description: Optional[bool] = None,
              ) -> Callable:
     if func is None:
         return functools.partial(register, app, methods=methods, description=description, generate_description=generate_description)
 
-    if description is None and generate_description:
-        print("Generating description for function", func.__name__)
-        description = _generate_description(func)
+    if description is None:
+        if generate_description is None:
+            # user did not specify whether to generate. generate if no docstring, otherwise use docstring
+            description = _generate_description(func) if func.__doc__ is None else func.__doc__
+        elif generate_description:
+            description = _generate_description(func)
+        else:  # generate_description is False. use docstring if it exists, otherwise use None (no description)
+            description = func.__doc__
     if methods is None:
         methods = ["POST"]
 
     @functools.wraps(func)
     async def wrapper(*args, **kwargs):
         return await func(*args, **kwargs)
```

### Comparing `autoplugin-0.1.1/autoplugin/testing.py` & `autoplugin-0.1.2/autoplugin/testing.py`

 * *Files identical despite different names*

### Comparing `autoplugin-0.1.1/autoplugin.egg-info/PKG-INFO` & `autoplugin-0.1.2/autoplugin.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoplugin
-Version: 0.1.1
+Version: 0.1.2
 Summary: Create ChatGPT plugins from Python code
 Home-page: https://github.com/suvansh/autoplugin
 Author: Suvansh Sanjeev
 Author-email: suvansh@brilliantly.ai
 Project-URL: Tracker, https://github.com/suvansh/autoplugin/issues
 Project-URL: Source, https://github.com/suvansh/autoplugin/
 Project-URL: Documentation, https://github.com/suvansh/AutoPlugin/blob/main/README.md
@@ -41,31 +41,33 @@
 ```
 
 ## Basic Usage
 To get started with AutoPlugin, follow these steps:
 
 1. Import the necessary functions from AutoPlugin and FastAPI:
 ```python
-from autoplugin.autoplugin import register, generate, launch
+from autoplugin import register, generate, launch
 from fastapi import FastAPI
 ```
 
 2. Create a FastAPI app instance:
 ```python
 app = FastAPI()
 ```
 
 3. Use the register decorator to register your functions as API endpoints.
 AutoPlugin generates function descriptions in the OpenAPI spec so that ChatGPT knows how to use your endpoints.
 By default, the description is fetched from the docstring. If there's no docstring, or if you specify `generate_description=True`, AutoPlugin will generate one automatically from OpenAI's API (requires setting the `OPENAI_API_KEY` environment variable).
-Finally, you can specify a description (e.g. if the docstring contains extra information not needed in the OpenAPI description) by passing the `description` keyword argument:
+Finally, you can specify a description (e.g. if the docstring contains extra information not needed in the OpenAPI description) by passing the `description` keyword argument.
 ```python
-@register(app, methods=["GET", "POST"], generate_description=True)
-async def hello(name: str, age: int = 5) -> str:
-    return f"Hello, {name}! Age {age}."
+@register(app, methods=["GET"])
+async def get_order(name: str) -> str:
+    order = await get_order_from_db(name)
+    return f"Order for {name}: {order}"
+# Generated description: "Retrieves an order from the database for a given name."
 ```
 
 4. Generate the necessary files (`openapi.yaml` and `ai-plugin.json`) for your ChatGPT plugin.
 Optionally, specify `out_dir` to change where they're saved to:
 ```python
 generate(app)  # generated files saved to `.well-known/` directory
 ```
```

### Comparing `autoplugin-0.1.1/setup.py` & `autoplugin-0.1.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name="autoplugin",
-    version="0.1.1",
+    version="0.1.2",
     packages=find_packages(),
     install_requires=[
         "fastapi",
         "pydantic",
         "uvicorn",
-        "requests"
+        "requests",
+        "PyYAML",
     ],
     extras_require={
         "gen": ["langchain"],
     },
     author="Suvansh Sanjeev",
     author_email="suvansh@brilliantly.ai",
     description="Create ChatGPT plugins from Python code",
```

