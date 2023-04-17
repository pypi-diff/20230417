# Comparing `tmp/redb-odm-1.1.6.tar.gz` & `tmp/redb-odm-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redb-odm-1.1.6.tar", last modified: Thu Mar 16 17:51:29 2023, max compression
+gzip compressed data, was "redb-odm-1.1.7.tar", last modified: Mon Apr 17 16:31:26 2023, max compression
```

## Comparing `redb-odm-1.1.6.tar` & `redb-odm-1.1.7.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 17:51:29.479709 redb-odm-1.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-16 17:51:16.000000 redb-odm-1.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-03-16 17:51:29.479709 redb-odm-1.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-16 17:51:16.000000 redb-odm-1.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 17:51:29.475709 redb-odm-1.1.6/redb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 17:51:29.475709 redb-odm-1.1.6/redb/behaviors/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-16 17:51:16.000000 redb-odm-1.1.6/redb/behaviors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-03-16 17:51:16.000000 redb-odm-1.1.6/redb/behaviors/soft_deletion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 17:51:29.475709 redb-odm-1.1.6/redb/core/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-03-16 17:51:16.000000 redb-odm-1.1.6/redb/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-03-16 17:51:16.000000 redb-odm-1.1.6/redb/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    16173 2023-03-16 17:51:16.000000 redb-odm-1.1.6/redb/core/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-03-16 17:51:16.000000 redb-odm-1.1.6/redb/core/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)    10019 2023-03-16 17:51:16.000000 redb-odm-1.1.6/redb/core/transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 17:51:29.479709 redb-odm-1.1.6/redb/interface/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 17:51:16.000000 redb-odm-1.1.6/redb/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-03-16 17:51:16.000000 redb-odm-1.1.6/redb/interface/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-03-16 17:51:16.000000 redb-odm-1.1.6/redb/interface/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-03-16 17:51:16.000000 redb-odm-1.1.6/redb/interface/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-03-16 17:51:16.000000 redb-odm-1.1.6/redb/interface/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-03-16 17:51:16.000000 redb-odm-1.1.6/redb/interface/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-03-16 17:51:16.000000 redb-odm-1.1.6/redb/interface/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-03-16 17:51:16.000000 redb-odm-1.1.6/redb/interface/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 17:51:29.479709 redb-odm-1.1.6/redb/json_system/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-16 17:51:16.000000 redb-odm-1.1.6/redb/json_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-03-16 17:51:16.000000 redb-odm-1.1.6/redb/json_system/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9263 2023-03-16 17:51:16.000000 redb-odm-1.1.6/redb/json_system/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-03-16 17:51:16.000000 redb-odm-1.1.6/redb/json_system/database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 17:51:29.479709 redb-odm-1.1.6/redb/migo_system/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-16 17:51:16.000000 redb-odm-1.1.6/redb/migo_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-03-16 17:51:16.000000 redb-odm-1.1.6/redb/migo_system/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-03-16 17:51:16.000000 redb-odm-1.1.6/redb/migo_system/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-03-16 17:51:16.000000 redb-odm-1.1.6/redb/migo_system/database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 17:51:29.479709 redb-odm-1.1.6/redb/mongo_system/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-16 17:51:16.000000 redb-odm-1.1.6/redb/mongo_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-03-16 17:51:16.000000 redb-odm-1.1.6/redb/mongo_system/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-03-16 17:51:16.000000 redb-odm-1.1.6/redb/mongo_system/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-03-16 17:51:16.000000 redb-odm-1.1.6/redb/mongo_system/database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 17:51:29.479709 redb-odm-1.1.6/redb_odm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-03-16 17:51:29.000000 redb-odm-1.1.6/redb_odm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-03-16 17:51:29.000000 redb-odm-1.1.6/redb_odm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 17:51:29.000000 redb-odm-1.1.6/redb_odm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-16 17:51:29.000000 redb-odm-1.1.6/redb_odm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-16 17:51:29.000000 redb-odm-1.1.6/redb_odm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-16 17:51:16.000000 redb-odm-1.1.6/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-16 17:51:16.000000 redb-odm-1.1.6/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-16 17:51:16.000000 redb-odm-1.1.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 17:51:29.479709 redb-odm-1.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-03-16 17:51:16.000000 redb-odm-1.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 17:51:29.479709 redb-odm-1.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-03-16 17:51:16.000000 redb-odm-1.1.6/tests/test_bson_objs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-03-16 17:51:16.000000 redb-odm-1.1.6/tests/test_hashing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-03-16 17:51:16.000000 redb-odm-1.1.6/tests/test_json_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-03-16 17:51:16.000000 redb-odm-1.1.6/tests/test_mongo_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-03-16 17:51:16.000000 redb-odm-1.1.6/tests/test_return_cls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-03-16 17:51:16.000000 redb-odm-1.1.6/tests/test_soft_deletion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:31:26.051141 redb-odm-1.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-17 16:31:10.000000 redb-odm-1.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-17 16:31:26.051141 redb-odm-1.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-17 16:31:10.000000 redb-odm-1.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:31:26.047141 redb-odm-1.1.7/redb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:31:26.047141 redb-odm-1.1.7/redb/behaviors/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-17 16:31:10.000000 redb-odm-1.1.7/redb/behaviors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-04-17 16:31:10.000000 redb-odm-1.1.7/redb/behaviors/soft_deletion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:31:26.047141 redb-odm-1.1.7/redb/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-17 16:31:10.000000 redb-odm-1.1.7/redb/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-04-17 16:31:10.000000 redb-odm-1.1.7/redb/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16207 2023-04-17 16:31:10.000000 redb-odm-1.1.7/redb/core/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-04-17 16:31:10.000000 redb-odm-1.1.7/redb/core/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10013 2023-04-17 16:31:10.000000 redb-odm-1.1.7/redb/core/transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:31:26.047141 redb-odm-1.1.7/redb/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 16:31:10.000000 redb-odm-1.1.7/redb/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-17 16:31:10.000000 redb-odm-1.1.7/redb/interface/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-17 16:31:10.000000 redb-odm-1.1.7/redb/interface/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-17 16:31:10.000000 redb-odm-1.1.7/redb/interface/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-17 16:31:10.000000 redb-odm-1.1.7/redb/interface/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-17 16:31:10.000000 redb-odm-1.1.7/redb/interface/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-04-17 16:31:10.000000 redb-odm-1.1.7/redb/interface/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-17 16:31:10.000000 redb-odm-1.1.7/redb/interface/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:31:26.051141 redb-odm-1.1.7/redb/json_system/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-17 16:31:10.000000 redb-odm-1.1.7/redb/json_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-17 16:31:10.000000 redb-odm-1.1.7/redb/json_system/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9263 2023-04-17 16:31:10.000000 redb-odm-1.1.7/redb/json_system/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-17 16:31:10.000000 redb-odm-1.1.7/redb/json_system/database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:31:26.051141 redb-odm-1.1.7/redb/migo_system/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-17 16:31:10.000000 redb-odm-1.1.7/redb/migo_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-17 16:31:10.000000 redb-odm-1.1.7/redb/migo_system/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-04-17 16:31:10.000000 redb-odm-1.1.7/redb/migo_system/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-17 16:31:10.000000 redb-odm-1.1.7/redb/migo_system/database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:31:26.051141 redb-odm-1.1.7/redb/mongo_system/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-17 16:31:10.000000 redb-odm-1.1.7/redb/mongo_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-04-17 16:31:10.000000 redb-odm-1.1.7/redb/mongo_system/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-04-17 16:31:10.000000 redb-odm-1.1.7/redb/mongo_system/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-17 16:31:10.000000 redb-odm-1.1.7/redb/mongo_system/database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:31:26.051141 redb-odm-1.1.7/redb_odm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-17 16:31:26.000000 redb-odm-1.1.7/redb_odm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-17 16:31:26.000000 redb-odm-1.1.7/redb_odm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 16:31:26.000000 redb-odm-1.1.7/redb_odm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-17 16:31:26.000000 redb-odm-1.1.7/redb_odm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-17 16:31:26.000000 redb-odm-1.1.7/redb_odm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-17 16:31:10.000000 redb-odm-1.1.7/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-17 16:31:10.000000 redb-odm-1.1.7/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-17 16:31:10.000000 redb-odm-1.1.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 16:31:26.051141 redb-odm-1.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-04-17 16:31:10.000000 redb-odm-1.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:31:26.051141 redb-odm-1.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-17 16:31:10.000000 redb-odm-1.1.7/tests/test_bson_objs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-04-17 16:31:10.000000 redb-odm-1.1.7/tests/test_hashing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-04-17 16:31:10.000000 redb-odm-1.1.7/tests/test_json_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-04-17 16:31:10.000000 redb-odm-1.1.7/tests/test_mongo_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-17 16:31:10.000000 redb-odm-1.1.7/tests/test_return_cls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-17 16:31:10.000000 redb-odm-1.1.7/tests/test_soft_deletion.py
```

### Comparing `redb-odm-1.1.6/redb/behaviors/soft_deletion.py` & `redb-odm-1.1.7/redb/behaviors/soft_deletion.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.6/redb/core/base.py` & `redb-odm-1.1.7/redb/core/base.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.6/redb/core/document.py` & `redb-odm-1.1.7/redb/core/document.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from datetime import datetime
 from typing import Any, Dict, Sequence, Type, TypeAlias, TypeVar, Union, cast
 
+import pytz
 from pymongo.errors import DuplicateKeyError
+
 from redb.interface.errors import (
     CannotUpdateIdentifyingField,
     UniqueConstraintViolation,
 )
 from redb.interface.fields import (
     CompoundIndex,
     DBRef,
@@ -34,20 +36,20 @@
 OptionalDocumentData: TypeAlias = Union["Document", dict[str, Any], None]
 SortColumns: TypeAlias = list[SortColumn] | SortColumn | None
 T = TypeVar("T", bound="Document")
 
 
 class Document(BaseDocument):
     id: str = Field(alias="_id")  # type: ignore
-    created_at: datetime = Field(default_factory=datetime.utcnow)  # type: ignore
-    updated_at: datetime = Field(default_factory=datetime.utcnow)  # type: ignore
+    created_at: datetime = Field(default_factory=lambda: datetime.now(pytz.UTC))  # type: ignore
+    updated_at: datetime = Field(default_factory=lambda: datetime.now(pytz.UTC))  # type: ignore
 
     class Config:
         json_encoders = {
-            datetime: lambda d: d.isoformat(),  # TODO: shouldn't we keep this as datetime?
+            datetime: lambda d: d.isoformat(),
             DBRef: lambda ref: dict(ref.as_doc()),
             ObjectId: str,
         }
         smart_union = True
 
     def __init__(self, **data: Any) -> None:
         calculate_hash = False
@@ -297,15 +299,15 @@
             filter=filter,
             update=update,
             upsert=upsert,
         )
         collection.update_one(
             cls=self.__class__,
             filter=filter,
-            update={"$set": {"updated_at": str(datetime.utcnow())}},
+            update={"$set": {"updated_at": datetime.now(pytz.UTC).isoformat()}},
         )
         return result
 
     @classmethod
     def update_one(
         cls,
         filter: DocumentData,
@@ -334,15 +336,15 @@
                 filter=filter,
                 update=update_data,
                 upsert=upsert,
             )
             collection.update_one(
                 cls=cls,
                 filter=filter,
-                update={"$set": {"updated_at": str(datetime.utcnow())}},
+                update={"$set": {"updated_at": datetime.now(pytz.UTC).isoformat()}},
             )
         except DuplicateKeyError as e:
             raise UniqueConstraintViolation(dup_keys=e.details["keyValue"])
         return result
 
     @classmethod
     def update_many(
@@ -373,15 +375,15 @@
                 filter=filter,
                 update=update,
                 upsert=upsert,
             )
             collection.update_many(
                 cls=cls,
                 filter=filter,
-                update={"$set": {"updated_at": str(datetime.utcnow())}},
+                update={"$set": {"updated_at": datetime.now(pytz.UTC).isoformat()}},
             )
         except DuplicateKeyError as e:
             raise UniqueConstraintViolation(dup_keys=e.details["keyValue"])
 
         return result
 
     def delete(self: T) -> DeleteOneResult:
```

### Comparing `redb-odm-1.1.6/redb/core/instance.py` & `redb-odm-1.1.7/redb/core/instance.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.6/redb/core/transaction.py` & `redb-odm-1.1.7/redb/core/transaction.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import contextlib
 from datetime import datetime
 from typing import Any, ContextManager, Dict, Sequence, Type, TypeVar, overload
 
+import pytz
 from pymongo.errors import DuplicateKeyError
-from redb.interface.errors import (
-    CannotUpdateIdentifyingField,
-    UniqueConstraintViolation,
-)
+
 from redb.core.document import (
     Document,
     DocumentData,
     IncludeColumns,
     OptionalDocumentData,
     SortColumns,
     _format_document_data,
@@ -37,14 +35,15 @@
 from redb.interface.configs import (
     CONFIG_TYPE,
     JSONConfig,
     MigoConfig,
     MongoConfig,
     check_config,
 )
+from redb.interface.errors import UniqueConstraintViolation
 
 T = TypeVar("T", bound=Document)
 
 
 class CollectionWrapper:
     def __init__(self, collection: Collection, collection_class: T) -> None:
         self.__collection = collection
@@ -215,15 +214,15 @@
             filter=filter,
             update=update,
             upsert=upsert,
         )
         self.__collection.update_one(
             cls=self.__collection_class,
             filter=filter,
-            update={"$set": {"updated_at": str(datetime.utcnow())}},
+            update={"$set": {"updated_at": datetime.now(pytz.UTC).isoformat()}},
         )
         return result
 
     def update_many(
         self,
         filter: DocumentData,
         update: DocumentData,
@@ -249,15 +248,15 @@
             filter=filter,
             update=update,
             upsert=upsert,
         )
         self.__collection.update_many(
             cls=self.__collection_class,
             filter=filter,
-            update={"$set": {"updated_at": str(datetime.utcnow())}},
+            update={"$set": {"updated_at": datetime.now(pytz.UTC).isoformat()}},
         )
         return result
 
     def delete_one(self, filter: DocumentData) -> DeleteOneResult:
         filter = _format_document_data(filter)
         return self.__collection.delete_one(
             cls=self.__collection_class,
```

### Comparing `redb-odm-1.1.6/redb/interface/client.py` & `redb-odm-1.1.7/redb/interface/client.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.6/redb/interface/collection.py` & `redb-odm-1.1.7/redb/interface/collection.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.6/redb/interface/configs.py` & `redb-odm-1.1.7/redb/interface/configs.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.6/redb/interface/database.py` & `redb-odm-1.1.7/redb/interface/database.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.6/redb/interface/fields.py` & `redb-odm-1.1.7/redb/interface/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 from types import UnionType
 from typing import Any, ForwardRef, Literal, TypeVar, Union, _UnionGenericAlias
 
 import pymongo
 from bson import DBRef as BsonDBRef
 from bson import ObjectId as BsonObjectId
 from pydantic import BaseModel
-from pydantic.fields import FieldInfo, ModelField
+from pydantic.fields import FieldInfo as PydanticFieldInfo
+from pydantic.fields import ModelField
 from pymongo.operations import (
     DeleteMany,
     DeleteOne,
     InsertOne,
     ReplaceOne,
     UpdateMany,
     UpdateOne,
@@ -86,27 +87,31 @@
     fields: list["ClassField"]
     name: str | None = None
     unique: bool = False
     direction: Direction = Direction.ASCENDING
     extras: dict | None = None
 
 
-class Field(FieldInfo):
+class FieldInfo(PydanticFieldInfo):
     def __init__(
         self,
         vector_type: str | None = None,
         dimensions: int | None = None,
         *args,
         **kwargs,
     ) -> None:
         super().__init__(*args, **kwargs)
         self.vector_type = vector_type
         self.dimensions = dimensions
 
 
+def Field(*args, **kwargs) -> Any:
+    return FieldInfo(*args, **kwargs)
+
+
 class ClassField:
     def __init__(self, model_field: ModelField, base_class: BaseModel):
         self.model_field = model_field
         self.base_class = base_class
         self.attr_names = [model_field.alias]
 
     def resolve(self, obj: T) -> T | None:
```

### Comparing `redb-odm-1.1.6/redb/interface/results.py` & `redb-odm-1.1.7/redb/interface/results.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.6/redb/json_system/client.py` & `redb-odm-1.1.7/redb/json_system/client.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.6/redb/json_system/collection.py` & `redb-odm-1.1.7/redb/json_system/collection.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.6/redb/json_system/database.py` & `redb-odm-1.1.7/redb/json_system/database.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.6/redb/migo_system/client.py` & `redb-odm-1.1.7/redb/migo_system/client.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.6/redb/migo_system/collection.py` & `redb-odm-1.1.7/redb/migo_system/collection.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.6/redb/migo_system/database.py` & `redb-odm-1.1.7/redb/migo_system/database.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.6/redb/mongo_system/client.py` & `redb-odm-1.1.7/redb/mongo_system/client.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.6/redb/mongo_system/collection.py` & `redb-odm-1.1.7/redb/mongo_system/collection.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.6/redb/mongo_system/database.py` & `redb-odm-1.1.7/redb/mongo_system/database.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.6/redb_odm.egg-info/SOURCES.txt` & `redb-odm-1.1.7/redb_odm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.6/setup.py` & `redb-odm-1.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.6/tests/test_bson_objs.py` & `redb-odm-1.1.7/tests/test_bson_objs.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.6/tests/test_hashing.py` & `redb-odm-1.1.7/tests/test_hashing.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.6/tests/test_json_client.py` & `redb-odm-1.1.7/tests/test_json_client.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.6/tests/test_mongo_system.py` & `redb-odm-1.1.7/tests/test_mongo_system.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.6/tests/test_return_cls.py` & `redb-odm-1.1.7/tests/test_return_cls.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.6/tests/test_soft_deletion.py` & `redb-odm-1.1.7/tests/test_soft_deletion.py`

 * *Files identical despite different names*

