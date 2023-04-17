# Comparing `tmp/aiosqlite-0.8.1.tar.gz` & `tmp/aiosqlite-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aiosqlite-0.8.1.tar", last modified: Fri Dec 28 01:47:51 2018, max compression
+gzip compressed data, was "dist/aiosqlite-0.9.0.tar", last modified: Thu Feb  7 03:27:24 2019, max compression
```

## Comparing `aiosqlite-0.8.1.tar` & `aiosqlite-0.9.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 jreese     (501) staff       (20)        0 2018-12-28 01:47:51.000000 aiosqlite-0.8.1/
--rw-r--r--   0 jreese     (501) staff       (20)     4307 2018-12-28 01:47:51.000000 aiosqlite-0.8.1/PKG-INFO
-drwxr-xr-x   0 jreese     (501) staff       (20)        0 2018-12-28 01:47:51.000000 aiosqlite-0.8.1/aiosqlite.egg-info/
--rw-r--r--   0 jreese     (501) staff       (20)     4307 2018-12-28 01:47:50.000000 aiosqlite-0.8.1/aiosqlite.egg-info/PKG-INFO
--rw-r--r--   0 jreese     (501) staff       (20)      231 2018-12-28 01:47:50.000000 aiosqlite-0.8.1/aiosqlite.egg-info/SOURCES.txt
--rw-r--r--   0 jreese     (501) staff       (20)       10 2018-12-28 01:47:50.000000 aiosqlite-0.8.1/aiosqlite.egg-info/top_level.txt
--rw-r--r--   0 jreese     (501) staff       (20)        1 2018-12-28 01:47:50.000000 aiosqlite-0.8.1/aiosqlite.egg-info/dependency_links.txt
--rw-r--r--   0 jreese     (501) staff       (20)     1067 2017-05-25 03:09:54.000000 aiosqlite-0.8.1/LICENSE
--rw-r--r--   0 jreese     (501) staff       (20)       26 2018-04-05 05:55:10.000000 aiosqlite-0.8.1/MANIFEST.in
-drwxr-xr-x   0 jreese     (501) staff       (20)        0 2018-12-28 01:47:51.000000 aiosqlite-0.8.1/aiosqlite/
--rw-r--r--   0 jreese     (501) staff       (20)      790 2018-12-28 01:42:04.000000 aiosqlite-0.8.1/aiosqlite/__init__.py
--rw-r--r--   0 jreese     (501) staff       (20)     9368 2018-12-28 01:39:11.000000 aiosqlite-0.8.1/aiosqlite/core.py
--rw-r--r--   0 jreese     (501) staff       (20)     1074 2018-09-03 18:54:36.000000 aiosqlite-0.8.1/aiosqlite/context.py
--rw-r--r--   0 jreese     (501) staff       (20)     2879 2018-12-28 01:00:51.000000 aiosqlite-0.8.1/README.md
--rw-r--r--   0 jreese     (501) staff       (20)     1129 2018-11-29 00:21:32.000000 aiosqlite-0.8.1/setup.py
--rw-r--r--   0 jreese     (501) staff       (20)       38 2018-12-28 01:47:51.000000 aiosqlite-0.8.1/setup.cfg
+drwxr-xr-x   0 jreese     (501) staff       (20)        0 2019-02-07 03:27:24.000000 aiosqlite-0.9.0/
+-rw-r--r--   0 jreese     (501) staff       (20)     4307 2019-02-07 03:27:24.000000 aiosqlite-0.9.0/PKG-INFO
+drwxr-xr-x   0 jreese     (501) staff       (20)        0 2019-02-07 03:27:24.000000 aiosqlite-0.9.0/aiosqlite.egg-info/
+-rw-r--r--   0 jreese     (501) staff       (20)     4307 2019-02-07 03:27:24.000000 aiosqlite-0.9.0/aiosqlite.egg-info/PKG-INFO
+-rw-r--r--   0 jreese     (501) staff       (20)      231 2019-02-07 03:27:24.000000 aiosqlite-0.9.0/aiosqlite.egg-info/SOURCES.txt
+-rw-r--r--   0 jreese     (501) staff       (20)       10 2019-02-07 03:27:24.000000 aiosqlite-0.9.0/aiosqlite.egg-info/top_level.txt
+-rw-r--r--   0 jreese     (501) staff       (20)        1 2019-02-07 03:27:24.000000 aiosqlite-0.9.0/aiosqlite.egg-info/dependency_links.txt
+-rw-r--r--   0 jreese     (501) staff       (20)     1067 2017-05-25 03:09:54.000000 aiosqlite-0.9.0/LICENSE
+-rw-r--r--   0 jreese     (501) staff       (20)       26 2018-04-05 05:55:10.000000 aiosqlite-0.9.0/MANIFEST.in
+drwxr-xr-x   0 jreese     (501) staff       (20)        0 2019-02-07 03:27:24.000000 aiosqlite-0.9.0/aiosqlite/
+-rw-r--r--   0 jreese     (501) staff       (20)      790 2019-02-07 02:53:48.000000 aiosqlite-0.9.0/aiosqlite/__init__.py
+-rw-r--r--   0 jreese     (501) staff       (20)     9695 2019-02-07 02:52:49.000000 aiosqlite-0.9.0/aiosqlite/core.py
+-rw-r--r--   0 jreese     (501) staff       (20)     1074 2018-09-03 18:54:36.000000 aiosqlite-0.9.0/aiosqlite/context.py
+-rw-r--r--   0 jreese     (501) staff       (20)     2879 2018-12-28 01:00:51.000000 aiosqlite-0.9.0/README.md
+-rw-r--r--   0 jreese     (501) staff       (20)     1129 2019-01-28 00:37:04.000000 aiosqlite-0.9.0/setup.py
+-rw-r--r--   0 jreese     (501) staff       (20)       38 2019-02-07 03:27:24.000000 aiosqlite-0.9.0/setup.cfg
```

### Comparing `aiosqlite-0.8.1/PKG-INFO` & `aiosqlite-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiosqlite
-Version: 0.8.1
+Version: 0.9.0
 Summary: asyncio bridge to the standard sqlite3 module
 Home-page: https://github.com/jreese/aiosqlite
 Author: John Reese
 Author-email: john@noswap.com
 License: MIT
 Description: aiosqlite
         =========
```

### Comparing `aiosqlite-0.8.1/aiosqlite.egg-info/PKG-INFO` & `aiosqlite-0.9.0/aiosqlite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiosqlite
-Version: 0.8.1
+Version: 0.9.0
 Summary: asyncio bridge to the standard sqlite3 module
 Home-page: https://github.com/jreese/aiosqlite
 Author: John Reese
 Author-email: john@noswap.com
 License: MIT
 Description: aiosqlite
         =========
```

### Comparing `aiosqlite-0.8.1/LICENSE` & `aiosqlite-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiosqlite-0.8.1/aiosqlite/__init__.py` & `aiosqlite-0.9.0/aiosqlite/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     ProgrammingError,
     OperationalError,
     NotSupportedError,
 )
 
 from .core import connect, Connection, Cursor
 
-__version__ = "0.8.1"
+__version__ = "0.9.0"
 __all__ = [
     "__version__",
     "register_adapter",
     "register_converter",
     "sqlite_version",
     "sqlite_version_info",
     "connect",
```

### Comparing `aiosqlite-0.8.1/aiosqlite/core.py` & `aiosqlite-0.9.0/aiosqlite/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -251,33 +251,39 @@
         return self._conn.isolation_level
 
     @isolation_level.setter
     def isolation_level(self, value: str) -> None:
         self._conn.isolation_level = value
 
     @property
-    def row_factory(self) -> Optional[Type]:
+    def row_factory(self) -> "Optional[Type]":  # py3.5.2 compat (#24)
         return self._conn.row_factory
 
     @row_factory.setter
-    def row_factory(self, factory: Optional[Type]) -> None:
+    def row_factory(self, factory: "Optional[Type]") -> None:  # py3.5.2 compat (#24)
         self._conn.row_factory = factory
 
     @property
     def text_factory(self) -> Type:
         return self._conn.text_factory
 
     @text_factory.setter
     def text_factory(self, factory: Type) -> None:
         self._conn.text_factory = factory
 
     @property
     def total_changes(self) -> int:
         return self._conn.total_changes
 
+    async def enable_load_extension(self, value: bool) -> None:
+        await self._execute(self._conn.enable_load_extension, value)  # type: ignore
+
+    async def load_extension(self, path: str):
+        await self._execute(self._conn.load_extension, path)  # type: ignore
+
 
 def connect(
     database: Union[str, Path], *, loop: asyncio.AbstractEventLoop = None, **kwargs: Any
 ) -> Connection:
     """Create and return a connection proxy to the sqlite database."""
     if loop is None:
         loop = asyncio.get_event_loop()
```

### Comparing `aiosqlite-0.8.1/aiosqlite/context.py` & `aiosqlite-0.9.0/aiosqlite/context.py`

 * *Files identical despite different names*

### Comparing `aiosqlite-0.8.1/README.md` & `aiosqlite-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `aiosqlite-0.8.1/setup.py` & `aiosqlite-0.9.0/setup.py`

 * *Files identical despite different names*

