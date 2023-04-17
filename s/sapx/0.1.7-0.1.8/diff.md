# Comparing `tmp/sapx-0.1.7.tar.gz` & `tmp/sapx-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sapx-0.1.7.tar", last modified: Wed Apr 12 07:48:55 2023, max compression
+gzip compressed data, was "sapx-0.1.8.tar", last modified: Mon Apr 17 14:56:23 2023, max compression
```

## Comparing `sapx-0.1.7.tar` & `sapx-0.1.8.tar`

### file list

```diff
@@ -1,50 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:48:55.029750 sapx-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-12 07:48:55.029750 sapx-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-12 07:48:45.000000 sapx-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-04-12 07:48:45.000000 sapx-0.1.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:48:55.017749 sapx-0.1.7/sap/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-12 07:48:45.000000 sapx-0.1.7/sap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:48:55.021750 sapx-0.1.7/sap/beanie/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-12 07:48:45.000000 sapx-0.1.7/sap/beanie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-12 07:48:45.000000 sapx-0.1.7/sap/beanie/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-04-12 07:48:45.000000 sapx-0.1.7/sap/beanie/document.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-12 07:48:45.000000 sapx-0.1.7/sap/beanie/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-12 07:48:45.000000 sapx-0.1.7/sap/beanie/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-04-12 07:48:45.000000 sapx-0.1.7/sap/beanie/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:48:55.021750 sapx-0.1.7/sap/fastapi/
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-12 07:48:45.000000 sapx-0.1.7/sap/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6461 2023-04-12 07:48:45.000000 sapx-0.1.7/sap/fastapi/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-12 07:48:45.000000 sapx-0.1.7/sap/fastapi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-04-12 07:48:45.000000 sapx-0.1.7/sap/fastapi/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-04-12 07:48:45.000000 sapx-0.1.7/sap/fastapi/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     9285 2023-04-12 07:48:45.000000 sapx-0.1.7/sap/fastapi/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-04-12 07:48:45.000000 sapx-0.1.7/sap/fastapi/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-12 07:48:45.000000 sapx-0.1.7/sap/loggers.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 07:48:45.000000 sapx-0.1.7/sap/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:48:55.021750 sapx-0.1.7/sap/rest/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-12 07:48:45.000000 sapx-0.1.7/sap/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-04-12 07:48:45.000000 sapx-0.1.7/sap/rest/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-04-12 07:48:45.000000 sapx-0.1.7/sap/rest/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-12 07:48:45.000000 sapx-0.1.7/sap/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:48:55.025750 sapx-0.1.7/sap/worker/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-12 07:48:45.000000 sapx-0.1.7/sap/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-12 07:48:45.000000 sapx-0.1.7/sap/worker/amqp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-12 07:48:45.000000 sapx-0.1.7/sap/worker/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-04-12 07:48:45.000000 sapx-0.1.7/sap/worker/crons.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-12 07:48:45.000000 sapx-0.1.7/sap/worker/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-04-12 07:48:45.000000 sapx-0.1.7/sap/worker/lambdas.py
--rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-04-12 07:48:45.000000 sapx-0.1.7/sap/worker/packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-04-12 07:48:45.000000 sapx-0.1.7/sap/worker/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:48:55.025750 sapx-0.1.7/sapx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-12 07:48:55.000000 sapx-0.1.7/sapx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-12 07:48:55.000000 sapx-0.1.7/sapx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 07:48:55.000000 sapx-0.1.7/sapx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-12 07:48:55.000000 sapx-0.1.7/sapx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-12 07:48:55.000000 sapx-0.1.7/sapx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 07:48:55.029750 sapx-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-04-12 07:48:45.000000 sapx-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:48:55.029750 sapx-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-04-12 07:48:45.000000 sapx-0.1.7/tests/test_fastapi_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-12 07:48:45.000000 sapx-0.1.7/tests/test_rest_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-04-12 07:48:45.000000 sapx-0.1.7/tests/test_worker_lambdas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-04-12 07:48:45.000000 sapx-0.1.7/tests/test_worker_packet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:56:23.179742 sapx-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-17 14:56:23.179742 sapx-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-17 14:56:06.000000 sapx-0.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-04-17 14:56:06.000000 sapx-0.1.8/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:56:23.175742 sapx-0.1.8/sap/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:56:23.175742 sapx-0.1.8/sap/beanie/
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/beanie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/beanie/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/beanie/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/beanie/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/beanie/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/beanie/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/beanie/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/beanie/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:56:23.175742 sapx-0.1.8/sap/chart/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/chart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/chart/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:56:23.175742 sapx-0.1.8/sap/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/fastapi/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/fastapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/fastapi/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/fastapi/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/fastapi/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7979 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/fastapi/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/fastapi/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/loggers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:56:23.175742 sapx-0.1.8/sap/rest/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/rest/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/rest/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:56:23.175742 sapx-0.1.8/sap/worker/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/worker/amqp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/worker/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/worker/crons.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/worker/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/worker/lambdas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/worker/packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/worker/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:56:23.179742 sapx-0.1.8/sapx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-17 14:56:23.000000 sapx-0.1.8/sapx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-17 14:56:23.000000 sapx-0.1.8/sapx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 14:56:23.000000 sapx-0.1.8/sapx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-17 14:56:23.000000 sapx-0.1.8/sapx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-17 14:56:23.000000 sapx-0.1.8/sapx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 14:56:23.179742 sapx-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-17 14:56:06.000000 sapx-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:56:23.179742 sapx-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-04-17 14:56:06.000000 sapx-0.1.8/tests/test_fastapi_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-17 14:56:06.000000 sapx-0.1.8/tests/test_rest_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-04-17 14:56:06.000000 sapx-0.1.8/tests/test_worker_lambdas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-04-17 14:56:06.000000 sapx-0.1.8/tests/test_worker_packet.py
```

### Comparing `sapx-0.1.7/PKG-INFO` & `sapx-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sapx
-Version: 0.1.7
+Version: 0.1.8
 Summary: Library of re-usable utilities for python web apps.
 Home-page: https://github.com/trellixio/sap
 Author: Trellix Dev
 Author-email: contact@trellix.io
 License: COPYRIGHT @ Trellix
 Classifier: Environment :: Web Environment
 Classifier: Framework :: FastAPI
```

### Comparing `sapx-0.1.7/pyproject.toml` & `sapx-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 disable = [
     "missing-module-docstring",
     "missing-class-docstring",
     "missing-function-docstring",
     "too-few-public-methods",
     "locally-disabled",
     "suppressed-message",
+    "too-many-arguments",
 ]
 
 [tool.pylint.design]
 min-public-methods = 1
 max-parents = 10
 max-complexity = 10
```

### Comparing `sapx-0.1.7/sap/beanie/client.py` & `sapx-0.1.8/sap/beanie/client.py`

 * *Files identical despite different names*

### Comparing `sapx-0.1.7/sap/beanie/document.py` & `sapx-0.1.8/sap/beanie/document.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,42 +1,66 @@
 """
 Documents.
 
 Override beanie Documents to useful methods.
 Most of the methods are inspired from Django behavior on querying data.
 """
 
-import datetime
+from datetime import datetime
 from typing import TYPE_CHECKING, Any, Mapping, Optional, Type, TypeVar, Union
 
 from pymongo.client_session import ClientSession
 
 import beanie
 import pydantic
 from beanie import PydanticObjectId
 
 from .exceptions import Object404Error
-from .models import _DocMeta
 
 if TYPE_CHECKING:
     from beanie.odm.documents import DocType
     from beanie.odm.interfaces.find import DocumentProjectionType
 
 
+class _DocMeta(pydantic.BaseModel):
+    """Meta Data allowing to keep trace of Documents versioning and updates."""
+
+    version: int = 0  # version of the document being imported
+    source: Optional[str] = ""  # where the data is coming from: webhook, cron
+    created: Optional[datetime] = None  # when the document was first imported
+    updated: Optional[datetime] = None  # when the document was last updated
+    deleted: Optional[datetime] = None  # when the document was deleted, (deleted document may be retained for logging)
+
+
+class DocMeta(pydantic.BaseModel):
+    """Manage meta data and ensure that it's correctly set."""
+
+    doc_meta: _DocMeta = _DocMeta()
+
+    @pydantic.root_validator
+    @classmethod
+    def validate_doc_meta(cls, values: dict[str, Any]) -> dict[str, Any]:
+        """Validate doc meta on each model update."""
+        doc_meta: _DocMeta = values["doc_meta"]
+        doc_meta.updated = datetime.now()
+        doc_meta.created = doc_meta.created or doc_meta.updated
+        return values
+
+
 class Document(beanie.Document):
     """Subclass beanie.Document that add handy methods."""
 
     doc_meta: _DocMeta = _DocMeta()
 
     @pydantic.root_validator
     @classmethod
     def validate_doc_meta(cls, values: dict[str, Any]) -> dict[str, Any]:
         """Validate doc meta on each model update."""
         doc_meta: _DocMeta = values["doc_meta"]
-        doc_meta.updated = datetime.datetime.now()
+        doc_meta.updated = datetime.now()
         doc_meta.created = doc_meta.created or doc_meta.updated
         return values
 
     @classmethod
     async def get_or_404(
         cls: Type["DocType"],
         document_id: Union[PydanticObjectId, str],
@@ -82,8 +106,9 @@
             **pymongo_kwargs,
         )
         if not result:
             raise Object404Error
         return result
 
 
-TDoc = TypeVar("TDoc", bound=Document)
+DocT = TypeVar("DocT", bound=Document)
+ModelT = TypeVar("ModelT", bound=pydantic.BaseModel)
```

### Comparing `sapx-0.1.7/sap/beanie/query.py` & `sapx-0.1.8/sap/beanie/query.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """
 Query.
 
 Utils that can be used to optimize db queries and avoid redundant requests.
 """
-import typing
+from typing import Callable, Optional, Type, TypeVar, Union
 
-from beanie import Document, Link, PydanticObjectId, operators
+from beanie import Document, PydanticObjectId, operators
 from beanie.odm.fields import ExpressionField, LinkInfo
 
-from .document import TDoc
+from .document import DocT
+from .link import Link
 
-RDoc = typing.TypeVar("RDoc", bound=Document)  # Related Model Type
+RDocT = TypeVar("RDocT", bound=Document)  # Related Model Type
 
 
-async def prefetch_related(item_list: list[TDoc], to_attribute: str) -> None:
+async def prefetch_related(item_list: list[DocT], to_attribute: str) -> None:
     """
     Optimize fetching of a related attribute of one-to-one relation.
 
     Fetch related attribute efficiently in order to avoid multiple queries that could kill the db.
 
     Example:
     ```python
@@ -42,42 +43,46 @@
     """
 
     # If item_list is empty there is no need to continue.
     if not item_list:
         return
 
     # Find the model of the related attributed
-    related_field: LinkInfo[Document] = type(item_list[0]).get_link_fields()[to_attribute]
-    related_model: Document = related_field.model_class
+    link_fields = type(item_list[0]).get_link_fields()
+    assert link_fields
+    related_field: LinkInfo = link_fields[to_attribute]
+    assert issubclass(related_field.model_class, Document)
+    related_model: Type[Document] = related_field.model_class
 
-    def get_related_id(item_: Document) -> typing.Optional[PydanticObjectId]:
+    def get_related_id(item_: Document) -> Optional[PydanticObjectId]:
         """Return the id of the related object."""
-        link: typing.Optional[Link[Document]] = getattr(item_, to_attribute)
+        link: Optional[Link[Document]] = getattr(item_, to_attribute)
         if link:
             return link.ref.id
         return None
 
     # Fetch the related attribute and map it to the each item in the item_list
     related_item_ids = list(set(get_related_id(item) for item in item_list))
     related_item_list = await related_model.find(operators.In(related_model.id, related_item_ids)).to_list()
     for item in item_list:
-        related_id = get_related_id(item)
-        related_item = next((rel for rel in related_item_list if rel.id == related_id), None) if related_id else None
-        setattr(item, to_attribute, related_item)
+        link: Optional[Link[Document]] = getattr(item, to_attribute)
+        if link:
+            related_item = next((rel for rel in related_item_list if rel.id == link.ref.id), None)
+            setattr(link, "doc", related_item)
 
 
 async def prefetch_related_children(
-    item_list: list[TDoc],
+    item_list: list[DocT],
     to_attribute: str,
-    related_model: type[RDoc],
+    related_model: type[RDocT],
     related_attribute: str,
-    filter_func: typing.Optional[
-        typing.Callable[
-            [list[RDoc], TDoc],
-            typing.Union[None, RDoc, list[RDoc]],
+    filter_func: Optional[
+        Callable[
+            [list[RDocT], DocT],
+            Union[None, RDocT, list[RDocT]],
         ]
     ] = None,
 ) -> None:
     """
     Optimize fetching of a related attributes of one-to-many relation.
 
     Fetch related attribute efficiently in order to avoid multiple queries that could kill the db.
@@ -114,18 +119,18 @@
     related_item_list = await related_model.find(
         operators.In(related_expression, item_ids), sort="-doc_meta.created"
     ).to_list()
 
     for item in item_list:
         related_items = []
         for rel in related_item_list:
-            rel_link: Link[RDoc] = getattr(rel, related_attribute)
+            rel_link: Link[RDocT] = getattr(rel, related_attribute)
             if item.id == rel_link.ref.id:
                 related_items.append(rel)
-        setattr(item, to_attribute, filter_func(related_items=related_items, item=item))
+        setattr(item, to_attribute, filter_func(related_items, item))
 
 
 def prepare_search_string(search_text: str) -> str:
     """Clean and reformat the search string."""
     res = search_text.strip()
     if "@" in res and not '"' in res:
         res = f'"{res}"'
```

### Comparing `sapx-0.1.7/sap/fastapi/__init__.py` & `sapx-0.1.8/sap/fastapi/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 FastAPI.
 
 This package regroups all common helpers exclusively for FastAPI.
 Learn more about FastAPI: https://github.com/tiangolo/fastapi
 """
 
 from .exceptions import Object404Error, Validation422Error
-from .forms import FormData, validate_form
+from .forms import FormValidation, validate_form
 from .serializers import ObjectSerializer, WriteObjectSerializer
 from .utils import Flash, FlashLevel, pydantic_format_errors
 
 __all__ = [
     "Flash",
     "FlashLevel",
     "pydantic_format_errors",
@@ -18,9 +18,9 @@
     "ObjectSerializer",
     "WriteObjectSerializer",
     # Exceptions
     "Validation422Error",
     "Object404Error",
     # Forms
     "validate_form",
-    "FormData",
+    "FormValidation",
 ]
```

### Comparing `sapx-0.1.7/sap/fastapi/auth.py` & `sapx-0.1.8/sap/fastapi/auth.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,167 +8,158 @@
 import time
 import typing
 
 import jwt
 
 from fastapi import Cookie, Depends, Request, Response, status
 from fastapi.exceptions import HTTPException
-from starlette.authentication import AuthCredentials, AuthenticationBackend, AuthenticationError
+from starlette.authentication import AuthCredentials, AuthenticationBackend, AuthenticationError, BaseUser
+from starlette.requests import HTTPConnection
 
 from AppMain.settings import AppSettings
 from sap.beanie import Document
+from sap.beanie.exceptions import Object404Error
+
+UserT = typing.TypeVar("UserT", bound=Document)
 
 
 class JWTAuth:
     """JWT cookie authentication utils.
 
     This can be used to login/logout user with persistent sessions.
     Mainly useful for Web Apps. For API, it is better to use Basic Authentication in Headers.
     """
 
     auth_login_url: typing.ClassVar[str] = "/pages/auth/login/"
     auth_cookie_key: typing.ClassVar[str] = "user_session"
     auth_cookie_expires: typing.ClassVar[int] = 60 * 60 * 12  # expiration = 12 hours
+    user_model: type[Document]
+
+    def __init__(self, user_model: type[UserT]) -> None:
+        """Initialize the JWT auth helper.
 
-    @classmethod
-    def get_auth_login_url(cls) -> str:
+        :param user_model: The User model class.
+        """
+        super().__init__()
+        self.user_model = user_model
+
+    def get_auth_login_url(self) -> str:
         """Retrieve the login url where user are redirect in case of auth failure."""
-        return cls.auth_login_url
+        return self.auth_login_url
 
-    @classmethod
-    def get_auth_cookie_key(cls) -> str:
+    def get_auth_cookie_key(self) -> str:
         """Retrieve key used to define the authentication cookie."""
-        return cls.auth_cookie_key
+        return self.auth_cookie_key
 
-    @classmethod
-    def get_auth_cookie_expires(cls) -> int:
+    def get_auth_cookie_expires(self) -> int:
         """Retrieve validity in seconds of the authentication cookie."""
-        return cls.auth_cookie_expires
+        return self.auth_cookie_expires
 
-    @classmethod
-    def create_token(cls, user: Document, expires: typing.Optional[int] = None) -> str:
+    def create_token(self, user: UserT) -> str:
         """Get JWT temporary token."""
-        expires = cls.get_auth_cookie_expires() if expires is None else expires
+        expires = self.get_auth_cookie_expires()
         jwt_data = {"exp": int(time.time()) + expires, "user_id": str(user.id)}
         return jwt.encode(payload=jwt_data, key=AppSettings.CRYPTO_SECRET, algorithm="HS256")
 
-    @classmethod
-    async def find_user(cls, jwt_token: str, user_model_class: type[Document]) -> Document:
+    async def find_user(self, jwt_token: str) -> Document:
         """
         Verify that JWT token is valid.
 
         :param jwt_token: The lifespan of the token in seconds.
-        :param user_model_class: user model class
         """
-        jwt_data = jwt.decode(jwt_token, key=AppSettings.CRYPTO_SECRET, algorithms=["HS256"])
-        # Raises: jwt.exceptions.InvalidTokenError => Token has expired or is invalid
 
-        user = await user_model_class.find_one_or_404(
-            user_model_class.id == jwt_data["user_id"],
-            user_model_class.is_active == True,
-        )
-        # Raise: Object404Error => User cannot be found
+        # Raises: jwt.exceptions.InvalidTokenError => Token has expired or is invalid
+        jwt_data = jwt.decode(jwt_token, key=AppSettings.CRYPTO_SECRET, algorithms=["HS256"])
+        if "user_id" not in jwt_data:
+            raise jwt.exceptions.InvalidAudienceError("Cannot read user_id.")
 
-        return user
+        # Raises: Object404Error => User cannot be found
+        return await self.user_model.get_or_404(jwt_data["user_id"])
 
-    @classmethod
-    async def login(cls, response: Response, user: Document) -> Response:
+    async def login(self, response: Response, user: UserT) -> Response:
         """Create a persistent cookie based session for the authenticated user."""
-        response.set_cookie(key=cls.get_auth_cookie_key(), value=cls.create_token(user=user), httponly=True)
+        response.set_cookie(
+            key=self.get_auth_cookie_key(),
+            value=self.create_token(user=user),
+            httponly=True,
+        )
         return response
 
-    @classmethod
-    async def logout(cls, response: Response) -> Response:
+    async def logout(self, response: Response) -> Response:
         """Create a persistent cookie based session for the authenticated user."""
-        response.delete_cookie(key=cls.get_auth_cookie_key(), httponly=True)
+        response.delete_cookie(key=self.get_auth_cookie_key(), httponly=True)
         return response
 
-    @classmethod
-    def depends(cls, user_model_class: type[Document]) -> typing.Any:
+    def depends(self) -> typing.Any:
         """Provide the authenticated user to views that require it."""
 
         async def retrieve_user(
-            request: Request, jwt_cookie: str = Cookie(default="", alias=cls.get_auth_cookie_key())
-        ) -> "Document":
-            user = None
-            if jwt_cookie:
-                try:
-                    jwt_data = jwt.decode(jwt_cookie, key=AppSettings.CRYPTO_SECRET, algorithms=["HS256"])
-                except jwt.exceptions.InvalidTokenError:
-                    pass
-                else:
-                    user = await user_model_class.get(jwt_data["user_id"])
-            if not user:
+            request: Request,
+            jwt_token: str = Cookie(default="", alias=self.get_auth_cookie_key()),
+        ) -> UserT:
+            try:
+                return await self.find_user(jwt_token=jwt_token)
+            except (Object404Error, jwt.exceptions.InvalidTokenError) as exc:
                 raise HTTPException(
-                    status_code=status.HTTP_307_TEMPORARY_REDIRECT, headers={"Location": cls.get_auth_login_url()}
-                )
-            return user
+                    status_code=status.HTTP_307_TEMPORARY_REDIRECT,
+                    headers={"Location": self.get_auth_login_url()},
+                ) from exc
 
         return Depends(retrieve_user)
 
 
 class JWTAuthBackend(AuthenticationBackend, JWTAuth):
     """Starlette Backend to authenticate use through JWT Token in Cookies."""
 
-    user_model: type[Document]
-
-    def __init__(self, user_model: type[Document]) -> None:
-        """Initialize the authentication backend.
-
-        :param user_model_class: The User model.
-        """
-        super().__init__()
-        self.user_model = user_model
-
-    async def authenticate(self, conn)-> typing.Optional[typing.Tuple["AuthCredentials", "BaseUser"]]:
+    async def authenticate(self, conn: HTTPConnection) -> typing.Optional[typing.Tuple["AuthCredentials", "BaseUser"]]:
         """Authenticate the user using Cookies."""
         if self.get_auth_cookie_key() not in conn.cookies:
-            return
+            return None
 
         jwt_cookie = conn.cookies[self.get_auth_cookie_key()]
 
         try:
             jwt_data = jwt.decode(jwt_cookie, key=AppSettings.CRYPTO_SECRET, algorithms=["HS256"])
-        except jwt.exceptions.InvalidTokenError:
-            raise AuthenticationError("Invalid JWT token")
-        else:
-            user = await self.user_model.get(jwt_data["user_id"])
+        except jwt.exceptions.InvalidTokenError as exc:
+            raise AuthenticationError("Invalid JWT token") from exc
+
+        user = await self.user_model.get_or_404(jwt_data["user_id"])
 
         return AuthCredentials([user.get_scopes()]), user
 
 
 class BasicAuthBackend(AuthenticationBackend):
     """Starlette Backend to authenticate use through Basic Token in Header."""
 
     user_model: type[Document]
     auth_key_attribute: str
 
-    def __init__(self, user_model: type[Document], auth_key_attribute: str = "auth_key") -> None:
+    def __init__(self, user_model: type[UserT], auth_key_attribute: str = "auth_key") -> None:
         """Initialize the authentication backend.
 
-        :param user_model_class: The User model
+        :param user_model: The User model
         :param auth_key_attribute: The authentication key attribute on the User model
         """
         super().__init__()
         self.user_model = user_model
         self.auth_key_attribute = auth_key_attribute
 
-    async def authenticate(self, conn):
+    async def authenticate(self, conn: HTTPConnection) -> typing.Optional[typing.Tuple["AuthCredentials", "BaseUser"]]:
         """Authenticate the user use the Authorization headers."""
         if "Authorization" not in conn.headers:
-            return
+            return None
 
         auth = conn.headers["Authorization"]
+        scheme, credentials = auth.split()
+        if scheme.lower() != "basic":
+            return None
         try:
-            scheme, credentials = auth.split()
-            if scheme.lower() != "basic":
-                return
             decoded = base64.b64decode(credentials).decode("ascii")
-        except (ValueError, UnicodeDecodeError, binascii.Error):
-            raise AuthenticationError("Invalid basic auth credentials")
+        except (ValueError, UnicodeDecodeError, binascii.Error) as exc:
+            raise AuthenticationError("Invalid basic auth credentials") from exc
 
         username, _, pwd = decoded.partition(":")
 
         auth_key = getattr(self.user_model, self.auth_key_attribute)
         user = await self.user_model.find_one_or_404(auth_key == (username or pwd))
 
         return AuthCredentials(user.get_scopes()), user
```

### Comparing `sapx-0.1.7/sap/fastapi/exceptions.py` & `sapx-0.1.8/sap/fastapi/exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 """
 Exceptions.
 
 Group common logic exceptions such as ValidationError
 """
 from fastapi import HTTPException, status
 
-from sap.beanie.exceptions import Object404Error as Object404Error
+from sap.beanie.exceptions import Object404Error
 
 
 class Validation422Error(HTTPException):
     """Raise when querying DB returns empty result."""
 
     status_code: int = status.HTTP_422_UNPROCESSABLE_ENTITY
     detail: str = "The data submitted is invalid"
 
     def __init__(self, detail: str = ""):
         """Init exception."""
         super().__init__(status_code=status.HTTP_422_UNPROCESSABLE_ENTITY, detail=detail or self.detail)
+
+
+__all__ = [
+    "Object404Error",
+    "Validation422Error",
+]
```

### Comparing `sapx-0.1.7/sap/fastapi/middleware.py` & `sapx-0.1.8/sap/fastapi/middleware.py`

 * *Files identical despite different names*

### Comparing `sapx-0.1.7/sap/fastapi/serializers.py` & `sapx-0.1.8/sap/fastapi/serializers.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,92 +8,53 @@
 import datetime
 from typing import TYPE_CHECKING, Any, Generic, Optional, TypeVar, Union
 
 from fastapi import Request
 from pydantic import BaseModel
 from pydantic.fields import SHAPE_LIST, ModelField
 
-from sap.beanie.document import Document, TDoc
+from sap.beanie.document import DocT, Document
 
-from . import utils
-
-# SerializerType = TypeVar("SerializerType", bound=BaseModel)
+from .pagination import CursorInfo, PaginatedData
 
 if TYPE_CHECKING:
     from pydantic.typing import AbstractSetIntStr, DictStrAny, MappingIntStrAny
 
-
-class CursorInfo:
-    """Contains information on how the list should paginated."""
-
-    offset: int = 0
-    limit: int = 10
-    sort: str = "-doc_meta.created"
-
-    def __init__(self, request: Request) -> None:
-        """Initialize the cursor info."""
-        cursor_str = request.query_params.get("cursor", "")
-        try:
-            limit, offset = utils.base64_url_decode(cursor_str).split(",")
-        except ValueError:
-            return
-        self.limit, self.offset = int(limit), int(offset)
-
-    def get_beanie_query_params(self) -> dict[str, Any[int, str]]:
-        """Return params to apply to the database query when using beanie."""
-        return {
-            "limit": self.limit,
-            "skip": self.offset,
-            "sort": self.sort,
-        }
-
-    def get_next(self) -> Optional[str]:
-        """Get the cursor to paginate forward."""
-        offset = self.offset + self.limit
-        return utils.base64_url_encode(f"{self.limit},{offset}")
-
-    def get_previous(self) -> Optional[str]:
-        """Get the cursor to paginate backward."""
-        offset = self.offset - self.limit
-        if offset <= 0:
-            return None
-        return utils.base64_url_encode(f"{self.limit},{offset}")
+    ExcludeType = Union[AbstractSetIntStr, MappingIntStrAny]
 
 
-class ObjectSerializer(Generic[TDoc], BaseModel):
+class ObjectSerializer(Generic[DocT], BaseModel):
     """Serialize an object for retrieve or list."""
 
     @classmethod
-    def get_id(cls, instance: TDoc) -> str:
+    def get_id(cls, instance: DocT) -> str:
         """Return the Mongo ID of the object."""
         return str(instance.id)
 
     @classmethod
-    def get_created(cls, instance: TDoc) -> datetime.datetime:
+    def get_created(cls, instance: DocT) -> datetime.datetime:
         """Return the user creation date."""
         assert instance.doc_meta.created  # let mypy know that this cannot be null
         return instance.doc_meta.created
 
     @classmethod
-    def get_updated(cls, instance: TDoc) -> datetime.datetime:
+    def get_updated(cls, instance: DocT) -> datetime.datetime:
         """Return the user creation date."""
         assert instance.doc_meta.updated  # let mypy know that this cannot be null
         return instance.doc_meta.updated
 
     @classmethod
-    def _get_instance_data(
-        cls, instance: TDoc, exclude: Union["AbstractSetIntStr", "MappingIntStrAny"] = None
-    ) -> dict[str, Any]:
+    def _get_instance_data(cls, instance: DocT, exclude: Optional["ExcludeType"] = None) -> dict[str, Any]:
         """Retrieve the serializer value from the instance and getters."""
         data = {}
         exclude = exclude or set()
         for field_name, field in cls.__fields__.items():
             if field_name in exclude:
                 continue
-            elif hasattr(cls, f"get_{field_name}"):
+            if hasattr(cls, f"get_{field_name}"):
                 data[field_name] = getattr(cls, f"get_{field_name}")(instance=instance)
             elif issubclass(field.type_, ObjectSerializer):
                 related_object = getattr(instance, field_name, None)
                 if field.shape == SHAPE_LIST:
                     data[field_name] = (
                         field.type_.read_list(related_object, exclude=field.field_info.exclude)
                         if related_object
@@ -104,151 +65,147 @@
                         field.type_.read(related_object, exclude=field.field_info.exclude) if related_object else None
                     )
             else:
                 data[field_name] = getattr(instance, field_name)
         return data
 
     @classmethod
-    def read(cls, instance: TDoc, exclude: Union["AbstractSetIntStr", "MappingIntStrAny"] = None) -> "SerializerType":
+    def read(cls: type["SerializerT"], instance: DocT, exclude: Optional["ExcludeType"] = None) -> "SerializerT":
         """Serialize a single object instance."""
         return cls(**cls._get_instance_data(instance, exclude=exclude))
 
     @classmethod
     def read_list(
-        cls, instance_list: list[TDoc], exclude: Union["AbstractSetIntStr", "MappingIntStrAny"] = None
-    ) -> list["SerializerType"]:
+        cls: type["SerializerT"], instance_list: list[DocT], exclude: Optional["ExcludeType"] = None
+    ) -> list["SerializerT"]:
         """Serialize a list of objects."""
         return [cls.read(instance, exclude=exclude) for instance in instance_list]
 
     @classmethod
     def read_page(
         cls,
-        instance_list: list[TDoc],
+        instance_list: list[DocT],
         cursor_info: CursorInfo,
         request: Request,
-    ) -> PaginatedData["SerializerType"]:
+    ) -> PaginatedData["SerializerT"]:
         """Serialize a list of objects."""
 
         # TODO: implemented proper cursor pagination, for now fake it till you make it.
 
-        next = cursor_info.get_next()
-        previous = cursor_info.get_previous()
+        page_next = cursor_info.get_next()
+        page_previous = cursor_info.get_previous()
         return PaginatedData(
             count=0,
-            next=str(request.url.include_query_params(cursor=next)) if next else None,
-            previous=str(request.url.include_query_params(cursor=previous)) if previous else None,
+            next=str(request.url.include_query_params(cursor=page_next)) if page_next else None,
+            previous=str(request.url.include_query_params(cursor=page_previous)) if page_previous else None,
             data=cls.read_list(instance_list),
         )
 
 
-SerializerType = TypeVar("SerializerType", bound=ObjectSerializer)
-
-
-class PaginatedData(Generic[SerializerType], BaseModel):
-    """Represent the structure of an API paginated list response."""
-
-    object: str = "list"
-    count: int
-    next: Optional[str]
-    previous: Optional[str]
-    data: list[Any]
+SerializerT = TypeVar("SerializerT", bound=ObjectSerializer[Any])
 
 
-class WriteObjectSerializer(Generic[TDoc], BaseModel):
+class WriteObjectSerializer(Generic[DocT], BaseModel):
     """Serialize an object for create or update."""
 
-    instance: Optional[TDoc] = None
+    instance: Optional[DocT] = None
 
     async def run_async_validators(self) -> None:
         """Check that data pass DB validation."""
 
         field: ModelField
         embedded_serializers = {}
         for field_name, field in self.__fields__.items():
             if issubclass(field.type_, WriteObjectSerializer):
                 embedded_serializers[field_name] = field
 
-        field_serializer: WriteObjectSerializer[TDoc]
+        field_serializer: WriteObjectSerializer[DocT]
         for field_name in embedded_serializers:
             if field_serializer := getattr(self, field_name):
                 if self.instance:
                     field_serializer.instance = getattr(self.instance, field_name)
                 await field_serializer.run_async_validators()
 
     def dict(
         self,
         *,
-        include: Optional[Union["AbstractSetIntStr", "MappingIntStrAny"]] = None,
-        exclude: Optional[Union["AbstractSetIntStr", "MappingIntStrAny"]] = None,
+        include: Optional["ExcludeType"] = None,
+        exclude: Optional["ExcludeType"] = None,
         by_alias: bool = False,
         skip_defaults: Optional[bool] = None,
         exclude_unset: bool = False,
         exclude_defaults: bool = False,
         exclude_none: bool = False,
     ) -> "DictStrAny":
         """Dump the serializer data with exclusion of unwanted fields."""
         # Exclude from dumping
-        exclude = (exclude or {}) | {"instance": True}
+        exclude_: dict[Union[int, str], bool] = {"instance": True}
+        if exclude:
+            for x in exclude:
+                exclude_[x] = True
 
         # Some fields are only excluded from being cascade dumps to dict,
         # but their original value is still needed
         exclude_doc_dumps = {}
 
         # Embedded documents need to be converted to object after dumps
         embedded_serializers = {}
 
         for field_name, field in self.__fields__.items():
-            if field_name in exclude:
+            if field_name in exclude_:
                 continue
 
             if issubclass(field.type_, Document):
                 exclude_doc_dumps[field_name] = True
+                exclude_[field_name] = True
 
-            if issubclass(field.type_, WriteObjectSerializer):
+            elif issubclass(field.type_, WriteObjectSerializer):
                 embedded_serializers[field_name] = field.type_.__fields__["instance"].type_
 
-            # Some fields are excluded as they are only needed for create
-            if field.field_info.extra.get("exclude_update") and self.instance:
-                exclude[field_name] = True
-
-            # Some fields are excluded as they are only needed for update
-            if field.field_info.extra.get("exclude_create") and not self.instance:
-                exclude[field_name] = True
-
-        exclude = exclude | exclude_doc_dumps
+            # # Some fields are excluded as they are only needed for create
+            # if field.field_info.extra.get("exclude_update") and self.instance:
+            #     exclude_[field_name] = True
+
+            # # Some fields are excluded as they are only needed for update
+            # elif field.field_info.extra.get("exclude_create") and not self.instance:
+            #     exclude_[field_name] = True
 
         result = super().dict(
             include=include,
-            exclude=exclude,
+            exclude=exclude_,
             by_alias=by_alias,
             skip_defaults=skip_defaults,
             exclude_unset=exclude_unset,
             exclude_defaults=exclude_defaults,
             exclude_none=exclude_none,
         )
 
         for field_name in exclude_doc_dumps:
             result[field_name] = getattr(self, field_name)
 
-        instance_embedded: BaseModel
+        instance_embedded: Optional[BaseModel]
         for field_name, field_model in embedded_serializers.items():
             if not result[field_name]:
                 continue
             if instance_embedded := getattr(self.instance, field_name, None):
                 result[field_name] = instance_embedded.copy(update=result[field_name])
             else:
                 result[field_name] = field_model(**result[field_name])
 
         return result
 
-    async def create(self, **kwargs: Any) -> TDoc:
+    async def create(self, **kwargs: Any) -> DocT:
         """Create the object in the database using the data extracted by the serializer."""
-        instance_class: type[TDoc] = self.__fields__["instance"].type_
+        instance_class: type[DocT] = self.__fields__["instance"].type_
         self.instance = await instance_class(**self.dict()).create()
         return self.instance
 
-    async def update(self, **kwargs: Any) -> TDoc:
+    async def update(self, **kwargs: Any) -> DocT:
         """Update the object in the database using the data extracted by the serializer."""
         assert self.instance
-        self.instance = self.instance.copy(update=self.dict())
-        await self.instance.save()
-        return self.instance
+        instance: DocT = self.instance.copy(update=self.dict())
+        await instance.save()
+        self.instance = instance
+        return instance
+
+
+WSerializerT = TypeVar("WSerializerT", bound=WriteObjectSerializer[Any])
```

### Comparing `sapx-0.1.7/sap/fastapi/utils.py` & `sapx-0.1.8/sap/fastapi/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 This file helps you centralized utility functions and classes
 that needs to be re-used but are not a core part of the app logic.
 """
 
 import base64
 import re
 from enum import Enum
-from typing import TYPE_CHECKING, Any
+from typing import TYPE_CHECKING, Any, Mapping, Optional
 
 from fastapi import Request
 
 if TYPE_CHECKING:
     from pydantic.error_wrappers import ErrorDict
 
 
@@ -80,15 +80,15 @@
 
 
 def base64_url_decode(text: str) -> str:
     """Decode a URL safely encoded b64."""
     return base64.urlsafe_b64decode(text.encode().ljust(len(text) + len(text) % 4, b"=")).decode()
 
 
-def merge_dict_deep(dict_a: dict[str, Any], dict_b: dict[str, Any], path=None) -> dict[str, Any]:
+def merge_dict_deep(dict_a: dict[str, Any], dict_b: dict[str, Any], path: Optional[list[str]] = None) -> dict[str, Any]:
     """
     Deep merge dictionaries. Merge b into a.
 
     ```python
         a = {1:{"a":{A}}, 2:{"b":{B}}}
         b = {2:{"c":{C}}, 3:{"d":{D}}}
 
@@ -113,15 +113,15 @@
             dict_a[key] = dict_b[key]
     return dict_a
 
 
 unflatten_regex = re.compile(r"(?P<key_parent>\w+)\[(?P<key_child>\w+)\]")
 
 
-def unflatten_form_data(form_data: dict[str, str]) -> dict[str, Any]:
+def unflatten_form_data(form_data: Mapping[str, Any]) -> dict[str, Any]:
     """
     Un-flatten a form data and return the corresponding cascading dict.
 
     ```python
     form_data = { "user[first_name]": "John", "user[last_name]": "Doe"}
 
     print(restructure_form_data(form_data))
```

### Comparing `sapx-0.1.7/sap/rest/client.py` & `sapx-0.1.8/sap/rest/client.py`

 * *Files identical despite different names*

### Comparing `sapx-0.1.7/sap/rest/exceptions.py` & `sapx-0.1.8/sap/rest/exceptions.py`

 * *Files identical despite different names*

### Comparing `sapx-0.1.7/sap/settings.py` & `sapx-0.1.8/sap/settings.py`

 * *Files identical despite different names*

### Comparing `sapx-0.1.7/sap/worker/__init__.py` & `sapx-0.1.8/sap/worker/__init__.py`

 * *Files identical despite different names*

### Comparing `sapx-0.1.7/sap/worker/amqp.py` & `sapx-0.1.8/sap/worker/amqp.py`

 * *Files identical despite different names*

### Comparing `sapx-0.1.7/sap/worker/config.py` & `sapx-0.1.8/sap/worker/config.py`

 * *Files identical despite different names*

### Comparing `sapx-0.1.7/sap/worker/crons.py` & `sapx-0.1.8/sap/worker/crons.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 Tasks.
 
 Background tasks that run a worker server.
 These tasks can run even while the user is not online,
 not making any active HTTP requests, or not using the application.
 """
 
-import typing
 from enum import IntEnum
+from typing import Any, Optional, TypedDict
 
 import celery
 import celery.schedules
 
 from sap.loggers import logger
 from sap.settings import SapSettings
 
@@ -19,53 +19,53 @@
 class FetchStrategy(IntEnum):
     """Define if new or old data should be fetched."""
 
     NEW: int = 1
     OLD: int = 2
 
 
-class CronResponse(typing.TypedDict, total=False):
+class CronResponse(TypedDict, total=False):
     """Define a standard cron task response."""
 
     error: dict[str, str]
     result: dict[str, int]
 
 
 class CronTask(celery.Task):
     """Define how cron task classes should be structured."""
 
     expires = 60 * 60  # automatically expires if not run within 1 hour
     time_limit = 60 * 60 * 3  # default to 3 hours, automatically kill the task if exceed the limit
-    args: list[typing.Any]
-    kwargs: dict[str, typing.Any]
+    args: list[Any]
+    kwargs: dict[str, Any]
     schedule: celery.schedules.crontab
 
-    def __init__(self, **kwargs: typing.Any) -> None:
+    def __init__(self, **kwargs: Any) -> None:
         """Initialize the cron task."""
         for k, v in kwargs.items():
             setattr(self, k, v)
 
     @classmethod
     def get_name(cls) -> str:
         """Get Name of the current Task."""
         return cls.__module__.split(".crons", maxsplit=1)[0] + "." + str(cls.__name__)
 
-    def get_queryset(self, *, batch_size: typing.Optional[int] = None, **kwargs: typing.Any) -> typing.Any:
+    def get_queryset(self, *, batch_size: Optional[int] = None, **kwargs: Any) -> Any:
         """Fetch the list of elements to process."""
         raise NotImplementedError
 
-    async def process(self, *, batch_size: int = 100, **kwargs: typing.Any) -> typing.Any:
+    async def process(self, *, batch_size: int = 100, **kwargs: Any) -> Any:
         """Run the cron task and process elements."""
         raise NotImplementedError
 
     async def get_stats(self) -> dict[str, int]:
         """Give stats about the number of elements left to process."""
         raise NotImplementedError
 
-    async def run(self) -> CronResponse:
+    async def run(self, *args: Any, **kwargs: Any) -> CronResponse:
         """Run the task and save meta info to Airtable."""
         response: CronResponse
 
         # B. Runs the task
         try:
             result = await self.process(**self.kwargs)
         except Exception as exc:  # pylint: disable=broad-except;
@@ -78,11 +78,11 @@
 
         return response
 
 
 def register_crontask(
     crontask_class: type[CronTask],
     schedule: celery.schedules.crontab,
-    kwargs: typing.Optional[dict[str, typing.Any]] = None,
+    kwargs: Optional[dict[str, Any]] = None,
 ) -> CronTask:
     """Register a task on the worker servers."""
     return crontask_class(schedule=schedule, kwargs=kwargs or {})
```

### Comparing `sapx-0.1.7/sap/worker/lambdas.py` & `sapx-0.1.8/sap/worker/lambdas.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Lambdas refers to async background tasks.
 
 They run code in response to events which are typically messages sent to a queue.
 """
 import asyncio
-import typing
+from typing import Any
 
 import celery
 import celery.bootsteps
 import celery.worker.consumer
 import kombu
 from kombu.transport.base import StdChannel  # Channel
 
@@ -25,32 +25,32 @@
     The Lambda will be connected to an AMQP Queue and will listen
     to packets sent to that queue that matches the packet's topic pattern.
     """
 
     time_limit: int = 60 * 1  # 1 minutes
     packet: SignalPacket
 
-    def __init__(self, **kwargs: typing.Any) -> None:
+    def __init__(self, **kwargs: Any) -> None:
         """Initialize lambda arguments."""
         self.name = self.get_name()
 
     def get_name(self) -> str:
         """Return a human-readable name for this lambda."""
         return self.__module__.split(".lambdas", maxsplit=1)[0] + "." + str(self.__name__)
 
-    def run(self, *args: str, **kwargs: typing.Any) -> dict[str, typing.Any]:
+    def run(self, *args: Any, **kwargs: Any) -> dict[str, Any]:
         """Run the task."""
         return asyncio.run(self.handle_receive(*args, **kwargs))
 
-    async def handle_receive(self, *args: str, **kwargs: typing.Any) -> dict[str, typing.Any]:
+    async def handle_receive(self, *args: Any, **kwargs: Any) -> dict[str, Any]:
         """Perform pre-check such as authentication and run the task."""
         raise NotImplementedError
 
 
-def register_lambda(lambda_task_class: typing.Type[LambdaTask]) -> LambdaTask:
+def register_lambda(lambda_task_class: type[LambdaTask]) -> LambdaTask:
     """Register the Lambda Task to make it discoverable by task runner (celery)."""
     return lambda_task_class()
 
 
 class LambdaWorker(celery.bootsteps.ConsumerStep):
     """Celery worker that consumes packets (messages) sent to lambda queues."""
 
@@ -91,15 +91,15 @@
                 queues=self._get_queues(channel),
                 callbacks=[self.consume],
                 accept=["json"],
                 prefetch_count=10,
             )
         ]
 
-    def consume(self, body: dict[str, typing.Any], message: kombu.Message) -> None:
+    def consume(self, body: dict[str, Any], message: kombu.Message) -> None:
         """
         Run the celery worker and consume messages.
 
         This is the entrypoint of the application once celery starts receiving messages.
         All packets received are sent to this function that will acknowledge reception and dispatch
         to registered Lambda tasks.
         """
@@ -112,15 +112,15 @@
             self._propagate_signal(body, message)
         except Exception as exc:  # pylint: disable=broad-except
             logger.exception(exc)
             message.reject()
         else:
             message.ack()
 
-    def _propagate_signal(self, body: dict[str, typing.Any], message: kombu.Message) -> None:
+    def _propagate_signal(self, body: dict[str, Any], message: kombu.Message) -> None:
         """
         Execute each lambda task that registered to that packet signal.
 
         Lambda tasks are all executed asynchronously and simultaneously through other background celery workers.
         Sometimes this can leads to duplicate key errors or integrity errors.
         """
         topic = message.delivery_info["routing_key"]
```

### Comparing `sapx-0.1.7/sap/worker/packet.py` & `sapx-0.1.8/sap/worker/packet.py`

 * *Files identical despite different names*

### Comparing `sapx-0.1.7/sap/worker/utils.py` & `sapx-0.1.8/sap/worker/utils.py`

 * *Files identical despite different names*

### Comparing `sapx-0.1.7/sapx.egg-info/PKG-INFO` & `sapx-0.1.8/sapx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sapx
-Version: 0.1.7
+Version: 0.1.8
 Summary: Library of re-usable utilities for python web apps.
 Home-page: https://github.com/trellixio/sap
 Author: Trellix Dev
 Author-email: contact@trellix.io
 License: COPYRIGHT @ Trellix
 Classifier: Environment :: Web Environment
 Classifier: Framework :: FastAPI
```

### Comparing `sapx-0.1.7/sapx.egg-info/SOURCES.txt` & `sapx-0.1.8/sapx.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -5,21 +5,26 @@
 sap/loggers.py
 sap/py.typed
 sap/settings.py
 sap/beanie/__init__.py
 sap/beanie/client.py
 sap/beanie/document.py
 sap/beanie/exceptions.py
-sap/beanie/models.py
+sap/beanie/link.py
+sap/beanie/mixins.py
+sap/beanie/patch.py
 sap/beanie/query.py
+sap/chart/__init__.py
+sap/chart/serializers.py
 sap/fastapi/__init__.py
 sap/fastapi/auth.py
 sap/fastapi/exceptions.py
 sap/fastapi/forms.py
 sap/fastapi/middleware.py
+sap/fastapi/pagination.py
 sap/fastapi/serializers.py
 sap/fastapi/utils.py
 sap/rest/__init__.py
 sap/rest/client.py
 sap/rest/exceptions.py
 sap/worker/__init__.py
 sap/worker/amqp.py
```

### Comparing `sapx-0.1.7/setup.py` & `sapx-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
-VERSION = "0.1.7"
+VERSION = "0.1.8"
 
 setup(
     name="sapx",
     version=VERSION,
     packages=find_packages(include=("sap.*", "sap")),
     package_data={"sap": ["py.typed"]},
     include_package_data=True,
@@ -31,14 +31,15 @@
         "redis~=4.5",
         "celery~=5.2",
         "pydantic~=1.10",
         "PyJWT~=2.6",
         "fastAPI~=0.89",
         "itsdangerous~=2.1",
         "beanie~=1.15",
+        "passlib~=1.7",
         "motor~=3.1",
         "sqlmodel~=0.0",
         "typing-extensions~=4.5",
         "PyYAML~=6.0",
     ],
     classifiers=[
         "Environment :: Web Environment",
```

### Comparing `sapx-0.1.7/tests/test_fastapi_utils.py` & `sapx-0.1.8/tests/test_fastapi_utils.py`

 * *Files identical despite different names*

### Comparing `sapx-0.1.7/tests/test_rest_client.py` & `sapx-0.1.8/tests/test_rest_client.py`

 * *Files identical despite different names*

### Comparing `sapx-0.1.7/tests/test_worker_lambdas.py` & `sapx-0.1.8/tests/test_worker_lambdas.py`

 * *Files identical despite different names*

### Comparing `sapx-0.1.7/tests/test_worker_packet.py` & `sapx-0.1.8/tests/test_worker_packet.py`

 * *Files identical despite different names*

