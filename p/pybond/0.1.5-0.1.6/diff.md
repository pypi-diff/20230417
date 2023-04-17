# Comparing `tmp/pybond-0.1.5.tar.gz` & `tmp/pybond-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybond-0.1.5.tar", max compression
+gzip compressed data, was "pybond-0.1.6.tar", max compression
```

## Comparing `pybond-0.1.5.tar` & `pybond-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     3059 2023-01-23 21:50:04.117553 pybond-0.1.5/README.md
--rw-r--r--   0        0        0      385 2023-01-23 06:22:02.588103 pybond-0.1.5/pybond/__init__.py
--rw-r--r--   0        0        0     1815 2023-01-23 06:22:02.612136 pybond-0.1.5/pybond/assertions.py
--rw-r--r--   0        0        0     4202 2023-01-23 21:47:07.077568 pybond-0.1.5/pybond/james.py
--rw-r--r--   0        0        0     1904 2023-01-23 07:54:23.440282 pybond-0.1.5/pybond/util.py
--rw-r--r--   0        0        0      984 2023-01-23 21:49:57.653784 pybond-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3785 1970-01-01 00:00:00.000000 pybond-0.1.5/setup.py
--rw-r--r--   0        0        0     4015 1970-01-01 00:00:00.000000 pybond-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     3030 2023-04-17 03:39:11.327283 pybond-0.1.6/README.md
+-rw-r--r--   0        0        0      385 2023-01-23 06:22:02.588103 pybond-0.1.6/pybond/__init__.py
+-rw-r--r--   0        0        0     1815 2023-01-23 06:22:02.612136 pybond-0.1.6/pybond/assertions.py
+-rw-r--r--   0        0        0     4654 2023-04-17 03:38:28.710994 pybond-0.1.6/pybond/james.py
+-rw-r--r--   0        0        0     1971 2023-04-17 03:29:56.232632 pybond-0.1.6/pybond/util.py
+-rw-r--r--   0        0        0      984 2023-04-17 03:39:14.992323 pybond-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3986 1970-01-01 00:00:00.000000 pybond-0.1.6/PKG-INFO
```

### Comparing `pybond-0.1.5/README.md` & `pybond-0.1.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,37 +7,38 @@
 [clojure `bond` library](https://github.com/circleci/bond/).
 
 ## Installation
 
 pip
 
 ```bash
-pip install pybond==0.1.5
+pip install pybond==0.1.6
 ```
 
 requirements.txt
 
 ```python
-pybond==0.1.5
+pybond==0.1.6
 ```
 
 pyproject.toml
 
 ```toml
-pybond = "0.1.5"
+pybond = "0.1.6"
 ```
 
 ## Example usage
 
 Let's say you wanted to test the functions in this module:
 
 ```python
-# /tests/sample_code/my_module.py
+# /sample_code/my_module.py
 from typing import Any
-import tests.sample_code.other_package as other_package
+
+import sample_code.other_package as other_package
 
 
 def foo(x: Any) -> None:
     response = other_package.make_a_network_request(x)
     other_package.write_to_disk(response)
     return response
 
@@ -49,17 +50,17 @@
 With `pybond` you can easily spy on any given function or stub out functions
 that perform IO:
 
 ```python
 # /tests/test_my_module.py
 from pybond import calls, called_with_args, spy, stub, times_called
 
-import tests.sample_code.other_package as other_package
-import tests.sample_code.my_module as my_module
-from tests.sample_code.my_module import bar
+import sample_code.other_package as other_package
+import sample_code.my_module as my_module
+from sample_code.my_module import bar
 
 
 def test_foo_is_called():
     with spy([my_module, "foo"]):
         assert times_called(my_module.foo, 0)
         bar(42)
         assert times_called(my_module.foo, 1)
```

### Comparing `pybond-0.1.5/pybond/assertions.py` & `pybond-0.1.6/pybond/assertions.py`

 * *Files identical despite different names*

### Comparing `pybond-0.1.5/pybond/james.py` & `pybond-0.1.6/pybond/james.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from copy import deepcopy
 from functools import wraps
 from inspect import isclass
 from typing import Any, Callable
 
 from pytest import MonkeyPatch
 
-from pybond.util import function_signatures_match
+from pybond.util import function_signatures_match, is_wrapped_function
 
 
 def _function_call(args, kwargs, error, return_value):
     return {
         "args": args,
         "kwargs": kwargs,
         "error": error,
@@ -77,14 +77,30 @@
     except Exception:
         raise ValueError(
             "The argument is not a spied function. Calls of an unspied "
             "function are not tracked and are therefore not known."
         )
 
 
+def _function_signatures_match(originalf, stubf):
+    """
+    Supports both regular functions and decorated functions using
+    functools.wraps
+    """
+    return (
+        (
+            is_wrapped_function(originalf)
+            and function_signatures_match(originalf.__wrapped__, stubf)
+        ) or (
+            not is_wrapped_function(originalf)
+            and function_signatures_match(originalf, stubf)
+        )
+    )
+
+
 @contextmanager
 def stub(*targets, check_function_signatures=True):
     """
     Context manager which takes a list of targets to stub and spy on.
 
     Example usage:
 
@@ -105,15 +121,15 @@
                 if isclass(originalf):
                     # For now, spying on classes and class methods is
                     # unsupported
                     m.setattr(target=module, name=fname, value=stubf)
                 else:
                     if (
                         check_function_signatures
-                        and not function_signatures_match(originalf, stubf)
+                        and not _function_signatures_match(originalf, stubf)
                     ):
                         raise ValueError(
                             f"Stub does not match the signature of {fname}."
                         )
                     m.setattr(
                         target=module,
                         name=fname,
```

### Comparing `pybond-0.1.5/pybond/util.py` & `pybond-0.1.6/pybond/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,7 +56,11 @@
             if [f.__module__, f.__name__] == ["time", "time"]:
                 return function_signatures_match(_fn_with_zero_arguments, g)
             # Add other specific cases here
             else:
                 raise
         else:
             raise
+
+
+def is_wrapped_function(f):
+    return hasattr(f, "__wrapped__")
```

### Comparing `pybond-0.1.5/pyproject.toml` & `pybond-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pybond"
-version = "0.1.5"
+version = "0.1.6"
 description = "pybond is a spying and stubbing library inspired by the clojure bond library."
 authors = ["Guillaume Pelletier <guigui.p@gmail.com>"]
 license = "Eclipse Public License - v 1.0"
 readme = "README.md"
 homepage = "https://github.com/epgui/pybond"
 repository = "https://github.com/epgui/pybond"
 keywords = [
```

### Comparing `pybond-0.1.5/setup.py` & `pybond-0.1.6/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,143 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pybond
+Version: 0.1.6
+Summary: pybond is a spying and stubbing library inspired by the clojure bond library.
+Home-page: https://github.com/epgui/pybond
+License: Eclipse Public License - v 1.0
+Keywords: bond,monkeypatch,spy,stub,clojure,functional programming
+Author: Guillaume Pelletier
+Author-email: guigui.p@gmail.com
+Requires-Python: >=3.10,<4.0
+Classifier: Intended Audience :: Developers
+Classifier: License :: Other/Proprietary License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Testing
+Classifier: Topic :: Utilities
+Project-URL: Repository, https://github.com/epgui/pybond
+Description-Content-Type: text/markdown
 
-packages = \
-['pybond']
+# pybond
 
-package_data = \
-{'': ['*']}
+[![Build](https://github.com/epgui/pybond/actions/workflows/build.yml/badge.svg)](https://github.com/epgui/pybond/actions/workflows/build.yml)
+[![codecov](https://codecov.io/github/epgui/pybond/branch/main/graph/badge.svg?token=tkq655ROg3)](https://app.codecov.io/github/epgui/pybond)
 
-setup_kwargs = {
-    'name': 'pybond',
-    'version': '0.1.5',
-    'description': 'pybond is a spying and stubbing library inspired by the clojure bond library.',
-    'long_description': '# pybond\n\n[![Build](https://github.com/epgui/pybond/actions/workflows/build.yml/badge.svg)](https://github.com/epgui/pybond/actions/workflows/build.yml)\n[![codecov](https://codecov.io/github/epgui/pybond/branch/main/graph/badge.svg?token=tkq655ROg3)](https://app.codecov.io/github/epgui/pybond)\n\n`pybond` is a spying and stubbing library inspired heavily by the\n[clojure `bond` library](https://github.com/circleci/bond/).\n\n## Installation\n\npip\n\n```bash\npip install pybond==0.1.5\n```\n\nrequirements.txt\n\n```python\npybond==0.1.5\n```\n\npyproject.toml\n\n```toml\npybond = "0.1.5"\n```\n\n## Example usage\n\nLet\'s say you wanted to test the functions in this module:\n\n```python\n# /tests/sample_code/my_module.py\nfrom typing import Any\nimport tests.sample_code.other_package as other_package\n\n\ndef foo(x: Any) -> None:\n    response = other_package.make_a_network_request(x)\n    other_package.write_to_disk(response)\n    return response\n\n\ndef bar(x: Any) -> None:\n    return foo(x)\n```\n\nWith `pybond` you can easily spy on any given function or stub out functions\nthat perform IO:\n\n```python\n# /tests/test_my_module.py\nfrom pybond import calls, called_with_args, spy, stub, times_called\n\nimport tests.sample_code.other_package as other_package\nimport tests.sample_code.my_module as my_module\nfrom tests.sample_code.my_module import bar\n\n\ndef test_foo_is_called():\n    with spy([my_module, "foo"]):\n        assert times_called(my_module.foo, 0)\n        bar(42)\n        assert times_called(my_module.foo, 1)\n        bar(42)\n        bar(42)\n        assert times_called(my_module.foo, 3)\n\n\ndef test_bar_handles_response():\n    with stub(\n        [other_package, "make_a_network_request", lambda x: {"result": x * 2}],\n        [other_package, "write_to_disk", lambda _: None],\n    ), spy(\n        [my_module, "foo"],\n    ):\n        assert times_called(my_module.foo, 0)\n        assert times_called(other_package.make_a_network_request, 0)\n        assert bar(21) == {"result": 42}\n        assert times_called(my_module.foo, 1)\n        assert times_called(other_package.make_a_network_request, 1)\n        assert called_with_args(my_module.foo, args=[21])\n        assert bar(20) == {"result": 40}\n        assert calls(my_module.foo) == [\n            {\n                "args": [21],\n                "kwargs": None,\n                "return": {"result": 42},\n                "error": None,\n            },\n            {\n                "args": [20],\n                "kwargs": None,\n                "return": {"result": 40},\n                "error": None,\n            },\n        ]\n        assert calls(other_package.write_to_disk) == [\n            {\n                "args": [{"result": 42}],\n                "kwargs": None,\n                "return": None,\n                "error": None,\n            },\n            {\n                "args": [{"result": 40}],\n                "kwargs": None,\n                "return": None,\n                "error": None,\n            },\n        ]\n```\n\n## License\n\nDistributed under the\n[Eclipse Public License](http://www.eclipse.org/legal/epl-v10.html).\n',
-    'author': 'Guillaume Pelletier',
-    'author_email': 'guigui.p@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/epgui/pybond',
-    'packages': packages,
-    'package_data': package_data,
-    'python_requires': '>=3.10,<4.0',
-}
+`pybond` is a spying and stubbing library inspired heavily by the
+[clojure `bond` library](https://github.com/circleci/bond/).
 
+## Installation
+
+pip
+
+```bash
+pip install pybond==0.1.6
+```
+
+requirements.txt
+
+```python
+pybond==0.1.6
+```
+
+pyproject.toml
+
+```toml
+pybond = "0.1.6"
+```
+
+## Example usage
+
+Let's say you wanted to test the functions in this module:
+
+```python
+# /sample_code/my_module.py
+from typing import Any
+
+import sample_code.other_package as other_package
+
+
+def foo(x: Any) -> None:
+    response = other_package.make_a_network_request(x)
+    other_package.write_to_disk(response)
+    return response
+
+
+def bar(x: Any) -> None:
+    return foo(x)
+```
+
+With `pybond` you can easily spy on any given function or stub out functions
+that perform IO:
+
+```python
+# /tests/test_my_module.py
+from pybond import calls, called_with_args, spy, stub, times_called
+
+import sample_code.other_package as other_package
+import sample_code.my_module as my_module
+from sample_code.my_module import bar
+
+
+def test_foo_is_called():
+    with spy([my_module, "foo"]):
+        assert times_called(my_module.foo, 0)
+        bar(42)
+        assert times_called(my_module.foo, 1)
+        bar(42)
+        bar(42)
+        assert times_called(my_module.foo, 3)
+
+
+def test_bar_handles_response():
+    with stub(
+        [other_package, "make_a_network_request", lambda x: {"result": x * 2}],
+        [other_package, "write_to_disk", lambda _: None],
+    ), spy(
+        [my_module, "foo"],
+    ):
+        assert times_called(my_module.foo, 0)
+        assert times_called(other_package.make_a_network_request, 0)
+        assert bar(21) == {"result": 42}
+        assert times_called(my_module.foo, 1)
+        assert times_called(other_package.make_a_network_request, 1)
+        assert called_with_args(my_module.foo, args=[21])
+        assert bar(20) == {"result": 40}
+        assert calls(my_module.foo) == [
+            {
+                "args": [21],
+                "kwargs": None,
+                "return": {"result": 42},
+                "error": None,
+            },
+            {
+                "args": [20],
+                "kwargs": None,
+                "return": {"result": 40},
+                "error": None,
+            },
+        ]
+        assert calls(other_package.write_to_disk) == [
+            {
+                "args": [{"result": 42}],
+                "kwargs": None,
+                "return": None,
+                "error": None,
+            },
+            {
+                "args": [{"result": 40}],
+                "kwargs": None,
+                "return": None,
+                "error": None,
+            },
+        ]
+```
+
+## License
+
+Distributed under the
+[Eclipse Public License](http://www.eclipse.org/legal/epl-v10.html).
 
-setup(**setup_kwargs)
```

