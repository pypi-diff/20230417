# Comparing `tmp/tum_esm_utils-1.3.0.tar.gz` & `tmp/tum_esm_utils-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tum_esm_utils-1.3.0.tar", max compression
+gzip compressed data, was "tum_esm_utils-1.4.0.tar", max compression
```

## Comparing `tum_esm_utils-1.3.0.tar` & `tum_esm_utils-1.4.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    34523 2023-03-19 02:25:01.728953 tum_esm_utils-1.3.0/LICENSE
--rw-r--r--   0        0        0      311 2023-03-19 01:58:42.297575 tum_esm_utils-1.3.0/README.md
--rw-r--r--   0        0        0     1288 2023-03-24 21:46:44.280153 tum_esm_utils-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      324 2023-03-24 22:12:39.730536 tum_esm_utils-1.3.0/tum_esm_utils/__init__.py
--rw-r--r--   0        0        0     3177 2023-03-18 15:06:07.312912 tum_esm_utils-1.3.0/tum_esm_utils/datastructures.py
--rw-r--r--   0        0        0     1094 2023-03-19 00:09:51.433019 tum_esm_utils-1.3.0/tum_esm_utils/decorators.py
--rw-r--r--   0        0        0     1000 2023-03-24 21:45:42.633163 tum_esm_utils-1.3.0/tum_esm_utils/files.py
--rw-r--r--   0        0        0      571 2023-03-18 12:27:22.283048 tum_esm_utils-1.3.0/tum_esm_utils/github.py
--rw-r--r--   0        0        0       44 2023-03-24 22:36:46.147084 tum_esm_utils-1.3.0/tum_esm_utils/ifg_parser/.gitignore
--rw-r--r--   0        0        0     2462 2023-03-24 21:29:53.767147 tum_esm_utils-1.3.0/tum_esm_utils/ifg_parser/glob_OPUSparms.F90
--rw-r--r--   0        0        0     2459 2023-03-24 21:29:53.777058 tum_esm_utils-1.3.0/tum_esm_utils/ifg_parser/glob_prepro4.F90
--rw-r--r--   0        0        0    28408 2023-03-24 21:29:53.783183 tum_esm_utils-1.3.0/tum_esm_utils/ifg_parser/ifg_parser.F90
--rw-r--r--   0        0        0      758 2023-03-24 21:29:53.790831 tum_esm_utils-1.3.0/tum_esm_utils/ifg_parser/ifg_parser.template.inp
--rw-r--r--   0        0        0   983040 2023-03-24 21:29:53.798327 tum_esm_utils-1.3.0/tum_esm_utils/ifg_parser/refspec.dat
--rw-r--r--   0        0        0   983040 2023-03-24 21:29:53.802664 tum_esm_utils-1.3.0/tum_esm_utils/ifg_parser/refspec2.dat
--rw-r--r--   0        0        0     3902 2023-03-24 22:39:47.173064 tum_esm_utils-1.3.0/tum_esm_utils/interferograms.py
--rw-r--r--   0        0        0     7829 2023-03-19 00:26:19.544914 tum_esm_utils-1.3.0/tum_esm_utils/logger.py
--rw-r--r--   0        0        0      309 2023-03-19 00:38:17.496564 tum_esm_utils-1.3.0/tum_esm_utils/mathematics.py
--rw-r--r--   0        0        0     1553 2023-03-18 13:50:38.104259 tum_esm_utils-1.3.0/tum_esm_utils/processes.py
--rw-r--r--   0        0        0        0 2023-03-18 12:27:05.965015 tum_esm_utils-1.3.0/tum_esm_utils/py.typed
--rw-r--r--   0        0        0     2005 2023-03-18 14:35:49.326738 tum_esm_utils-1.3.0/tum_esm_utils/shell.py
--rw-r--r--   0        0        0     1289 2023-03-18 14:22:32.105297 tum_esm_utils-1.3.0/tum_esm_utils/system.py
--rw-r--r--   0        0        0      851 2023-03-18 14:37:55.541792 tum_esm_utils-1.3.0/tum_esm_utils/testing.py
--rw-r--r--   0        0        0     2391 2023-03-24 10:08:38.856355 tum_esm_utils-1.3.0/tum_esm_utils/text.py
--rw-r--r--   0        0        0     6147 2023-03-24 10:19:28.065528 tum_esm_utils-1.3.0/tum_esm_utils/validators.py
--rw-r--r--   0        0        0     3607 1970-01-01 00:00:00.000000 tum_esm_utils-1.3.0/setup.py
--rw-r--r--   0        0        0     1299 1970-01-01 00:00:00.000000 tum_esm_utils-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-03-19 02:25:01.728953 tum_esm_utils-1.4.0/LICENSE
+-rw-r--r--   0        0        0      311 2023-03-19 01:58:42.297575 tum_esm_utils-1.4.0/README.md
+-rw-r--r--   0        0        0     1288 2023-04-17 17:10:34.521783 tum_esm_utils-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0      324 2023-03-24 22:12:39.730536 tum_esm_utils-1.4.0/tum_esm_utils/__init__.py
+-rw-r--r--   0        0        0     3177 2023-04-15 14:16:07.544110 tum_esm_utils-1.4.0/tum_esm_utils/datastructures.py
+-rw-r--r--   0        0        0     1094 2023-03-19 00:09:51.433019 tum_esm_utils-1.4.0/tum_esm_utils/decorators.py
+-rw-r--r--   0        0        0     1052 2023-04-17 17:40:27.776962 tum_esm_utils-1.4.0/tum_esm_utils/files.py
+-rw-r--r--   0        0        0      571 2023-03-18 12:27:22.283048 tum_esm_utils-1.4.0/tum_esm_utils/github.py
+-rw-r--r--   0        0        0       44 2023-03-24 22:36:46.147084 tum_esm_utils-1.4.0/tum_esm_utils/ifg_parser/.gitignore
+-rw-r--r--   0        0        0     2462 2023-03-24 21:29:53.767147 tum_esm_utils-1.4.0/tum_esm_utils/ifg_parser/glob_OPUSparms.F90
+-rw-r--r--   0        0        0     2459 2023-03-24 21:29:53.777058 tum_esm_utils-1.4.0/tum_esm_utils/ifg_parser/glob_prepro4.F90
+-rw-r--r--   0        0        0    28408 2023-03-24 21:29:53.783183 tum_esm_utils-1.4.0/tum_esm_utils/ifg_parser/ifg_parser.F90
+-rw-r--r--   0        0        0      758 2023-03-24 21:29:53.790831 tum_esm_utils-1.4.0/tum_esm_utils/ifg_parser/ifg_parser.template.inp
+-rw-r--r--   0        0        0   983040 2023-03-24 21:29:53.798327 tum_esm_utils-1.4.0/tum_esm_utils/ifg_parser/refspec.dat
+-rw-r--r--   0        0        0   983040 2023-03-24 21:29:53.802664 tum_esm_utils-1.4.0/tum_esm_utils/ifg_parser/refspec2.dat
+-rw-r--r--   0        0        0     3902 2023-03-24 22:39:47.173064 tum_esm_utils-1.4.0/tum_esm_utils/interferograms.py
+-rw-r--r--   0        0        0     7829 2023-03-19 00:26:19.544914 tum_esm_utils-1.4.0/tum_esm_utils/logger.py
+-rw-r--r--   0        0        0      309 2023-03-19 00:38:17.496564 tum_esm_utils-1.4.0/tum_esm_utils/mathematics.py
+-rw-r--r--   0        0        0     1553 2023-03-18 13:50:38.104259 tum_esm_utils-1.4.0/tum_esm_utils/processes.py
+-rw-r--r--   0        0        0        0 2023-03-18 12:27:05.965015 tum_esm_utils-1.4.0/tum_esm_utils/py.typed
+-rw-r--r--   0        0        0     2856 2023-04-17 17:10:20.854083 tum_esm_utils-1.4.0/tum_esm_utils/shell.py
+-rw-r--r--   0        0        0     1289 2023-03-18 14:22:32.105297 tum_esm_utils-1.4.0/tum_esm_utils/system.py
+-rw-r--r--   0        0        0      851 2023-03-18 14:37:55.541792 tum_esm_utils-1.4.0/tum_esm_utils/testing.py
+-rw-r--r--   0        0        0     3129 2023-04-17 17:44:42.149505 tum_esm_utils-1.4.0/tum_esm_utils/text.py
+-rw-r--r--   0        0        0     6777 2023-04-17 17:41:44.557063 tum_esm_utils-1.4.0/tum_esm_utils/validators.py
+-rw-r--r--   0        0        0     3607 1970-01-01 00:00:00.000000 tum_esm_utils-1.4.0/setup.py
+-rw-r--r--   0        0        0     1299 1970-01-01 00:00:00.000000 tum_esm_utils-1.4.0/PKG-INFO
```

### Comparing `tum_esm_utils-1.3.0/LICENSE` & `tum_esm_utils-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.3.0/pyproject.toml` & `tum_esm_utils-1.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tum_esm_utils"
-version = "1.3.0"
+version = "1.4.0"
 description = "Python utilities by the Professorship of Environmental Sensing and Modeling at the Technical University of Munich"
 authors = ["Moritz Makowski <moritz.makowski@tum.de>"]
 readme = "README.md"
 packages = [
     {include = "tum_esm_utils"},
     {include = "tum_esm_utils/py.typed"}
 ]
```

### Comparing `tum_esm_utils-1.3.0/tum_esm_utils/datastructures.py` & `tum_esm_utils-1.4.0/tum_esm_utils/datastructures.py`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.3.0/tum_esm_utils/decorators.py` & `tum_esm_utils-1.4.0/tum_esm_utils/decorators.py`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.3.0/tum_esm_utils/files.py` & `tum_esm_utils-1.4.0/tum_esm_utils/files.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 import os
-from typing import Any
+from typing import Any, Optional
 
 
 def load_file(path: str) -> str:
     with open(path, "r") as f:
         return f.read()
 
 
@@ -14,17 +14,17 @@
 
 
 def load_json_file(path: str) -> Any:
     with open(path, "r") as f:
         return json.load(f)
 
 
-def dump_json_file(path: str, content: Any) -> None:
+def dump_json_file(path: str, content: Any, indent: Optional[int] = 4) -> None:
     with open(path, "w") as f:
-        json.dump(content, f)
+        json.dump(content, f, indent=indent)
 
 
 def get_parent_dir_path(script_path: str, current_depth: int = 1) -> str:
     """Get the absolute path of a parent directory based on the
     current script path. Simply pass the `__file__` variable of
     the current script to this function. Depth of 1 will return
     the direct parent directory of the current script."""
```

### Comparing `tum_esm_utils-1.3.0/tum_esm_utils/github.py` & `tum_esm_utils-1.4.0/tum_esm_utils/github.py`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.3.0/tum_esm_utils/ifg_parser/glob_OPUSparms.F90` & `tum_esm_utils-1.4.0/tum_esm_utils/ifg_parser/glob_OPUSparms.F90`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.3.0/tum_esm_utils/ifg_parser/glob_prepro4.F90` & `tum_esm_utils-1.4.0/tum_esm_utils/ifg_parser/glob_prepro4.F90`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.3.0/tum_esm_utils/ifg_parser/ifg_parser.F90` & `tum_esm_utils-1.4.0/tum_esm_utils/ifg_parser/ifg_parser.F90`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.3.0/tum_esm_utils/ifg_parser/ifg_parser.template.inp` & `tum_esm_utils-1.4.0/tum_esm_utils/ifg_parser/ifg_parser.template.inp`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.3.0/tum_esm_utils/ifg_parser/refspec.dat` & `tum_esm_utils-1.4.0/tum_esm_utils/ifg_parser/refspec.dat`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.3.0/tum_esm_utils/ifg_parser/refspec2.dat` & `tum_esm_utils-1.4.0/tum_esm_utils/ifg_parser/refspec2.dat`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.3.0/tum_esm_utils/interferograms.py` & `tum_esm_utils-1.4.0/tum_esm_utils/interferograms.py`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.3.0/tum_esm_utils/logger.py` & `tum_esm_utils-1.4.0/tum_esm_utils/logger.py`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.3.0/tum_esm_utils/processes.py` & `tum_esm_utils-1.4.0/tum_esm_utils/processes.py`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.3.0/tum_esm_utils/system.py` & `tum_esm_utils-1.4.0/tum_esm_utils/system.py`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.3.0/tum_esm_utils/testing.py` & `tum_esm_utils-1.4.0/tum_esm_utils/testing.py`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.3.0/tum_esm_utils/text.py` & `tum_esm_utils-1.4.0/tum_esm_utils/text.py`

 * *Files 23% similar despite different names*

```diff
@@ -34,14 +34,37 @@
     try:
         pendulum.from_format(date_string, "YYYYMMDD")
         return True
     except ValueError:
         return False
 
 
+def date_range(from_date_string: str, to_date_string: str) -> list[str]:
+    """Returns a list of dates between `from_date_string` and `to_date_string`.
+
+    Example:
+
+    ```python
+    date_range("20210101", "20210103") == ["20210101", "20210102", "20210103"]
+    ```
+    """
+
+    assert is_date_string(from_date_string), "from_date_string is not a valid date"
+    assert is_date_string(to_date_string), "to_date_string is not a valid date"
+    assert (
+        from_date_string <= to_date_string
+    ), "from_date_string cannot be after to_date_string"
+
+    output = []
+    for date in range(int(from_date_string), int(to_date_string) + 1):
+        if is_date_string(str(date)):
+            output.append(str(date))
+    return output
+
+
 def is_datetime_string(datetime_string: str) -> bool:
     """Returns `True` if string is in a valid `YYYYMMDD HH:mm:ss` format"""
     try:
         pendulum.from_format(datetime_string, "YYYYMMDD HH:mm:ss")
         return True
     except ValueError:
         return False
```

### Comparing `tum_esm_utils-1.3.0/tum_esm_utils/validators.py` & `tum_esm_utils-1.4.0/tum_esm_utils/validators.py`

 * *Files 18% similar despite different names*

```diff
@@ -155,18 +155,33 @@
 
 T = TypeVar("T")
 
 
 def validate_list(
     min_len: Optional[float] = None,
     max_len: Optional[float] = None,
+    allowed: Optional[list[T]] = None,
+    required: Optional[list[T]] = None,
+    forbidden: Optional[list[T]] = None,
 ) -> Callable[[Any, list[T]], list[T]]:
     def f(cls: Any, v: list[T]) -> list[T]:
         if not isinstance(v, list):
             raise ValueError(f'"{v}" is not a list')
         if min_len is not None and len(v) < min_len:
             raise ValueError(f'"{v}" has less than {min_len} elements')
         if max_len is not None and len(v) > max_len:
             raise ValueError(f'"{v}" has more than {max_len} elements')
+        if allowed is not None:
+            for item in v:
+                if item not in allowed:
+                    raise ValueError(f'"{item}" is not allowed')
+        if required is not None:
+            for item in required:
+                if item not in v:
+                    raise ValueError(f'"{v}" has to include "{item}"')
+        if forbidden is not None:
+            for item in forbidden:
+                if item in v:
+                    raise ValueError(f'"{v}" should not include "{item}"')
         return v
 
     return f
```

### Comparing `tum_esm_utils-1.3.0/setup.py` & `tum_esm_utils-1.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 ['filelock>=3.10.0,<4.0.0',
  'pendulum>=2.1.2,<3.0.0',
  'psutil>=5.9.4,<6.0.0',
  'requests>=2.28.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'tum-esm-utils',
-    'version': '1.3.0',
+    'version': '1.4.0',
     'description': 'Python utilities by the Professorship of Environmental Sensing and Modeling at the Technical University of Munich',
     'long_description': '# 🔬 &nbsp;TUM ESM Python Utilities\n\n**Install the Python library with:**\n\n```bash\npoetry add tum_esm_utils\n# or\npip install tum_esm_utils\n```\n\n<br/>\n\n## For Developers\n\n**Publish the Package to PyPI:**\n\n```bash\npoetry build\npoetry publish\n```\n\n**Serve documentation page:**\n\n```bash\ndocsify serve ./docs\n```\n',
     'author': 'Moritz Makowski',
     'author_email': 'moritz.makowski@tum.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/tum-esm/utils',
```

### Comparing `tum_esm_utils-1.3.0/PKG-INFO` & `tum_esm_utils-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tum-esm-utils
-Version: 1.3.0
+Version: 1.4.0
 Summary: Python utilities by the Professorship of Environmental Sensing and Modeling at the Technical University of Munich
 Home-page: https://github.com/tum-esm/utils
 License: AGPL-3.0-only
 Keywords: python,library,utilities,lazydocs,docsify
 Author: Moritz Makowski
 Author-email: moritz.makowski@tum.de
 Requires-Python: >=3.9,<4.0
```

