# Comparing `tmp/quilt_py-0.5.1.tar.gz` & `tmp/quilt_py-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quilt_py-0.5.1.tar", max compression
+gzip compressed data, was "quilt_py-0.5.2.tar", max compression
```

## Comparing `quilt_py-0.5.1.tar` & `quilt_py-0.5.2.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0        6 2023-03-01 17:17:36.767217 quilt_py-0.5.1/README.md
--rw-r--r--   0        0        0      622 2023-04-17 16:26:14.308043 quilt_py-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      739 2023-03-29 22:05:11.666467 quilt_py-0.5.1/quilt/__init__.py
--rw-r--r--   0        0        0     1226 2023-03-29 22:20:58.486400 quilt_py-0.5.1/quilt/config.py
--rw-r--r--   0        0        0      161 2023-04-04 23:13:40.240939 quilt_py-0.5.1/quilt/context_base/__init__.py
--rw-r--r--   0        0        0     1413 2023-02-26 20:47:23.221097 quilt_py-0.5.1/quilt/context_base/request_manager.py
--rw-r--r--   0        0        0     5130 2023-04-13 19:52:51.910432 quilt_py-0.5.1/quilt/context_base/user_manager.py
--rw-r--r--   0        0        0      894 2023-02-22 22:13:46.914009 quilt_py-0.5.1/quilt/errors.py
--rw-r--r--   0        0        0        0 2023-02-28 23:17:18.661730 quilt_py-0.5.1/quilt/extensions/__init__.py
--rw-r--r--   0        0        0     2536 2023-03-10 00:23:33.299180 quilt_py-0.5.1/quilt/extensions/calls.py
--rw-r--r--   0        0        0      656 2023-02-28 23:20:38.295883 quilt_py-0.5.1/quilt/extensions/mask_errors.py
--rw-r--r--   0        0        0     5204 2023-03-10 00:23:13.749469 quilt_py-0.5.1/quilt/extensions/sentry.py
--rw-r--r--   0        0        0        0 2023-02-16 01:36:16.094733 quilt_py-0.5.1/quilt/gql_utils/__init__.py
--rw-r--r--   0        0        0        0 2023-02-16 01:36:33.862640 quilt_py-0.5.1/quilt/gql_utils/resolvers/__init__.py
--rw-r--r--   0        0        0     3020 2023-04-17 16:26:06.569138 quilt_py-0.5.1/quilt/gql_utils/resolvers/helpers.py
--rw-r--r--   0        0        0     5538 2023-04-17 16:39:17.191876 quilt_py-0.5.1/quilt/gql_utils/resolvers/hydrate.py
--rw-r--r--   0        0        0     1481 2023-02-28 18:35:05.783183 quilt_py-0.5.1/quilt/gql_utils/resolvers/logic.py
--rw-r--r--   0        0        0     4969 2023-02-28 18:24:17.300741 quilt_py-0.5.1/quilt/gql_utils/resolvers/models.py
--rw-r--r--   0        0        0     3447 2023-04-17 16:35:37.558846 quilt_py-0.5.1/quilt/gql_utils/resolvers/startup.py
--rw-r--r--   0        0        0     2306 2023-04-16 23:52:37.211790 quilt_py-0.5.1/quilt/gql_utils/strawberry_utils.py
--rw-r--r--   0        0        0     2761 2023-02-28 02:30:06.521864 quilt_py-0.5.1/quilt/helpers.py
--rw-r--r--   0        0        0     2483 2023-02-28 23:43:32.442836 quilt_py-0.5.1/quilt/logs.py
--rw-r--r--   0        0        0        0 2023-02-28 23:52:18.384266 quilt_py-0.5.1/quilt/middlewares/__init__.py
--rw-r--r--   0        0        0      705 2023-02-28 23:51:42.871147 quilt_py-0.5.1/quilt/middlewares/main.py
--rw-r--r--   0        0        0      333 2023-03-01 00:15:36.825263 quilt_py-0.5.1/quilt/models/__init__.py
--rw-r--r--   0        0        0      895 2023-02-15 22:59:50.014980 quilt_py-0.5.1/quilt/models/image.py
--rw-r--r--   0        0        0     1215 2023-02-15 22:53:17.404819 quilt_py-0.5.1/quilt/models/input_datetime.py
--rw-r--r--   0        0        0     2106 2023-03-01 00:18:57.093892 quilt_py-0.5.1/quilt/models/location/__init__.py
--rw-r--r--   0        0        0      363 2023-02-28 23:58:20.825046 quilt_py-0.5.1/quilt/models/location/queries.py
--rw-r--r--   0        0        0     2264 2023-03-01 16:20:22.425244 quilt_py-0.5.1/quilt/models/phone_number.py
--rw-r--r--   0        0        0    11199 2023-03-09 21:45:18.322425 quilt_py-0.5.1/quilt/plugins/StrawberryFilters/default_filters.py
--rw-r--r--   0        0        0    11017 2023-04-11 03:03:58.673379 quilt_py-0.5.1/quilt/plugins/StrawberryFilters/generator.py
--rw-r--r--   0        0        0     6440 2023-03-01 17:29:02.000000 quilt_py-0.5.1/quilt/plugins/StrawberryFilters/logic.py
--rw-r--r--   0        0        0     1530 2023-03-10 00:17:35.041938 quilt_py-0.5.1/quilt/plugins/StrawberryFilters/mixins.py
--rw-r--r--   0        0        0       38 2023-02-08 20:08:53.856234 quilt_py-0.5.1/quilt/scalars/__init__.py
--rw-r--r--   0        0        0      265 2023-03-01 00:19:45.027572 quilt_py-0.5.1/quilt/scalars/phone_number.py
--rw-r--r--   0        0        0        0 2023-02-08 20:08:53.841842 quilt_py-0.5.1/quilt/services/auth/__init__.py
--rw-r--r--   0        0        0     1252 2023-02-28 23:13:42.662358 quilt_py-0.5.1/quilt/services/auth/logic.py
--rw-r--r--   0        0        0     1167 2023-02-28 23:08:56.113002 quilt_py-0.5.1/quilt/services/auth/routes.py
--rw-r--r--   0        0        0      230 2023-02-28 23:14:31.585735 quilt_py-0.5.1/quilt/services/auth/tests.py
--rw-r--r--   0        0        0      266 2023-02-28 17:20:20.325597 quilt_py-0.5.1/quilt/types.py
--rw-r--r--   0        0        0      295 2023-02-28 23:25:02.984361 quilt_py-0.5.1/quilt/utils.py
--rw-r--r--   0        0        0     1178 2023-02-21 16:53:32.720011 quilt_py-0.5.1/quilt/vendors/Cloudinary/__init__.py
--rw-r--r--   0        0        0      639 2023-02-08 20:08:37.141779 quilt_py-0.5.1/quilt/vendors/Cloudinary/schemas.py
--rw-r--r--   0        0        0      808 2023-02-16 02:06:37.085257 quilt_py-0.5.1/quilt/vendors/Firebase/__init__.py
--rw-r--r--   0        0        0        0 2023-02-08 20:08:53.856627 quilt_py-0.5.1/quilt/vendors/GooglePlaces/__init__.py
--rw-r--r--   0        0        0     3653 2023-03-01 00:16:13.108728 quilt_py-0.5.1/quilt/vendors/GooglePlaces/main.py
--rw-r--r--   0        0        0      802 2023-03-01 00:01:11.153247 quilt_py-0.5.1/quilt/vendors/GooglePlaces/tests/__init__.py
--rw-r--r--   0        0        0     4431 2023-02-28 23:59:18.353088 quilt_py-0.5.1/quilt/vendors/GooglePlaces/tests/example_response.json
--rw-r--r--   0        0        0     1111 2023-02-16 02:24:02.140992 quilt_py-0.5.1/quilt/vendors/IPInfo/__init__.py
--rw-r--r--   0        0        0        0 2023-02-21 21:40:23.708710 quilt_py-0.5.1/quilt/vendors/Sentry/__init__.py
--rw-r--r--   0        0        0     1240 2023-02-21 21:42:43.021407 quilt_py-0.5.1/quilt/vendors/Sentry/context_managers.py
--rw-r--r--   0        0        0      758 2023-02-21 21:22:10.849578 quilt_py-0.5.1/quilt/vendors/Sentry/decorators.py
--rw-r--r--   0        0        0        0 2023-02-16 02:06:06.850816 quilt_py-0.5.1/quilt/vendors/__init__.py
--rw-r--r--   0        0        0     1144 1970-01-01 00:00:00.000000 quilt_py-0.5.1/setup.py
--rw-r--r--   0        0        0      520 1970-01-01 00:00:00.000000 quilt_py-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0        6 2023-03-01 17:17:36.767217 quilt_py-0.5.2/README.md
+-rw-r--r--   0        0        0      622 2023-04-17 19:01:39.996199 quilt_py-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0      739 2023-03-29 22:05:11.666467 quilt_py-0.5.2/quilt/__init__.py
+-rw-r--r--   0        0        0     1226 2023-03-29 22:20:58.486400 quilt_py-0.5.2/quilt/config.py
+-rw-r--r--   0        0        0      161 2023-04-04 23:13:40.240939 quilt_py-0.5.2/quilt/context_base/__init__.py
+-rw-r--r--   0        0        0     1413 2023-02-26 20:47:23.221097 quilt_py-0.5.2/quilt/context_base/request_manager.py
+-rw-r--r--   0        0        0     5130 2023-04-13 19:52:51.910432 quilt_py-0.5.2/quilt/context_base/user_manager.py
+-rw-r--r--   0        0        0      894 2023-02-22 22:13:46.914009 quilt_py-0.5.2/quilt/errors.py
+-rw-r--r--   0        0        0        0 2023-02-28 23:17:18.661730 quilt_py-0.5.2/quilt/extensions/__init__.py
+-rw-r--r--   0        0        0     2536 2023-03-10 00:23:33.299180 quilt_py-0.5.2/quilt/extensions/calls.py
+-rw-r--r--   0        0        0      656 2023-02-28 23:20:38.295883 quilt_py-0.5.2/quilt/extensions/mask_errors.py
+-rw-r--r--   0        0        0     5204 2023-03-10 00:23:13.749469 quilt_py-0.5.2/quilt/extensions/sentry.py
+-rw-r--r--   0        0        0        0 2023-02-16 01:36:16.094733 quilt_py-0.5.2/quilt/gql_utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-16 01:36:33.862640 quilt_py-0.5.2/quilt/gql_utils/resolvers/__init__.py
+-rw-r--r--   0        0        0     3049 2023-04-17 19:01:12.278052 quilt_py-0.5.2/quilt/gql_utils/resolvers/helpers.py
+-rw-r--r--   0        0        0     5538 2023-04-17 16:39:17.191876 quilt_py-0.5.2/quilt/gql_utils/resolvers/hydrate.py
+-rw-r--r--   0        0        0     1481 2023-02-28 18:35:05.783183 quilt_py-0.5.2/quilt/gql_utils/resolvers/logic.py
+-rw-r--r--   0        0        0     4969 2023-02-28 18:24:17.300741 quilt_py-0.5.2/quilt/gql_utils/resolvers/models.py
+-rw-r--r--   0        0        0     3447 2023-04-17 16:35:37.558846 quilt_py-0.5.2/quilt/gql_utils/resolvers/startup.py
+-rw-r--r--   0        0        0     2306 2023-04-16 23:52:37.211790 quilt_py-0.5.2/quilt/gql_utils/strawberry_utils.py
+-rw-r--r--   0        0        0     2761 2023-02-28 02:30:06.521864 quilt_py-0.5.2/quilt/helpers.py
+-rw-r--r--   0        0        0     2483 2023-02-28 23:43:32.442836 quilt_py-0.5.2/quilt/logs.py
+-rw-r--r--   0        0        0        0 2023-02-28 23:52:18.384266 quilt_py-0.5.2/quilt/middlewares/__init__.py
+-rw-r--r--   0        0        0      705 2023-02-28 23:51:42.871147 quilt_py-0.5.2/quilt/middlewares/main.py
+-rw-r--r--   0        0        0      333 2023-03-01 00:15:36.825263 quilt_py-0.5.2/quilt/models/__init__.py
+-rw-r--r--   0        0        0      895 2023-02-15 22:59:50.014980 quilt_py-0.5.2/quilt/models/image.py
+-rw-r--r--   0        0        0     1215 2023-02-15 22:53:17.404819 quilt_py-0.5.2/quilt/models/input_datetime.py
+-rw-r--r--   0        0        0     2106 2023-03-01 00:18:57.093892 quilt_py-0.5.2/quilt/models/location/__init__.py
+-rw-r--r--   0        0        0      363 2023-02-28 23:58:20.825046 quilt_py-0.5.2/quilt/models/location/queries.py
+-rw-r--r--   0        0        0     2264 2023-03-01 16:20:22.425244 quilt_py-0.5.2/quilt/models/phone_number.py
+-rw-r--r--   0        0        0    11199 2023-03-09 21:45:18.322425 quilt_py-0.5.2/quilt/plugins/StrawberryFilters/default_filters.py
+-rw-r--r--   0        0        0    11017 2023-04-11 03:03:58.673379 quilt_py-0.5.2/quilt/plugins/StrawberryFilters/generator.py
+-rw-r--r--   0        0        0     6440 2023-03-01 17:29:02.000000 quilt_py-0.5.2/quilt/plugins/StrawberryFilters/logic.py
+-rw-r--r--   0        0        0     1530 2023-03-10 00:17:35.041938 quilt_py-0.5.2/quilt/plugins/StrawberryFilters/mixins.py
+-rw-r--r--   0        0        0       38 2023-02-08 20:08:53.856234 quilt_py-0.5.2/quilt/scalars/__init__.py
+-rw-r--r--   0        0        0      265 2023-03-01 00:19:45.027572 quilt_py-0.5.2/quilt/scalars/phone_number.py
+-rw-r--r--   0        0        0        0 2023-02-08 20:08:53.841842 quilt_py-0.5.2/quilt/services/auth/__init__.py
+-rw-r--r--   0        0        0     1252 2023-02-28 23:13:42.662358 quilt_py-0.5.2/quilt/services/auth/logic.py
+-rw-r--r--   0        0        0     1167 2023-02-28 23:08:56.113002 quilt_py-0.5.2/quilt/services/auth/routes.py
+-rw-r--r--   0        0        0      230 2023-02-28 23:14:31.585735 quilt_py-0.5.2/quilt/services/auth/tests.py
+-rw-r--r--   0        0        0      266 2023-02-28 17:20:20.325597 quilt_py-0.5.2/quilt/types.py
+-rw-r--r--   0        0        0      295 2023-02-28 23:25:02.984361 quilt_py-0.5.2/quilt/utils.py
+-rw-r--r--   0        0        0     1178 2023-02-21 16:53:32.720011 quilt_py-0.5.2/quilt/vendors/Cloudinary/__init__.py
+-rw-r--r--   0        0        0      639 2023-02-08 20:08:37.141779 quilt_py-0.5.2/quilt/vendors/Cloudinary/schemas.py
+-rw-r--r--   0        0        0      808 2023-02-16 02:06:37.085257 quilt_py-0.5.2/quilt/vendors/Firebase/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-08 20:08:53.856627 quilt_py-0.5.2/quilt/vendors/GooglePlaces/__init__.py
+-rw-r--r--   0        0        0     3653 2023-03-01 00:16:13.108728 quilt_py-0.5.2/quilt/vendors/GooglePlaces/main.py
+-rw-r--r--   0        0        0      802 2023-03-01 00:01:11.153247 quilt_py-0.5.2/quilt/vendors/GooglePlaces/tests/__init__.py
+-rw-r--r--   0        0        0     4431 2023-02-28 23:59:18.353088 quilt_py-0.5.2/quilt/vendors/GooglePlaces/tests/example_response.json
+-rw-r--r--   0        0        0     1111 2023-02-16 02:24:02.140992 quilt_py-0.5.2/quilt/vendors/IPInfo/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-21 21:40:23.708710 quilt_py-0.5.2/quilt/vendors/Sentry/__init__.py
+-rw-r--r--   0        0        0     1240 2023-02-21 21:42:43.021407 quilt_py-0.5.2/quilt/vendors/Sentry/context_managers.py
+-rw-r--r--   0        0        0      758 2023-02-21 21:22:10.849578 quilt_py-0.5.2/quilt/vendors/Sentry/decorators.py
+-rw-r--r--   0        0        0        0 2023-02-16 02:06:06.850816 quilt_py-0.5.2/quilt/vendors/__init__.py
+-rw-r--r--   0        0        0     1144 1970-01-01 00:00:00.000000 quilt_py-0.5.2/setup.py
+-rw-r--r--   0        0        0      520 1970-01-01 00:00:00.000000 quilt_py-0.5.2/PKG-INFO
```

### Comparing `quilt_py-0.5.1/pyproject.toml` & `quilt_py-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "quilt-py"
-version = "0.5.1"
+version = "0.5.2"
 description = ""
 authors = ["Jeremy Berman <jerber@sas.upenn.edu>"]
 readme = "README.md"
 packages = [{include = "quilt"}]
 exclude = ["tests/**/*"]
```

### Comparing `quilt_py-0.5.1/quilt/__init__.py` & `quilt_py-0.5.2/quilt/__init__.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.5.1/quilt/config.py` & `quilt_py-0.5.2/quilt/config.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.5.1/quilt/context_base/request_manager.py` & `quilt_py-0.5.2/quilt/context_base/request_manager.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.5.1/quilt/context_base/user_manager.py` & `quilt_py-0.5.2/quilt/context_base/user_manager.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.5.1/quilt/errors.py` & `quilt_py-0.5.2/quilt/errors.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.5.1/quilt/extensions/calls.py` & `quilt_py-0.5.2/quilt/extensions/calls.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.5.1/quilt/extensions/mask_errors.py` & `quilt_py-0.5.2/quilt/extensions/mask_errors.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.5.1/quilt/extensions/sentry.py` & `quilt_py-0.5.2/quilt/extensions/sentry.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.5.1/quilt/gql_utils/resolvers/helpers.py` & `quilt_py-0.5.2/quilt/gql_utils/resolvers/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,16 @@
     )
     if isinstance(return_type, str) and (
         return_type == current_straw_type.__name__
         or f"['{current_straw_type.__name__}']" in str(return_type)
     ):
         return current_straw_type
     if isinstance(return_type, str):
-        return current_straw_type  # TODO gogoog need to test
+        # return current_straw_type  # TODO gogoog need to test
+        return return_type
         raise Exception(
             f"Return type cannot be str but is: {return_type=}, {raw_return_type=}, {current_straw_type=}."
         )
     return return_type
 
 
 def selected_field_from_path(
```

### Comparing `quilt_py-0.5.1/quilt/gql_utils/resolvers/hydrate.py` & `quilt_py-0.5.2/quilt/gql_utils/resolvers/hydrate.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.5.1/quilt/gql_utils/resolvers/logic.py` & `quilt_py-0.5.2/quilt/gql_utils/resolvers/logic.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.5.1/quilt/gql_utils/resolvers/models.py` & `quilt_py-0.5.2/quilt/gql_utils/resolvers/models.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.5.1/quilt/gql_utils/resolvers/startup.py` & `quilt_py-0.5.2/quilt/gql_utils/resolvers/startup.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.5.1/quilt/gql_utils/strawberry_utils.py` & `quilt_py-0.5.2/quilt/gql_utils/strawberry_utils.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.5.1/quilt/helpers.py` & `quilt_py-0.5.2/quilt/helpers.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.5.1/quilt/logs.py` & `quilt_py-0.5.2/quilt/logs.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.5.1/quilt/middlewares/main.py` & `quilt_py-0.5.2/quilt/middlewares/main.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.5.1/quilt/models/image.py` & `quilt_py-0.5.2/quilt/models/image.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.5.1/quilt/models/input_datetime.py` & `quilt_py-0.5.2/quilt/models/input_datetime.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.5.1/quilt/models/location/__init__.py` & `quilt_py-0.5.2/quilt/models/location/__init__.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.5.1/quilt/models/phone_number.py` & `quilt_py-0.5.2/quilt/models/phone_number.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.5.1/quilt/plugins/StrawberryFilters/default_filters.py` & `quilt_py-0.5.2/quilt/plugins/StrawberryFilters/default_filters.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.5.1/quilt/plugins/StrawberryFilters/generator.py` & `quilt_py-0.5.2/quilt/plugins/StrawberryFilters/generator.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.5.1/quilt/plugins/StrawberryFilters/logic.py` & `quilt_py-0.5.2/quilt/plugins/StrawberryFilters/logic.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.5.1/quilt/plugins/StrawberryFilters/mixins.py` & `quilt_py-0.5.2/quilt/plugins/StrawberryFilters/mixins.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.5.1/quilt/services/auth/logic.py` & `quilt_py-0.5.2/quilt/services/auth/logic.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.5.1/quilt/services/auth/routes.py` & `quilt_py-0.5.2/quilt/services/auth/routes.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.5.1/quilt/vendors/Cloudinary/__init__.py` & `quilt_py-0.5.2/quilt/vendors/Cloudinary/__init__.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.5.1/quilt/vendors/Cloudinary/schemas.py` & `quilt_py-0.5.2/quilt/vendors/Cloudinary/schemas.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.5.1/quilt/vendors/Firebase/__init__.py` & `quilt_py-0.5.2/quilt/vendors/Firebase/__init__.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.5.1/quilt/vendors/GooglePlaces/main.py` & `quilt_py-0.5.2/quilt/vendors/GooglePlaces/main.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.5.1/quilt/vendors/GooglePlaces/tests/__init__.py` & `quilt_py-0.5.2/quilt/vendors/GooglePlaces/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.5.1/quilt/vendors/GooglePlaces/tests/example_response.json` & `quilt_py-0.5.2/quilt/vendors/GooglePlaces/tests/example_response.json`

 * *Files identical despite different names*

### Comparing `quilt_py-0.5.1/quilt/vendors/IPInfo/__init__.py` & `quilt_py-0.5.2/quilt/vendors/IPInfo/__init__.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.5.1/quilt/vendors/Sentry/context_managers.py` & `quilt_py-0.5.2/quilt/vendors/Sentry/context_managers.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.5.1/quilt/vendors/Sentry/decorators.py` & `quilt_py-0.5.2/quilt/vendors/Sentry/decorators.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.5.1/setup.py` & `quilt_py-0.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
  'phonenumbers',
  'pydantic[email]',
  'sentry-sdk[httpx,pure-eval]>=1.15,<2.0',
  'strawberry-graphql']
 
 setup_kwargs = {
     'name': 'quilt-py',
-    'version': '0.5.1',
+    'version': '0.5.2',
     'description': '',
     'long_description': 'hello!',
     'author': 'Jeremy Berman',
     'author_email': 'jerber@sas.upenn.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `quilt_py-0.5.1/PKG-INFO` & `quilt_py-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quilt-py
-Version: 0.5.1
+Version: 0.5.2
 Summary: 
 Author: Jeremy Berman
 Author-email: jerber@sas.upenn.edu
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: devtools
```

