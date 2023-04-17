# Comparing `tmp/pydantic-avro-0.4.2.tar.gz` & `tmp/pydantic_avro-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic-avro-0.4.2.tar", max compression
+gzip compressed data, was "pydantic_avro-0.4.3.tar", max compression
```

## Comparing `pydantic-avro-0.4.2.tar` & `pydantic_avro-0.4.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2021-12-17 10:39:19.013474 pydantic-avro-0.4.2/LICENSE
--rw-r--r--   0        0        0     1863 2021-12-30 18:43:33.078382 pydantic-avro-0.4.2/README.md
--rw-r--r--   0        0        0     1517 2022-08-15 11:01:01.673139 pydantic-avro-0.4.2/pyproject.toml
--rw-r--r--   0        0        0        0 2021-12-17 10:46:42.844382 pydantic-avro-0.4.2/src/pydantic_avro/__init__.py
--rw-r--r--   0        0        0      685 2021-12-17 15:30:57.013907 pydantic-avro-0.4.2/src/pydantic_avro/__main__.py
--rw-r--r--   0        0        0     4408 2022-07-04 10:53:19.276525 pydantic-avro-0.4.2/src/pydantic_avro/avro_to_pydantic.py
--rw-r--r--   0        0        0     6187 2022-08-15 11:00:42.106117 pydantic-avro-0.4.2/src/pydantic_avro/base.py
--rw-r--r--   0        0        0     2820 2022-08-15 11:02:39.309545 pydantic-avro-0.4.2/setup.py
--rw-r--r--   0        0        0     2622 2022-08-15 11:02:39.309833 pydantic-avro-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-17 12:47:37.923945 pydantic_avro-0.4.3/LICENSE
+-rw-r--r--   0        0        0     1863 2023-04-17 12:47:37.923945 pydantic_avro-0.4.3/README.md
+-rw-r--r--   0        0        0     1515 2023-04-17 12:47:52.588143 pydantic_avro-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-17 12:47:37.923945 pydantic_avro-0.4.3/src/pydantic_avro/__init__.py
+-rw-r--r--   0        0        0      685 2023-04-17 12:47:37.923945 pydantic_avro-0.4.3/src/pydantic_avro/__main__.py
+-rw-r--r--   0        0        0     4473 2023-04-17 12:47:37.923945 pydantic_avro-0.4.3/src/pydantic_avro/avro_to_pydantic.py
+-rw-r--r--   0        0        0     6286 2023-04-17 12:47:37.923945 pydantic_avro-0.4.3/src/pydantic_avro/base.py
+-rw-r--r--   0        0        0     2822 1970-01-01 00:00:00.000000 pydantic_avro-0.4.3/setup.py
+-rw-r--r--   0        0        0     2671 1970-01-01 00:00:00.000000 pydantic_avro-0.4.3/PKG-INFO
```

### Comparing `pydantic-avro-0.4.2/LICENSE` & `pydantic_avro-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic-avro-0.4.2/README.md` & `pydantic_avro-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `pydantic-avro-0.4.2/src/pydantic_avro/__main__.py` & `pydantic_avro-0.4.3/src/pydantic_avro/__main__.py`

 * *Files identical despite different names*

### Comparing `pydantic-avro-0.4.2/src/pydantic_avro/avro_to_pydantic.py` & `pydantic_avro-0.4.3/src/pydantic_avro/avro_to_pydantic.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,16 @@
                 py_type = "str"
             elif t == "long" or t == "int":
                 py_type = "int"
             elif t == "boolean":
                 py_type = "bool"
             elif t == "double" or t == "float":
                 py_type = "float"
+            elif t == "bytes":
+                py_type = "bytes"
             elif t in classes:
                 py_type = t
             else:
                 raise NotImplementedError(f"Type {t} not supported yet")
         elif isinstance(t, list):
             if "null" in t:
                 optional = True
```

### Comparing `pydantic-avro-0.4.2/src/pydantic_avro/base.py` & `pydantic_avro-0.4.3/src/pydantic_avro/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,14 +101,16 @@
                     "logicalType": "time-micros",
                 }
             elif t == "string" and f == "uuid":
                 avro_type_dict["type"] = {
                     "type": "string",
                     "logicalType": "uuid",
                 }
+            elif t == "string" and f == "binary":
+                avro_type_dict["type"] = "bytes"
             elif t == "string":
                 avro_type_dict["type"] = "string"
             elif t == "number":
                 avro_type_dict["type"] = "double"
             elif t == "integer":
                 # integer in python can be a long
                 avro_type_dict["type"] = "long"
```

### Comparing `pydantic-avro-0.4.2/setup.py` & `pydantic_avro-0.4.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,25 +14,25 @@
 ['pydantic>=1.4.0,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['pydantic-avro = pydantic_avro.__main__:root_main']}
 
 setup_kwargs = {
     'name': 'pydantic-avro',
-    'version': '0.4.2',
+    'version': '0.4.3',
     'description': 'Converting pydantic classes to avro schemas',
     'long_description': '[![Python package](https://github.com/godatadriven/pydantic-avro/actions/workflows/python-package.yml/badge.svg)](https://github.com/godatadriven/pydantic-avro/actions/workflows/python-package.yml)\n[![codecov](https://codecov.io/gh/godatadriven/pydantic-avro/branch/main/graph/badge.svg?token=5L08GOERAW)](https://codecov.io/gh/godatadriven/pydantic-avro)\n[![PyPI version](https://badge.fury.io/py/pydantic-avro.svg)](https://badge.fury.io/py/pydantic-avro)\n[![CodeQL](https://github.com/godatadriven/pydantic-avro/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/godatadriven/pydantic-avro/actions/workflows/codeql-analysis.yml)\n\n# pydantic-avro\n\nThis library can convert a pydantic class to a avro schema or generate python code from a avro schema.\n\n### Install\n\n```bash\npip install pydantic-avro\n```\n\n### Pydantic class to avro schema\n\n```python\nimport json\nfrom typing import Optional\n\nfrom pydantic_avro.base import AvroBase\n\nclass TestModel(AvroBase):\n    key1: str\n    key2: int\n    key2: Optional[str]\n\nschema_dict: dict = TestModel.avro_schema()\nprint(json.dumps(schema_dict))\n\n```\n\n### Avro schema to pydantic\n\n```shell\n# Print to stdout\npydantic-avro avro_to_pydantic --asvc /path/to/schema.asvc\n\n# Save it to a file\npydantic-avro avro_to_pydantic --asvc /path/to/schema.asvc --output /path/to/output.py\n```\n\n\n### Install for developers\n\n###### Install package\n\n- Requirement: Poetry 1.*\n\n```shell\npoetry install\n```\n\n###### Run unit tests\n```shell\npytest\ncoverage run -m pytest  # with coverage\n# or (depends on your local env) \npoetry run pytest\npoetry run coverage run -m pytest  # with coverage\n```\n\n##### Run linting\n\nThe linting is checked in the github workflow. To fix and review issues run this:\n```shell\nblack .   # Auto fix all issues\nisort .   # Auto fix all issues\npflake .  # Only display issues, fixing is manual\n```\n',
     'author': "Peter van 't Hof'",
     'author_email': 'peter.vanthof@godatadriven.com',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/godatadriven/pydantic-avro',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.6.1,<4.0',
+    'python_requires': '>=3.7,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `pydantic-avro-0.4.2/PKG-INFO` & `pydantic_avro-0.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: pydantic-avro
-Version: 0.4.2
+Version: 0.4.3
 Summary: Converting pydantic classes to avro schemas
 Home-page: https://github.com/godatadriven/pydantic-avro
 License: MIT
 Keywords: pydantic,avro
 Author: Peter van 't Hof'
 Author-email: peter.vanthof@godatadriven.com
-Requires-Python: >=3.6.1,<4.0
+Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pydantic (>=1.4.0,<2.0.0)
 Project-URL: Repository, https://github.com/godatadriven/pydantic-avro
 Description-Content-Type: text/markdown
 
 [![Python package](https://github.com/godatadriven/pydantic-avro/actions/workflows/python-package.yml/badge.svg)](https://github.com/godatadriven/pydantic-avro/actions/workflows/python-package.yml)
 [![codecov](https://codecov.io/gh/godatadriven/pydantic-avro/branch/main/graph/badge.svg?token=5L08GOERAW)](https://codecov.io/gh/godatadriven/pydantic-avro)
 [![PyPI version](https://badge.fury.io/py/pydantic-avro.svg)](https://badge.fury.io/py/pydantic-avro)
```

