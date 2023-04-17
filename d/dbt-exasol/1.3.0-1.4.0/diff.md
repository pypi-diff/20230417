# Comparing `tmp/dbt_exasol-1.3.0.tar.gz` & `tmp/dbt_exasol-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_exasol-1.3.0.tar", max compression
+gzip compressed data, was "dbt_exasol-1.4.0.tar", max compression
```

## Comparing `dbt_exasol-1.3.0.tar` & `dbt_exasol-1.4.0.tar`

### file list

```diff
@@ -1,52 +1,56 @@
--rwxr-xr-x   0        0        0    35148 2021-12-30 07:56:19.472113 dbt_exasol-1.3.0/LICENSE
--rw-r--r--   0        0        0     2366 2023-04-14 08:24:45.854787 dbt_exasol-1.3.0/README.md
--rw-r--r--   0        0        0       65 2022-10-31 12:37:40.605136 dbt_exasol-1.3.0/dbt/__init__.py
--rw-r--r--   0        0        0       65 2022-10-31 12:37:40.605307 dbt_exasol-1.3.0/dbt/adapters/__init__.py
--rw-r--r--   0        0        0      508 2022-09-24 11:49:10.227324 dbt_exasol-1.3.0/dbt/adapters/exasol/__init__.py
--rw-r--r--   0        0        0     3681 2023-04-14 08:24:39.818253 dbt_exasol-1.3.0/dbt/adapters/exasol/column.py
--rw-r--r--   0        0        0    10262 2023-04-14 08:24:45.855156 dbt_exasol-1.3.0/dbt/adapters/exasol/connections.py
--rw-r--r--   0        0        0     2808 2023-04-14 08:24:45.855514 dbt_exasol-1.3.0/dbt/adapters/exasol/impl.py
--rw-r--r--   0        0        0     1921 2023-04-14 08:24:39.820270 dbt_exasol-1.3.0/dbt/adapters/exasol/relation.py
--rw-r--r--   0        0        0       65 2022-10-31 12:37:40.606232 dbt_exasol-1.3.0/dbt/include/__init__.py
--rw-r--r--   0        0        0       52 2022-10-31 12:37:40.606685 dbt_exasol-1.3.0/dbt/include/exasol/__init__.py
--rwxr-xr-x   0        0        0      236 2021-12-30 07:56:19.481658 dbt_exasol-1.3.0/dbt/include/exasol/__pycache__/__init__.cpython-37.pyc
--rwxr-xr-x   0        0        0       74 2021-12-30 07:56:19.482361 dbt_exasol-1.3.0/dbt/include/exasol/dbt_project.yml
--rw-r--r--   0        0        0     6477 2023-04-14 08:24:39.820776 dbt_exasol-1.3.0/dbt/include/exasol/macros/adapters.sql
--rw-r--r--   0        0        0      673 2022-09-24 11:49:10.228097 dbt_exasol-1.3.0/dbt/include/exasol/macros/apply_grants.sql
--rwxr-xr-x   0        0        0     1458 2021-12-30 07:56:19.483484 dbt_exasol-1.3.0/dbt/include/exasol/macros/catalog.sql
--rw-r--r--   0        0        0     4239 2023-04-14 08:24:45.855768 dbt_exasol-1.3.0/dbt/include/exasol/macros/materializations/incremental.sql
--rw-r--r--   0        0        0      259 2023-04-14 08:24:45.855900 dbt_exasol-1.3.0/dbt/include/exasol/macros/materializations/incremental_strategies.sql
--rw-r--r--   0        0        0      997 2023-04-14 08:24:45.856031 dbt_exasol-1.3.0/dbt/include/exasol/macros/materializations/merge.sql
--rwxr-xr-x   0        0        0      470 2021-12-30 07:56:19.484675 dbt_exasol-1.3.0/dbt/include/exasol/macros/materializations/seed.sql
--rw-r--r--   0        0        0     8044 2022-12-14 10:37:34.599267 dbt_exasol-1.3.0/dbt/include/exasol/macros/materializations/snapshot.sql
--rw-r--r--   0        0        0      748 2022-09-23 10:36:06.838210 dbt_exasol-1.3.0/dbt/include/exasol/macros/materializations/snapshot_merge.sql
--rw-r--r--   0        0        0     3258 2023-04-05 08:18:56.802378 dbt_exasol-1.3.0/dbt/include/exasol/macros/materializations/strategies.sql
--rw-r--r--   0        0        0     3524 2023-04-02 07:58:27.134719 dbt_exasol-1.3.0/dbt/include/exasol/macros/materializations/table.sql
--rw-r--r--   0        0        0      178 2022-09-24 11:49:10.228609 dbt_exasol-1.3.0/dbt/include/exasol/macros/utils/any_value.sql
--rw-r--r--   0        0        0       85 2022-09-24 11:49:10.228793 dbt_exasol-1.3.0/dbt/include/exasol/macros/utils/bool_or.sql
--rw-r--r--   0        0        0      469 2023-04-05 08:14:10.615503 dbt_exasol-1.3.0/dbt/include/exasol/macros/utils/dateadd.sql
--rw-r--r--   0        0        0      441 2023-04-04 22:40:13.470680 dbt_exasol-1.3.0/dbt/include/exasol/macros/utils/datediff.sql
--rw-r--r--   0        0        0      130 2022-09-24 11:49:10.229328 dbt_exasol-1.3.0/dbt/include/exasol/macros/utils/hash.sql
--rw-r--r--   0        0        0      381 2023-04-03 10:32:45.345850 dbt_exasol-1.3.0/dbt/include/exasol/macros/utils/last_day.sql
--rw-r--r--   0        0        0      415 2023-04-05 08:14:16.076524 dbt_exasol-1.3.0/dbt/include/exasol/macros/utils/listagg.sql
--rw-r--r--   0        0        0      775 2022-09-24 11:49:10.229642 dbt_exasol-1.3.0/dbt/include/exasol/macros/utils/safe_cast.sql
--rw-r--r--   0        0        0      165 2023-04-04 22:33:31.780189 dbt_exasol-1.3.0/dbt/include/exasol/macros/utils/split_part.sql
--rw-r--r--   0        0        0      898 2023-04-14 08:24:45.857180 dbt_exasol-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      606 2023-04-03 10:32:45.347355 dbt_exasol-1.3.0/tests/conftest.py
--rw-r--r--   0        0        0     7729 2023-04-03 10:32:45.347626 dbt_exasol-1.3.0/tests/functional/adapter/expected_catalog.py
--rw-r--r--   0        0        0     1438 2023-04-03 10:32:45.347717 dbt_exasol-1.3.0/tests/functional/adapter/files.py
--rw-r--r--   0        0        0      521 2023-04-03 10:32:45.347798 dbt_exasol-1.3.0/tests/functional/adapter/fixtures.py
--rw-r--r--   0        0        0     2708 2023-04-03 10:32:45.347983 dbt_exasol-1.3.0/tests/functional/adapter/test_basic.py
--rw-r--r--   0        0        0     1255 2023-04-03 10:32:45.348130 dbt_exasol-1.3.0/tests/functional/adapter/test_concurrency.py
--rw-r--r--   0        0        0    12762 2023-04-03 10:32:45.348333 dbt_exasol-1.3.0/tests/functional/adapter/test_docs_generate.py
--rw-r--r--   0        0        0      457 2023-04-03 10:32:45.348436 dbt_exasol-1.3.0/tests/functional/adapter/test_ephemeral.py
--rw-r--r--   0        0        0     2068 2023-04-03 10:32:45.348518 dbt_exasol-1.3.0/tests/functional/adapter/test_failing_test.py
--rw-r--r--   0        0        0     1406 2023-04-14 08:24:39.823789 dbt_exasol-1.3.0/tests/functional/adapter/utils/data_types/test_data_types.py
--rw-r--r--   0        0        0      591 2023-04-05 08:20:04.514413 dbt_exasol-1.3.0/tests/functional/adapter/utils/data_types/test_type_bigint.py
--rw-r--r--   0        0        0    12256 2023-04-14 08:24:39.824139 dbt_exasol-1.3.0/tests/functional/adapter/utils/test_utils.py
--rw-r--r--   0        0        0    14496 2023-04-03 10:32:45.349250 dbt_exasol-1.3.0/tests/functional/adapter/utils/utils_fixtures.py
--rw-r--r--   0        0        0      932 2023-04-14 08:24:39.824767 dbt_exasol-1.3.0/tests/functional/test_grants.py
--rw-r--r--   0        0        0     8096 2022-12-14 12:35:07.724147 dbt_exasol-1.3.0/tests/functional/test_incremental.py
--rw-r--r--   0        0        0     1465 2022-12-09 10:46:24.315528 dbt_exasol-1.3.0/tests/functional/test_issues.py
--rw-r--r--   0        0        0     3485 1970-01-01 00:00:00.000000 dbt_exasol-1.3.0/setup.py
--rw-r--r--   0        0        0     3443 1970-01-01 00:00:00.000000 dbt_exasol-1.3.0/PKG-INFO
+-rwxr-xr-x   0        0        0    35148 2021-12-30 07:56:19.472113 dbt_exasol-1.4.0/LICENSE
+-rw-r--r--   0        0        0     2366 2023-04-14 09:01:39.934780 dbt_exasol-1.4.0/README.md
+-rw-r--r--   0        0        0       65 2022-10-31 12:37:40.605136 dbt_exasol-1.4.0/dbt/__init__.py
+-rw-r--r--   0        0        0       65 2022-10-31 12:37:40.605307 dbt_exasol-1.4.0/dbt/adapters/__init__.py
+-rw-r--r--   0        0        0      508 2022-09-24 11:49:10.227324 dbt_exasol-1.4.0/dbt/adapters/exasol/__init__.py
+-rw-r--r--   0        0        0     3675 2023-04-17 08:26:55.459892 dbt_exasol-1.4.0/dbt/adapters/exasol/column.py
+-rw-r--r--   0        0        0    10259 2023-04-17 08:26:55.460269 dbt_exasol-1.4.0/dbt/adapters/exasol/connections.py
+-rw-r--r--   0        0        0     2806 2023-04-17 08:26:55.460569 dbt_exasol-1.4.0/dbt/adapters/exasol/impl.py
+-rw-r--r--   0        0        0     1959 2023-04-17 08:26:55.460846 dbt_exasol-1.4.0/dbt/adapters/exasol/relation.py
+-rw-r--r--   0        0        0       65 2022-10-31 12:37:40.606232 dbt_exasol-1.4.0/dbt/include/__init__.py
+-rw-r--r--   0        0        0       52 2022-10-31 12:37:40.606685 dbt_exasol-1.4.0/dbt/include/exasol/__init__.py
+-rwxr-xr-x   0        0        0      236 2021-12-30 07:56:19.481658 dbt_exasol-1.4.0/dbt/include/exasol/__pycache__/__init__.cpython-37.pyc
+-rwxr-xr-x   0        0        0       74 2021-12-30 07:56:19.482361 dbt_exasol-1.4.0/dbt/include/exasol/dbt_project.yml
+-rw-r--r--   0        0        0     6240 2023-04-17 08:26:55.461167 dbt_exasol-1.4.0/dbt/include/exasol/macros/adapters.sql
+-rw-r--r--   0        0        0      673 2022-09-24 11:49:10.228097 dbt_exasol-1.4.0/dbt/include/exasol/macros/apply_grants.sql
+-rwxr-xr-x   0        0        0     1458 2021-12-30 07:56:19.483484 dbt_exasol-1.4.0/dbt/include/exasol/macros/catalog.sql
+-rw-r--r--   0        0        0     4239 2023-04-14 09:01:39.935574 dbt_exasol-1.4.0/dbt/include/exasol/macros/materializations/incremental.sql
+-rw-r--r--   0        0        0      259 2023-04-14 09:01:39.935866 dbt_exasol-1.4.0/dbt/include/exasol/macros/materializations/incremental_strategies.sql
+-rw-r--r--   0        0        0     1025 2023-04-17 08:26:55.461462 dbt_exasol-1.4.0/dbt/include/exasol/macros/materializations/merge.sql
+-rwxr-xr-x   0        0        0      470 2021-12-30 07:56:19.484675 dbt_exasol-1.4.0/dbt/include/exasol/macros/materializations/seed.sql
+-rw-r--r--   0        0        0     8044 2022-12-14 10:37:34.599267 dbt_exasol-1.4.0/dbt/include/exasol/macros/materializations/snapshot.sql
+-rw-r--r--   0        0        0      748 2022-09-23 10:36:06.838210 dbt_exasol-1.4.0/dbt/include/exasol/macros/materializations/snapshot_merge.sql
+-rw-r--r--   0        0        0     3258 2023-04-05 08:18:56.802378 dbt_exasol-1.4.0/dbt/include/exasol/macros/materializations/strategies.sql
+-rw-r--r--   0        0        0     3524 2023-04-02 07:58:27.134719 dbt_exasol-1.4.0/dbt/include/exasol/macros/materializations/table.sql
+-rw-r--r--   0        0        0      178 2022-09-24 11:49:10.228609 dbt_exasol-1.4.0/dbt/include/exasol/macros/utils/any_value.sql
+-rw-r--r--   0        0        0       85 2022-09-24 11:49:10.228793 dbt_exasol-1.4.0/dbt/include/exasol/macros/utils/bool_or.sql
+-rw-r--r--   0        0        0      469 2023-04-05 08:14:10.615503 dbt_exasol-1.4.0/dbt/include/exasol/macros/utils/dateadd.sql
+-rw-r--r--   0        0        0      441 2023-04-04 22:40:13.470680 dbt_exasol-1.4.0/dbt/include/exasol/macros/utils/datediff.sql
+-rw-r--r--   0        0        0      130 2022-09-24 11:49:10.229328 dbt_exasol-1.4.0/dbt/include/exasol/macros/utils/hash.sql
+-rw-r--r--   0        0        0      381 2023-04-03 10:32:45.345850 dbt_exasol-1.4.0/dbt/include/exasol/macros/utils/last_day.sql
+-rw-r--r--   0        0        0      415 2023-04-05 08:14:16.076524 dbt_exasol-1.4.0/dbt/include/exasol/macros/utils/listagg.sql
+-rw-r--r--   0        0        0      775 2022-09-24 11:49:10.229642 dbt_exasol-1.4.0/dbt/include/exasol/macros/utils/safe_cast.sql
+-rw-r--r--   0        0        0      165 2023-04-04 22:33:31.780189 dbt_exasol-1.4.0/dbt/include/exasol/macros/utils/split_part.sql
+-rw-r--r--   0        0        0      519 2023-04-17 08:26:55.461725 dbt_exasol-1.4.0/dbt/include/exasol/macros/utils/timestamps.sql
+-rw-r--r--   0        0        0      906 2023-04-17 08:26:55.463958 dbt_exasol-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0      606 2023-04-03 10:32:45.347355 dbt_exasol-1.4.0/tests/conftest.py
+-rw-r--r--   0        0        0     7729 2023-04-03 10:32:45.347626 dbt_exasol-1.4.0/tests/functional/adapter/expected_catalog.py
+-rw-r--r--   0        0        0     1438 2023-04-03 10:32:45.347717 dbt_exasol-1.4.0/tests/functional/adapter/files.py
+-rw-r--r--   0        0        0      521 2023-04-03 10:32:45.347798 dbt_exasol-1.4.0/tests/functional/adapter/fixtures.py
+-rw-r--r--   0        0        0      676 2023-04-17 08:26:55.464235 dbt_exasol-1.4.0/tests/functional/adapter/query_comment_tests/test_query_comment.py
+-rw-r--r--   0        0        0      190 2023-04-17 08:26:55.464501 dbt_exasol-1.4.0/tests/functional/adapter/relations/test_changing_relation_type.py
+-rw-r--r--   0        0        0     2708 2023-04-03 10:32:45.347983 dbt_exasol-1.4.0/tests/functional/adapter/test_basic.py
+-rw-r--r--   0        0        0     1255 2023-04-03 10:32:45.348130 dbt_exasol-1.4.0/tests/functional/adapter/test_concurrency.py
+-rw-r--r--   0        0        0    12762 2023-04-03 10:32:45.348333 dbt_exasol-1.4.0/tests/functional/adapter/test_docs_generate.py
+-rw-r--r--   0        0        0      457 2023-04-03 10:32:45.348436 dbt_exasol-1.4.0/tests/functional/adapter/test_ephemeral.py
+-rw-r--r--   0        0        0     2068 2023-04-03 10:32:45.348518 dbt_exasol-1.4.0/tests/functional/adapter/test_failing_test.py
+-rw-r--r--   0        0        0     1350 2023-04-17 08:26:55.464832 dbt_exasol-1.4.0/tests/functional/adapter/utils/data_types/test_data_types.py
+-rw-r--r--   0        0        0      591 2023-04-05 08:20:04.514413 dbt_exasol-1.4.0/tests/functional/adapter/utils/data_types/test_type_bigint.py
+-rw-r--r--   0        0        0     1167 2023-04-17 08:26:55.465064 dbt_exasol-1.4.0/tests/functional/adapter/utils/test_timestamps.py
+-rw-r--r--   0        0        0    12212 2023-04-17 08:26:55.465321 dbt_exasol-1.4.0/tests/functional/adapter/utils/test_utils.py
+-rw-r--r--   0        0        0    14496 2023-04-03 10:32:45.349250 dbt_exasol-1.4.0/tests/functional/adapter/utils/utils_fixtures.py
+-rw-r--r--   0        0        0      924 2023-04-17 08:26:55.465618 dbt_exasol-1.4.0/tests/functional/test_grants.py
+-rw-r--r--   0        0        0     8096 2022-12-14 12:35:07.724147 dbt_exasol-1.4.0/tests/functional/test_incremental.py
+-rw-r--r--   0        0        0     1465 2022-12-09 10:46:24.315528 dbt_exasol-1.4.0/tests/functional/test_issues.py
+-rw-r--r--   0        0        0     3604 1970-01-01 00:00:00.000000 dbt_exasol-1.4.0/setup.py
+-rw-r--r--   0        0        0     3169 1970-01-01 00:00:00.000000 dbt_exasol-1.4.0/PKG-INFO
```

### Comparing `dbt_exasol-1.3.0/LICENSE` & `dbt_exasol-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.3.0/README.md` & `dbt_exasol-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.3.0/dbt/adapters/exasol/column.py` & `dbt_exasol-1.4.0/dbt/adapters/exasol/column.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 dbt exasol adapter column module
 """
 import re
 from dataclasses import dataclass
 from typing import ClassVar, Dict
 
 from dbt.adapters.base.column import Column
-from dbt.exceptions import RuntimeException
+from dbt.exceptions import DbtRuntimeError
 
 
 @dataclass
 # pylint: disable=missing-function-docstring
 class ExasolColumn(Column):
     """Column implementation for exasol"""
 
@@ -48,57 +48,57 @@
         return self.dtype.lower().startswith("timestamp")
 
     def is_date(self) -> bool:
         return self.dtype.lower() == "date"
 
     def string_size(self) -> int:
         if not self.is_string():
-            raise RuntimeException("Called string_size() on non-string field!")
+            raise DbtRuntimeError("Called string_size() on non-string field!")
         if self.char_size is None:
             return 2000000
         return int(self.char_size)
 
     @classmethod
     def string_type(cls, size: int) -> str:
         return f"VARCHAR({size})"
 
     @classmethod
     # pylint: disable=raise-missing-from
     def from_description(cls, name: str, raw_data_type: str) -> "Column":
         match = re.match(r"([^(]+)(\([^)]+\))?", raw_data_type)
         if match is None:
-            raise RuntimeException(f'Could not interpret data type "{raw_data_type}"')
+            raise DbtRuntimeError(f'Could not interpret data type "{raw_data_type}"')
         data_type, size_info = match.groups()
         char_size = None
         numeric_precision = None
         numeric_scale = None
         if size_info is not None:
             # strip out the parentheses
             size_info = size_info[1:-1]
             parts = size_info.split(",")
             if len(parts) == 1:
                 try:
                     # handle things like HASHTYPE(16 BYTE)
                     size = re.sub(r"[^\d]", "", parts[0])
                     char_size = int(size)
                 except ValueError:
-                    raise RuntimeException(
+                    raise DbtRuntimeError(
                         f'Could not interpret data_type "{raw_data_type}": '
                         f'could not convert "{size}" to an integer'
                     )
             elif len(parts) == 2:
                 try:
                     numeric_precision = int(parts[0])
                 except ValueError:
-                    raise RuntimeException(
+                    raise DbtRuntimeError(
                         f'Could not interpret data_type "{raw_data_type}": '
                         f'could not convert "{parts[0]}" to an integer'
                     )
                 try:
                     numeric_scale = int(parts[1])
                 except ValueError:
-                    raise RuntimeException(
+                    raise DbtRuntimeError(
                         f'Could not interpret data_type "{raw_data_type}": '
                         f'could not convert "{parts[1]}" to an integer'
                     )
 
         return cls(name, data_type, char_size, numeric_precision, numeric_scale)
```

### Comparing `dbt_exasol-1.3.0/dbt/adapters/exasol/connections.py` & `dbt_exasol-1.4.0/dbt/adapters/exasol/connections.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,21 +132,21 @@
         try:
             yield
 
         except Exception as yielded_exception:
             LOGGER.debug(f"Error running SQL: {sql}")
             LOGGER.debug("Rolling back transaction.")
             self.rollback_if_open()
-            if isinstance(yielded_exception, dbt.exceptions.RuntimeException):
+            if isinstance(yielded_exception, dbt.exceptions.DbtRuntimeError):
                 # during a sql query, an internal to dbt exception was raised.
                 # this sounds a lot like a signal handler and probably has
                 # useful information, so raise it without modification.
                 raise
 
-            raise dbt.exceptions.RuntimeException(yielded_exception)
+            raise dbt.exceptions.DbtRuntimeError(yielded_exception)
 
     @classmethod
     def get_result_from_cursor(cls, cursor: Any) -> agate.Table:
         data: List[Any] = []
         column_names: List[str] = []
 
         if cursor.description is not None:
@@ -180,15 +180,15 @@
             if version == ProtocolVersionType.V1:
                 protocol_version = pyexasol.PROTOCOL_V1
             elif version == ProtocolVersionType.V2:
                 protocol_version = pyexasol.PROTOCOL_V2
             else:
                 protocol_version = pyexasol.PROTOCOL_V3
         except:
-            raise dbt.exceptions.RuntimeException(
+            raise dbt.exceptions.DbtRuntimeError(
                 f"{credentials.protocol_version} is not a valid protocol version."
             )
 
         def _connect():
             conn = connect(
                 dsn=credentials.dsn,
                 user=credentials.user,
```

### Comparing `dbt_exasol-1.3.0/dbt/adapters/exasol/impl.py` & `dbt_exasol-1.4.0/dbt/adapters/exasol/impl.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """dbt-exasol Adapter implementation extending SQLAdapter"""
 from __future__ import absolute_import
 
 from typing import Dict, Optional
 
 import agate
 from dbt.adapters.sql import SQLAdapter
-from dbt.exceptions import raise_compiler_error
+from dbt.exceptions import CompilationError
 from dbt.utils import filter_null_values
 
 from dbt.adapters.exasol import (ExasolColumn, ExasolConnectionManager,
                                  ExasolRelation)
 
 
 class ExasolAdapter(SQLAdapter):
@@ -68,15 +68,15 @@
     def quote_seed_column(self, column: str, quote_config: Optional[bool]) -> str:  # type: ignore
         quote_columns: bool = False
         if isinstance(quote_config, bool):
             quote_columns = quote_config
         elif quote_config is None:
             pass
         else:
-            raise_compiler_error(
+            raise CompilationError(
                 f'The seed configuration value of "quote_columns" has an '
                 f"invalid type {type(quote_config)}"
             )
 
         if quote_columns:
             return self.quote(column)
         return column
```

### Comparing `dbt_exasol-1.3.0/dbt/adapters/exasol/relation.py` & `dbt_exasol-1.4.0/dbt/adapters/exasol/relation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """dbt-exasol adapter relation module"""
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from typing import Optional, Type, TypeVar
 
 from dbt.adapters.base.relation import BaseRelation, Policy
 from dbt.contracts.relation import RelationType
 
 
 @dataclass
@@ -18,15 +18,15 @@
 Self = TypeVar("Self", bound="BaseRelation")
 
 
 @dataclass(frozen=True, eq=False, repr=False)
 class ExasolRelation(BaseRelation):
     """Relation implementation for exasol"""
 
-    quote_policy: ExasolQuotePolicy = ExasolQuotePolicy()
+    quote_policy: ExasolQuotePolicy = field(default_factory=lambda: ExasolQuotePolicy())
 
     @classmethod
     # pylint: disable=too-many-arguments
     # pylint: disable=redefined-builtin
     # pylint: disable=unused-argument
     def create(
         cls: Type[Self],
```

### Comparing `dbt_exasol-1.3.0/dbt/include/exasol/macros/adapters.sql` & `dbt_exasol-1.4.0/dbt/include/exasol/macros/adapters.sql`

 * *Files 1% similar despite different names*

```diff
@@ -81,23 +81,14 @@
 {% endmacro %}
 
 {% macro exasol__create_table_as(temporary, relation, sql) -%}
     CREATE OR REPLACE TABLE {{ relation.schema }}.{{ relation.identifier }} AS 
     {{ sql }}
 {% endmacro %}
 
-{% macro exasol__current_timestamp() -%}
-  current_timestamp
-{%- endmacro %}
-
-{% macro exasol__snapshot_string_as_time(timestamp) -%}
-    {%- set result = "to_timestamp('" ~ timestamp ~ "')" -%}
-    {{ return(result) }}
-{%- endmacro %}
-
 {% macro exasol__truncate_relation(relation) -%}
   {% call statement('truncate_relation') -%}
     truncate table {{ relation | replace('"', '') }}
   {%- endcall %}
 {% endmacro %}
 
 {% macro exasol__get_columns_in_relation(relation) -%}
```

### Comparing `dbt_exasol-1.3.0/dbt/include/exasol/macros/apply_grants.sql` & `dbt_exasol-1.4.0/dbt/include/exasol/macros/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.3.0/dbt/include/exasol/macros/catalog.sql` & `dbt_exasol-1.4.0/dbt/include/exasol/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.3.0/dbt/include/exasol/macros/materializations/incremental.sql` & `dbt_exasol-1.4.0/dbt/include/exasol/macros/materializations/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.3.0/dbt/include/exasol/macros/materializations/merge.sql` & `dbt_exasol-1.4.0/dbt/include/exasol/macros/materializations/merge.sql`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% macro exasol__get_delete_insert_merge_sql(target, source, unique_key, dest_columns) -%}
+{% macro exasol__get_delete_insert_merge_sql(target, source, unique_key, dest_columns,incremental_predicates=none) -%}
 
     {%- set dest_cols_csv = get_quoted_csv(dest_columns | map(attribute="name")) -%}
 
     {% if unique_key %}
         {% if unique_key is sequence and unique_key is not string %}
             delete from {{ target }}
             where exists ( select 1 from {{ source }}
```

### Comparing `dbt_exasol-1.3.0/dbt/include/exasol/macros/materializations/snapshot.sql` & `dbt_exasol-1.4.0/dbt/include/exasol/macros/materializations/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.3.0/dbt/include/exasol/macros/materializations/snapshot_merge.sql` & `dbt_exasol-1.4.0/dbt/include/exasol/macros/materializations/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.3.0/dbt/include/exasol/macros/materializations/strategies.sql` & `dbt_exasol-1.4.0/dbt/include/exasol/macros/materializations/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.3.0/dbt/include/exasol/macros/materializations/table.sql` & `dbt_exasol-1.4.0/dbt/include/exasol/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.3.0/dbt/include/exasol/macros/utils/safe_cast.sql` & `dbt_exasol-1.4.0/dbt/include/exasol/macros/utils/safe_cast.sql`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.3.0/pyproject.toml` & `dbt_exasol-1.4.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [tool.poetry]
 name = "dbt-exasol"
-version = "1.3.0"
+version = "1.4.0"
 description = "Adapter to dbt-core for warehouse Exasol"
 authors = ["Torsten Glunde <torsten.glunde@alligator-company.com>", "Ilija Kutle <ilija.kutle@alligator-company.com>"]
 homepage = "https://alligatorcompany.gitlab.io/dbt-exasol"
 repository = "https://github.com/tglunde/dbt-exasol"
 packages = [
   { include = "dbt" },
   { include = "dbt/**/*.py" },
   { include = "tests/**/*.py"}
 ]
 license = "GPL3"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-dbt-core = "^1.3, <1.4"
+python = "^3.8, <3.12"
+dbt-core = "^1.4, <1.5"
 pyexasol = "^0.25.0"
-dbt-tests-adapter = "^1.3, <1.4"
+sqlfluff = "^2.0.2"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
+pylint = "^2.15.8"
+exceptiongroup = "^1.1.1"
 black = "^22.8.0"
 pytest = "^7.1.3"
 pytest-dotenv = "^0.5.2"
 tox = "^3.26.0"
-
-[tool.poetry.group.dev.dependencies]
-dbt-tests-adapter = "^1.3.2"
-pylint = "^2.15.8"
+dbt-tests-adapter = "^1.4, <1.5"
 pytest-parallel = "^0.1.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `dbt_exasol-1.3.0/tests/conftest.py` & `dbt_exasol-1.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.3.0/tests/functional/adapter/expected_catalog.py` & `dbt_exasol-1.4.0/tests/functional/adapter/expected_catalog.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.3.0/tests/functional/adapter/files.py` & `dbt_exasol-1.4.0/tests/functional/adapter/files.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.3.0/tests/functional/adapter/fixtures.py` & `dbt_exasol-1.4.0/tests/functional/adapter/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.3.0/tests/functional/adapter/test_basic.py` & `dbt_exasol-1.4.0/tests/functional/adapter/test_basic.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.3.0/tests/functional/adapter/test_concurrency.py` & `dbt_exasol-1.4.0/tests/functional/adapter/test_concurrency.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.3.0/tests/functional/adapter/test_docs_generate.py` & `dbt_exasol-1.4.0/tests/functional/adapter/test_docs_generate.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.3.0/tests/functional/adapter/test_failing_test.py` & `dbt_exasol-1.4.0/tests/functional/adapter/test_failing_test.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.3.0/tests/functional/adapter/utils/data_types/test_data_types.py` & `dbt_exasol-1.4.0/tests/functional/adapter/utils/data_types/test_data_types.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,20 @@
-import pytest, os
-#from dbt.tests.adapter.utils.data_types.test_type_bigint import BaseTypeBigInt
+import os
+
+import pytest
+from dbt.tests.adapter.utils.data_types.test_type_boolean import \
+    BaseTypeBoolean
 from dbt.tests.adapter.utils.data_types.test_type_float import BaseTypeFloat
 from dbt.tests.adapter.utils.data_types.test_type_int import BaseTypeInt
-from dbt.tests.adapter.utils.data_types.test_type_numeric import BaseTypeNumeric
+from dbt.tests.adapter.utils.data_types.test_type_numeric import \
+    BaseTypeNumeric
 from dbt.tests.adapter.utils.data_types.test_type_string import BaseTypeString
-from dbt.tests.adapter.utils.data_types.test_type_timestamp import BaseTypeTimestamp
+from dbt.tests.adapter.utils.data_types.test_type_timestamp import \
+    BaseTypeTimestamp
 from test_type_bigint import BaseTypeBigInt
-from dbt.tests.adapter.utils.data_types.test_type_boolean import BaseTypeBoolean
-
 
 
 class TestTypeBigIntExasol(BaseTypeBigInt):
     pass
 
     
 class TestTypeFloatExasol(BaseTypeFloat):
```

### Comparing `dbt_exasol-1.3.0/tests/functional/adapter/utils/data_types/test_type_bigint.py` & `dbt_exasol-1.4.0/tests/functional/adapter/utils/data_types/test_type_bigint.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.3.0/tests/functional/adapter/utils/test_utils.py` & `dbt_exasol-1.4.0/tests/functional/adapter/utils/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,43 +1,40 @@
 import os
 
 import pytest
-from utils_fixtures import *
-from dbt.exceptions import CompilationException
+from dbt.exceptions import CompilationError
 from dbt.tests.adapter.utils.base_utils import BaseUtils
-
+from dbt.tests.adapter.utils.test_any_value import BaseAnyValue
 from dbt.tests.adapter.utils.test_array_append import BaseArrayAppend
 from dbt.tests.adapter.utils.test_array_concat import BaseArrayConcat
 from dbt.tests.adapter.utils.test_array_construct import BaseArrayConstruct
-from dbt.tests.adapter.utils.test_any_value import BaseAnyValue
 from dbt.tests.adapter.utils.test_bool_or import BaseBoolOr
 from dbt.tests.adapter.utils.test_cast_bool_to_text import BaseCastBoolToText
 from dbt.tests.adapter.utils.test_concat import BaseConcat
+from dbt.tests.adapter.utils.test_current_timestamp import \
+    BaseCurrentTimestampNaive
 from dbt.tests.adapter.utils.test_date_trunc import BaseDateTrunc
-
-from dbt.tests.adapter.utils.test_current_timestamp import BaseCurrentTimestampNaive
 from dbt.tests.adapter.utils.test_dateadd import BaseDateAdd
 from dbt.tests.adapter.utils.test_datediff import BaseDateDiff
-from dbt.tests.adapter.utils.test_escape_single_quotes import (
-    BaseEscapeSingleQuotesBackslash,
-    BaseEscapeSingleQuotesQuote,
-)
+from dbt.tests.adapter.utils.test_escape_single_quotes import \
+    BaseEscapeSingleQuotesBackslash
 from dbt.tests.adapter.utils.test_except import BaseExcept
 from dbt.tests.adapter.utils.test_hash import BaseHash
 from dbt.tests.adapter.utils.test_intersect import BaseIntersect
 from dbt.tests.adapter.utils.test_last_day import BaseLastDay
 from dbt.tests.adapter.utils.test_length import BaseLength
 from dbt.tests.adapter.utils.test_listagg import BaseListagg
 from dbt.tests.adapter.utils.test_position import BasePosition
 from dbt.tests.adapter.utils.test_replace import BaseReplace
 from dbt.tests.adapter.utils.test_right import BaseRight
 from dbt.tests.adapter.utils.test_safe_cast import BaseSafeCast
 from dbt.tests.adapter.utils.test_split_part import BaseSplitPart
 from dbt.tests.adapter.utils.test_string_literal import BaseStringLiteral
 from dbt.tests.util import run_dbt
+from utils_fixtures import *
 
 
 class TestAnyValueExasol(BaseAnyValue):
     @pytest.fixture(scope="class")
     def models(self):
         return {
             "test_any_value.yml": exasol__models__test_any_value_yml,
@@ -278,15 +275,15 @@
             "test_listagg.yml": exasol__models__test_listagg_yml,
             "test_listagg.sql": self.interpolate_macro_namespace(
                 exasol__models__test_listagg_sql, "listagg"
             ),
         }
 
     def test_build_assert_equal(self, project):
-        with pytest.raises(CompilationException) as exc_info:
+        with pytest.raises(CompilationError) as exc_info:
             run_dbt(["build"], expect_pass=False)
         assert exc_info.value.msg == "`limit_num` parameter is not supported on Exasol!"
 
 
 class TestPositionExasol(BasePosition):
     @pytest.fixture(scope="class")
     def seeds(self):
@@ -361,14 +358,14 @@
             "test_split_part.yml": exasol__models__test_split_part_yml,
             "test_split_part.sql": self.interpolate_macro_namespace(
                 exasol__models__test_split_part_sql, "split_part"
             ),
         }
 
     def test_build_assert_equal(self, project):
-        with pytest.raises(CompilationException) as exc_info:
+        with pytest.raises(CompilationError) as exc_info:
             run_dbt(["build"], expect_pass=False)
         assert exc_info.value.msg == "Unsupported on Exasol! Sorry..."
 
 
 class TestStringLiteralExasol(BaseStringLiteral):
     pass
```

### Comparing `dbt_exasol-1.3.0/tests/functional/adapter/utils/utils_fixtures.py` & `dbt_exasol-1.4.0/tests/functional/adapter/utils/utils_fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.3.0/tests/functional/test_grants.py` & `dbt_exasol-1.4.0/tests/functional/test_grants.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import pytest
-from dbt.tests.adapter.grants.test_incremental_grants import BaseIncrementalGrants
+from dbt.tests.adapter.grants.test_incremental_grants import \
+    BaseIncrementalGrants
 from dbt.tests.adapter.grants.test_invalid_grants import BaseInvalidGrants
 from dbt.tests.adapter.grants.test_model_grants import BaseModelGrants
 from dbt.tests.adapter.grants.test_seed_grants import BaseSeedGrants
 from dbt.tests.adapter.grants.test_snapshot_grants import BaseSnapshotGrants
 
 
 class TestIncrementalGrantsExasol(BaseIncrementalGrants):
```

### Comparing `dbt_exasol-1.3.0/tests/functional/test_incremental.py` & `dbt_exasol-1.4.0/tests/functional/test_incremental.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.3.0/tests/functional/test_issues.py` & `dbt_exasol-1.4.0/tests/functional/test_issues.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.3.0/setup.py` & `dbt_exasol-1.4.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,38 +6,39 @@
  'dbt.adapters',
  'dbt.adapters.exasol',
  'dbt.include',
  'dbt.include.exasol',
  'tests',
  'tests.functional',
  'tests.functional.adapter',
+ 'tests.functional.adapter.query_comment_tests',
+ 'tests.functional.adapter.relations',
  'tests.functional.adapter.utils',
  'tests.functional.adapter.utils.data_types']
 
 package_data = \
 {'': ['*'],
  'dbt.include.exasol': ['macros/*',
                         'macros/materializations/*',
                         'macros/utils/*']}
 
 install_requires = \
-['dbt-core>=1.3,<1.4',
- 'dbt-tests-adapter>=1.3,<1.4',
- 'pyexasol>=0.25.0,<0.26.0']
+['dbt-core>=1.4,<1.5', 'pyexasol>=0.25.0,<0.26.0', 'sqlfluff>=2.0.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'dbt-exasol',
-    'version': '1.3.0',
+    'version': '1.4.0',
     'description': 'Adapter to dbt-core for warehouse Exasol',
     'long_description': "# dbt-exasol\n**[dbt](https://www.getdbt.com/)** enables data analysts and engineers to transform their data using the same practices that software engineers use to build applications.\n\nPlease see the dbt documentation on **[Exasol setup](https://docs.getdbt.com/reference/warehouse-setups/exasol-setup)** for more information on how to start using the Exasol adapter.\n\n# Current profile.yml settings\n<File name='profiles.yml'>\n\n```yaml\ndbt-exasol:\n  target: dev\n  outputs:\n    dev:\n      type: exasol\n      threads: 1\n      dsn: HOST:PORT\n      user: USERNAME\n      password: PASSWORD\n      dbname: db\n      schema: SCHEMA\n```\n\n#### Optional parameters\n<ul>\n  <li><strong>connection_timeout</strong>: defaults to pyexasol default</li>\n  <li><strong>socket_timeout</strong>: defaults to pyexasol default</li>\n  <li><strong>query_timeout</strong>: defaults to pyexasol default</li>\n  <li><strong>compression</strong>: default: False</li>\n  <li><strong>encryption</strong>: default: False</li>\n  <li><strong>protocol_version</strong>: default: v3</li>\n  <li><strong>row_separator</strong>: default: CRLF for windows - LF otherwise</li>\n  <li><strong>timestamp_format</strong>: default: YYYY-MM-DDTHH:MI:SS.FF6</li>\n</ul>\n\n# Known isues\n\n## >=1.3 Python model not yet supported - WIP\n- Please follow [this pull request](https://github.com/tglunde/dbt-exasol/pull/59) \n\n## Breaking changes with release 1.2.2\n- Timestamp format defaults to YYYY-MM-DDTHH:MI:SS.FF6\n\n## SQL functions compatibility\n\n### split_part\nThere is no equivalent SQL function in Exasol for split_part.\n\n### listagg part_num\nThe SQL function listagg in Exasol does not support the num_part parameter.\n\n## Utilities shim package\nIn order to support packages like dbt-utils and dbt-audit-helper, we needed to create the [shim package exasol-utils](https://github.com/tglunde/exasol-utils). In this shim package we need to adapt to parts of the SQL functionality that is not compatible with Exasol - e.g. when 'final' is being used which is a keyword in Exasol. Please visit [Adaopter dispatch documentation](https://docs.getdbt.com/guides/advanced/adapter-development/3-building-a-new-adapter#adapter-dispatch) of dbt-labs for more information. \n# Reporting bugs and contributing code\n- Please report bugs using the issues\n\n# Releases\n\n[GitHub Releases](https://github.com/tglunde/dbt-exasol/releases)\n",
     'author': 'Torsten Glunde',
     'author_email': 'torsten.glunde@alligator-company.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://alligatorcompany.gitlab.io/dbt-exasol',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
+    'python_requires': '>=3.8,<3.12',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `dbt_exasol-1.3.0/PKG-INFO` & `dbt_exasol-1.4.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 Metadata-Version: 2.1
 Name: dbt-exasol
-Version: 1.3.0
+Version: 1.4.0
 Summary: Adapter to dbt-core for warehouse Exasol
 Home-page: https://alligatorcompany.gitlab.io/dbt-exasol
 License: GPL3
 Author: Torsten Glunde
 Author-email: torsten.glunde@alligator-company.com
+Requires-Python: >=3.8,<3.12
 Classifier: License :: Other/Proprietary License
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: dbt-core (>=1.3,<1.4)
-Requires-Dist: dbt-tests-adapter (>=1.3,<1.4)
+Requires-Dist: dbt-core (>=1.4,<1.5)
 Requires-Dist: pyexasol (>=0.25.0,<0.26.0)
+Requires-Dist: sqlfluff (>=2.0.2,<3.0.0)
 Project-URL: Repository, https://github.com/tglunde/dbt-exasol
 Description-Content-Type: text/markdown
 
 # dbt-exasol
 **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to transform their data using the same practices that software engineers use to build applications.
 
 Please see the dbt documentation on **[Exasol setup](https://docs.getdbt.com/reference/warehouse-setups/exasol-setup)** for more information on how to start using the Exasol adapter.
```

