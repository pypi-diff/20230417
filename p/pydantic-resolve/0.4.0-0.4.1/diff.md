# Comparing `tmp/pydantic_resolve-0.4.0.tar.gz` & `tmp/pydantic_resolve-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_resolve-0.4.0.tar", max compression
+gzip compressed data, was "pydantic_resolve-0.4.1.tar", max compression
```

## Comparing `pydantic_resolve-0.4.0.tar` & `pydantic_resolve-0.4.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1081 2023-03-07 14:12:05.553679 pydantic_resolve-0.4.0/LICENSE
--rw-r--r--   0        0        0      365 2023-04-06 03:44:06.193459 pydantic_resolve-0.4.0/pydantic_resolve/__init__.py
--rw-r--r--   0        0        0       19 2023-04-05 08:27:57.212146 pydantic_resolve-0.4.0/pydantic_resolve/constant.py
--rw-r--r--   0        0        0     1865 2023-04-06 02:31:57.953441 pydantic_resolve-0.4.0/pydantic_resolve/core.py
--rw-r--r--   0        0        0      175 2023-04-06 03:28:36.782802 pydantic_resolve-0.4.0/pydantic_resolve/exceptions.py
--rw-r--r--   0        0        0     3388 2023-04-06 03:53:59.182161 pydantic_resolve-0.4.0/pydantic_resolve/resolver.py
--rw-r--r--   0        0        0      148 2023-04-06 03:27:46.383675 pydantic_resolve-0.4.0/pydantic_resolve/util.py
--rw-r--r--   0        0        0      900 2023-04-06 05:12:17.016907 pydantic_resolve-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     7350 2023-04-05 14:26:28.408177 pydantic_resolve-0.4.0/README.md
--rw-r--r--   0        0        0     7943 1970-01-01 00:00:00.000000 pydantic_resolve-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-03-07 14:12:05.553679 pydantic_resolve-0.4.1/LICENSE
+-rw-r--r--   0        0        0      365 2023-04-06 09:30:37.392196 pydantic_resolve-0.4.1/pydantic_resolve/__init__.py
+-rw-r--r--   0        0        0       19 2023-04-05 08:27:57.212146 pydantic_resolve-0.4.1/pydantic_resolve/constant.py
+-rw-r--r--   0        0        0     1865 2023-04-06 09:30:37.393198 pydantic_resolve-0.4.1/pydantic_resolve/core.py
+-rw-r--r--   0        0        0      175 2023-04-06 09:30:37.394196 pydantic_resolve-0.4.1/pydantic_resolve/exceptions.py
+-rw-r--r--   0        0        0     3388 2023-04-06 09:30:37.395197 pydantic_resolve-0.4.1/pydantic_resolve/resolver.py
+-rw-r--r--   0        0        0      148 2023-04-06 09:30:37.396199 pydantic_resolve-0.4.1/pydantic_resolve/util.py
+-rw-r--r--   0        0        0      900 2023-04-17 07:38:38.573336 pydantic_resolve-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0    11699 2023-04-11 14:31:01.356851 pydantic_resolve-0.4.1/README.md
+-rw-r--r--   0        0        0    12303 1970-01-01 00:00:00.000000 pydantic_resolve-0.4.1/PKG-INFO
```

### Comparing `pydantic_resolve-0.4.0/LICENSE` & `pydantic_resolve-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-0.4.0/pydantic_resolve/core.py` & `pydantic_resolve-0.4.1/pydantic_resolve/core.py`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-0.4.0/pydantic_resolve/resolver.py` & `pydantic_resolve-0.4.1/pydantic_resolve/resolver.py`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-0.4.0/pyproject.toml` & `pydantic_resolve-0.4.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "pydantic-resolve"
-version = "0.4.0"
+version = "0.4.1"
 description = "Make pydantic have a GraphQL-like assembly experience."
 authors = ["tangkikodo <allmonday@126.com>"]
 readme = "README.md"
 repository = "https://github.com/allmonday/pydantic_resolve"
 keywords = ["pydantic", "fastapi"]
 license = "MIT"
 packages = [{include = "pydantic_resolve"}]
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.7"
 pydantic = "^1.10.4"
 
 # optional
 aiodataloader = { version = "^0.4.0", optional = true } 
 
 [tool.poetry.extras]
 dataloader = ['aiodataloader']
```

