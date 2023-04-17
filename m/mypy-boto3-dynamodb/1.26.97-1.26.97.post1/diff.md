# Comparing `tmp/mypy-boto3-dynamodb-1.26.97.tar.gz` & `tmp/mypy-boto3-dynamodb-1.26.97.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-dynamodb-1.26.97.tar", last modified: Wed Mar 22 20:21:41 2023, max compression
+gzip compressed data, was "mypy-boto3-dynamodb-1.26.97.post1.tar", last modified: Thu Mar 23 01:30:37 2023, max compression
```

## Comparing `mypy-boto3-dynamodb-1.26.97.tar` & `mypy-boto3-dynamodb-1.26.97.post1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-03-22 20:21:41.795140 mypy-boto3-dynamodb-1.26.97/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-03-22 20:21:10.000000 mypy-boto3-dynamodb-1.26.97/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    28235 2023-03-22 20:21:41.795140 mypy-boto3-dynamodb-1.26.97/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    26744 2023-03-22 20:21:10.000000 mypy-boto3-dynamodb-1.26.97/README.md
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-03-22 20:21:41.795140 mypy-boto3-dynamodb-1.26.97/mypy_boto3_dynamodb/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1858 2023-03-22 20:21:10.000000 mypy-boto3-dynamodb-1.26.97/mypy_boto3_dynamodb/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1856 2023-03-22 20:21:10.000000 mypy-boto3-dynamodb-1.26.97/mypy_boto3_dynamodb/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      911 2023-03-22 20:21:10.000000 mypy-boto3-dynamodb-1.26.97/mypy_boto3_dynamodb/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    53995 2023-03-22 20:21:11.000000 mypy-boto3-dynamodb-1.26.97/mypy_boto3_dynamodb/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    53928 2023-03-22 20:21:11.000000 mypy-boto3-dynamodb-1.26.97/mypy_boto3_dynamodb/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12660 2023-03-22 20:21:12.000000 mypy-boto3-dynamodb-1.26.97/mypy_boto3_dynamodb/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12658 2023-03-22 20:21:12.000000 mypy-boto3-dynamodb-1.26.97/mypy_boto3_dynamodb/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8387 2023-03-22 20:21:12.000000 mypy-boto3-dynamodb-1.26.97/mypy_boto3_dynamodb/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8380 2023-03-22 20:21:12.000000 mypy-boto3-dynamodb-1.26.97/mypy_boto3_dynamodb/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-03-22 20:21:10.000000 mypy-boto3-dynamodb-1.26.97/mypy_boto3_dynamodb/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    27160 2023-03-22 20:21:12.000000 mypy-boto3-dynamodb-1.26.97/mypy_boto3_dynamodb/service_resource.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    27133 2023-03-22 20:21:11.000000 mypy-boto3-dynamodb-1.26.97/mypy_boto3_dynamodb/service_resource.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)   151931 2023-03-22 20:21:15.000000 mypy-boto3-dynamodb-1.26.97/mypy_boto3_dynamodb/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)   151778 2023-03-22 20:21:14.000000 mypy-boto3-dynamodb-1.26.97/mypy_boto3_dynamodb/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       61 2023-03-22 20:21:10.000000 mypy-boto3-dynamodb-1.26.97/mypy_boto3_dynamodb/version.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2258 2023-03-22 20:21:12.000000 mypy-boto3-dynamodb-1.26.97/mypy_boto3_dynamodb/waiter.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2256 2023-03-22 20:21:12.000000 mypy-boto3-dynamodb-1.26.97/mypy_boto3_dynamodb/waiter.pyi
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-03-22 20:21:41.795140 mypy-boto3-dynamodb-1.26.97/mypy_boto3_dynamodb.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    28235 2023-03-22 20:21:41.000000 mypy-boto3-dynamodb-1.26.97/mypy_boto3_dynamodb.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      841 2023-03-22 20:21:41.000000 mypy-boto3-dynamodb-1.26.97/mypy_boto3_dynamodb.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-03-22 20:21:41.000000 mypy-boto3-dynamodb-1.26.97/mypy_boto3_dynamodb.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-03-22 20:21:41.000000 mypy-boto3-dynamodb-1.26.97/mypy_boto3_dynamodb.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-03-22 20:21:41.000000 mypy-boto3-dynamodb-1.26.97/mypy_boto3_dynamodb.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       20 2023-03-22 20:21:41.000000 mypy-boto3-dynamodb-1.26.97/mypy_boto3_dynamodb.egg-info/top_level.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-03-22 20:21:41.795140 mypy-boto3-dynamodb-1.26.97/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2003 2023-03-22 20:21:10.000000 mypy-boto3-dynamodb-1.26.97/setup.py
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-03-23 01:30:37.291124 mypy-boto3-dynamodb-1.26.97.post1/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     1070 2023-03-23 01:29:16.000000 mypy-boto3-dynamodb-1.26.97.post1/LICENSE
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)    28241 2023-03-23 01:30:37.291124 mypy-boto3-dynamodb-1.26.97.post1/PKG-INFO
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)    26744 2023-03-23 01:29:16.000000 mypy-boto3-dynamodb-1.26.97.post1/README.md
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-03-23 01:30:37.287124 mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     1858 2023-03-23 01:29:16.000000 mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/__init__.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     1856 2023-03-23 01:29:16.000000 mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/__init__.pyi
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)      923 2023-03-23 01:29:16.000000 mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/__main__.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)    53968 2023-03-23 01:29:17.000000 mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/client.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)    53901 2023-03-23 01:29:17.000000 mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/client.pyi
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)    12660 2023-03-23 01:29:18.000000 mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/literals.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)    12658 2023-03-23 01:29:18.000000 mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/literals.pyi
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     8360 2023-03-23 01:29:18.000000 mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/paginator.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     8353 2023-03-23 01:29:18.000000 mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/paginator.pyi
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-23 01:29:16.000000 mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/py.typed
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)    27133 2023-03-23 01:29:17.000000 mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/service_resource.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)    27106 2023-03-23 01:29:17.000000 mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/service_resource.pyi
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)   151904 2023-03-23 01:29:21.000000 mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/type_defs.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)   151751 2023-03-23 01:29:20.000000 mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/type_defs.pyi
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)       67 2023-03-23 01:29:16.000000 mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/version.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     2258 2023-03-23 01:29:18.000000 mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/waiter.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     2256 2023-03-23 01:29:18.000000 mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/waiter.pyi
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-03-23 01:30:37.291124 mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb.egg-info/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)    28241 2023-03-23 01:30:37.000000 mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb.egg-info/PKG-INFO
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)      841 2023-03-23 01:30:37.000000 mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb.egg-info/SOURCES.txt
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        1 2023-03-23 01:30:37.000000 mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb.egg-info/dependency_links.txt
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        1 2023-03-23 01:30:37.000000 mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb.egg-info/not-zip-safe
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)       52 2023-03-23 01:30:37.000000 mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb.egg-info/requires.txt
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)       20 2023-03-23 01:30:37.000000 mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb.egg-info/top_level.txt
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)       38 2023-03-23 01:30:37.291124 mypy-boto3-dynamodb-1.26.97.post1/setup.cfg
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     2009 2023-03-23 01:29:16.000000 mypy-boto3-dynamodb-1.26.97.post1/setup.py
```

### Comparing `mypy-boto3-dynamodb-1.26.97/LICENSE` & `mypy-boto3-dynamodb-1.26.97.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.26.97/PKG-INFO` & `mypy-boto3-dynamodb-1.26.97.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-dynamodb
-Version: 1.26.97
-Summary: Type annotations for boto3.DynamoDB 1.26.97 service generated with mypy-boto3-builder 7.13.0
+Version: 1.26.97.post1
+Summary: Type annotations for boto3.DynamoDB 1.26.97 service generated with mypy-boto3-builder 7.14.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -47,15 +47,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.13.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-dynamodb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-dynamodb-1.26.97/README.md` & `mypy-boto3-dynamodb-1.26.97.post1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.13.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-dynamodb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-dynamodb-1.26.97/mypy_boto3_dynamodb/__init__.py` & `mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.26.97/mypy_boto3_dynamodb/__init__.pyi` & `mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.26.97/mypy_boto3_dynamodb/__main__.py` & `mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DynamoDB 1.26.97\nVersion:         1.26.97\nBuilder version:"
-        " 7.13.0\nDocs:           "
+        "Type annotations for boto3.DynamoDB 1.26.97\nVersion:         1.26.97.post1\nBuilder"
+        " version: 7.14.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.97")
+    print("1.26.97.post1")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-dynamodb-1.26.97/mypy_boto3_dynamodb/client.py` & `mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,18 +10,17 @@
     from mypy_boto3_dynamodb.client import DynamoDBClient
 
     session = Session()
     client: DynamoDBClient = session.client("dynamodb")
     ```
 """
 import sys
-from collections.abc import Mapping, Sequence
 from datetime import datetime
 from decimal import Decimal
-from typing import Any, Dict, Set, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Set, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     BackupTypeFilterType,
     BillingModeType,
     ConditionalOperatorType,
```

### Comparing `mypy-boto3-dynamodb-1.26.97/mypy_boto3_dynamodb/client.pyi` & `mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -10,18 +10,17 @@
     from mypy_boto3_dynamodb.client import DynamoDBClient
 
     session = Session()
     client: DynamoDBClient = session.client("dynamodb")
     ```
 """
 import sys
-from collections.abc import Mapping, Sequence
 from datetime import datetime
 from decimal import Decimal
-from typing import Any, Dict, Set, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Set, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     BackupTypeFilterType,
     BillingModeType,
     ConditionalOperatorType,
```

### Comparing `mypy-boto3-dynamodb-1.26.97/mypy_boto3_dynamodb/literals.py` & `mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.26.97/mypy_boto3_dynamodb/literals.pyi` & `mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.26.97/mypy_boto3_dynamodb/paginator.py` & `mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,18 +23,17 @@
     list_backups_paginator: ListBackupsPaginator = client.get_paginator("list_backups")
     list_tables_paginator: ListTablesPaginator = client.get_paginator("list_tables")
     list_tags_of_resource_paginator: ListTagsOfResourcePaginator = client.get_paginator("list_tags_of_resource")
     query_paginator: QueryPaginator = client.get_paginator("query")
     scan_paginator: ScanPaginator = client.get_paginator("scan")
     ```
 """
-from collections.abc import Mapping, Sequence
 from datetime import datetime
 from decimal import Decimal
-from typing import Any, Generic, Iterator, Set, TypeVar, Union
+from typing import Any, Generic, Iterator, Mapping, Sequence, Set, TypeVar, Union
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import (
     BackupTypeFilterType,
     ConditionalOperatorType,
     ReturnConsumedCapacityType,
```

### Comparing `mypy-boto3-dynamodb-1.26.97/mypy_boto3_dynamodb/paginator.pyi` & `mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -23,18 +23,17 @@
     list_backups_paginator: ListBackupsPaginator = client.get_paginator("list_backups")
     list_tables_paginator: ListTablesPaginator = client.get_paginator("list_tables")
     list_tags_of_resource_paginator: ListTagsOfResourcePaginator = client.get_paginator("list_tags_of_resource")
     query_paginator: QueryPaginator = client.get_paginator("query")
     scan_paginator: ScanPaginator = client.get_paginator("scan")
     ```
 """
-from collections.abc import Mapping, Sequence
 from datetime import datetime
 from decimal import Decimal
-from typing import Any, Generic, Iterator, Set, TypeVar, Union
+from typing import Any, Generic, Iterator, Mapping, Sequence, Set, TypeVar, Union
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import (
     BackupTypeFilterType,
     ConditionalOperatorType,
     ReturnConsumedCapacityType,
```

### Comparing `mypy-boto3-dynamodb-1.26.97/mypy_boto3_dynamodb/service_resource.py` & `mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/service_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,18 +13,17 @@
 
     session = Session()
     resource: DynamoDBServiceResource = session.resource("dynamodb")
 
     my_table: dynamodb_resources.Table = resource.Table(...)
 ```
 """
-from collections.abc import Iterator, Mapping, Sequence
 from datetime import datetime
 from decimal import Decimal
-from typing import Any, List, Set, Union
+from typing import Any, Iterator, List, Mapping, Sequence, Set, Union
 
 from boto3.dynamodb.conditions import ConditionBase
 from boto3.dynamodb.table import BatchWriter
 from boto3.resources.base import ResourceMeta, ServiceResource
 from boto3.resources.collection import ResourceCollection
 
 from .client import DynamoDBClient
```

### Comparing `mypy-boto3-dynamodb-1.26.97/mypy_boto3_dynamodb/service_resource.pyi` & `mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/service_resource.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -13,18 +13,17 @@
 
     session = Session()
     resource: DynamoDBServiceResource = session.resource("dynamodb")
 
     my_table: dynamodb_resources.Table = resource.Table(...)
 ```
 """
-from collections.abc import Iterator, Mapping, Sequence
 from datetime import datetime
 from decimal import Decimal
-from typing import Any, List, Set, Union
+from typing import Any, Iterator, List, Mapping, Sequence, Set, Union
 
 from boto3.dynamodb.conditions import ConditionBase
 from boto3.dynamodb.table import BatchWriter
 from boto3.resources.base import ResourceMeta, ServiceResource
 from boto3.resources.collection import ResourceCollection
 
 from .client import DynamoDBClient
```

### Comparing `mypy-boto3-dynamodb-1.26.97/mypy_boto3_dynamodb/type_defs.py` & `mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,18 +8,17 @@
     ```python
     from mypy_boto3_dynamodb.type_defs import ResponseMetadataTypeDef
 
     data: ResponseMetadataTypeDef = {...}
     ```
 """
 import sys
-from collections.abc import Mapping, Sequence
 from datetime import datetime
 from decimal import Decimal
-from typing import Any, Dict, List, Set, Union
+from typing import Any, Dict, List, Mapping, Sequence, Set, Union
 
 from boto3.dynamodb.conditions import ConditionBase
 
 from .literals import (
     AttributeActionType,
     BackupStatusType,
     BackupTypeFilterType,
```

### Comparing `mypy-boto3-dynamodb-1.26.97/mypy_boto3_dynamodb/type_defs.pyi` & `mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -8,18 +8,17 @@
     ```python
     from mypy_boto3_dynamodb.type_defs import ResponseMetadataTypeDef
 
     data: ResponseMetadataTypeDef = {...}
     ```
 """
 import sys
-from collections.abc import Mapping, Sequence
 from datetime import datetime
 from decimal import Decimal
-from typing import Any, Dict, List, Set, Union
+from typing import Any, Dict, List, Mapping, Sequence, Set, Union
 
 from boto3.dynamodb.conditions import ConditionBase
 
 from .literals import (
     AttributeActionType,
     BackupStatusType,
     BackupTypeFilterType,
```

### Comparing `mypy-boto3-dynamodb-1.26.97/mypy_boto3_dynamodb/waiter.py` & `mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.26.97/mypy_boto3_dynamodb/waiter.pyi` & `mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.26.97/mypy_boto3_dynamodb.egg-info/PKG-INFO` & `mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-dynamodb
-Version: 1.26.97
-Summary: Type annotations for boto3.DynamoDB 1.26.97 service generated with mypy-boto3-builder 7.13.0
+Version: 1.26.97.post1
+Summary: Type annotations for boto3.DynamoDB 1.26.97 service generated with mypy-boto3-builder 7.14.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -47,15 +47,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.13.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-dynamodb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-dynamodb-1.26.97/mypy_boto3_dynamodb.egg-info/SOURCES.txt` & `mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.26.97/setup.py` & `mypy-boto3-dynamodb-1.26.97.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-dynamodb",
-    version="1.26.97",
+    version="1.26.97.post1",
     packages=["mypy_boto3_dynamodb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.DynamoDB 1.26.97 service generated with mypy-boto3-builder"
-        " 7.13.0"
+        " 7.14.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

