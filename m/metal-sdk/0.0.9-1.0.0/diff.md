# Comparing `tmp/metal_sdk-0.0.9.tar.gz` & `tmp/metal_sdk-1.0.0.tar.gz`

## Comparing `metal_sdk-0.0.9.tar` & `metal_sdk-1.0.0.tar`

### file list

```diff
@@ -1,9 +1,16 @@
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 metal_sdk-0.0.9/src/metal_sdk/Metal.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 metal_sdk-0.0.9/src/metal_sdk/__init__.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 metal_sdk-0.0.9/src/metal_sdk/typings.py
--rw-r--r--   0        0        0     4599 2020-02-02 00:00:00.000000 metal_sdk-0.0.9/tests/test_metal.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 metal_sdk-0.0.9/.gitignore
--rw-r--r--   0        0        0    10942 2020-02-02 00:00:00.000000 metal_sdk-0.0.9/LICENSE
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 metal_sdk-0.0.9/README.md
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 metal_sdk-0.0.9/pyproject.toml
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 metal_sdk-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 metal_sdk-1.0.0/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 metal_sdk-1.0.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 metal_sdk-1.0.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 metal_sdk-1.0.0/examples/example.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 metal_sdk-1.0.0/examples/example_async.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 metal_sdk-1.0.0/src/metal_sdk/__init__.py
+-rw-r--r--   0        0        0     3778 2020-02-02 00:00:00.000000 metal_sdk-1.0.0/src/metal_sdk/metal.py
+-rw-r--r--   0        0        0     3825 2020-02-02 00:00:00.000000 metal_sdk-1.0.0/src/metal_sdk/metal_async.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 metal_sdk-1.0.0/src/metal_sdk/typings.py
+-rw-r--r--   0        0        0     5646 2020-02-02 00:00:00.000000 metal_sdk-1.0.0/tests/test_metal.py
+-rw-r--r--   0        0        0     5785 2020-02-02 00:00:00.000000 metal_sdk-1.0.0/tests/test_metal_async.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 metal_sdk-1.0.0/.gitignore
+-rw-r--r--   0        0        0    10942 2020-02-02 00:00:00.000000 metal_sdk-1.0.0/LICENSE
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 metal_sdk-1.0.0/README.md
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 metal_sdk-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 metal_sdk-1.0.0/PKG-INFO
```

### Comparing `metal_sdk-0.0.9/.gitignore` & `metal_sdk-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `metal_sdk-0.0.9/LICENSE` & `metal_sdk-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metal_sdk-0.0.9/PKG-INFO` & `metal_sdk-1.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,47 @@
 Metadata-Version: 2.1
 Name: metal_sdk
-Version: 0.0.9
+Version: 1.0.0
 Summary: SDK for getmetal.io
 Project-URL: Github, https://github.com/getmetal/metal-python
 Author-email: Metal Technologies Inc <james@getmetal.io>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
-Requires-Dist: requests
+Requires-Dist: httpx
+Requires-Dist: typing-extensions
 Description-Content-Type: text/markdown
 
 # 🤘 Metal Python SDK
 
 - [**Developer Documentation**](https://docs.getmetal.io/sdk-python)
 - [**PyPi Package**](https://pypi.org/project/metal-sdk/)
 
 ## Setup
 
 ```bash
-pip install metal-sdk
+$ pip3 install metal-sdk
 ```
 
 ## Usage
 
 ```python
-  metal = MetalSDK("api_key", "client_id", "app_id");
-  metal.index({ text: 'a' })
-  metal.index({ text: 'b' })
-  metal.index({ text: 'c' })
+from metal_sdk.metal import Metal
+
+
+metal = Metal("api_key", "client_id", "index_id");
+
+metal.index({ text: 'a' })
+metal.index({ text: 'b' })
+metal.index({ text: 'c' })
 ```
 
-## Contributing
+[Async example](./examples/example_async.py)
+
+## Testing
 
 ```bash
-$ python3 -m build
-$ python3 -m twine upload dist/*
+$ python3 -m unittest tests/test_metal.py
 ```
 
 [Reference](https://packaging.python.org/en/latest/tutorials/packaging-projects/)
```

