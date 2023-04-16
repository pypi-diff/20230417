# Comparing `tmp/symdexer-0.2.3.tar.gz` & `tmp/symdexer-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symdexer-0.2.3.tar", last modified: Sat Apr 15 00:04:42 2023, max compression
+gzip compressed data, was "symdexer-0.2.4.tar", last modified: Sun Apr 16 23:49:47 2023, max compression
```

## Comparing `symdexer-0.2.3.tar` & `symdexer-0.2.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 00:04:42.544843 symdexer-0.2.3/
--rw-rw-rw-   0        0        0     1090 2023-04-13 01:46:40.000000 symdexer-0.2.3/LICENSE.txt
--rw-rw-rw-   0        0        0      635 2023-04-15 00:04:42.543830 symdexer-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0      176 2023-04-14 20:55:22.000000 symdexer-0.2.3/README.md
--rw-rw-rw-   0        0        0      595 2023-04-15 00:04:15.000000 symdexer-0.2.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-15 00:04:42.544843 symdexer-0.2.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-15 00:04:42.497233 symdexer-0.2.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-15 00:04:42.517239 symdexer-0.2.3/src/symdexer/
--rw-rw-rw-   0        0        0        0 2023-04-13 01:32:58.000000 symdexer-0.2.3/src/symdexer/__init__.py
--rw-rw-rw-   0        0        0       74 2023-04-13 19:01:25.000000 symdexer-0.2.3/src/symdexer/__main__.py
--rw-rw-rw-   0        0        0     2926 2023-04-14 23:57:47.000000 symdexer-0.2.3/src/symdexer/cache.py
--rw-rw-rw-   0        0        0     4161 2023-04-14 23:54:59.000000 symdexer-0.2.3/src/symdexer/main.py
--rw-rw-rw-   0        0        0      723 2023-04-14 19:54:18.000000 symdexer-0.2.3/src/symdexer/modules.py
--rw-rw-rw-   0        0        0      886 2023-04-14 19:53:25.000000 symdexer-0.2.3/src/symdexer/symbols.py
--rw-rw-rw-   0        0        0      667 2023-04-14 20:33:35.000000 symdexer-0.2.3/src/symdexer/types.py
--rw-rw-rw-   0        0        0       19 2023-04-15 00:04:17.000000 symdexer-0.2.3/src/symdexer/version.py
-drwxrwxrwx   0        0        0        0 2023-04-15 00:04:42.541840 symdexer-0.2.3/src/symdexer.egg-info/
--rw-rw-rw-   0        0        0      635 2023-04-15 00:04:42.000000 symdexer-0.2.3/src/symdexer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      406 2023-04-15 00:04:42.000000 symdexer-0.2.3/src/symdexer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 00:04:42.000000 symdexer-0.2.3/src/symdexer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-04-15 00:04:42.000000 symdexer-0.2.3/src/symdexer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-04-15 00:04:42.000000 symdexer-0.2.3/src/symdexer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 23:49:47.630170 symdexer-0.2.4/
+-rw-rw-rw-   0        0        0     1090 2023-04-13 01:46:40.000000 symdexer-0.2.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      635 2023-04-16 23:49:47.629170 symdexer-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0      176 2023-04-14 20:55:22.000000 symdexer-0.2.4/README.md
+-rw-rw-rw-   0        0        0      595 2023-04-16 23:40:53.000000 symdexer-0.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-16 23:49:47.630170 symdexer-0.2.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-16 23:49:47.568641 symdexer-0.2.4/src/
+drwxrwxrwx   0        0        0        0 2023-04-16 23:49:47.601169 symdexer-0.2.4/src/symdexer/
+-rw-rw-rw-   0        0        0        0 2023-04-13 01:32:58.000000 symdexer-0.2.4/src/symdexer/__init__.py
+-rw-rw-rw-   0        0        0       74 2023-04-13 19:01:25.000000 symdexer-0.2.4/src/symdexer/__main__.py
+-rw-rw-rw-   0        0        0     3014 2023-04-16 23:47:52.000000 symdexer-0.2.4/src/symdexer/cache.py
+-rw-rw-rw-   0        0        0     4138 2023-04-16 23:43:51.000000 symdexer-0.2.4/src/symdexer/main.py
+-rw-rw-rw-   0        0        0      723 2023-04-14 19:54:18.000000 symdexer-0.2.4/src/symdexer/modules.py
+-rw-rw-rw-   0        0        0      886 2023-04-14 19:53:25.000000 symdexer-0.2.4/src/symdexer/symbols.py
+-rw-rw-rw-   0        0        0      667 2023-04-14 20:33:35.000000 symdexer-0.2.4/src/symdexer/types.py
+-rw-rw-rw-   0        0        0       19 2023-04-16 23:40:50.000000 symdexer-0.2.4/src/symdexer/version.py
+drwxrwxrwx   0        0        0        0 2023-04-16 23:49:47.627169 symdexer-0.2.4/src/symdexer.egg-info/
+-rw-rw-rw-   0        0        0      635 2023-04-16 23:49:47.000000 symdexer-0.2.4/src/symdexer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      406 2023-04-16 23:49:47.000000 symdexer-0.2.4/src/symdexer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 23:49:47.000000 symdexer-0.2.4/src/symdexer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-04-16 23:49:47.000000 symdexer-0.2.4/src/symdexer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-04-16 23:49:47.000000 symdexer-0.2.4/src/symdexer.egg-info/top_level.txt
```

### Comparing `symdexer-0.2.3/LICENSE.txt` & `symdexer-0.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `symdexer-0.2.3/PKG-INFO` & `symdexer-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symdexer
-Version: 0.2.3
+Version: 0.2.4
 Summary: A CLI for finding and indexing symbols
 Author-email: AntiMach <themachinumps@gmail.com>
 Project-URL: Homepage, https://github.com/antimach/symdexer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `symdexer-0.2.3/pyproject.toml` & `symdexer-0.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "symdexer"
-version = "0.2.3"
+version = "0.2.4"
 authors = [
   { name="AntiMach", email="themachinumps@gmail.com" },
 ]
 description = "A CLI for finding and indexing symbols"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `symdexer-0.2.3/src/symdexer/cache.py` & `symdexer-0.2.4/src/symdexer/cache.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,31 +43,34 @@
         for path in packages:
             for module in walk_modules(path):
                 self._cache_module(module)
 
         self.db.commit()
 
     def _cache_module(self, module: Module):
-        # checks if the module already exists and is outdated
+        moduleInfo = module.name, str(module.path.resolve()), module.mtime
+
+        # guard clause that returns when the module being indexed
+        # hasn't changed location or mtime since last index
         if self.db.execute(
             """
-            SELECT name, changed
+            SELECT name
             FROM Module
-            WHERE name = ? AND changed < ?
+            WHERE name = ? AND (path != ? OR changed != ?)
             """,
-            (module.name, module.mtime),
+            moduleInfo,
         ).fetchall():
             return
 
         self.db.execute(
             """
             INSERT OR IGNORE INTO Module (name, path, changed)
             VALUES (?, ? ,?)
             """,
-            (module.name, str(module.path.resolve()), module.mtime),
+            moduleInfo,
         )
 
         for symbol, sym_type in iter_symbols(module.path):
             self.db.execute(
                 """
                 INSERT OR IGNORE INTO Symbol (name, type, module)
                 VALUES (?, ? ,?)
```

### Comparing `symdexer-0.2.3/src/symdexer/main.py` & `symdexer-0.2.4/src/symdexer/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,31 +11,30 @@
     if not cache_p.is_file():
         raise FileNotFoundError(f"Cache `{cache_p}` not found.")
 
     with Cache(cache_p) as cache:
         yield from cache.search(symbols, fuzzy, types)
 
 
-def find_command(cache_p: Path, symbols: list[str], fuzzy: bool, types: list[str]) -> None:
-    for names, module, _ in search_cache(cache_p, symbols, fuzzy, types):
+def find_command(cache: Path, symbols: list[str], fuzzy: bool, types: list[str]) -> None:
+    for names, module, _ in search_cache(cache, symbols, fuzzy, types):
         yield f"from {module} import {names}"
 
 
-def locate_command(cache_p: Path, symbols: list[str], fuzzy: bool, types: list[str]) -> None:
-    for name, module, path in search_cache(cache_p, symbols, fuzzy, types):
+def locate_command(cache: Path, symbols: list[str], fuzzy: bool, types: list[str]) -> None:
+    for name, module, path in search_cache(cache, symbols, fuzzy, types):
         yield name
         yield module
         yield path
 
 
-def index_command(cache_p: Path, packages: list[Path], reset: bool):
-    if not cache_p.exists():
-        reset = True
+def index_command(cache: Path, packages: list[Path], reset: bool):
+    reset = reset or not cache.exists()
 
-    with Cache(cache_p) as cache:
+    with Cache(cache) as cache:
         if reset:
             cache.reset()
         cache.update(packages)
 
     yield "Done indexing"
 
 
@@ -110,27 +109,27 @@
         metavar="SYM_TYPE",
         choices=SYM_TYPES,
         default=SYM_TYPES,
         nargs="+",
         help="Symbol types to show",
     )
 
-    cache_parser = sub_parsers.add_parser(
+    index_parser = sub_parsers.add_parser(
         "index",
         help="Load symbols into cache",
     )
-    cache_parser.add_argument(
+    index_parser.add_argument(
         "-r",
         "--reset",
         dest="reset",
         action="store_true",
         default=False,
         help="If the cache should be completely wiped",
     )
-    cache_parser.add_argument(
+    index_parser.add_argument(
         "packages",
         metavar="PACKAGE",
         nargs="+",
         type=package_type,
         help="The packages to add to cache. May be package names or paths",
     )
```

### Comparing `symdexer-0.2.3/src/symdexer/modules.py` & `symdexer-0.2.4/src/symdexer/modules.py`

 * *Files identical despite different names*

### Comparing `symdexer-0.2.3/src/symdexer/symbols.py` & `symdexer-0.2.4/src/symdexer/symbols.py`

 * *Files identical despite different names*

### Comparing `symdexer-0.2.3/src/symdexer/types.py` & `symdexer-0.2.4/src/symdexer/types.py`

 * *Files identical despite different names*

### Comparing `symdexer-0.2.3/src/symdexer.egg-info/PKG-INFO` & `symdexer-0.2.4/src/symdexer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symdexer
-Version: 0.2.3
+Version: 0.2.4
 Summary: A CLI for finding and indexing symbols
 Author-email: AntiMach <themachinumps@gmail.com>
 Project-URL: Homepage, https://github.com/antimach/symdexer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

