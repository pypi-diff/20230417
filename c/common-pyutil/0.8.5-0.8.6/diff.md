# Comparing `tmp/common-pyutil-0.8.5.tar.gz` & `tmp/common-pyutil-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "common-pyutil-0.8.5.tar", max compression
+gzip compressed data, was "common-pyutil-0.8.6.tar", max compression
```

## Comparing `common-pyutil-0.8.5.tar` & `common-pyutil-0.8.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1080 2021-10-31 18:50:10.780585 common-pyutil-0.8.5/LICENSE.md
--rw-r--r--   0        0        0      563 2021-11-12 13:24:48.487758 common-pyutil-0.8.5/README.md
--rw-r--r--   0        0        0       22 2023-01-11 21:22:10.499253 common-pyutil-0.8.5/common_pyutil/__init__.py
--rw-r--r--   0        0        0      219 2021-11-12 13:24:48.488758 common-pyutil-0.8.5/common_pyutil/contexts.py
--rw-r--r--   0        0        0     2086 2021-10-31 18:50:06.586667 common-pyutil-0.8.5/common_pyutil/decorators.py
--rw-r--r--   0        0        0    16001 2023-01-30 01:52:58.449867 common-pyutil-0.8.5/common_pyutil/functional.py
--rw-r--r--   0        0        0      860 2021-10-31 18:50:06.596667 common-pyutil-0.8.5/common_pyutil/io.py
--rw-r--r--   0        0        0     6816 2021-10-31 18:50:06.577667 common-pyutil-0.8.5/common_pyutil/log.py
--rw-r--r--   0        0        0     1543 2022-11-26 16:51:57.704616 common-pyutil-0.8.5/common_pyutil/monitor.py
--rw-r--r--   0        0        0     6165 2022-06-09 20:05:34.150703 common-pyutil-0.8.5/common_pyutil/net.py
--rw-r--r--   0        0        0     1686 2023-01-11 14:33:05.379827 common-pyutil-0.8.5/common_pyutil/proc.py
--rw-r--r--   0        0        0        0 2021-10-31 18:50:05.672685 common-pyutil-0.8.5/common_pyutil/py.typed
--rw-r--r--   0        0        0     2592 2021-11-12 13:24:48.490758 common-pyutil-0.8.5/common_pyutil/structures.py
--rw-r--r--   0        0        0     8553 2022-10-17 23:37:58.242608 common-pyutil-0.8.5/common_pyutil/system.py
--rw-r--r--   0        0        0     1476 2022-02-06 10:37:09.214421 common-pyutil-0.8.5/common_pyutil/venv.py
--rw-r--r--   0        0        0     1109 2023-01-11 21:21:21.303114 common-pyutil-0.8.5/pyproject.toml
--rw-r--r--   0        0        0     1370 2023-01-30 07:16:11.054125 common-pyutil-0.8.5/setup.py
--rw-r--r--   0        0        0     1662 2023-01-30 07:16:11.054349 common-pyutil-0.8.5/PKG-INFO
+-rw-r--r--   0        0        0     1080 2021-10-31 18:50:10.780585 common-pyutil-0.8.6/LICENSE.md
+-rw-r--r--   0        0        0      563 2021-11-12 13:24:48.487758 common-pyutil-0.8.6/README.md
+-rw-r--r--   0        0        0       22 2023-04-17 02:55:22.633110 common-pyutil-0.8.6/common_pyutil/__init__.py
+-rw-r--r--   0        0        0      219 2021-11-12 13:24:48.488758 common-pyutil-0.8.6/common_pyutil/contexts.py
+-rw-r--r--   0        0        0     2086 2021-10-31 18:50:06.586667 common-pyutil-0.8.6/common_pyutil/decorators.py
+-rw-r--r--   0        0        0    15900 2023-04-14 10:37:51.995391 common-pyutil-0.8.6/common_pyutil/functional.py
+-rw-r--r--   0        0        0      860 2021-10-31 18:50:06.596667 common-pyutil-0.8.6/common_pyutil/io.py
+-rw-r--r--   0        0        0     6816 2021-10-31 18:50:06.577667 common-pyutil-0.8.6/common_pyutil/log.py
+-rw-r--r--   0        0        0     1543 2022-11-26 16:51:57.704616 common-pyutil-0.8.6/common_pyutil/monitor.py
+-rw-r--r--   0        0        0     6165 2022-06-09 20:05:34.150703 common-pyutil-0.8.6/common_pyutil/net.py
+-rw-r--r--   0        0        0     1686 2023-01-11 14:33:05.379827 common-pyutil-0.8.6/common_pyutil/proc.py
+-rw-r--r--   0        0        0        0 2021-10-31 18:50:05.672685 common-pyutil-0.8.6/common_pyutil/py.typed
+-rw-r--r--   0        0        0     2592 2021-11-12 13:24:48.490758 common-pyutil-0.8.6/common_pyutil/structures.py
+-rw-r--r--   0        0        0     8552 2023-04-13 00:12:02.441705 common-pyutil-0.8.6/common_pyutil/system.py
+-rw-r--r--   0        0        0     1476 2022-02-06 10:37:09.214421 common-pyutil-0.8.6/common_pyutil/venv.py
+-rw-r--r--   0        0        0     1109 2023-04-17 02:55:22.511112 common-pyutil-0.8.6/pyproject.toml
+-rw-r--r--   0        0        0     1370 2023-04-17 02:56:46.788309 common-pyutil-0.8.6/setup.py
+-rw-r--r--   0        0        0     1662 2023-04-17 02:56:46.788537 common-pyutil-0.8.6/PKG-INFO
```

### Comparing `common-pyutil-0.8.5/LICENSE.md` & `common-pyutil-0.8.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `common-pyutil-0.8.5/README.md` & `common-pyutil-0.8.6/README.md`

 * *Files identical despite different names*

### Comparing `common-pyutil-0.8.5/common_pyutil/decorators.py` & `common-pyutil-0.8.6/common_pyutil/decorators.py`

 * *Files identical despite different names*

### Comparing `common-pyutil-0.8.5/common_pyutil/functional.py` & `common-pyutil-0.8.6/common_pyutil/functional.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     ret = []
     for x in ll:
         if x not in ret:
             ret.append(x)
     return ret
 
 
-def identity(x: Any):
+def identity(x: Any) -> Any:
     """Identity function.
 
     Example:
         >>> identity(10)
         10
         >>> identity(None) is None
         True
@@ -147,42 +147,43 @@
         while True:
             try:
                 x = next(it)
                 if predicate(by(x)):
                     return x
             except StopIteration:
                 return None
+    return None
 
 
 def any_attr(obj: object, attrs: List[str],
              predicate: Callable[[Any], bool] = identity):
     """Return True if any attribute in :code:`obj` satisfies :code:`predicate` for a given
     list of attributes :code:`attrs`.
 
     Args:
         obj: Any :code:`python` object
         attrs: A :code:`list` of names of attributes
         predicat: A boolean function
 
     """
-    return any(map(lambda x: predicate(getattr(obj, x, None)), attrs))
+    return any(predicate(getattr(obj, x, None)) for x in attrs)
 
 
 def all_attrs(obj: object, attrs: List[str],
               predicate: Callable[[Any], bool] = identity):
     """Return True if all attributes in :code:`obj` satisfy :code:`predicate` for a given
     list of attributes :code:`attrs`.
 
     Args:
         obj: Any :code:`python` object
         attrs: A :code:`list` of names of attributes
         predicat: A boolean function
 
     """
-    return all(map(lambda x: predicate(getattr(obj, x, None)), attrs))
+    return all(predicate(getattr(obj, x, None)) for x in attrs)
 
 
 def last_item(struct: Optional[Iterable]):
     """Return last item of `struct`.
 
     Args:
         struct: The struct of which to get the last item
@@ -194,14 +195,15 @@
     if struct:
         it = iter(struct)
         while True:
             try:
                 x = next(it)
             except StopIteration:
                 return x
+    return None
 
 
 def first(struct: Iterable, predicate: Callable):
     """Return first item of `struct` which satisfies `predicate`.
     """
     return first_by(struct, identity, predicate)
 
@@ -355,89 +357,84 @@
     """Return a value in a nested object and also print it.
 
     Like :func:`lens` but with more feedback
     """
     if obj is None:
         print(prefix + " (NOT FOUND)")
         return None
-    elif args:
+    if args:
         return print_lens(obj.get(args[0]), *args[1:],
                           prefix=(prefix + " -> " if prefix else "") + str(args[0]))
-    else:
-        print(prefix + " -> " + str(obj))
-        return obj
+    print(prefix + " -> " + str(obj))
+    return obj
 
 
 def set_lens(obj: Optional[Dict], keys: List[str], val: Any) -> bool:
     """Return a value in a nested object.
     """
     if obj is None:
         return False
-    elif keys and len(keys) == 1:
+    if keys and len(keys) == 1:
         obj[keys[0]] = val
         return True
-    elif keys:
+    if keys:
         return set_lens(obj.get(keys[0]), keys[1:], val)
-    else:
-        return False
+    return False
 
 
 def lens(obj: Optional[Dict], *args) -> Any:
     """Recursively access values for given keys in :class:`dict` `obj`
 
     Args:
         obj: The object to scope
         args: variable number of arguments
 
     Returns None if a value isn't found for a sequence of keys.
     """
-    if obj is None:
-        return None
-    elif args:
+    if args and obj:
         return lens(obj.get(args[0]), *args[1:])
-    else:
-        return obj
+    return obj
 
 
 def difference(a: Iterable, b: Iterable) -> set:
     """Return :class:`set` difference of two iterables
 
     Args:
         a: first iterable
         b: second iterable
 
     """
-    a = set([*a])
-    b = set([*b])
+    a = set(*a)
+    b = set(*b)
     return a - b
 
 
 def intersection(a: Iterable, b: Iterable) -> set:
     """Return :class:`set` intersection of two iterables
 
     Args:
         a: first iterable
         b: second iterable
 
     """
-    a = set([*a])
-    b = set([*b])
+    a = set(*a)
+    b = set(*b)
     return a.intersection(b)
 
 
 def union(a: Iterable, b: Iterable) -> set:
     """Return :class:`set` union of two iterables
 
     Args:
         a: first set
         b: second set
 
     """
-    a = set([*a])
-    b = set([*b])
+    a = set(*a)
+    b = set(*b)
     return a.union(b)
 
 
 def concat(_list: Iterable[List]) -> List:
     """Return a new list from concatenating a given list of lists
 
     Args:
@@ -589,16 +586,15 @@
 
         >>> exactly_one(False, None, 0) is None
         True
 
     """
     if sum(map(bool, args)) == 1:
         return first(args, identity)
-    else:
-        return None
+    return None
 
 
 def exactly_k(k, *args):
     """Return all arguments which are :code:`True` if only if
     exactly :code:`k` are :code:`True` among all arguments.
 
     Args:
@@ -606,16 +602,15 @@
 
     Returns:
         The arguments which evaluates to True.
 
     """
     if sum(map(bool, args)) == k:
         return [*filter(identity, args)]
-    else:
-        return None
+    return None
 
 
 def keep(func: Callable, struct: Iterable) -> Iterable:
     """Return a list of only those elements for which :code:`func`
     evaluates to True
 
     Args:
```

### Comparing `common-pyutil-0.8.5/common_pyutil/io.py` & `common-pyutil-0.8.6/common_pyutil/io.py`

 * *Files identical despite different names*

### Comparing `common-pyutil-0.8.5/common_pyutil/log.py` & `common-pyutil-0.8.6/common_pyutil/log.py`

 * *Files identical despite different names*

### Comparing `common-pyutil-0.8.5/common_pyutil/monitor.py` & `common-pyutil-0.8.6/common_pyutil/monitor.py`

 * *Files identical despite different names*

### Comparing `common-pyutil-0.8.5/common_pyutil/net.py` & `common-pyutil-0.8.6/common_pyutil/net.py`

 * *Files identical despite different names*

### Comparing `common-pyutil-0.8.5/common_pyutil/proc.py` & `common-pyutil-0.8.6/common_pyutil/proc.py`

 * *Files identical despite different names*

### Comparing `common-pyutil-0.8.5/common_pyutil/structures.py` & `common-pyutil-0.8.6/common_pyutil/structures.py`

 * *Files identical despite different names*

### Comparing `common-pyutil-0.8.5/common_pyutil/system.py` & `common-pyutil-0.8.6/common_pyutil/system.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,20 +174,21 @@
     # NOTE: The global opts is a bit tricky. If we don't parse and interpret the
     #       arguments here, then the actions will have to be provided alongside
     #       the args.
     #
     #       Or let the user parse and interpret the global opts but then help
     #       display and all must be controlled by the user.
     def __call__(self):
+        cmds = ", ".join(f'"{x}"' for x in self.cmd_map)
         parser = argparse.ArgumentParser(self.name, allow_abbrev=False, add_help=False,
                                          formatter_class=argparse.RawTextHelpFormatter,
                                          usage=self.usage)
         parser.add_argument("command", help=f"""Command to run.
 
-command is one of {", ".join(map(lambda x: f'"{x}"', self.cmd_map.keys()))}
+command is one of {cmds}
 
 Type "{self.name} command --help" to get help about the individual commands.""")
         if self.version_str:
             parser.add_argument("--version", action="store_true", help="Print version and exit")
         if len(sys.argv) == 1:
             print("No command given\n")
             parser.print_help()
@@ -199,15 +200,15 @@
             print(self.version_str)
             sys.exit(0)
         if sys.argv[1].startswith("-"):
             pre_cmd_args = [*takewhile(lambda x: x.startswith("-"), sys.argv[1:])]
             if self.gopts_parser is not None:
                 gopts = self.gopts_parser(pre_cmd_args)
             else:
-                msg = ", ".join(map(lambda x: f'"{x}"', pre_cmd_args))
+                msg = ", ".join(f'"{x}"' for x in pre_cmd_args)
                 print(f"Unknown options {msg}")
                 parser.print_help()
                 sys.exit(1)
         else:
             gopts = None
         post_cmd_args = [*dropwhile(lambda x: x.startswith("-"), sys.argv[1:])]
         if not post_cmd_args:
```

### Comparing `common-pyutil-0.8.5/common_pyutil/venv.py` & `common-pyutil-0.8.6/common_pyutil/venv.py`

 * *Files identical despite different names*

### Comparing `common-pyutil-0.8.5/pyproject.toml` & `common-pyutil-0.8.6/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "common-pyutil"
-version = "0.8.5"
+version = "0.8.6"
 description = "Some common python utility functions"
 authors = ["Akshay <atavist13@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/akshaybadola/common-pyutil"
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `common-pyutil-0.8.5/setup.py` & `common-pyutil-0.8.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['file-magic>=0.4.0,<0.5.0', 'requests>=2.26.0,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['test = pytest:main']}
 
 setup_kwargs = {
     'name': 'common-pyutil',
-    'version': '0.8.5',
+    'version': '0.8.6',
     'description': 'Some common python utility functions',
     'long_description': "# common-pyutil\nBunch of common utility functions I've used in various projects. This package\nprovides a uniform interface to them.\n\n# Features\n\n- Pure python stdlib with no external dependencies (except [requests](https://github.com/psf/requests))\n- Bunch of useful modules like:\n  1. A simple hierarchical argument parser.\n  2. Functional programming library.\n  3. A `Timer` context for easy monitoring\n  4. A `Tag` decorator for function tagging\n  5. A logging module to get generate a logger with sensible defaults.\n  6. A `Get` class with progress tracking.\n",
     'author': 'Akshay',
     'author_email': 'atavist13@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/akshaybadola/common-pyutil',
```

### Comparing `common-pyutil-0.8.5/PKG-INFO` & `common-pyutil-0.8.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: common-pyutil
-Version: 0.8.5
+Version: 0.8.6
 Summary: Some common python utility functions
 Home-page: https://github.com/akshaybadola/common-pyutil
 License: MIT
 Keywords: utilities,functional
 Author: Akshay
 Author-email: atavist13@gmail.com
 Requires-Python: >=3.7,<4.0
```

