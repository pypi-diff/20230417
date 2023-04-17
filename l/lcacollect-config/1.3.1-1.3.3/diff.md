# Comparing `tmp/lcacollect_config-1.3.1.tar.gz` & `tmp/lcacollect_config-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lcacollect_config-1.3.1.tar", max compression
+gzip compressed data, was "lcacollect_config-1.3.3.tar", max compression
```

## Comparing `lcacollect_config-1.3.1.tar` & `lcacollect_config-1.3.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1030 2023-04-04 12:38:53.313205 lcacollect_config-1.3.1/README.md
--rw-r--r--   0        0        0     2152 2023-04-04 12:38:53.313205 lcacollect_config-1.3.1/pyproject.toml
--rw-r--r--   0        0        0       22 2023-04-04 12:38:53.313205 lcacollect_config-1.3.1/src/lcacollect_config/__init__.py
--rw-r--r--   0        0        0     1882 2023-04-04 12:38:53.313205 lcacollect_config-1.3.1/src/lcacollect_config/config.py
--rw-r--r--   0        0        0     1507 2023-04-04 12:38:53.313205 lcacollect_config-1.3.1/src/lcacollect_config/connection.py
--rw-r--r--   0        0        0      372 2023-04-04 12:38:53.313205 lcacollect_config-1.3.1/src/lcacollect_config/context.py
--rw-r--r--   0        0        0      217 2023-04-04 12:38:53.313205 lcacollect_config-1.3.1/src/lcacollect_config/exceptions.py
--rw-r--r--   0        0        0      637 2023-04-04 12:38:53.313205 lcacollect_config-1.3.1/src/lcacollect_config/fastapi.py
--rw-r--r--   0        0        0      597 2023-04-04 12:38:53.313205 lcacollect_config-1.3.1/src/lcacollect_config/formatting.py
--rw-r--r--   0        0        0        0 2023-04-04 12:38:53.313205 lcacollect_config-1.3.1/src/lcacollect_config/graphql/__init__.py
--rw-r--r--   0        0        0     2653 2023-04-04 12:38:53.313205 lcacollect_config-1.3.1/src/lcacollect_config/graphql/input_filters.py
--rw-r--r--   0        0        0     1270 2023-04-04 12:38:53.313205 lcacollect_config-1.3.1/src/lcacollect_config/graphql/pagination.py
--rw-r--r--   0        0        0      400 2023-04-04 12:38:53.313205 lcacollect_config-1.3.1/src/lcacollect_config/permissions.py
--rw-r--r--   0        0        0     1043 2023-04-04 12:38:53.313205 lcacollect_config-1.3.1/src/lcacollect_config/router.py
--rw-r--r--   0        0        0      507 2023-04-04 12:38:53.313205 lcacollect_config-1.3.1/src/lcacollect_config/security.py
--rw-r--r--   0        0        0     2637 2023-04-04 12:38:53.313205 lcacollect_config-1.3.1/src/lcacollect_config/validate.py
--rw-r--r--   0        0        0     2079 1970-01-01 00:00:00.000000 lcacollect_config-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1030 2023-04-17 13:14:21.424693 lcacollect_config-1.3.3/README.md
+-rw-r--r--   0        0        0     2152 2023-04-17 13:14:21.424693 lcacollect_config-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-04-17 13:14:21.424693 lcacollect_config-1.3.3/src/lcacollect_config/__init__.py
+-rw-r--r--   0        0        0     1882 2023-04-17 13:14:21.424693 lcacollect_config-1.3.3/src/lcacollect_config/config.py
+-rw-r--r--   0        0        0     1507 2023-04-17 13:14:21.424693 lcacollect_config-1.3.3/src/lcacollect_config/connection.py
+-rw-r--r--   0        0        0      372 2023-04-17 13:14:21.424693 lcacollect_config-1.3.3/src/lcacollect_config/context.py
+-rw-r--r--   0        0        0      217 2023-04-17 13:14:21.424693 lcacollect_config-1.3.3/src/lcacollect_config/exceptions.py
+-rw-r--r--   0        0        0      637 2023-04-17 13:14:21.424693 lcacollect_config-1.3.3/src/lcacollect_config/fastapi.py
+-rw-r--r--   0        0        0      597 2023-04-17 13:14:21.424693 lcacollect_config-1.3.3/src/lcacollect_config/formatting.py
+-rw-r--r--   0        0        0        0 2023-04-17 13:14:21.424693 lcacollect_config-1.3.3/src/lcacollect_config/graphql/__init__.py
+-rw-r--r--   0        0        0     2772 2023-04-17 13:14:21.424693 lcacollect_config-1.3.3/src/lcacollect_config/graphql/input_filters.py
+-rw-r--r--   0        0        0     1270 2023-04-17 13:14:21.424693 lcacollect_config-1.3.3/src/lcacollect_config/graphql/pagination.py
+-rw-r--r--   0        0        0      400 2023-04-17 13:14:21.424693 lcacollect_config-1.3.3/src/lcacollect_config/permissions.py
+-rw-r--r--   0        0        0     1043 2023-04-17 13:14:21.424693 lcacollect_config-1.3.3/src/lcacollect_config/router.py
+-rw-r--r--   0        0        0      535 2023-04-17 13:14:21.424693 lcacollect_config-1.3.3/src/lcacollect_config/security.py
+-rw-r--r--   0        0        0     2634 2023-04-17 13:14:21.424693 lcacollect_config-1.3.3/src/lcacollect_config/validate.py
+-rw-r--r--   0        0        0     2079 1970-01-01 00:00:00.000000 lcacollect_config-1.3.3/PKG-INFO
```

### Comparing `lcacollect_config-1.3.1/README.md` & `lcacollect_config-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `lcacollect_config-1.3.1/pyproject.toml` & `lcacollect_config-1.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lcacollect-config"
-version = "1.3.1"
+version = "1.3.3"
 description = "This package contains shared config and utils to be used across LCAcollect backends."
 authors = ["Christian Kongsgaard <chrk@arkitema.com>"]
 repository = "https://github.com/lcacollect/shared-config-backend"
 license = "LGPL-3.0-or-later"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `lcacollect_config-1.3.1/src/lcacollect_config/config.py` & `lcacollect_config-1.3.3/src/lcacollect_config/config.py`

 * *Files identical despite different names*

### Comparing `lcacollect_config-1.3.1/src/lcacollect_config/connection.py` & `lcacollect_config-1.3.3/src/lcacollect_config/connection.py`

 * *Files identical despite different names*

### Comparing `lcacollect_config-1.3.1/src/lcacollect_config/fastapi.py` & `lcacollect_config-1.3.3/src/lcacollect_config/fastapi.py`

 * *Files identical despite different names*

### Comparing `lcacollect_config-1.3.1/src/lcacollect_config/formatting.py` & `lcacollect_config-1.3.3/src/lcacollect_config/formatting.py`

 * *Files identical despite different names*

### Comparing `lcacollect_config-1.3.1/src/lcacollect_config/graphql/input_filters.py` & `lcacollect_config-1.3.3/src/lcacollect_config/graphql/input_filters.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,17 +50,19 @@
         elif _filter.is_not_empty:
             query = query.where(or_(field != "", field != None))
         elif _filter.is_any_of:
             query = query.where(col(field).in_(_filter.is_any_of))
         elif _filter.json_contains and str(field.type) == "JSON":
             try:
                 obj_filter = json.loads(_filter.json_contains)
+                for key, value in obj_filter.items():
+                    query = query.where(col(field)[key].astext.contains(value))
             except json.decoder.JSONDecodeError:
                 continue
-            for key, value in obj_filter.items():
+            except AttributeError:
                 query = query.where(col(field)[key].contains(value))
 
     return query
 
 
 @strawberry.enum
 class SortOptions(Enum):
```

### Comparing `lcacollect_config-1.3.1/src/lcacollect_config/graphql/pagination.py` & `lcacollect_config-1.3.3/src/lcacollect_config/graphql/pagination.py`

 * *Files identical despite different names*

### Comparing `lcacollect_config-1.3.1/src/lcacollect_config/router.py` & `lcacollect_config-1.3.3/src/lcacollect_config/router.py`

 * *Files identical despite different names*

### Comparing `lcacollect_config-1.3.1/src/lcacollect_config/validate.py` & `lcacollect_config-1.3.3/src/lcacollect_config/validate.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
     from lcacollect_config import config
 
     settings = config.Settings()
 
 
 @cached(ttl=60)
 async def project_exists(project_id: str, token: str) -> Union[bool, list[dict]]:
-
     """
     Checks whether the project exists. The function is cached with a decorator.
     Args:
         project_id: the ProjectID that the user is navigating inside.
         token: the user's PAT
 
     Returns:
@@ -48,23 +47,21 @@
         data = response.json()
         if response.is_error or data.get("errors"):
             return False
         return data.get("data")
 
 
 def is_super_admin(user: User) -> bool:
-
     """Checks whether the user is an Admin and so can access all resources."""
 
     return "lca_super_admin" in user.roles
 
 
 @cached(ttl=60)
 async def group_exists(project_id: str, group_id: str, token: str) -> bool:
-
     """
     Checks whether the group exists. The function is cached with a decorator.
     Args:
         project_id: the ProjectID that the user is navigating inside.
         group_id: the GroupID of the Project Group the user is interacting with.
         token: the user's PAT
```

### Comparing `lcacollect_config-1.3.1/PKG-INFO` & `lcacollect_config-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lcacollect-config
-Version: 1.3.1
+Version: 1.3.3
 Summary: This package contains shared config and utils to be used across LCAcollect backends.
 Home-page: https://github.com/lcacollect/shared-config-backend
 License: LGPL-3.0-or-later
 Author: Christian Kongsgaard
 Author-email: chrk@arkitema.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

