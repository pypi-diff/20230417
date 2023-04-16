# Comparing `tmp/hhoppe-tools-1.2.8.tar.gz` & `tmp/hhoppe-tools-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hhoppe-tools-1.2.8.tar", last modified: Sat Apr  8 04:13:37 2023, max compression
+gzip compressed data, was "hhoppe-tools-1.2.9.tar", last modified: Sun Apr 16 23:57:55 2023, max compression
```

## Comparing `hhoppe-tools-1.2.8.tar` & `hhoppe-tools-1.2.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1069 2023-04-08 04:13:29.845101 hhoppe-tools-1.2.8/LICENSE
--rw-r--r--   0        0        0      147 2023-04-08 04:13:29.845101 hhoppe-tools-1.2.8/README.md
--rw-r--r--   0        0        0    76399 2023-04-08 04:13:29.845101 hhoppe-tools-1.2.8/hhoppe_tools/__init__.py
--rw-r--r--   0        0        0        0 2023-04-08 04:13:29.845101 hhoppe-tools-1.2.8/hhoppe_tools/py.typed
--rw-r--r--   0        0        0     2569 2023-04-08 04:13:29.845101 hhoppe-tools-1.2.8/pyproject.toml
--rw-r--r--   0        0        0      919 1970-01-01 00:00:00.000000 hhoppe-tools-1.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-16 23:57:47.691275 hhoppe-tools-1.2.9/LICENSE
+-rw-r--r--   0        0        0      147 2023-04-16 23:57:47.691275 hhoppe-tools-1.2.9/README.md
+-rw-r--r--   0        0        0    75696 2023-04-16 23:57:47.691275 hhoppe-tools-1.2.9/hhoppe_tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-16 23:57:47.691275 hhoppe-tools-1.2.9/hhoppe_tools/py.typed
+-rw-r--r--   0        0        0     2569 2023-04-16 23:57:47.691275 hhoppe-tools-1.2.9/pyproject.toml
+-rw-r--r--   0        0        0      919 1970-01-01 00:00:00.000000 hhoppe-tools-1.2.9/PKG-INFO
```

### Comparing `hhoppe-tools-1.2.8/LICENSE` & `hhoppe-tools-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hhoppe-tools-1.2.8/hhoppe_tools/__init__.py` & `hhoppe-tools-1.2.9/hhoppe_tools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 
 Useful commands to lint and test this module:
 ```shell
 cd ..; c:/windows/sysnative/wsl -e bash -lc 'echo autopep8; autopep8 -j8 -d .; echo pyink; pyink --diff .; echo mypy; mypy .; echo pylint; pylint -j8 .; echo pytest; pytest -qq; echo All ran.'
 
 env python3 -m doctest -v __init__.py | perl -ne 'print if /had no tests/../passed all/' | tail -n +2 | head -n -1
 ```
-."""
+"""
 
 from __future__ import annotations
 
 __docformat__ = 'google'
-__version__ = '1.2.8'
+__version__ = '1.2.9'
 __version_info__ = tuple(int(num) for num in __version__.split('.'))
 
 import ast
 import collections.abc
 from collections.abc import Callable, Iterable, Iterator, Mapping, Sequence
 import contextlib
 import cProfile
@@ -165,16 +165,16 @@
   r"""Prints arguments to `stderr` immediately.
 
   >>> with unittest.mock.patch('sys.stderr', new_callable=io.StringIO) as m:
   ...   print_err('hello')
   ...   print(repr(m.getvalue()))
   'hello\n'
   """
-  kwargs = {**dict(file=sys.stderr, flush=True), **kwargs}
-  print(*args, **kwargs)
+  kwargs2: Any = dict(file=sys.stderr, flush=True) | kwargs
+  print(*args, **kwargs2)
 
 
 def _dump_vars(*args: Any) -> str:
   """Return a string showing the values of each expression.
 
   Specifically, convert each expression (contributed by the caller to the variable-parameter
   list `*args`) into a substring `f'expression = {expression}'` and join these substrings
@@ -481,15 +481,16 @@
       <div>
           {% block content %}{% endblock %}
           {% filter minify_css %}
                   <style>{% include "syntax-highlighting.css" %}</style>
                   <style>{% include "theme.css" %}</style>
                   <style>{% include "content.css" %}</style>
           {% endfilter %}
-      </div>"""
+      </div>
+      """
     )
     (template_dir / 'module.html.jinja2').write_text(
         """\
       {% extends "default/module.html.jinja2" %}
       {% macro is_public(doc) %}
           {% if should_show(doc.qualname) %}
               {{ default_is_public(doc) }}
@@ -1429,14 +1430,36 @@
          [3, 4]])
   """
   if isinstance(a, collections.abc.Iterator):
     return np.array(tuple(a))
   return np.asarray(a)
 
 
+def to_image(a: _ArrayLike, /, color0: _ArrayLike = 0, color1: _ArrayLike = 255) -> _NDArray:
+  """Return a 3-channel uint8 image given a boolean array and specified colors.
+
+  >>> to_image([False, True, True], 10, 240)
+  array([[ 10,  10,  10],
+         [240, 240, 240],
+         [240, 240, 240]], dtype=uint8)
+
+  >>> to_image(np.eye(2) == 1, (240, 241, 242), (255, 0, 0))
+  array([[[255,   0,   0],
+          [240, 241, 242]],
+  <BLANKLINE>
+         [[240, 241, 242],
+          [255,   0,   0]]], dtype=uint8)
+  """
+  a = np.asarray(a)
+  assert a.dtype == bool
+  image = np.full((*a.shape, 3), color0, np.uint8)
+  image[a] = color1
+  return image
+
+
 def pad_array(array: _ArrayLike, /, pad: _ArrayLike, value: _ArrayLike = 0) -> _NDArray:
   """Return `array` padded along initial dimensions by `value`, which may be an array.
 
   Args:
     array: Input data.
     pad: Sequence of tuples representing pad widths before and after each desired dimension.
       The length of `pad` may be less than `array.ndim`.  If `pad` is scalar, it is broadcast
@@ -1854,15 +1877,15 @@
     shape = tuple((num + slice_size - 1) // slice_size if dim == -1 else dim for dim in shape)
   elif math.prod(shape) < num:
     raise ValueError(f'{shape} is insufficiently large for {num} elements.')
   return shape
 
 
 def assemble_arrays(
-    arrays: Sequence[_NDArray],
+    arrays: Sequence[_NDArray] | _NDArray,
     shape: Sequence[int],
     *,
     background: _ArrayLike = 0,
     align: str = 'center',
     spacing: _ArrayLike = 0,
     round_to_even: _ArrayLike = False,
 ) -> _NDArray:
@@ -2253,57 +2276,14 @@
       parents.append(a)
       a = parent
     for p in parents:
       self._rep[p] = a
     return a
 
 
-def topological_sort(graph: Mapping[_T, Sequence[_T]], /, *, cycle_check: bool = False) -> list[_T]:
-  """Given a dag (directed acyclic graph), return a list of graph nodes such that for every
-  directed edge `(u, v)` in the graph, `u` is before `v` in the list.
-  See https://en.wikipedia.org/wiki/Topological_sorting and https://stackoverflow.com/a/47234034 .
-
-  >>> graph = {2: [3], 3: [4], 1: [2], 4: []}
-  >>> topological_sort(graph)
-  [1, 2, 3, 4]
-
-  >>> topological_sort({2: [3], 3: [4, 5], 1: [2], 4: [5], 5: []})
-  [1, 2, 3, 4, 5]
-  """
-  if sys.version_info >= (3, 9):
-    import graphlib  # pylint: disable=import-error
-
-    return list(graphlib.TopologicalSorter(graph).static_order())[::-1]
-
-  result = []
-  seen = set()
-
-  def recurse(node: _T) -> None:
-    for dependent in reversed(graph[node]):
-      if dependent not in seen:
-        seen.add(dependent)
-        recurse(dependent)
-    result.append(node)
-
-  all_dependents: set[_T] = set()
-  all_dependents.update(*graph.values())
-  for node in reversed(list(graph)):
-    if node not in all_dependents:
-      recurse(node)
-
-  if cycle_check:
-    position = {node: i for i, node in enumerate(result)}
-    for node, dependents in graph.items():
-      for dependent in dependents:
-        if position[node] < position[dependent]:
-          raise ValueError('Graph contains a cycle')
-
-  return result[::-1]
-
-
 # ** Plotting
 
 
 def image_from_plt(fig: Any, background: _ArrayLike = 255) -> _NDArray:
   """Return an RGB image by rasterizing a matplotlib figure `fig` over a `background` color."""
   # isinstance(fig, matplotlib.figure.Figure)
   with io.BytesIO() as io_buf:
```

### Comparing `hhoppe-tools-1.2.8/pyproject.toml` & `hhoppe-tools-1.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hhoppe-tools-1.2.8/PKG-INFO` & `hhoppe-tools-1.2.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hhoppe-tools
-Version: 1.2.8
+Version: 1.2.9
 Summary: Library of Python tools by Hugues Hoppe
 Keywords: 
 Author-email: Hugues Hoppe <hhoppe@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

