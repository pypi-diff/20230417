# Comparing `tmp/symdexer-0.2.4.tar.gz` & `tmp/symdexer-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symdexer-0.2.4.tar", last modified: Sun Apr 16 23:49:47 2023, max compression
+gzip compressed data, was "C:\Users\AntiMach\Desktop\symdexer\dist\.tmp-i62y9un0\symdexer-0.2.5.tar", last modified: Mon Apr 17 01:28:15 2023, max compression
```

## Comparing `symdexer-0.2.4.tar` & `symdexer-0.2.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 23:49:47.630170 symdexer-0.2.4/
--rw-rw-rw-   0        0        0     1090 2023-04-13 01:46:40.000000 symdexer-0.2.4/LICENSE.txt
--rw-rw-rw-   0        0        0      635 2023-04-16 23:49:47.629170 symdexer-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0      176 2023-04-14 20:55:22.000000 symdexer-0.2.4/README.md
--rw-rw-rw-   0        0        0      595 2023-04-16 23:40:53.000000 symdexer-0.2.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-16 23:49:47.630170 symdexer-0.2.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-16 23:49:47.568641 symdexer-0.2.4/src/
-drwxrwxrwx   0        0        0        0 2023-04-16 23:49:47.601169 symdexer-0.2.4/src/symdexer/
--rw-rw-rw-   0        0        0        0 2023-04-13 01:32:58.000000 symdexer-0.2.4/src/symdexer/__init__.py
--rw-rw-rw-   0        0        0       74 2023-04-13 19:01:25.000000 symdexer-0.2.4/src/symdexer/__main__.py
--rw-rw-rw-   0        0        0     3014 2023-04-16 23:47:52.000000 symdexer-0.2.4/src/symdexer/cache.py
--rw-rw-rw-   0        0        0     4138 2023-04-16 23:43:51.000000 symdexer-0.2.4/src/symdexer/main.py
--rw-rw-rw-   0        0        0      723 2023-04-14 19:54:18.000000 symdexer-0.2.4/src/symdexer/modules.py
--rw-rw-rw-   0        0        0      886 2023-04-14 19:53:25.000000 symdexer-0.2.4/src/symdexer/symbols.py
--rw-rw-rw-   0        0        0      667 2023-04-14 20:33:35.000000 symdexer-0.2.4/src/symdexer/types.py
--rw-rw-rw-   0        0        0       19 2023-04-16 23:40:50.000000 symdexer-0.2.4/src/symdexer/version.py
-drwxrwxrwx   0        0        0        0 2023-04-16 23:49:47.627169 symdexer-0.2.4/src/symdexer.egg-info/
--rw-rw-rw-   0        0        0      635 2023-04-16 23:49:47.000000 symdexer-0.2.4/src/symdexer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      406 2023-04-16 23:49:47.000000 symdexer-0.2.4/src/symdexer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 23:49:47.000000 symdexer-0.2.4/src/symdexer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-04-16 23:49:47.000000 symdexer-0.2.4/src/symdexer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-04-16 23:49:47.000000 symdexer-0.2.4/src/symdexer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 01:28:15.000000 symdexer-0.2.5/
+-rw-rw-rw-   0        0        0     1090 2023-04-13 01:46:40.000000 symdexer-0.2.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      634 2023-04-17 01:28:15.000000 symdexer-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0      176 2023-04-14 20:55:22.000000 symdexer-0.2.5/README.md
+-rw-rw-rw-   0        0        0      588 2023-04-17 01:22:43.000000 symdexer-0.2.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-17 01:28:15.000000 symdexer-0.2.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-17 01:28:15.000000 symdexer-0.2.5/src/
+drwxrwxrwx   0        0        0        0 2023-04-17 01:28:15.000000 symdexer-0.2.5/src/symdexer/
+-rw-rw-rw-   0        0        0        0 2023-04-13 01:32:58.000000 symdexer-0.2.5/src/symdexer/__init__.py
+-rw-rw-rw-   0        0        0       74 2023-04-13 19:01:25.000000 symdexer-0.2.5/src/symdexer/__main__.py
+-rw-rw-rw-   0        0        0     3052 2023-04-17 01:26:42.000000 symdexer-0.2.5/src/symdexer/cache.py
+-rw-rw-rw-   0        0        0     4176 2023-04-17 01:26:35.000000 symdexer-0.2.5/src/symdexer/main.py
+-rw-rw-rw-   0        0        0      791 2023-04-17 01:27:16.000000 symdexer-0.2.5/src/symdexer/modules.py
+-rw-rw-rw-   0        0        0      980 2023-04-17 01:26:21.000000 symdexer-0.2.5/src/symdexer/symbols.py
+-rw-rw-rw-   0        0        0      705 2023-04-17 01:26:25.000000 symdexer-0.2.5/src/symdexer/types.py
+-rw-rw-rw-   0        0        0       19 2023-04-17 01:22:36.000000 symdexer-0.2.5/src/symdexer/version.py
+drwxrwxrwx   0        0        0        0 2023-04-17 01:28:15.000000 symdexer-0.2.5/src/symdexer.egg-info/
+-rw-rw-rw-   0        0        0      634 2023-04-17 01:28:15.000000 symdexer-0.2.5/src/symdexer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      406 2023-04-17 01:28:15.000000 symdexer-0.2.5/src/symdexer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 01:28:15.000000 symdexer-0.2.5/src/symdexer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-04-17 01:28:15.000000 symdexer-0.2.5/src/symdexer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-04-17 01:28:15.000000 symdexer-0.2.5/src/symdexer.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `symdexer-0.2.4/LICENSE.txt` & `symdexer-0.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `symdexer-0.2.4/PKG-INFO` & `symdexer-0.2.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: symdexer
-Version: 0.2.4
+Version: 0.2.5
 Summary: A CLI for finding and indexing symbols
 Author-email: AntiMach <themachinumps@gmail.com>
 Project-URL: Homepage, https://github.com/antimach/symdexer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Symdexer
 
 A command line utility for indexing and finding those pesky symbols in large packages.
```

### Comparing `symdexer-0.2.4/pyproject.toml` & `symdexer-0.2.5/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "symdexer"
-version = "0.2.4"
+version = "0.2.5"
 authors = [
   { name="AntiMach", email="themachinumps@gmail.com" },
 ]
 description = "A CLI for finding and indexing symbols"
 readme = "README.md"
-requires-python = ">=3.11"
+requires-python = ">=3.7"
 classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
+  "Programming Language :: Python :: 3",
+  "License :: OSI Approved :: MIT License",
+  "Operating System :: OS Independent",
 ]
 
 
 [project.scripts]
 symdexer = "symdexer.main:main"
 
 [project.urls]
```

### Comparing `symdexer-0.2.4/src/symdexer/cache.py` & `symdexer-0.2.5/src/symdexer/cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import sqlite3
 from pathlib import Path
 from typing import Generator
 
 from symdexer.symbols import iter_symbols
 from symdexer.modules import walk_modules, Module
```

### Comparing `symdexer-0.2.4/src/symdexer/main.py` & `symdexer-0.2.5/src/symdexer/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from pathlib import Path
 from argparse import ArgumentParser
 
 from symdexer.version import VERSION
 from symdexer.cache import Cache
 from symdexer.symbols import SYM_TYPES
 from symdexer.types import package_type
```

### Comparing `symdexer-0.2.4/src/symdexer/modules.py` & `symdexer-0.2.5/src/symdexer/modules.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,22 @@
+from __future__ import annotations
+
 from pathlib import Path
 from typing import Generator
 from dataclasses import dataclass
-from functools import cached_property
+from functools import lru_cache
 
 
-@dataclass
+@dataclass(frozen=True)
 class Module:
     path: Path
     name: str
 
-    @cached_property
+    @property
+    @lru_cache(maxsize=None)
     def mtime(self):
         return int(self.path.stat().st_mtime)
 
 
 def walk_modules(path: Path, prefix: str = "") -> Generator[Module, None, None]:
     if not prefix:
         prefix = path.stem
```

### Comparing `symdexer-0.2.4/src/symdexer/symbols.py` & `symdexer-0.2.5/src/symdexer/symbols.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import ast
 from pathlib import Path
 
 
 IMPORTS = "imports"
 DEFINES = "defines"
 ASSIGNS = "assigns"
@@ -29,15 +31,17 @@
     ast.ClassDef: _defines,
     ast.Import: _imports,
     ast.ImportFrom: _imports,
 }
 
 
 def iter_symbols(path: Path):
+    # sourcery skip: use-named-expression
     try:
         root = ast.parse(path.read_text("utf-8"))
     except SyntaxError:
         return
 
     for node in ast.iter_child_nodes(root):
-        if func := SYM_MAP.get(type(node)):
+        func = SYM_MAP.get(type(node))
+        if func:
             yield from func(node)
```

### Comparing `symdexer-0.2.4/src/symdexer/types.py` & `symdexer-0.2.5/src/symdexer/types.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import importlib
 from pathlib import Path
 from argparse import ArgumentTypeError
 
 
 def is_package(path: Path) -> bool:
     return path.is_dir() or (path.is_file() and path.suffix == ".py")
```

### Comparing `symdexer-0.2.4/src/symdexer.egg-info/PKG-INFO` & `symdexer-0.2.5/src/symdexer.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: symdexer
-Version: 0.2.4
+Version: 0.2.5
 Summary: A CLI for finding and indexing symbols
 Author-email: AntiMach <themachinumps@gmail.com>
 Project-URL: Homepage, https://github.com/antimach/symdexer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Symdexer
 
 A command line utility for indexing and finding those pesky symbols in large packages.
```

