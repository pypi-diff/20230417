# Comparing `tmp/pyfredapi-0.5.3.tar.gz` & `tmp/pyfredapi-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfredapi-0.5.3.tar", max compression
+gzip compressed data, was "pyfredapi-0.5.4.tar", max compression
```

## Comparing `pyfredapi-0.5.3.tar` & `pyfredapi-0.5.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1067 2022-09-27 22:09:06.134268 pyfredapi-0.5.3/LICENSE
--rw-r--r--   0        0        0     1941 2022-10-28 22:07:01.709700 pyfredapi-0.5.3/README.md
--rw-r--r--   0        0        0     1704 2023-03-31 23:49:08.792034 pyfredapi-0.5.3/pyfredapi/__init__.py
--rw-r--r--   0        0        0     2537 2023-04-02 21:15:19.116259 pyfredapi-0.5.3/pyfredapi/_base.py
--rw-r--r--   0        0        0     8489 2023-04-02 21:20:19.911345 pyfredapi-0.5.3/pyfredapi/category.py
--rw-r--r--   0        0        0      148 2023-03-31 23:49:08.794567 pyfredapi-0.5.3/pyfredapi/exceptions/__init__.py
--rw-r--r--   0        0        0     1160 2023-03-31 23:49:08.795190 pyfredapi-0.5.3/pyfredapi/exceptions/exceptions.py
--rw-r--r--   0        0        0     5810 2023-04-02 21:16:16.026529 pyfredapi-0.5.3/pyfredapi/maps.py
--rw-r--r--   0        0        0        0 2022-10-12 01:34:52.474192 pyfredapi-0.5.3/pyfredapi/py.typed
--rw-r--r--   0        0        0     9609 2023-04-02 21:16:35.752229 pyfredapi-0.5.3/pyfredapi/releases.py
--rw-r--r--   0        0        0    20891 2023-04-02 15:39:51.999581 pyfredapi-0.5.3/pyfredapi/series.py
--rw-r--r--   0        0        0    13493 2023-04-02 20:58:44.394082 pyfredapi-0.5.3/pyfredapi/series_collection.py
--rw-r--r--   0        0        0     3570 2023-04-02 15:39:51.995699 pyfredapi-0.5.3/pyfredapi/sources.py
--rw-r--r--   0        0        0     4369 2023-04-02 21:15:33.284540 pyfredapi-0.5.3/pyfredapi/tags.py
--rw-r--r--   0        0        0       76 2023-03-31 23:49:08.800945 pyfredapi-0.5.3/pyfredapi/utils/__init__.py
--rw-r--r--   0        0        0      387 2022-10-27 01:47:28.858898 pyfredapi-0.5.3/pyfredapi/utils/_common_type_hints.py
--rw-r--r--   0        0        0     1511 2023-03-31 23:49:08.801548 pyfredapi-0.5.3/pyfredapi/utils/_convert_to_pandas.py
--rw-r--r--   0        0        0      221 2023-03-31 23:49:08.802190 pyfredapi-0.5.3/pyfredapi/utils/enums.py
--rw-r--r--   0        0        0     3373 2023-04-02 21:17:57.161816 pyfredapi-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     3188 1970-01-01 00:00:00.000000 pyfredapi-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2022-09-27 22:09:06.134268 pyfredapi-0.5.4/LICENSE
+-rw-r--r--   0        0        0     1941 2022-10-28 22:07:01.709700 pyfredapi-0.5.4/README.md
+-rw-r--r--   0        0        0     1704 2023-03-31 23:49:08.792034 pyfredapi-0.5.4/pyfredapi/__init__.py
+-rw-r--r--   0        0        0     2521 2023-04-02 21:22:06.505837 pyfredapi-0.5.4/pyfredapi/_base.py
+-rw-r--r--   0        0        0     8441 2023-04-17 01:31:33.691827 pyfredapi-0.5.4/pyfredapi/category.py
+-rw-r--r--   0        0        0      148 2023-03-31 23:49:08.794567 pyfredapi-0.5.4/pyfredapi/exceptions/__init__.py
+-rw-r--r--   0        0        0     1160 2023-03-31 23:49:08.795190 pyfredapi-0.5.4/pyfredapi/exceptions/exceptions.py
+-rw-r--r--   0        0        0     5794 2023-04-17 01:26:06.450096 pyfredapi-0.5.4/pyfredapi/maps.py
+-rw-r--r--   0        0        0        0 2022-10-12 01:34:52.474192 pyfredapi-0.5.4/pyfredapi/py.typed
+-rw-r--r--   0        0        0     9561 2023-04-02 21:22:06.507234 pyfredapi-0.5.4/pyfredapi/releases.py
+-rw-r--r--   0        0        0    20891 2023-04-02 21:22:06.508030 pyfredapi-0.5.4/pyfredapi/series.py
+-rw-r--r--   0        0        0    13493 2023-04-02 20:58:44.394082 pyfredapi-0.5.4/pyfredapi/series_collection.py
+-rw-r--r--   0        0        0     3570 2023-04-02 21:22:06.514616 pyfredapi-0.5.4/pyfredapi/sources.py
+-rw-r--r--   0        0        0     4337 2023-04-02 21:22:06.514999 pyfredapi-0.5.4/pyfredapi/tags.py
+-rw-r--r--   0        0        0       76 2023-03-31 23:49:08.800945 pyfredapi-0.5.4/pyfredapi/utils/__init__.py
+-rw-r--r--   0        0        0      387 2022-10-27 01:47:28.858898 pyfredapi-0.5.4/pyfredapi/utils/_common_type_hints.py
+-rw-r--r--   0        0        0     1511 2023-03-31 23:49:08.801548 pyfredapi-0.5.4/pyfredapi/utils/_convert_to_pandas.py
+-rw-r--r--   0        0        0      221 2023-03-31 23:49:08.802190 pyfredapi-0.5.4/pyfredapi/utils/enums.py
+-rw-r--r--   0        0        0     3380 2023-04-17 01:42:41.082084 pyfredapi-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0     3118 1970-01-01 00:00:00.000000 pyfredapi-0.5.4/PKG-INFO
```

### Comparing `pyfredapi-0.5.3/LICENSE` & `pyfredapi-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.5.3/README.md` & `pyfredapi-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.5.3/pyfredapi/__init__.py` & `pyfredapi-0.5.4/pyfredapi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.5.3/pyfredapi/_base.py` & `pyfredapi-0.5.4/pyfredapi/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     _base_params = BaseApiParameters(api_key=api_key)
 
     if not params:
         params = {}
     try:
         response = requests.get(
             f"{base_url}/{endpoint}",
-            params=frozendict({**_base_params.dict(), **params}),  # type: ignore
+            params=frozendict({**_base_params.dict(), **params}),
             timeout=30,
         )
     except requests.exceptions.RequestException as e:
         raise FredAPIRequestError(
             message=f"Error invoking Fred API: {e}", status_code=None
         ) from e
     if response.status_code != HTTPStatus.OK:
```

### Comparing `pyfredapi-0.5.3/pyfredapi/category.py` & `pyfredapi-0.5.4/pyfredapi/category.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,15 +168,15 @@
     dict
         A dictionary where the keys are series ids and the values for SeriesInfo objects.
     """
     params = CategoryApiParameters(category_id=category_id, **kwargs)
     response = _get_request(
         api_key=api_key,
         endpoint="category/series",
-        params=frozendict(params.dict(exclude_none=True)),  # type: ignore
+        params=frozendict(params.dict(exclude_none=True)),
     )
 
     return {series["id"]: SeriesInfo(**series) for series in response["seriess"]}
 
 
 def get_category_tags(
     category_id: Optional[int] = None,
@@ -204,15 +204,15 @@
     """
     return_format = ReturnFormat(return_format)
 
     params = CategoryApiParameters(category_id=category_id, **kwargs)
     response = _get_request(
         api_key=api_key,
         endpoint="category/tags",
-        params=frozendict(params.dict(exclude_none=True)),  # type: ignore
+        params=frozendict(params.dict(exclude_none=True)),
     )
 
     if return_format == ReturnFormat.pandas:
         return _convert_to_pandas(response["tags"])
     return response
 
 
@@ -242,13 +242,13 @@
     """
     return_format = ReturnFormat(return_format)
 
     params = CategoryApiParameters(category_id=category_id, **kwargs)
     response = _get_request(
         api_key=api_key,
         endpoint="category/related_tags",
-        params=frozendict(params.dict(exclude_none=True)),  # type: ignore
+        params=frozendict(params.dict(exclude_none=True)),
     )
 
     if return_format == ReturnFormat.pandas:
         return _convert_to_pandas(response["tags"])
     return response
```

### Comparing `pyfredapi-0.5.3/pyfredapi/exceptions/exceptions.py` & `pyfredapi-0.5.4/pyfredapi/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.5.3/pyfredapi/maps.py` & `pyfredapi-0.5.4/pyfredapi/maps.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,15 +159,15 @@
     GeoseriesData
         GeoseriesData object containing the geoseries data and metadata.
     """
     params = MapApiParameters(series_id=series_id, date=end_date, start_date=start_date)
     response = _get_request(
         endpoint="series/data",
         api_key=api_key,
-        params=frozendict(params.dict(exclude_none=True)),  # type: ignore
+        params=frozendict(params.dict(exclude_none=True)),
         base_url=_geo_fred_url,
     )
 
     geoseries_info = get_geoseries_info(series_id=series_id)
 
     if return_format == ReturnFormat.pandas:
         dfs = []
```

### Comparing `pyfredapi-0.5.3/pyfredapi/releases.py` & `pyfredapi-0.5.4/pyfredapi/releases.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,15 +135,15 @@
     -------
     Dictionary representing the Json response.
     """
     params = ReleaseApiParameters(release_id=release_id, **kwargs)
     return _get_request(
         endpoint="release/dates",
         api_key=api_key,
-        params=frozendict(params.dict(exclude_none=True)),  # type: ignore
+        params=frozendict(params.dict(exclude_none=True)),
     )
 
 
 def get_release_series(
     release_id: int, api_key: ApiKeyType = None, **kwargs: KwargsType
 ) -> JsonType:
     """Get the series on a release of economic data. https://fred.stlouisfed.org/docs/api/fred/release_series.html.
@@ -213,15 +213,15 @@
     -------
     Dictionary representing the Json response.
     """
     params = ReleaseApiParameters(release_id=release_id, **kwargs)
     return _get_request(
         endpoint="release/tags",
         api_key=api_key,
-        params=frozendict(params.dict(exclude_none=True)),  # type: ignore
+        params=frozendict(params.dict(exclude_none=True)),
     )
 
 
 def get_release_related_tags(
     release_id: int, tag_names: str, api_key: ApiKeyType = None, **kwargs: KwargsType
 ) -> JsonType:
     """Get the related FRED tags for one or more FRED tags within a release. https://fred.stlouisfed.org/docs/api/fred/release_related_tags.html.
@@ -241,15 +241,15 @@
     -------
     Dictionary representing the Json response.
     """
     params = ReleaseApiParameters(release_id=release_id, tag_names=tag_names, **kwargs)
     return _get_request(
         endpoint="release/related_tags",
         api_key=api_key,
-        params=frozendict(params.dict(exclude_none=True)),  # type: ignore
+        params=frozendict(params.dict(exclude_none=True)),
     )
 
 
 def get_release_tables(
     release_id: int, api_key: ApiKeyType = None, **kwargs: KwargsType
 ) -> JsonType:
     """Get release table trees for a given release. https://fred.stlouisfed.org/docs/api/fred/release_tables.html.
```

### Comparing `pyfredapi-0.5.3/pyfredapi/series.py` & `pyfredapi-0.5.4/pyfredapi/series.py`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.5.3/pyfredapi/series_collection.py` & `pyfredapi-0.5.4/pyfredapi/series_collection.py`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.5.3/pyfredapi/sources.py` & `pyfredapi-0.5.4/pyfredapi/sources.py`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.5.3/pyfredapi/tags.py` & `pyfredapi-0.5.4/pyfredapi/tags.py`

 * *Files 11% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     params = TagsApiParameters(
         tag_names=tag_names,
         **kwargs,
     )
     return _get_request(
         endpoint="related_tags",
         api_key=api_key,
-        params=frozendict(**params.dict(exclude_none=True)),  # type: ignore
+        params=frozendict(**params.dict(exclude_none=True)),
     )
 
 
 def get_series_matching_tags(
     tag_names: str, api_key: ApiKeyType = None, **kwargs: KwargsType
 ) -> JsonType:
     """Get the series matching all tags in the tag_names parameter. https://fred.stlouisfed.org/docs/api/fred/tags_series.html.
@@ -115,14 +115,14 @@
     dict
         A dictionary representing the json response.
     """
     params = TagsApiParameters(**kwargs)
     return _get_request(
         endpoint="tags/series",
         api_key=api_key,
-        params=frozendict(  # type: ignore
+        params=frozendict(
             {
                 "tag_names": tag_names,
                 **params.dict(exclude_none=True),
             }
         ),
     )
```

### Comparing `pyfredapi-0.5.3/pyfredapi/utils/_convert_to_pandas.py` & `pyfredapi-0.5.4/pyfredapi/utils/_convert_to_pandas.py`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.5.3/pyproject.toml` & `pyfredapi-0.5.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pyfredapi"
-version = "0.5.3"
+version = "0.5.4"
 description = "A full featured API client for the FRED API web service."
 authors = ["Greg Moore <gwmoore.career@gmail.com>"]
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Intended Audience :: Financial and Insurance Industry",
@@ -19,20 +19,20 @@
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0.0"
-requests = "^2.28.2"
-pandas = "^1.5.3"
-pydantic = "^1.10.7"
-rich = "^13.3.3"
-plotly = "^5.14.0"
-frozendict = "^2.3.6"
+requests = ">=2"
+pandas = ">=1"
+pydantic = ">=1"
+rich = ">=13"
+plotly = ">=5"
+frozendict = ">=2"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.lint]
 optional = true
 
@@ -53,14 +53,15 @@
 types-requests = "^2.28.11.17"
 types-setuptools = "^67.6.0.6"
 black = {extras = ["jupyter"], version = "^23.3.0"}
 ruff = "^0.0.260"
 # pandas-stubs = "^1.5.3.230321"
 mypy = "^1.1.1"
 pre-commit = "^3.2.1"
+types-frozendict = "^2.0.9"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.2.2"
 tox = "^4.4.8"
 coverage = "^7.2.2"
 pytest-cov = "^4.0.0"
```

### Comparing `pyfredapi-0.5.3/PKG-INFO` & `pyfredapi-0.5.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfredapi
-Version: 0.5.3
+Version: 0.5.4
 Summary: A full featured API client for the FRED API web service.
 Author: Greg Moore
 Author-email: gwmoore.career@gmail.com
 Requires-Python: >=3.8,<4.0.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
@@ -16,20 +16,20 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: frozendict (>=2.3.6,<3.0.0)
-Requires-Dist: pandas (>=1.5.3,<2.0.0)
-Requires-Dist: plotly (>=5.14.0,<6.0.0)
-Requires-Dist: pydantic (>=1.10.7,<2.0.0)
-Requires-Dist: requests (>=2.28.2,<3.0.0)
-Requires-Dist: rich (>=13.3.3,<14.0.0)
+Requires-Dist: frozendict (>=2)
+Requires-Dist: pandas (>=1)
+Requires-Dist: plotly (>=5)
+Requires-Dist: pydantic (>=1)
+Requires-Dist: requests (>=2)
+Requires-Dist: rich (>=13)
 Description-Content-Type: text/markdown
 
 # pyfredapi - Python library for the Federal Reserve Economic Data (FRED) API
 <!-- badges: start -->
 
 [![PyPi Version](https://img.shields.io/pypi/v/pyfredapi.svg)](https://pypi.python.org/pypi/pyfredapi/)
 [![Supported Python Versions](https://img.shields.io/pypi/pyversions/pyfredapi)](https://pypi.python.org/pypi/pyfredapi)
```

