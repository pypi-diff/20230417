# Comparing `tmp/pyastgrep-0.9.tar.gz` & `tmp/pyastgrep-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyastgrep-0.9.tar", last modified: Wed Nov 16 20:47:52 2022, max compression
+gzip compressed data, was "pyastgrep-1.0.tar", last modified: Mon Apr 17 15:42:17 2023, max compression
```

## Comparing `pyastgrep-0.9.tar` & `pyastgrep-1.0.tar`

### file list

```diff
@@ -1,27 +1,36 @@
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2022-11-16 20:47:52.826556 pyastgrep-0.9/
--rw-r--r--   0 luke      (1000) luke      (1000)      378 2022-10-17 13:09:58.000000 pyastgrep-0.9/.gitattributes
--rw-r--r--   0 luke      (1000) luke      (1000)     1771 2022-11-07 12:01:43.000000 pyastgrep-0.9/.gitignore
--rw-rw-rw-   0 luke      (1000) luke      (1000)    13751 2022-11-16 20:47:52.826556 pyastgrep-0.9/PKG-INFO
--rw-r--r--   0 luke      (1000) luke      (1000)    12904 2022-11-16 20:46:57.000000 pyastgrep-0.9/README.rst
--rw-r--r--   0 luke      (1000) luke      (1000)      670 2022-11-06 19:59:49.000000 pyastgrep-0.9/pyproject.toml
--rw-r--r--   0 luke      (1000) luke      (1000)     1135 2022-11-16 20:47:52.830556 pyastgrep-0.9/setup.cfg
--rw-r--r--   0 luke      (1000) luke      (1000)       38 2022-10-21 16:01:47.000000 pyastgrep-0.9/setup.py
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2022-11-16 20:47:52.826556 pyastgrep-0.9/src/
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2022-11-16 20:47:52.826556 pyastgrep-0.9/src/pyastgrep/
--rw-r--r--   0 luke      (1000) luke      (1000)       20 2022-11-16 20:47:22.000000 pyastgrep-0.9/src/pyastgrep/__init__.py
--rw-r--r--   0 luke      (1000) luke      (1000)     3158 2022-11-16 20:46:57.000000 pyastgrep-0.9/src/pyastgrep/asts.py
--rw-r--r--   0 luke      (1000) luke      (1000)     3930 2022-11-16 20:46:57.000000 pyastgrep-0.9/src/pyastgrep/cli.py
--rw-r--r--   0 luke      (1000) luke      (1000)      810 2022-11-16 20:46:57.000000 pyastgrep-0.9/src/pyastgrep/dump.py
--rw-r--r--   0 luke      (1000) luke      (1000)     2068 2022-11-16 20:46:57.000000 pyastgrep-0.9/src/pyastgrep/files.py
--rw-r--r--   0 luke      (1000) luke      (1000)     7268 2022-11-16 19:57:35.000000 pyastgrep-0.9/src/pyastgrep/ignores.py
--rw-r--r--   0 luke      (1000) luke      (1000)     4285 2022-11-16 19:43:20.000000 pyastgrep-0.9/src/pyastgrep/printer.py
--rw-r--r--   0 luke      (1000) luke      (1000)     3892 2022-11-16 20:46:57.000000 pyastgrep-0.9/src/pyastgrep/search.py
--rw-r--r--   0 luke      (1000) luke      (1000)      696 2022-11-14 14:54:35.000000 pyastgrep-0.9/src/pyastgrep/xml.py
--rw-r--r--   0 luke      (1000) luke      (1000)      366 2022-11-06 20:21:35.000000 pyastgrep-0.9/src/pyastgrep/xpath2.py
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2022-11-16 20:47:52.826556 pyastgrep-0.9/src/pyastgrep.egg-info/
--rw-r-----   0 luke      (1000) luke      (1000)    13751 2022-11-16 20:47:52.000000 pyastgrep-0.9/src/pyastgrep.egg-info/PKG-INFO
--rw-r-----   0 luke      (1000) luke      (1000)      527 2022-11-16 20:47:52.000000 pyastgrep-0.9/src/pyastgrep.egg-info/SOURCES.txt
--rw-r-----   0 luke      (1000) luke      (1000)        1 2022-11-16 20:47:52.000000 pyastgrep-0.9/src/pyastgrep.egg-info/dependency_links.txt
--rw-r-----   0 luke      (1000) luke      (1000)       81 2022-11-16 20:47:52.000000 pyastgrep-0.9/src/pyastgrep.egg-info/entry_points.txt
--rw-r-----   0 luke      (1000) luke      (1000)       58 2022-11-16 20:47:52.000000 pyastgrep-0.9/src/pyastgrep.egg-info/requires.txt
--rw-r-----   0 luke      (1000) luke      (1000)       10 2022-11-16 20:47:52.000000 pyastgrep-0.9/src/pyastgrep.egg-info/top_level.txt
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-04-17 15:42:17.788971 pyastgrep-1.0/
+-rw-r--r--   0 luke      (1000) luke      (1000)      378 2022-10-17 13:09:58.000000 pyastgrep-1.0/.gitattributes
+-rw-r--r--   0 luke      (1000) luke      (1000)     1771 2022-11-07 12:01:43.000000 pyastgrep-1.0/.gitignore
+-rw-rw-rw-   0 luke      (1000) luke      (1000)    14968 2023-04-17 15:42:17.788971 pyastgrep-1.0/PKG-INFO
+-rw-r--r--   0 luke      (1000) luke      (1000)    14121 2023-02-20 15:44:13.000000 pyastgrep-1.0/README.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)      755 2023-04-17 15:02:16.000000 pyastgrep-1.0/pyproject.toml
+-rw-r--r--   0 luke      (1000) luke      (1000)     1135 2023-04-17 15:42:17.788971 pyastgrep-1.0/setup.cfg
+-rw-r--r--   0 luke      (1000) luke      (1000)       38 2022-10-21 16:01:47.000000 pyastgrep-1.0/setup.py
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-04-17 15:42:17.784970 pyastgrep-1.0/src/
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-04-17 15:42:17.788971 pyastgrep-1.0/src/pyastgrep/
+-rw-r--r--   0 luke      (1000) luke      (1000)       20 2023-04-17 15:41:15.000000 pyastgrep-1.0/src/pyastgrep/__init__.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     3158 2022-11-18 11:57:27.000000 pyastgrep-1.0/src/pyastgrep/asts.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     3930 2022-11-16 20:46:57.000000 pyastgrep-1.0/src/pyastgrep/cli.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      890 2022-11-25 07:36:32.000000 pyastgrep-1.0/src/pyastgrep/dump.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     3244 2023-02-20 15:43:43.000000 pyastgrep-1.0/src/pyastgrep/files.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     7904 2023-04-17 15:37:35.000000 pyastgrep-1.0/src/pyastgrep/ignores.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     4276 2023-04-17 14:55:13.000000 pyastgrep-1.0/src/pyastgrep/printer.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     4207 2023-04-17 14:55:57.000000 pyastgrep-1.0/src/pyastgrep/search.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      696 2022-11-14 14:54:35.000000 pyastgrep-1.0/src/pyastgrep/xml.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      366 2022-11-06 20:21:35.000000 pyastgrep-1.0/src/pyastgrep/xpath2.py
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-04-17 15:42:17.788971 pyastgrep-1.0/src/pyastgrep.egg-info/
+-rw-r-----   0 luke      (1000) luke      (1000)    14968 2023-04-17 15:42:17.000000 pyastgrep-1.0/src/pyastgrep.egg-info/PKG-INFO
+-rw-r-----   0 luke      (1000) luke      (1000)      698 2023-04-17 15:42:17.000000 pyastgrep-1.0/src/pyastgrep.egg-info/SOURCES.txt
+-rw-r-----   0 luke      (1000) luke      (1000)        1 2023-04-17 15:42:17.000000 pyastgrep-1.0/src/pyastgrep.egg-info/dependency_links.txt
+-rw-r-----   0 luke      (1000) luke      (1000)       81 2023-04-17 15:42:17.000000 pyastgrep-1.0/src/pyastgrep.egg-info/entry_points.txt
+-rw-r-----   0 luke      (1000) luke      (1000)       58 2023-04-17 15:42:17.000000 pyastgrep-1.0/src/pyastgrep.egg-info/requires.txt
+-rw-r-----   0 luke      (1000) luke      (1000)       10 2023-04-17 15:42:17.000000 pyastgrep-1.0/src/pyastgrep.egg-info/top_level.txt
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-04-17 15:42:17.788971 pyastgrep-1.0/tests/
+-rw-r--r--   0 luke      (1000) luke      (1000)     6800 2022-11-25 07:33:14.000000 pyastgrep-1.0/tests/test_cli.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      733 2022-11-06 19:59:49.000000 pyastgrep-1.0/tests/test_encodings.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      648 2022-11-07 12:52:05.000000 pyastgrep-1.0/tests/test_errors.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     3591 2023-02-20 15:21:15.000000 pyastgrep-1.0/tests/test_ignores.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      449 2022-11-25 08:08:17.000000 pyastgrep-1.0/tests/test_parsing.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     2190 2022-11-07 12:01:43.000000 pyastgrep-1.0/tests/test_printing.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      410 2023-02-20 15:45:50.000000 pyastgrep-1.0/tests/test_symlinks.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     1682 2022-11-07 12:01:43.000000 pyastgrep-1.0/tests/test_xml.py
```

### Comparing `pyastgrep-0.9/.gitignore` & `pyastgrep-1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pyastgrep-0.9/PKG-INFO` & `pyastgrep-1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyastgrep
-Version: 0.9
+Version: 1.0
 Summary: A query tool for Python abstract syntax trees
 Home-page: https://github.com/spookylukey/pyastgrep
 Author: Luke Plant
 License: MIT
 Keywords: xpath xml ast asts syntax query css grep
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
@@ -36,14 +36,16 @@
 In other words, this allows you to search Python code against specific syntax
 elements (function definitions, arguments, assignments, variables etc), instead
 of grepping for string matches.
 
 The interface and behaviour is designed to match grep and ripgrep as far as it
 makes sense to do so.
 
+.. contents:: Contents
+
 
 Installation
 ------------
 
 Python 3.7+ required.
 
 We recommend `pipx <https://pipxproject.github.io/pipx/>`_ to install it
@@ -91,14 +93,16 @@
               <Constant lineno="1" col_offset="4" type="int" value="1"/>
             </value>
           </Assign>
         </body>
         <type_ignores/>
       </Module>
 
+   (When piping input in this way, code will be automatically dedented, making
+   this easier to do from partial Python snippets.)
 
    You can also use the ``pyastgrep`` command, but since the top-level XML
    elements are ``<Module><body>``, and don’t correspond to actual source lines,
    you’ll need to use an XPath expression ``./*/*`` to get a match for each
    statement within the body, and pass ``--xml`` and/or ``--ast`` to dump the
    XML/AST structure:
 
@@ -247,14 +251,25 @@
 “Call nodes that have descendants that match …”, rather than matching those
 descendant nodes themselves.
 
 .. code:: bash
 
    $ pyastgrep './/Call[./func/Attribute[@attr="encode"]]/args/Constant'
 
+
+For a Django code base, find all ``.filter`` and ``.exclude`` method calls, and
+all ``Q`` object calls, which have a keyword argument where the name contains
+the string ``"user"``, for finding ORM calls like
+``.filter(user__id__in=...)`` or ``Q(thing__user=...)``:
+
+.. code:: bash
+
+   pyastgrep '(.//Call[./func/Attribute[@attr="filter" or @attr="exclude"]] | .//Call[./func/Name[@id="Q"]]) [./keywords/keyword[contains(@arg, "user")]]'
+
+
 Ignoring files
 --------------
 
 Files/directories matching ``.gitignore`` entries (global and local) are
 automatically ignored, unless specified as paths on the command line.
 
 Currently there are no other methods to add or remove this ignoring logic.
@@ -368,14 +383,42 @@
 Use as a library
 ----------------
 
 pyastgrep is structured internally to make it easy to use a library as well as
 a CLI. However, while we will try not to break things without good reason, at this
 point we are not documenting or guaranteeing API stability for these functions.
 
+Editor integration
+------------------
+
+Emacs
+~~~~~
+
+pyastgrep works very well with ``compilation-mode`` and wrappers like
+``projectile-compile-project`` from `Projectile
+<https://docs.projectile.mx/projectile/usage.html#basic-usage>`_. We recommend
+setting up a keyboard shortcut for ``next-error`` to enable you to step through
+results easily.
+
+Visual Studio Code
+~~~~~~~~~~~~~~~~~~
+
+Run pyastgrep from a terminal and results will be hyperlinked automatically.
+
+PyCharm
+~~~~~~~
+
+Run pyastgrep from a terminal and results will be hyperlinked automatically.
+
+Others
+~~~~~~
+
+Contributions to this section gladly accepted!
+
+
 
 Contributing
 ------------
 
 Get test suite running::
 
   pip install -r requirements-test.txt
```

### Comparing `pyastgrep-0.9/README.rst` & `pyastgrep-1.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 In other words, this allows you to search Python code against specific syntax
 elements (function definitions, arguments, assignments, variables etc), instead
 of grepping for string matches.
 
 The interface and behaviour is designed to match grep and ripgrep as far as it
 makes sense to do so.
 
+.. contents:: Contents
+
 
 Installation
 ------------
 
 Python 3.7+ required.
 
 We recommend `pipx <https://pipxproject.github.io/pipx/>`_ to install it
@@ -69,14 +71,16 @@
               <Constant lineno="1" col_offset="4" type="int" value="1"/>
             </value>
           </Assign>
         </body>
         <type_ignores/>
       </Module>
 
+   (When piping input in this way, code will be automatically dedented, making
+   this easier to do from partial Python snippets.)
 
    You can also use the ``pyastgrep`` command, but since the top-level XML
    elements are ``<Module><body>``, and don’t correspond to actual source lines,
    you’ll need to use an XPath expression ``./*/*`` to get a match for each
    statement within the body, and pass ``--xml`` and/or ``--ast`` to dump the
    XML/AST structure:
 
@@ -225,14 +229,25 @@
 “Call nodes that have descendants that match …”, rather than matching those
 descendant nodes themselves.
 
 .. code:: bash
 
    $ pyastgrep './/Call[./func/Attribute[@attr="encode"]]/args/Constant'
 
+
+For a Django code base, find all ``.filter`` and ``.exclude`` method calls, and
+all ``Q`` object calls, which have a keyword argument where the name contains
+the string ``"user"``, for finding ORM calls like
+``.filter(user__id__in=...)`` or ``Q(thing__user=...)``:
+
+.. code:: bash
+
+   pyastgrep '(.//Call[./func/Attribute[@attr="filter" or @attr="exclude"]] | .//Call[./func/Name[@id="Q"]]) [./keywords/keyword[contains(@arg, "user")]]'
+
+
 Ignoring files
 --------------
 
 Files/directories matching ``.gitignore`` entries (global and local) are
 automatically ignored, unless specified as paths on the command line.
 
 Currently there are no other methods to add or remove this ignoring logic.
@@ -346,14 +361,42 @@
 Use as a library
 ----------------
 
 pyastgrep is structured internally to make it easy to use a library as well as
 a CLI. However, while we will try not to break things without good reason, at this
 point we are not documenting or guaranteeing API stability for these functions.
 
+Editor integration
+------------------
+
+Emacs
+~~~~~
+
+pyastgrep works very well with ``compilation-mode`` and wrappers like
+``projectile-compile-project`` from `Projectile
+<https://docs.projectile.mx/projectile/usage.html#basic-usage>`_. We recommend
+setting up a keyboard shortcut for ``next-error`` to enable you to step through
+results easily.
+
+Visual Studio Code
+~~~~~~~~~~~~~~~~~~
+
+Run pyastgrep from a terminal and results will be hyperlinked automatically.
+
+PyCharm
+~~~~~~~
+
+Run pyastgrep from a terminal and results will be hyperlinked automatically.
+
+Others
+~~~~~~
+
+Contributions to this section gladly accepted!
+
+
 
 Contributing
 ------------
 
 Get test suite running::
 
   pip install -r requirements-test.txt
```

### Comparing `pyastgrep-0.9/pyproject.toml` & `pyastgrep-1.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -6,21 +6,27 @@
 
 [tool.isort]
 line_length = 120
 profile = "black"
 multi_line_output = 3
 
 
+[tool.ruff]
+line-length = 120
+target-version = 'py310'
+
+
 [tool.mypy]
 ignore_missing_imports = true
 check_untyped_defs = true
 disallow_untyped_calls = true
 disallow_untyped_defs = true
 disallow_incomplete_defs = true
 show_error_codes = true
+exclude = ['dist', 'build']
 
 
 [[tool.mypy.overrides]]
 module = "tests.examples.*"
 ignore_errors = true
 disallow_untyped_calls = false
 disallow_untyped_defs = false
```

### Comparing `pyastgrep-0.9/setup.cfg` & `pyastgrep-1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyastgrep-0.9/src/pyastgrep/asts.py` & `pyastgrep-1.0/src/pyastgrep/asts.py`

 * *Files identical despite different names*

### Comparing `pyastgrep-0.9/src/pyastgrep/cli.py` & `pyastgrep-1.0/src/pyastgrep/cli.py`

 * *Files identical despite different names*

### Comparing `pyastgrep-0.9/src/pyastgrep/dump.py` & `pyastgrep-1.0/src/pyastgrep/dump.py`

 * *Files 25% similar despite different names*

```diff
@@ -19,18 +19,20 @@
 )
 
 
 def main() -> int:
     args = parser.parse_args()
     path = args.path
     if path == "-":
+        auto_dedent = True
         contents = sys.stdin.buffer.read()
     else:
+        auto_dedent = False
         contents = Path(path).read_bytes()
-    _, ast = parse_python_file(contents, path)
+    _, ast = parse_python_file(contents, path, auto_dedent=auto_dedent)
     xml_root = ast_to_xml(ast, {})
     print(xml.tostring(xml_root, pretty_print=True).decode("utf-8"), file=sys.stdout, end="")
     return 0
 
 
 if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `pyastgrep-0.9/src/pyastgrep/ignores.py` & `pyastgrep-1.0/src/pyastgrep/ignores.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,77 @@
 from __future__ import annotations
 
 import subprocess
 from pathlib import Path
-from typing import Generator
+from typing import Generator, Union, overload
 
 from pathspec import GitIgnoreSpec, PathSpec
 from pathspec.patterns.gitwildmatch import GitWildMatchPattern
 
 
+class DirectoryPathSpec:
+    """
+    PathSpec object for a specific directory.
+    """
+
+    # We have to keep track of the location of a .gitignore file, as well as
+    # its contents, in order to correctly handle patterns like:
+    #
+    #   /foo
+    #
+    # which should match `foo` in the same directory as the .gitignore file,
+    # but not in other directories.
+    def __init__(self, location: Path, pathspec: PathSpec):
+        self.location = location
+        self.pathspec = pathspec
+
+    def match_file(self, path: Path) -> bool:
+        try:
+            relative = path.relative_to(self.location)
+        except ValueError:
+            # Could happen if `path` is not relative to (i.e. below) self.location.
+            # Possible for symlinks perhaps? How do we interpret the
+            # .gitignore file correctly if we don't know where the file
+            # is relative to it?
+            # Rather than crash, we ignore the file
+            return False
+        else:
+            return self.pathspec.match_file(relative)
+
+
+PathSpecLike = Union[PathSpec, DirectoryPathSpec]
+
+
+@overload
+def add_negative_dir_pattern(pathspec: PathSpec, directory: Path) -> PathSpec:
+    pass
+
+
+@overload
+def add_negative_dir_pattern(pathspec: DirectoryPathSpec, directory: Path) -> DirectoryPathSpec:
+    pass
+
+
+def add_negative_dir_pattern(pathspec: PathSpec | DirectoryPathSpec, directory: Path) -> PathSpec | DirectoryPathSpec:
+    if isinstance(pathspec, DirectoryPathSpec):
+        return DirectoryPathSpec(pathspec.location, add_negative_dir_pattern(pathspec.pathspec, directory))
+    return pathspec.__class__(list(pathspec.patterns) + [GitWildMatchPattern(f"!{directory}/")])
+
+
 class DirWalker:
     """
     Walks a directory recursively, returning files that match a glob,
     while automatically respecting dot-ignore files
     """
 
     def __init__(
         self,
         *,
         glob: str,
-        pathspecs: list[PathSpec] | None = None,
+        pathspecs: list[PathSpecLike] | None = None,
         init_global_pathspecs: bool = True,
         start_directory: Path | None = None,
         working_dir: Path | None = None,
         absolute_base: bool = False,
     ):
         # DirWalker is immutable outside __init__
         self.glob: str = glob
@@ -30,15 +79,15 @@
             pathspecs = []
         if init_global_pathspecs:
             global_gitignore = get_global_gitignore()
             if global_gitignore:
                 pathspecs.append(pathspec_for_gitignore(global_gitignore, is_global_gitignore=True))
             # POSIX hidden files:
             pathspecs.append(PathSpec([GitWildMatchPattern(".*")]))
-        self.pathspecs: list[PathSpec] = pathspecs
+        self.pathspecs: list[PathSpecLike] = pathspecs
         self.start_directory: Path | None = start_directory
         self.working_dir = working_dir
         self.absolute_base: bool = absolute_base
 
     def for_dir(self, directory: Path, working_dir: Path) -> DirWalker:
         """
         Return a new DirWalker, customised for the directory.
@@ -71,15 +120,15 @@
         the directory the parent current walker is for.
         """
         # This is distinct from `for_dir`, so that we can re-use the work
         # that has already been done in checking parent dirs for .gitignore files,
         # and just check the new current dir.
         if self.start_directory is None:
             raise AssertionError("Must use `for_dir` before `for_subdir`")
-        extra_pathspecs = [
+        extra_pathspecs: list[PathSpecLike] = [
             pathspec_for_gitignore(ignorepath) for ignorepath in find_gitignore_files(directory, recurse_up=False)
         ]
 
         return DirWalker(
             glob=self.glob,
             pathspecs=self.pathspecs + extra_pathspecs,
             init_global_pathspecs=False,
@@ -88,29 +137,35 @@
             absolute_base=self.absolute_base,
         )
 
     def walk(self) -> Generator[Path, None, None]:
         if self.start_directory is None or self.working_dir is None:
             raise AssertionError("Must use `for_dir` before `walk`")
         for filepath in self.start_directory.glob(self.glob):
+            if filepath.is_symlink():
+                # Follow default behaviour of ripgrep, and avoid issues with
+                # `resolve().relative_to(working_dir)
+                continue
             if filepath.is_file():
                 if any(pathspec.match_file(filepath) for pathspec in self.pathspecs):
                     continue
                 if self.absolute_base:
                     yield filepath
                 else:
                     yield filepath.resolve().relative_to(self.working_dir)
         for subdir in self.start_directory.iterdir():
+            if subdir.is_symlink():
+                continue
             if subdir.is_dir():
                 if any(pathspec.match_file(subdir) for pathspec in self.pathspecs):
                     continue
                 yield from self.for_subdir(subdir).walk()
 
 
-def pathspec_for_gitignore(gitignore_file: Path, is_global_gitignore: bool = False) -> PathSpec:
+def pathspec_for_gitignore(gitignore_file: Path, is_global_gitignore: bool = False) -> PathSpec | DirectoryPathSpec:
     with open(gitignore_file) as fp:
         spec = GitIgnoreSpec.from_lines(fp)
         if is_global_gitignore:
             return spec
         else:
             return DirectoryPathSpec(gitignore_file.parent, spec)
 
@@ -148,43 +203,7 @@
         path = subprocess.check_output(["git", "config", "--get", "core.excludesfile"], text=True).strip()
         return Path(path).expanduser()
     except Exception:
         # Most likely the user doesn't have git installed, or it's not configured
         # correctly. In this case we don't want to bug the user with irrelevant
         # warnings, so just ignore completely.
         return None
-
-
-class DirectoryPathSpec:
-    """
-    PathSpec object for a specific directory.
-    """
-
-    # We have to keep track of the location of a .gitignore file, as well as
-    # its contents, in order to correctly handle patterns like:
-    #
-    #   /foo
-    #
-    # which should match `foo` in the same directory as the .gitignore file,
-    # but not in other directories.
-    def __init__(self, location: Path, pathspec: PathSpec):
-        self.location = location
-        self.pathspec = pathspec
-
-    def match_file(self, path: Path) -> bool:
-        try:
-            relative = path.relative_to(self.location)
-        except ValueError:
-            # Could happen if `path` is not relative to (i.e. below) self.location.
-            # Possible for symlinks perhaps? How do we interpret the
-            # .gitignore file correctly if we don't know where the file
-            # is relative to it?
-            # Rather than crash, we ignore the file
-            return False
-        else:
-            return self.pathspec.match_file(relative)
-
-
-def add_negative_dir_pattern(pathspec: PathSpec, directory: Path) -> PathSpec:
-    if isinstance(pathspec, DirectoryPathSpec):
-        return DirectoryPathSpec(pathspec.location, add_negative_dir_pattern(pathspec.pathspec, directory))
-    return pathspec.__class__(pathspec.patterns + [GitWildMatchPattern(f"!{directory}/")])
```

### Comparing `pyastgrep-0.9/src/pyastgrep/printer.py` & `pyastgrep-1.0/src/pyastgrep/printer.py`

 * *Files 5% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         elif isinstance(result, NonElementReturned):
             do_error(f"Error: XPath expression returned a value that is not an AST node: {result.args[0]}")
             continue
 
         matches += 1
         position = result.position
         line_index = position.lineno - 1
-        line = result.file_lines[line_index]
+        line = result.matching_line
         if quiet:
             break
         # Previous result's 'after' lines
         flush_context_lines(before_result=result)
 
         # This result's 'before' lines
         if before_context:
```

### Comparing `pyastgrep-0.9/src/pyastgrep/search.py` & `pyastgrep-1.0/src/pyastgrep/search.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,14 +26,18 @@
 class Match:
     path: Pathlike
     file_lines: list[str]
     xml_element: _Element
     position: Position
     ast_node: ast.AST
 
+    @property
+    def matching_line(self) -> str:
+        return self.file_lines[self.position.lineno - 1]
+
 
 @dataclass
 class Position:
     lineno: int  # 1-indexed, as per AST
     col_offset: int  # 0-indexed, as per AST
 
 
@@ -76,36 +80,41 @@
     paths: Sequence[Path | BinaryIO],
     expression: str,
     xpath2: bool = False,
 ) -> Generator[Match | MissingPath | ReadError | NonElementReturned, None, None]:
     """
     Perform a recursive search through Python files.
 
+    Paths may include directories, e.g "." for the current directory.
+    .gitignore rules will be applied automatically.
+
     """
     query_func = get_query_func(xpath2=xpath2)
 
     for path in get_files_to_search(paths):
         node_mappings: dict[_Element, ast.AST] = {}
         source: Pathlike
+        auto_dedent = False
         if isinstance(path, MissingPath):
             yield path
             continue
         elif isinstance(path, Path):
             source = path
             try:
                 contents = path.read_bytes()
             except OSError as ex:
                 yield ReadError(str(path), ex)
                 continue
         else:
             source = "<stdin>"
             contents = path.read()
+            auto_dedent = True
 
         try:
-            str_contents, parsed_ast = parse_python_file(contents, source)
+            str_contents, parsed_ast = parse_python_file(contents, source, auto_dedent=auto_dedent)
         except SyntaxError as ex:
             yield ReadError(str(source), ex)
             continue
 
         file_lines = str_contents.splitlines()
         xml_ast = ast_to_xml(
             parsed_ast,
```

### Comparing `pyastgrep-0.9/src/pyastgrep/xml.py` & `pyastgrep-1.0/src/pyastgrep/xml.py`

 * *Files identical despite different names*

### Comparing `pyastgrep-0.9/src/pyastgrep.egg-info/PKG-INFO` & `pyastgrep-1.0/src/pyastgrep.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyastgrep
-Version: 0.9
+Version: 1.0
 Summary: A query tool for Python abstract syntax trees
 Home-page: https://github.com/spookylukey/pyastgrep
 Author: Luke Plant
 License: MIT
 Keywords: xpath xml ast asts syntax query css grep
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
@@ -36,14 +36,16 @@
 In other words, this allows you to search Python code against specific syntax
 elements (function definitions, arguments, assignments, variables etc), instead
 of grepping for string matches.
 
 The interface and behaviour is designed to match grep and ripgrep as far as it
 makes sense to do so.
 
+.. contents:: Contents
+
 
 Installation
 ------------
 
 Python 3.7+ required.
 
 We recommend `pipx <https://pipxproject.github.io/pipx/>`_ to install it
@@ -91,14 +93,16 @@
               <Constant lineno="1" col_offset="4" type="int" value="1"/>
             </value>
           </Assign>
         </body>
         <type_ignores/>
       </Module>
 
+   (When piping input in this way, code will be automatically dedented, making
+   this easier to do from partial Python snippets.)
 
    You can also use the ``pyastgrep`` command, but since the top-level XML
    elements are ``<Module><body>``, and don’t correspond to actual source lines,
    you’ll need to use an XPath expression ``./*/*`` to get a match for each
    statement within the body, and pass ``--xml`` and/or ``--ast`` to dump the
    XML/AST structure:
 
@@ -247,14 +251,25 @@
 “Call nodes that have descendants that match …”, rather than matching those
 descendant nodes themselves.
 
 .. code:: bash
 
    $ pyastgrep './/Call[./func/Attribute[@attr="encode"]]/args/Constant'
 
+
+For a Django code base, find all ``.filter`` and ``.exclude`` method calls, and
+all ``Q`` object calls, which have a keyword argument where the name contains
+the string ``"user"``, for finding ORM calls like
+``.filter(user__id__in=...)`` or ``Q(thing__user=...)``:
+
+.. code:: bash
+
+   pyastgrep '(.//Call[./func/Attribute[@attr="filter" or @attr="exclude"]] | .//Call[./func/Name[@id="Q"]]) [./keywords/keyword[contains(@arg, "user")]]'
+
+
 Ignoring files
 --------------
 
 Files/directories matching ``.gitignore`` entries (global and local) are
 automatically ignored, unless specified as paths on the command line.
 
 Currently there are no other methods to add or remove this ignoring logic.
@@ -368,14 +383,42 @@
 Use as a library
 ----------------
 
 pyastgrep is structured internally to make it easy to use a library as well as
 a CLI. However, while we will try not to break things without good reason, at this
 point we are not documenting or guaranteeing API stability for these functions.
 
+Editor integration
+------------------
+
+Emacs
+~~~~~
+
+pyastgrep works very well with ``compilation-mode`` and wrappers like
+``projectile-compile-project`` from `Projectile
+<https://docs.projectile.mx/projectile/usage.html#basic-usage>`_. We recommend
+setting up a keyboard shortcut for ``next-error`` to enable you to step through
+results easily.
+
+Visual Studio Code
+~~~~~~~~~~~~~~~~~~
+
+Run pyastgrep from a terminal and results will be hyperlinked automatically.
+
+PyCharm
+~~~~~~~
+
+Run pyastgrep from a terminal and results will be hyperlinked automatically.
+
+Others
+~~~~~~
+
+Contributions to this section gladly accepted!
+
+
 
 Contributing
 ------------
 
 Get test suite running::
 
   pip install -r requirements-test.txt
```

