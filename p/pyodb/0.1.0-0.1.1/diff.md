# Comparing `tmp/pyodb-0.1.0.tar.gz` & `tmp/pyodb-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyodb-0.1.0.tar", last modified: Thu Apr 13 14:20:17 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `pyodb-0.1.0.tar` & `pyodb-0.1.1.tar`

### file list

```diff
@@ -1,35 +1,50 @@
-drwxrwxrwx   0 teuschl   (1000) teuschl   (1000)        0 2023-04-13 14:20:17.813783 pyodb-0.1.0/
--rwxrwxrwx   0 teuschl   (1000) teuschl   (1000)     1072 2023-03-23 09:15:39.000000 pyodb-0.1.0/LICENSE
--rwxrwxrwx   0 teuschl   (1000) teuschl   (1000)       35 2023-04-13 14:14:30.000000 pyodb-0.1.0/MANIFEST.in
--rwxrwxrwx   0 teuschl   (1000) teuschl   (1000)     9595 2023-04-13 14:20:17.807772 pyodb-0.1.0/PKG-INFO
--rwxrwxrwx   0 teuschl   (1000) teuschl   (1000)     8956 2023-04-13 14:14:30.000000 pyodb-0.1.0/README.md
-drwxrwxrwx   0 teuschl   (1000) teuschl   (1000)        0 2023-04-13 14:20:16.371045 pyodb-0.1.0/docs/
--rwxrwxrwx   0 teuschl   (1000) teuschl   (1000)     2882 2023-04-13 14:14:30.000000 pyodb-0.1.0/docs/PyODBCacheExamples.md
--rwxrwxrwx   0 teuschl   (1000) teuschl   (1000)     5905 2023-04-13 14:14:30.000000 pyodb-0.1.0/docs/PyODBExamples.md
-drwxrwxrwx   0 teuschl   (1000) teuschl   (1000)        0 2023-04-13 14:20:16.525504 pyodb-0.1.0/docs/img/
--rwxrwxrwx   0 teuschl   (1000) teuschl   (1000)     7088 2023-04-13 14:14:30.000000 pyodb-0.1.0/docs/img/Logo.svg
--rwxrwxrwx   0 teuschl   (1000) teuschl   (1000)    25699 2023-04-13 14:14:30.000000 pyodb-0.1.0/docs/img/conversion_example.svg
--rwxrwxrwx   0 teuschl   (1000) teuschl   (1000)     1738 2023-04-13 14:14:31.000000 pyodb-0.1.0/pyproject.toml
--rwxrwxrwx   0 teuschl   (1000) teuschl   (1000)       38 2023-04-13 14:20:17.815783 pyodb-0.1.0/setup.cfg
-drwxrwxrwx   0 teuschl   (1000) teuschl   (1000)        0 2023-04-13 14:20:16.072212 pyodb-0.1.0/src/
-drwxrwxrwx   0 teuschl   (1000) teuschl   (1000)        0 2023-04-13 14:20:16.794312 pyodb-0.1.0/src/pyodb/
--rwxrwxrwx   0 teuschl   (1000) teuschl   (1000)       49 2023-03-23 09:15:39.000000 pyodb-0.1.0/src/pyodb/__init__.py
--rwxrwxrwx   0 teuschl   (1000) teuschl   (1000)     1248 2023-03-30 09:20:50.000000 pyodb-0.1.0/src/pyodb/_util.py
--rwxrwxrwx   0 teuschl   (1000) teuschl   (1000)     1182 2023-04-13 09:14:04.000000 pyodb-0.1.0/src/pyodb/error.py
--rwxrwxrwx   0 teuschl   (1000) teuschl   (1000)    15108 2023-04-13 14:14:31.000000 pyodb-0.1.0/src/pyodb/pyodb.py
-drwxrwxrwx   0 teuschl   (1000) teuschl   (1000)        0 2023-04-13 14:20:17.316229 pyodb-0.1.0/src/pyodb/schema/
--rwxrwxrwx   0 teuschl   (1000) teuschl   (1000)        0 2023-03-30 09:20:50.000000 pyodb-0.1.0/src/pyodb/schema/__init__.py
--rwxrwxrwx   0 teuschl   (1000) teuschl   (1000)    14415 2023-04-13 09:14:04.000000 pyodb-0.1.0/src/pyodb/schema/_base_schema.py
-drwxrwxrwx   0 teuschl   (1000) teuschl   (1000)        0 2023-04-13 14:20:17.729256 pyodb-0.1.0/src/pyodb/schema/base/
--rwxrwxrwx   0 teuschl   (1000) teuschl   (1000)        0 2023-03-30 09:20:50.000000 pyodb-0.1.0/src/pyodb/schema/base/__init__.py
--rwxrwxrwx   0 teuschl   (1000) teuschl   (1000)     9280 2023-04-13 09:14:04.000000 pyodb-0.1.0/src/pyodb/schema/base/_operators.py
--rwxrwxrwx   0 teuschl   (1000) teuschl   (1000)    19425 2023-04-13 09:14:04.000000 pyodb-0.1.0/src/pyodb/schema/base/_sql_builders.py
--rwxrwxrwx   0 teuschl   (1000) teuschl   (1000)     5053 2023-04-13 09:14:04.000000 pyodb-0.1.0/src/pyodb/schema/base/_table.py
--rwxrwxrwx   0 teuschl   (1000) teuschl   (1000)      973 2023-03-31 07:30:29.000000 pyodb-0.1.0/src/pyodb/schema/base/_type_defs.py
--rwxrwxrwx   0 teuschl   (1000) teuschl   (1000)     1610 2023-04-13 09:14:04.000000 pyodb-0.1.0/src/pyodb/schema/shard_schema.py
--rwxrwxrwx   0 teuschl   (1000) teuschl   (1000)     1663 2023-04-13 09:14:04.000000 pyodb-0.1.0/src/pyodb/schema/unified_schema.py
-drwxrwxrwx   0 teuschl   (1000) teuschl   (1000)        0 2023-04-13 14:20:17.025956 pyodb-0.1.0/src/pyodb.egg-info/
--rwxrwxrwx   0 teuschl   (1000) teuschl   (1000)     9595 2023-04-13 14:20:15.000000 pyodb-0.1.0/src/pyodb.egg-info/PKG-INFO
--rwxrwxrwx   0 teuschl   (1000) teuschl   (1000)      661 2023-04-13 14:20:15.000000 pyodb-0.1.0/src/pyodb.egg-info/SOURCES.txt
--rwxrwxrwx   0 teuschl   (1000) teuschl   (1000)        1 2023-04-13 14:20:15.000000 pyodb-0.1.0/src/pyodb.egg-info/dependency_links.txt
--rwxrwxrwx   0 teuschl   (1000) teuschl   (1000)        6 2023-04-13 14:20:15.000000 pyodb-0.1.0/src/pyodb.egg-info/top_level.txt
+-rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 pyodb-0.1.1/.coveragerc
+-rwxr-xr-x   0        0        0      701 2020-02-02 00:00:00.000000 pyodb-0.1.1/.pre-commit-config.yaml
+-rwxr-xr-x   0        0        0       35 2020-02-02 00:00:00.000000 pyodb-0.1.1/MANIFEST.in
+-rwxr-xr-x   0        0        0     2774 2020-02-02 00:00:00.000000 pyodb-0.1.1/environment.yaml
+-rwxr-xr-x   0        0        0     7206 2020-02-02 00:00:00.000000 pyodb-0.1.1/performance.ipynb
+-rwxr-xr-x   0        0        0      555 2020-02-02 00:00:00.000000 pyodb-0.1.1/requirements.txt
+-rwxr-xr-x   0        0        0      241 2020-02-02 00:00:00.000000 pyodb-0.1.1/tox.ini
+-rwxr-xr-x   0        0        0     1221 2020-02-02 00:00:00.000000 pyodb-0.1.1/.github/workflows/python-package.yml
+-rwxr-xr-x   0        0        0     2882 2020-02-02 00:00:00.000000 pyodb-0.1.1/docs/PyODBCacheExamples.md
+-rwxr-xr-x   0        0        0     5905 2020-02-02 00:00:00.000000 pyodb-0.1.1/docs/PyODBExamples.md
+-rwxr-xr-x   0        0        0     1927 2020-02-02 00:00:00.000000 pyodb-0.1.1/docs/conversion_example.puml
+-rwxr-xr-x   0        0        0     7088 2020-02-02 00:00:00.000000 pyodb-0.1.1/docs/img/Logo.svg
+-rwxr-xr-x   0        0        0    25699 2020-02-02 00:00:00.000000 pyodb-0.1.1/docs/img/conversion_example.svg
+-rwxr-xr-x   0        0        0     1962 2020-02-02 00:00:00.000000 pyodb-0.1.1/scripts/activate.sh
+-rwxr-xr-x   0        0        0      637 2020-02-02 00:00:00.000000 pyodb-0.1.1/scripts/deactivate.sh
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyodb-0.1.1/src/__init__.py
+-rwxr-xr-x   0        0        0       51 2020-02-02 00:00:00.000000 pyodb-0.1.1/src/pyodb/__init__.py
+-rwxr-xr-x   0        0        0      396 2020-02-02 00:00:00.000000 pyodb-0.1.1/src/pyodb/_util.py
+-rwxr-xr-x   0        0        0      855 2020-02-02 00:00:00.000000 pyodb-0.1.1/src/pyodb/error.py
+-rwxr-xr-x   0        0        0    12732 2020-02-02 00:00:00.000000 pyodb-0.1.1/src/pyodb/pyodb.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyodb-0.1.1/src/pyodb/schema/__init__.py
+-rwxr-xr-x   0        0        0    12188 2020-02-02 00:00:00.000000 pyodb-0.1.1/src/pyodb/schema/_base_schema.py
+-rwxr-xr-x   0        0        0     1634 2020-02-02 00:00:00.000000 pyodb-0.1.1/src/pyodb/schema/shard_schema.py
+-rwxr-xr-x   0        0        0     1398 2020-02-02 00:00:00.000000 pyodb-0.1.1/src/pyodb/schema/unified_schema.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyodb-0.1.1/src/pyodb/schema/base/__init__.py
+-rwxr-xr-x   0        0        0     9414 2020-02-02 00:00:00.000000 pyodb-0.1.1/src/pyodb/schema/base/_operators.py
+-rwxr-xr-x   0        0        0    19128 2020-02-02 00:00:00.000000 pyodb-0.1.1/src/pyodb/schema/base/_sql_builders.py
+-rwxr-xr-x   0        0        0     5006 2020-02-02 00:00:00.000000 pyodb-0.1.1/src/pyodb/schema/base/_table.py
+-rwxr-xr-x   0        0        0      973 2020-02-02 00:00:00.000000 pyodb-0.1.1/src/pyodb/schema/base/_type_defs.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyodb-0.1.1/test/__init__.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyodb-0.1.1/test/pyodb/__init__.py
+-rwxr-xr-x   0        0        0    10884 2020-02-02 00:00:00.000000 pyodb-0.1.1/test/pyodb/pyodb_test.py
+-rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 pyodb-0.1.1/test/pyodb/util_test.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyodb-0.1.1/test/pyodb/schema/__init__.py
+-rwxr-xr-x   0        0        0     6535 2020-02-02 00:00:00.000000 pyodb-0.1.1/test/pyodb/schema/base_schema_test.py
+-rwxr-xr-x   0        0        0     1198 2020-02-02 00:00:00.000000 pyodb-0.1.1/test/pyodb/schema/shard_schema_test.py
+-rwxr-xr-x   0        0        0      669 2020-02-02 00:00:00.000000 pyodb-0.1.1/test/pyodb/schema/unified_schema_test.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyodb-0.1.1/test/pyodb/schema/base/__init__.py
+-rwxr-xr-x   0        0        0     3388 2020-02-02 00:00:00.000000 pyodb-0.1.1/test/pyodb/schema/base/operators_test.py
+-rwxr-xr-x   0        0        0     7777 2020-02-02 00:00:00.000000 pyodb-0.1.1/test/pyodb/schema/base/sql_builders_test.py
+-rwxr-xr-x   0        0        0     1589 2020-02-02 00:00:00.000000 pyodb-0.1.1/test/pyodb/schema/base/table_test.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyodb-0.1.1/test/test_models/__init__.py
+-rwxr-xr-x   0        0        0     2635 2020-02-02 00:00:00.000000 pyodb-0.1.1/test/test_models/complex_models.py
+-rwxr-xr-x   0        0        0     2135 2020-02-02 00:00:00.000000 pyodb-0.1.1/test/test_models/high_complex_models.py
+-rwxr-xr-x   0        0        0     4821 2020-02-02 00:00:00.000000 pyodb-0.1.1/test/test_models/primitive_models.py
+-rwxr-xr-x   0        0        0     1533 2020-02-02 00:00:00.000000 pyodb-0.1.1/.gitignore
+-rwxr-xr-x   0        0        0     1072 2020-02-02 00:00:00.000000 pyodb-0.1.1/LICENSE
+-rwxr-xr-x   0        0        0     8956 2020-02-02 00:00:00.000000 pyodb-0.1.1/README.md
+-rwxr-xr-x   0        0        0     1782 2020-02-02 00:00:00.000000 pyodb-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     9596 2020-02-02 00:00:00.000000 pyodb-0.1.1/PKG-INFO
```

### Comparing `pyodb-0.1.0/LICENSE` & `pyodb-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyodb-0.1.0/PKG-INFO` & `pyodb-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: pyodb
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python Object DataBase (PyODB) is an ORM library aiming to be as simple to use as possible.
-Author-email: Nikolas Teuschl <nikolas.teuschl@alpha-origin.biz>
 Project-URL: Homepage, https://github.com/NeoSecundus/PyODB
 Project-URL: Bug Tracker, https://github.com/NeoSecundus/PyODB/issues
-Keywords: cache,caching,datacache,orm,database,sqlite,sqlite3
-Classifier: Programming Language :: Python :: 3
+Author-email: Nikolas Teuschl <nikolas.teuschl@alpha-origin.biz>
+License-File: LICENSE
+Keywords: cache,caching,database,datacache,orm,sqlite,sqlite3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # PyODB
 
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/NeoSecundus/PyODB/python-package.yml)
 [![codecov](https://codecov.io/gh/NeoSecundus/PyODB/branch/main/graph/badge.svg?token=AEXOJTNDWZ)](https://codecov.io/gh/NeoSecundus/PyODB)
 
 Python Object DataBase (PyODB) is a SQLite3 ORM library aiming to be as simple to use as possible.
```

### Comparing `pyodb-0.1.0/README.md` & `pyodb-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pyodb-0.1.0/docs/PyODBCacheExamples.md` & `pyodb-0.1.1/docs/PyODBCacheExamples.md`

 * *Files identical despite different names*

### Comparing `pyodb-0.1.0/docs/PyODBExamples.md` & `pyodb-0.1.1/docs/PyODBExamples.md`

 * *Files identical despite different names*

### Comparing `pyodb-0.1.0/docs/img/Logo.svg` & `pyodb-0.1.1/docs/img/Logo.svg`

 * *Files identical despite different names*

### Comparing `pyodb-0.1.0/docs/img/conversion_example.svg` & `pyodb-0.1.1/docs/img/conversion_example.svg`

 * *Files identical despite different names*

### Comparing `pyodb-0.1.0/pyproject.toml` & `pyodb-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 [project]
 name = "pyodb"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Nikolas Teuschl", email="nikolas.teuschl@alpha-origin.biz" },
 ]
 description = "Python Object DataBase (PyODB) is an ORM library aiming to be as simple to use as possible."
 readme = "README.md"
-requires-python = ">=3.9"
+requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 keywords = [
     "cache", "caching", "datacache",
     "orm", "database", "sqlite",
     "sqlite3",
 ]
 dependencies = []
 
 [build-system]
-requires = ["setuptools>=40.8.0", "wheel"]
-build-backend = "setuptools.build_meta"
+requires = ["hatchling"]
+build-backend = "hatchling.build"
 
 [project.urls]
 "Homepage" = "https://github.com/NeoSecundus/PyODB"
 "Bug Tracker" = "https://github.com/NeoSecundus/PyODB/issues"
 
 [tool.ruff]
 # Which types of errors to include
@@ -38,15 +38,15 @@
     "PLC", # Pylint Conventions
     "PLE", # Pylint Errors
     "PLR", # Pylint Refactors
     "PLW", # Pylint Warnings
     "RUF", # Ruff specific errors
     ]
 
-ignore = ["N818", "PLR2004", "E701", "RUF005"]
+ignore = ["N818", "PLR2004", "E701", "RUF005", "PLW2901", "I001"]
 line-length = 100
 force-exclude = true
 exclude = [
     ".git",
     ".vscode",
     ".mypy_cache",
     ".ruff_cache",
@@ -72,7 +72,10 @@
 [tool.ruff.pylint]
 max-args = 6
 max-returns = 4
 
 [tool.ruff.pycodestyle]
 ignore-overlong-task-comments = true
 max-doc-length = 100
+
+[tool.pytest.ini_options]
+pythonpath = ["src"]
```

### Comparing `pyodb-0.1.0/src/pyodb/pyodb.py` & `pyodb-0.1.1/src/pyodb/pyodb.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 """Main module handling containing the main capabilities of the library.
 """
-import logging
 from pathlib import Path
 from time import time
 from typing import Any, Callable
 
-from src.pyodb._util import create_logger
-from src.pyodb.error import BadTypeError, CacheError, PyODBError
-from src.pyodb.schema.base._sql_builders import Delete, Select
-from src.pyodb.schema.shard_schema import ShardSchema
-from src.pyodb.schema.unified_schema import UnifiedSchema
+from pyodb.error import BadTypeError, CacheError
+from pyodb.schema.base._sql_builders import Delete, Select
+from pyodb.schema.shard_schema import ShardSchema
+from pyodb.schema.unified_schema import UnifiedSchema
 
 
 class PyODB:
     """
     A persistent object database for Python based on SQLite3.
 
     Values of your classes can be saved by using either attribute annotations:
@@ -47,108 +45,75 @@
         max_depth (int, optional): Maximum recursion depth. Defaults to 0.
         pyodb_folder (str | Path, optional): Folder where the database is stored.
             Defaults to ".pyodb".
         persistent (bool, optional): Whether the database should be persistent after closing.
             Defaults to False.
         sharding (bool, optional): Whether to use sharding.
             Defaults to False.
-        write_log (bool, optional): Whether to enable logging.
-            Defaults to True.
-        log_to_console (bool, optional): Whether to output logs in the console as well.
-            Defaults to False.
         load_existing (bool, optional): Whether to load an existing schema or ignore it.
             Defaults to True.
     """
-    _logger: logging.Logger | None
     _schema: ShardSchema | UnifiedSchema
 
 
-    def __init__( # noqa: PLR0913
+    def __init__(
             self,
             max_depth: int = 2,
             pyodb_folder: str | Path = ".pyodb",
             persistent: bool = False,
             sharding: bool = False,
-            write_log: bool = True,
-            log_to_console: bool = False,
             load_existing: bool = True
         ) -> None:
         if not isinstance(pyodb_folder, Path):
             pyodb_folder = Path(pyodb_folder)
         pyodb_folder.mkdir(mode=755, exist_ok=True)
 
         self._schema = (
             ShardSchema(pyodb_folder, max_depth, persistent)
             if sharding
             else UnifiedSchema(pyodb_folder, max_depth, persistent)
         )
         if load_existing:
             self._schema.load_existing()
 
-        self.modify_logging(
-            do_logging=write_log,
-            log_folder=pyodb_folder,
-            console_output=log_to_console
-        )
-
-
-    def modify_logging(
-        self,
-        do_logging: bool = True,
-        log_level: int = logging.WARN,
-        log_folder: str | Path = ".pyodb",
-        console_output: bool = False
-    ):
-        """Modifies the libraries logging. Log files will have a maximum of 2MiB, with 2 rotating
-        files. So the logs will take up 6MiB at max.
-
-        Args:
-            log_level (int, optional): Defaults to WARN.
-            log_folder (str, optional): Defaults to "./logs". Folder must exist!
-            console_output (bool, optional): Whether to output logs in the console as well or only
-                to the file(s). Defaults to False.
-        """
-        if isinstance(log_folder, str):
-            log_folder = Path(log_folder)
-        log_folder.mkdir(mode=755, exist_ok=True)
-
-        if do_logging:
-            self._logger = create_logger(log_folder.as_posix(), log_level, console_output)
-        else:
-            self._logger = None
-        self._schema.logger = self._logger
-        PyODBError.set_logger(self._logger)
-
 
     @property
     def max_depth(self) -> int:
         """Maximum recursion depth."""
         return self._schema.max_depth
 
 
     @max_depth.setter
     def max_depth(self, val: int):
         self._schema.max_depth = val
 
 
+    @property
+    def persistent(self) -> bool:
+        """Whether the database is persistent after closing.
+        In multiprocessing/threading this should always be set to true!"""
+        return self._schema.is_persistent
+
+
+    @persistent.setter
+    def persistent(self, val: bool):
+        self._schema.is_persistent = val
+
+
     def save(self, obj: object, expires: float | None = None):
         """Saves object to the database. Adds type in case it is not known.
 
         Args:
             obj (object): The object to save.
             expires (float | None, optional): When the object expires and gets removed from the
                 database. Defaults to None.
         """
         obj_type = type(obj)
-        if self._logger:
-            self._logger.debug(f"Saving object of type {obj_type}")
 
         if not self._schema.is_known_type(obj_type):
-            if self._logger:
-                self._logger.info(f"Adding new type '{obj_type}'")
             self._schema.add_type(obj_type)
         self._schema.insert(obj, expires)
 
 
     @property
     def known_types(self) -> list[type]:
         return [type_ for type_ in self._schema._tables.keys() if type_.__name__ != "Table"]
@@ -237,42 +202,26 @@
             bool: True if contained in schema, else False
         """
         if not isinstance(type_, type):
             raise BadTypeError("Argument 'type_' must be a non-union and non-generic type!")
         return self._schema.is_known_type(type_)
 
 
-    @property
-    def persistent(self) -> bool:
-        """Whether the database is persistent after closing.
-        In multiprocessing/threading this should always be set to true!"""
-        return self._schema.is_persistent
-
-
-    @persistent.setter
-    def persistent(self, val: bool):
-        self._schema.is_persistent = val
-
-
 class PyODBCache:
     """Class that caches arbitrary data and returns cached data if available.
     Also updates the data if it is expired. Expiry times are set when adding a new cache.
 
     Args:
         max_depth (int, optional): Maximum recursion depth. Defaults to 0.
         pyodb_folder (str | Path, optional): Folder where the database is stored.
             Defaults to ".pyodb".
         persistent (bool, optional): Whether the database should be persistent after closing.
             Defaults to False.
         sharding (bool, optional): Whether to use sharding.
             Defaults to False.
-        write_log (bool, optional): Whether to enable logging.
-            Defaults to True.
-        log_to_console (bool, optional): Whether to output logs in the console as well.
-            Defaults to False.
     """
     class _CacheItem:
         """Cache-Definition containing the data function, the data type and the lifetime."""
         def __init__(
                 self,
                 data_func: Callable,
                 data_type: type,
@@ -283,69 +232,62 @@
             self.data_type = data_type
             self.lifetime = lifetime
             self.dataclass = dataclass
             self.data = []
             self.expires = 0
 
 
-        def get_data(self):
+        def get_data(self) -> list | None:
             if self.expires < time():
                 self.data = []
                 return None
             return self.data
 
 
         def set_data(self, data: list, expires: float):
             self.data = data
             self.expires = expires
 
 
     _caches: dict[str, _CacheItem]
     _pyodb: PyODB
 
-    @property
-    def logger(self) -> logging.Logger | None:
-        return self._pyodb._logger
-
 
     @property
     def pyodb(self) -> PyODB:
         """The internal pyodb instance"""
         return self._pyodb
 
 
     @property
     def caches(self) -> dict[str, _CacheItem]:
         """The currently known caches"""
         return self._caches.copy()
 
 
-    def __init__( # noqa: PLR0913
+    def __init__(
             self,
             max_depth: int = 0,
             pyodb_folder: str | Path = ".pyodb",
             persistent: bool = False,
             sharding: bool = False,
-            write_log: bool = True,
-            log_to_console: bool = False
         ) -> None:
         self._pyodb = PyODB(
             max_depth=max_depth,
             pyodb_folder=pyodb_folder,
             persistent=persistent,
             sharding=sharding,
-            write_log=write_log,
-            log_to_console=log_to_console,
             load_existing=False
         )
+        self._pyodb._schema.save_table_defs = False
         self._caches = {}
 
 
     def cache_exists(self, cache_key: str) -> bool:
-        """Check the existance of a cache with key `cache_key`
+        """Check the existence of a cache with key `cache_key`
 
         Args:
             cache_key (str): Key of the cache to check for.
 
         Returns:
             bool: True if found, else False
         """
@@ -381,27 +323,29 @@
             CacheError: Is thrown in case the cache already exists and `force` is False.
         """
         if self.cache_exists(cache_key):
             if not force:
                 raise CacheError(
                     f"Cache '{cache_key}' already exists! Use 'force=True' to suppress this error."
                 )
+            elif data_type != self._caches[cache_key].data_type:
+                    self.pyodb.remove_type(self.caches[cache_key].dataclass)
             else:
-                self.pyodb.remove_type(self.caches[cache_key].dataclass)
+                self._caches[cache_key].data_func = data_func
+                self._caches[cache_key].lifetime = lifetime
+                return
 
-        dataclass = type(f"PyODBCache_{data_type.__name__}", (), {
+        dataclass = type(f"PyODBCache_{cache_key}", (), {
                 "__init__": self._dataclass_constructor,
                 "__annotations__": {"data": data_type | None, "expires": float}
             }
         )
         globals().update({dataclass.__name__: dataclass})
         self.pyodb.add_type(dataclass)
         self._caches[cache_key] = self._CacheItem(data_func, data_type, lifetime, dataclass)
-        if self.logger:
-            self.logger.info(f"Added cache definition for '{cache_key}'")
 
 
     def get_data(self, cache_key: str, *args, **kwargs) -> list[Any]:
         """Gets the data from the specified cache.
 
         Accessing data via dictionary style `cache["key"]` is also possible, as long as no arguments
         are needed for the cache's data function.
@@ -435,20 +379,14 @@
             return data
 
         try:
             data = cache.data_func(*args, **kwargs)
             expires = time() + cache.lifetime
             self.pyodb.save_multiple([cache.dataclass(dp, expires) for dp in data], expires)
             cache.set_data(data, expires)
-            if self.logger:
-                self.logger.debug(f"Refreshed cached {cache_key}")
             return data
         except Exception as err:
-            if self.logger:
-                self.logger.error(
-                    f"Failed to get/refresh datacache {cache_key}! Details: {err}"
-                )
             raise err
 
 
     def __getitem__(self, key: str) -> list[Any]:
         return self.get_data(key)
```

### Comparing `pyodb-0.1.0/src/pyodb/schema/_base_schema.py` & `pyodb-0.1.1/src/pyodb/schema/_base_schema.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import pickle
-from logging import Logger
 from pathlib import Path
-from sqlite3 import Connection, OperationalError, Row, connect
-from types import GenericAlias, UnionType
+from types import UnionType
 
-from src.pyodb.error import DBConnError, DisassemblyError, ParentError, UnknownTypeError
-from src.pyodb.schema.base._sql_builders import Delete, Insert, MultiInsert, Select
-from src.pyodb.schema.base._table import Table
-from src.pyodb.schema.base._type_defs import BASE_TYPES
+from pyodb.error import DisassemblyError, ParentError, UnknownTypeError
+from pyodb.schema.base._sql_builders import Delete, Insert, MultiInsert, Select
+from pyodb.schema.base._table import Table
+from pyodb.schema.base._type_defs import BASE_TYPES
 
 
 class BaseSchema:
     """Base class for defining database schemas.
 
     This class defines methods for creating, dropping, and modifying tables to hold objects in a
     database. Objects are added to the schema by their respective types, which shall be defined as
@@ -23,51 +21,23 @@
         max_depth (int): The maximum depth to which nested objects are inserted into the database.
         persistent (bool): If True, the schema instance will be saved to disk upon exit.
     """
     _tables: dict[type, Table]
     _base_path: Path
     _max_depth: int
     is_persistent: bool
-    logger: Logger | None
-
-
-    def _create_dbconn(self, path: Path) -> Connection:
-        """Static method for creating a new database connection with standard performance boosting
-            pragmas.
-
-        Args:
-            path (Path): The path to the database file.
-
-        Returns:
-            Connection: A new connection object.
-        """
-        conn = connect(path.as_posix(), check_same_thread=True, isolation_level="IMMEDIATE")
-        try:
-            conn.execute("pragma journal_mode = WAL;")
-            conn.execute("pragma synchronous = normal;")
-            conn.execute("pragma page_size = 2048;")
-            conn.commit()
-        except OperationalError:
-            # These pragmas are only for performance
-            # They may fail because the database is locked or because they are not supported
-            # it is not critical in any case
-            if self.logger:
-                self.logger.warning(
-                    "Failed to set performance pragmas. You may want to update your sqlite version."
-                )
-
-        conn.row_factory = Row
-        return conn
+    save_table_defs: bool
 
 
     def __init__(self, base_path: Path, max_depth: int, persistent: bool) -> None:
         self._tables = {}
         self._max_depth = max_depth
         self._base_path = base_path
         self.is_persistent = persistent
+        self.save_table_defs = True
 
 
     def is_known_type(self, obj_type: type) -> bool:
         """Check whether the type is already defined in the schema
 
         Args:
             obj_type (type): Type to check for a schema definition
@@ -130,20 +100,14 @@
         table.drop_table()
         for _, type_ in table.members.items():
             if isinstance(type_, UnionType):
                 types = type_.__args__
                 for sub_type in types:
                     if self.is_known_type(sub_type):
                         self._remove_type(table, sub_type)
-            elif isinstance(type_, GenericAlias):
-                for sbt in type_.__args__:
-                    sbt = sbt.__args__ if isinstance(sbt, UnionType) else [sbt] # noqa: PLW2901
-                    for t in sbt:
-                        if self.is_known_type(t):
-                            self._remove_type(table, t)
             elif self.is_known_type(type_):
                 self._remove_type(table, type_)
 
 
     def get_parent(self, base_type: type) -> type | None:
         """
         Returns the parent type for the given base_type, if any.
@@ -165,20 +129,14 @@
                 if type_ in BASE_TYPES:
                     continue
 
                 if isinstance(type_, UnionType):
                     if any(base_type == t for t in type_.__args__):
                         return ttype
                     continue
-                if isinstance(type_, GenericAlias):
-                    for sbt in type_.__args__:
-                        sbt = sbt.__args__ if isinstance(sbt, UnionType) else [sbt] # noqa: PLW2901
-                        if any(base_type == t for t in sbt):
-                            return ttype
-                    continue
                 elif type_ == base_type:
                     return ttype
         return None
 
 
     def insert(
             self, obj: object,
@@ -201,24 +159,22 @@
             UnknownTypeError: In case the wanted type is not within the schema
 
         """
         if not self.is_known_type(type(obj)):
             raise UnknownTypeError(f"Tried to insert object of unknown type {type(obj)}")
 
         table = self._tables[type(obj)]
-        if not table.dbconn:
-            raise DBConnError("Table has no valid connection to a database")
 
         if parent:
             inserter = Insert(table.fqcn, parent.uid, parent.table_name, expires)
         else:
             inserter = Insert(table.fqcn, None, None, expires)
 
         for member in table.members.keys():
-            member = getattr(obj, member) # noqa: PLW2901
+            member = getattr(obj, member)
             if member and type(member) not in BASE_TYPES:
                 if depth >= self._max_depth:
                     inserter.add_val(pickle.dumps(member))
                     continue
                 self.insert(member, expires, inserter, depth+1)
             inserter.add_val(member)
         inserter.commit(table.dbconn)
@@ -238,27 +194,25 @@
             DisassemblyError: In case the objs within the list are not all of the same type.
         """
         base_type = type(objs[0])
         if not self.is_known_type(base_type):
             raise UnknownTypeError(f"Tried to insert object of unknown type {base_type}")
 
         table = self._tables[base_type]
-        if not table.dbconn:
-            raise DBConnError("Table has no valid connection to a database")
         multi_inserter = MultiInsert(table.fqcn)
 
         if any(type(obj) != base_type for obj in objs):
             raise DisassemblyError("Types in inserted list must all be the same!")
 
         subtypes: dict[type, list[tuple[object, Insert]]] = {}
         for obj in objs:
             inserter = Insert(table.fqcn, None, None, expires)
 
             for member in table.members.keys():
-                member = getattr(obj, member) # noqa: PLW2901
+                member = getattr(obj, member)
                 membertype = type(member)
                 if member and membertype not in BASE_TYPES:
                     if self._max_depth == 0:
                         inserter.add_val(pickle.dumps(member))
                         continue
 
                     if membertype not in subtypes:
@@ -286,24 +240,22 @@
 
     Raises:
         DBConnError: If the current table does not have a valid database connection.
     """
         base_type = type(objs[0][0])
 
         table = self._tables[base_type]
-        if not table.dbconn:
-            raise DBConnError("Table has no valid connection to a database")
         multi_inserter = MultiInsert(table.fqcn)
 
         subtypes: dict[type, list[tuple[object, Insert]]] = {}
         for obj in objs:
             inserter = Insert(table.fqcn, obj[1].uid, obj[1].table_name, expires)
 
             for member in table.members.keys():
-                member = getattr(obj[0], member) # noqa: PLW2901
+                member = getattr(obj[0], member)
                 membertype = type(member)
                 if member and membertype not in BASE_TYPES:
                     if depth >= self._max_depth:
                         inserter.add_val(pickle.dumps(member))
                         continue
 
                     if membertype not in subtypes:
@@ -354,15 +306,15 @@
             raise UnknownTypeError(f"Tried to delete instance of unknown type: {type_}")
         return Delete(type_, self._tables)
 
 
     def clear(self):
         """Deletes all objects from the database but keeps the table definitions."""
         for table in self._tables.values():
-            if not table.dbconn or not table.is_parent:
+            if not table.is_parent:
                 continue
             Delete(table.base_type, self._tables).commit()
 
 
     @property
     def max_depth(self) -> int:
         return self._max_depth
```

### Comparing `pyodb-0.1.0/src/pyodb/schema/base/_operators.py` & `pyodb-0.1.1/src/pyodb/schema/base/_operators.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import pickle
 import sqlite3 as sql
 from pydoc import locate
 from time import time
 from types import GenericAlias, NoneType, UnionType
 from typing import Any
 
-from src.pyodb.error import DBConnError, DisassemblyError, MixedTypesError
-from src.pyodb.schema.base._table import Table
-from src.pyodb.schema.base._type_defs import BASE_TYPES, CONTAINERS, PRIMITIVES
+from pyodb.error import DisassemblyError, MixedTypesError
+from pyodb.schema.base._table import Table
+from pyodb.schema.base._type_defs import BASE_TYPES, CONTAINERS, PRIMITIVES
 
 
 class Assembler:
     last_clean = 0
     @classmethod
     def _get_sub_rows(
             cls,
@@ -29,51 +29,41 @@
 
         Returns:
             dict[str, object]: A dictionary containing the retrieved rows.
 
         Raises:
             DBConnError: If the table does not have a valid database connection.
         """
-        if not table.dbconn:
-            raise DBConnError(
-                f"Table '{table.name}' has no valid database connection!"
-            )
         if cls.last_clean < time()-1:
             table.dbconn.execute(f"DELETE FROM \"{table.fqcn}\" WHERE _expires_ < {time()}")
             table.dbconn.commit()
             cls.last_clean = time()
         rows = table.dbconn.execute(
             f"SELECT * FROM \"{table.fqcn}\" WHERE _parent_table_ = ? ORDER BY _parent_ DESC",
             [parent]
         ).fetchall()
         objs = cls.assemble_types(table.base_type, tables, rows)
         return {rows[i]["_parent_"]: objs[i] for i in range(len(rows))}
 
 
     @classmethod
-    def get_base_type(cls, type_: UnionType | GenericAlias) -> type:
+    def get_base_type(cls, type_: UnionType) -> type:
         """
-        Given a UnionType or a GenericAlias, this method returns the most basic type.
+        Given a UnionType, this method returns the most basic type.
 
         Args:
-            type_ (UnionType | GenericAlias): A UnionType or a GenericAlias.
+            type_ (UnionType): A UnionType.
 
         Returns:
             type: The base type of the given type.
         """
-        if isinstance(type_, UnionType):
-            args = type_.__args__
-            subtype = args[0] if not isinstance(args[0], NoneType) else args[1]
+        args = type_.__args__
+        subtype = args[0] if not isinstance(args[0], NoneType) else args[1]
 
-            if isinstance(subtype, GenericAlias):
-                return subtype.__origin__
-
-            return subtype
-        else:
-            return type_.__origin__
+        return subtype
 
 
     @classmethod
     def assemble_types(
             cls,
             base_type: type,
             tables: dict[type, Table],
@@ -97,15 +87,15 @@
             obj = object.__new__(base_type)
             for name, type_ in table.members.items():
                 if row[name] is None:
                     setattr(obj, name, None)
                     continue
 
                 if isinstance(type_, (GenericAlias, UnionType)):
-                    type_ = cls.get_base_type(type_) # noqa: PLW2901
+                    type_ = cls.get_base_type(type_)
 
                 if type_ in PRIMITIVES:
                     setattr(obj, name, type_(row[name]))
 
                 elif type_ in CONTAINERS:
                     setattr(obj, name, pickle.loads(row[name]))
 
@@ -145,72 +135,91 @@
         obj = object.__new__(base_type)
         for name, type_ in table.members.items():
             if row[name] is None:
                 setattr(obj, name, None)
                 continue
 
             if isinstance(type_, (GenericAlias, UnionType)):
-                type_ = cls.get_base_type(type_) # noqa: PLW2901
+                type_ = cls.get_base_type(type_)
 
             if type_ in PRIMITIVES:
                 setattr(obj, name, type_(row[name]))
 
             elif type_ in CONTAINERS:
                 setattr(obj, name, pickle.loads(row[name]))
 
             elif isinstance(type_, type):
                 if str(row[name])[:2] == "b'" or str(row[name])[:2] == "b\"":
                     setattr(obj, name, pickle.loads(row[name]))
                     continue
 
                 ttype: type = locate(row[name]) # type: ignore
                 subtable = tables[ttype]
-                if not subtable.dbconn:
-                    raise DBConnError("Table does not have a valid database connection!")
                 subrow: sql.Row = subtable.dbconn.execute(
                     f"SELECT * FROM \"{subtable.fqcn}\" WHERE _parent_ = '{row['_uid_']}'"
                 ).fetchone()
                 setattr(obj, name, cls.assemble_type(ttype, tables, subrow))
         if "__odb_reassemble__" in base_type.__dict__:
             obj.__odb_reassemble__()
         return obj
 
 
 class Disassembler:
+    sharded = False
+
     @classmethod
-    def _disassemble_union_type(cls, type_: UnionType) -> list[Table]:
+    def _disassemble_union_type(cls, type_: UnionType) -> dict[type, dict]:
         """
         Given a UnionType object, returns a list of Table objects associated with the input type.
 
         Args:
             type_: A UnionType object.
 
         Returns:
             A list of Table objects associated with each type of the Union.
 
         Raises:
             MixedTypesError: If the input type is a UnionType with mixed primitive and custom type
             annotations or multiple primitives.
         """
-        tables = []
+        tables = {}
         if any([t in BASE_TYPES for t in type_.__args__]):
             raise MixedTypesError(
                 f"Cannot save object with mixed primitive and custom type annotations \
 or multiple primitives! Got: {type_}"
             )
         for t in type_.__args__:
-            if t is NoneType or isinstance(t, GenericAlias):
+            if t is NoneType:
                 continue
             else:
-                tables += cls.disassemble_type(t)
+                tables |= cls.disassemble_type(t)
         return tables
 
 
     @classmethod
-    def disassemble_type(cls, obj_type: type) -> list[Table]:
+    def _break_down_type(cls, type_: type | UnionType | GenericAlias) -> type | UnionType:
+        if isinstance(type_, UnionType):
+            subtypes = type_.__args__
+            for i, arg in enumerate(subtypes):
+                if isinstance(arg, GenericAlias):
+                    if len(subtypes) != 2 or subtypes[1-i] is not NoneType:
+                        raise MixedTypesError(
+                            "Cannot save object with multiple primitive or mixed types"
+                        )
+                    type_ = arg.__origin__ | None
+                    break
+
+        if isinstance(type_, GenericAlias):
+            type_ = type_.__origin__
+
+        return type_
+
+
+    @classmethod
+    def disassemble_type(cls, obj_type: type) -> dict[type, dict[str, type | UnionType]]:
         """Disassembles a custom object type into a list of tables that represent the object's
         structure in the database.
 
         Args:
             obj_type (type): A custom object type to be disassembled.
 
         Returns:
@@ -219,37 +228,38 @@
                 attributes represent the columns in that table.
 
         Raises:
             DisassemblyError: If obj_type is Any, NoneType, a primitive type or the passed argument
                 is not a type at all.
         """
         if obj_type is Any or obj_type is NoneType or obj_type in BASE_TYPES:
-            raise DisassemblyError("'Any', 'None' and 'Primitive' types are not supported!")
+            raise DisassemblyError("'Any', 'None' and Primitive types are not supported!")
 
         if not isinstance(obj_type, type):
             raise DisassemblyError("Passed argument must be a type!")
 
-        tables = [Table(obj_type)]
+        tables = {obj_type: {}}
 
         if "__odb_members__" in obj_type.__annotations__:
             members = getattr(obj_type, "__odb_members__")
         else:
             members: dict[str, type | UnionType | GenericAlias] = {
                 key: type_
                 for key, type_
                 in obj_type.__annotations__.items()
                 if key[:2] != "__"
             }
 
         for key, type_ in members.items():
-            tables[0].add_member(key, type_)
-            if isinstance(type_, GenericAlias) or type_ is type:
-                continue
+            type_ = cls._break_down_type(type_)
 
+            tables[obj_type][key] = type_
+            if type_ is type:
+                continue
 
             if type_ not in BASE_TYPES:
                 if isinstance(type_, UnionType):
-                    tables += cls._disassemble_union_type(type_)
+                    tables |= cls._disassemble_union_type(type_)
                 else:
-                    tables += cls.disassemble_type(type_)
+                    tables |= cls.disassemble_type(type_)
 
         return tables
```

### Comparing `pyodb-0.1.0/src/pyodb/schema/base/_sql_builders.py` & `pyodb-0.1.1/src/pyodb/schema/base/_sql_builders.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import pickle
 import sqlite3.dbapi2 as sql
 from pydoc import locate
 from time import time
 from types import GenericAlias, NoneType, UnionType
 from typing import Any
 
-from src.pyodb._util import generate_uid
-from src.pyodb.error import BadTypeError, DBConnError, ExpiryError, ParentError, QueryError
-from src.pyodb.schema.base._operators import Assembler
-from src.pyodb.schema.base._table import Table
-from src.pyodb.schema.base._type_defs import BASE_TYPES, CONTAINERS, PRIMITIVES
+from pyodb._util import generate_uid
+from pyodb.error import BadTypeError, ExpiryError, ParentError, QueryError
+from pyodb.schema.base._operators import Assembler
+from pyodb.schema.base._table import Table
+from pyodb.schema.base._type_defs import BASE_TYPES, CONTAINERS, PRIMITIVES
 
 
 class Insert:
     """A class for constructing and committing SQL INSERT statements to a database.
 
     Args:
         table_name (str): The name of the table to insert data into.
@@ -435,25 +435,22 @@
 
             Parameters:
                 count (bool): Whether to count the deleted children or not. Defaults to False.
 
             Returns:
                 int: The number of records deleted.
         """
-        if not self._table.dbconn:
-            raise DBConnError(f"Table {self._table.name} has no valid connection to database!")
-
         res: list[sql.Row] = self._compile("SELECT * FROM", self._table.dbconn, False).fetchall()
         rlen = len(res)
         self._compile("DELETE FROM", self._table.dbconn)
         self._table.dbconn.commit()
 
         for key, type_ in self._table.members.items():
             if isinstance(type_, GenericAlias | UnionType):
-                type_ = Assembler.get_base_type(type_) # noqa: PLW2901
+                type_ = Assembler.get_base_type(type_)
 
             if type_ in BASE_TYPES:
                 continue
 
             for item in res:
                 if str(item[key])[:2] == "b'" or str(item[key])[:2] == "b\"":
                     continue
@@ -560,13 +557,11 @@
 
         Returns:
             sql.Cursor: A cursor object representing the results of the query.
 
         Raises:
             DBConnError: If the table does not have a valid database connection.
         """
-        if not self._table.dbconn:
-            raise DBConnError("Table does not have a valid database connection")
         self._table.dbconn.execute(f"DELETE FROM \"{self._table.fqcn}\" WHERE _expires_ < {time()}")
         self._table.dbconn.commit()
 
         return super()._compile(f"SELECT {get_what} FROM", self._table.dbconn)
```

### Comparing `pyodb-0.1.0/src/pyodb/schema/base/_table.py` & `pyodb-0.1.1/src/pyodb/schema/base/_table.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 """The main module which processes python primitives (and lists and dicts) and generates sql
 statements.
 Including create and remove table statements in case the fields contained by a class were changed.
 """
 import sqlite3 as sql
-from types import GenericAlias, NoneType, UnionType
+from pathlib import Path
+from threading import get_ident as get_thread_id
+from types import UnionType
 
-from src.pyodb.error import DBConnError
-from src.pyodb.schema.base._type_defs import BASE_TYPE_SQL_MAP, BASE_TYPES
+from pyodb.schema.base._type_defs import BASE_TYPE_SQL_MAP, BASE_TYPES
 
 
 class Table:
     """A class representing a table in a database, used to store objects of a specific type.
 
     Args:
         base_type (type): The type of objects that the table will store.
-        is_parent (bool, optional): A flag indicating whether the table is a parent table.
-            Defaults to False.
+        sharded (bool): A flag indicating whether the table has it's own db file or not.
     """
-    _members: dict[str, type | UnionType | GenericAlias]
     base_type: type
     is_parent: bool
+    _sharded: bool
 
 
-    def __init__(self, base_type: type, is_parent: bool = False) -> None:
+    def __init__(
+            self,
+            base_type: type,
+            base_path: Path,
+            members: dict[str, type | UnionType],
+            sharded: bool
+        ) -> None:
         self._members = {}
         self.base_type = base_type
-        self.is_parent = is_parent
-        self.dbconn: sql.Connection | None = None
-
-
-    def add_member(self, name: str, type_: type | UnionType | GenericAlias):
-        """Adds a new member to the internal members
-
-        Args:
-            name (str): Name of the member (field name)
-            type_ (type): Member's datatype
-        """
-        self._members[name] = type_
+        self.is_parent = False
+        self._sharded = sharded
+        self.base_path = base_path
+        self._members = members
+        self._dbconn = self._create_dbconn()
+        self._cur_thread = get_thread_id()
 
 
     @property
-    def members(self) -> dict[str, type | UnionType | GenericAlias]:
+    def members(self) -> dict[str, type | UnionType]:
         """A dictionary containing the members (fields) of the table with their
         corresponding data types."""
 
         return self._members.copy()
 
 
     @property
@@ -55,101 +55,107 @@
 
     @property
     def fqcn(self) -> str:
         """Fully qualified class name"""
         return f"{self.base_type.__module__}.{self.base_type.__name__}"
 
 
+    @property
+    def dbconn(self) -> sql.Connection:
+        """SQLite3 Database Connection"""
+        tid = get_thread_id()
+        if self._cur_thread != tid:
+            self._dbconn = self._create_dbconn()
+            self._cur_thread = tid
+
+        return self._dbconn
+
+
     def create_table(self):
         """
         Creates a new table in the database.
 
         Raises:
             DBConnError: If the table does not have a valid connection to any database.
         """
-        if not self.dbconn:
-            raise DBConnError(f"Table '{self.name}' has no valid connection to any Database!")
         self.dbconn.execute(self._create_table_sql())
         self.dbconn.commit()
 
 
     def drop_table(self):
         """
         Deletes the table from the database.
 
         Raises:
             DBConnError: If the table does not have a valid connection to any database.
         """
-        if not self.dbconn:
-            raise DBConnError(f"Table '{self.name}' has no valid connection to any Database!")
         self.dbconn.execute(self._drop_table_sql())
         self.dbconn.commit()
 
 
     def delete_parent_entries(self, parent):
         """
         Deletes all rows in the table that have a parent of the specified parent table.
 
         Args:
             parent (Table): The parent table whose rows should be deleted.
 
         Raises:
             DBConnError: If the table does not have a valid connection to a database.
         """
-        if not self.dbconn:
-            raise DBConnError(f"Table '{self.name}' has no valid connection to any Database!")
         self.dbconn.execute(f"DELETE FROM \"{self.fqcn}\" WHERE _parent_table_ = '{parent.name}'")
         self.dbconn.commit()
 
 
     def _create_table_sql(self) -> str:
         """Returns the SQL statement needed to create the table."""
         sql = f"CREATE TABLE IF NOT EXISTS \"{self.fqcn}\" (_uid_ TEXT PRIMARY KEY,_parent_ TEXT,\
 _parent_table_ TEXT,_expires_ REAL,"
         for name, type_ in self.members.items():
-            if isinstance(type_, (GenericAlias, UnionType)):
-                type_ = self._get_base_type(type_) # noqa: PLW2901
-
             if type_ in BASE_TYPES:
                 sql += f"{name} {BASE_TYPE_SQL_MAP[type_]},"
             else:
                 sql += f"{name} TEXT,"
 
         return sql[:-1] + ");"
 
 
-    @classmethod
-    def _get_base_type(cls, type_: GenericAlias | UnionType) -> type | UnionType:
-        """
-        Returns the base type for the specified type. (Includes None)
+    def _drop_table_sql(self) -> str:
+        """Returns the drop table sql for this table."""
+        return f"DROP TABLE IF EXISTS \"{self.fqcn}\";"
+
+
+    def _create_dbconn(self) -> sql.Connection:
+        """Static method for creating a new database connection with standard performance boosting
+            pragmas.
 
         Args:
-            type_ (GenericAlias | UnionType): The type for which to get the base type.
+            path (Path): The path to the database file.
 
         Returns:
-            type | UnionType: The base type for the specified type.
+            Connection: A new connection object.
         """
-        if isinstance(type_, UnionType):
-            if type_ in BASE_TYPES:
-                return type_
+        conn = sql.connect(
+            self.base_path / (self.base_type.__name__ + ".db")
+                if self._sharded
+                else self.base_path / "pyodb.db",
+            check_same_thread=True,
+            isolation_level="IMMEDIATE"
+        )
+        try:
+            conn.execute("pragma journal_mode = WAL;")
+            conn.execute("pragma synchronous = normal;")
+            conn.execute("pragma page_size = 2048;")
+            conn.commit()
+        except sql.OperationalError:
+            # These pragmas are only for performance
+            # They may fail because the database is locked or because they are not supported
+            # it is not critical in any case
+            print("PyODB WARNING: Could not set database performance pragmas.")
 
-            ret = type_
-            for t in type_.__args__:
-                if isinstance(t, GenericAlias):
-                    ret = cls._get_base_type(t)
-                    continue
-
-                if isinstance(ret, type) and t is NoneType:
-                    ret = ret | None
-            return ret
-        else:
-            return type_.__origin__
-
-
-    def _drop_table_sql(self) -> str:
-        """Returns the drop table sql for this table."""
-        return f"DROP TABLE IF EXISTS \"{self.fqcn}\";"
+        conn.row_factory = sql.Row
+        return conn
 
 
     def __repr__(self) -> str:
         return f"{self.base_type.__name__}: \
 { {k: str(t) if isinstance(t, UnionType) else t.__name__ for k, t in self._members.items()} };"
```

### Comparing `pyodb-0.1.0/src/pyodb/schema/base/_type_defs.py` & `pyodb-0.1.1/src/pyodb/schema/base/_type_defs.py`

 * *Files identical despite different names*

### Comparing `pyodb-0.1.0/src/pyodb/schema/shard_schema.py` & `pyodb-0.1.1/src/pyodb/schema/unified_schema.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,42 @@
-from src.pyodb.schema._base_schema import BaseSchema
-from src.pyodb.schema.base._operators import Disassembler
-from src.pyodb.schema.base._table import Table
+from pyodb.schema._base_schema import BaseSchema
+from pyodb.schema.base._operators import Disassembler
+from pyodb.schema.base._table import Table
 
 
-class ShardSchema(BaseSchema):
+class UnifiedSchema(BaseSchema):
     def add_type(self, base_type: type):
-        tables = Disassembler.disassemble_type(base_type)
-        for table in tables:
-            if self.is_known_type(table.base_type):
+        ttypes = Disassembler.disassemble_type(base_type)
+        for ttype, members in ttypes.items():
+            if self.is_known_type(ttype):
                 continue
-            table.dbconn = self._create_dbconn(self._base_path / f"{table.name}.db")
-            self._tables[table.base_type] = table
-            table.create_table()
+            self._tables[ttype] = Table(ttype, self._base_path, members, False)
+            self._tables[ttype].create_table()
         self._tables[base_type].is_parent = True
 
 
     def load_existing(self):
         self.add_type(Table)
         old_tables: list[Table] = self.select(Table).all()
         for old_table in old_tables:
             self.add_type(old_table.base_type)
-            self._tables[old_table.base_type].dbconn = self._create_dbconn(
-                self._base_path / f"{old_table.name}.db"
-            )
             self._tables[old_table.base_type].is_parent = old_table.is_parent
 
 
     def _save_schema(self):
         self.add_type(Table)
+        self._dbconn = None
         self.delete(Table).commit()
         self.max_depth = 0
         self.insert_many(list(self._tables.values()), None)
 
 
     def __del__(self):
         if self.is_persistent:
-            self._save_schema()
+            if self.save_table_defs:
+                self._save_schema()
             return
 
-        for table in self._tables.values():
-            del table.dbconn
-            (self._base_path / (table.name + ".db")).unlink(True)
-            (self._base_path / (table.name + ".db-shm")).unlink(True)
-            (self._base_path / (table.name + ".db-wal")).unlink(True)
+        del self._tables
+        (self._base_path / "pyodb.db").unlink(True)
+        (self._base_path / "pyodb.db-shm").unlink(True)
+        (self._base_path / "pyodb.db-wal").unlink(True)
```

### Comparing `pyodb-0.1.0/src/pyodb/schema/unified_schema.py` & `pyodb-0.1.1/src/pyodb/schema/shard_schema.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,50 +1,48 @@
 from pathlib import Path
 
-from src.pyodb.schema._base_schema import BaseSchema
-from src.pyodb.schema.base._operators import Disassembler
-from src.pyodb.schema.base._table import Table
+from pyodb.schema._base_schema import BaseSchema
+from pyodb.schema.base._operators import Disassembler
+from pyodb.schema.base._table import Table
 
 
-class UnifiedSchema(BaseSchema):
+class ShardSchema(BaseSchema):
     def __init__(self, base_path: Path, max_depth: int, persistent: bool) -> None:
-        self._dbconn = self._create_dbconn(base_path / "pyodb.db")
+        Disassembler.sharded = True
         super().__init__(base_path, max_depth, persistent)
 
 
     def add_type(self, base_type: type):
-        tables = Disassembler.disassemble_type(base_type)
-        for table in tables:
-            if self.is_known_type(table.base_type):
+        ttypes = Disassembler.disassemble_type(base_type)
+        for ttype, members in ttypes.items():
+            if self.is_known_type(ttype):
                 continue
-            self._tables[table.base_type] = table
-            table.dbconn = self._dbconn
-            table.create_table()
+            self._tables[ttype] = Table(ttype, self._base_path, members, True)
+            self._tables[ttype].create_table()
         self._tables[base_type].is_parent = True
 
 
     def load_existing(self):
         self.add_type(Table)
         old_tables: list[Table] = self.select(Table).all()
         for old_table in old_tables:
             self.add_type(old_table.base_type)
-            self._tables[old_table.base_type].dbconn = self._dbconn
             self._tables[old_table.base_type].is_parent = old_table.is_parent
 
 
     def _save_schema(self):
         self.add_type(Table)
-        self._dbconn = None
         self.delete(Table).commit()
         self.max_depth = 0
         self.insert_many(list(self._tables.values()), None)
 
 
     def __del__(self):
         if self.is_persistent:
-            self._save_schema()
+            if self.save_table_defs:
+                self._save_schema()
             return
 
-        del self._tables
-        (self._base_path / "pyodb.db").unlink(True)
-        (self._base_path / "pyodb.db-shm").unlink(True)
-        (self._base_path / "pyodb.db-wal").unlink(True)
+        for table in self._tables.values():
+            (self._base_path / (table.name + ".db")).unlink(True)
+            (self._base_path / (table.name + ".db-shm")).unlink(True)
+            (self._base_path / (table.name + ".db-wal")).unlink(True)
```

