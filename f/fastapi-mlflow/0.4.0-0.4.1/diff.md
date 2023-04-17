# Comparing `tmp/fastapi-mlflow-0.4.0.tar.gz` & `tmp/fastapi_mlflow-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-mlflow-0.4.0.tar", max compression
+gzip compressed data, was "fastapi_mlflow-0.4.1.tar", max compression
```

## Comparing `fastapi-mlflow-0.4.0.tar` & `fastapi_mlflow-0.4.1.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0    11352 2022-08-11 12:06:12.040233 fastapi-mlflow-0.4.0/LICENSE
--rw-r--r--   0        0        0     2650 2023-01-06 15:26:32.995842 fastapi-mlflow-0.4.0/README.md
--rw-r--r--   0        0        0       22 2022-08-10 14:33:30.741155 fastapi-mlflow-0.4.0/fastapi_mlflow/__init__.py
--rw-r--r--   0        0        0     1272 2023-01-31 13:18:49.969492 fastapi-mlflow-0.4.0/fastapi_mlflow/_mlflow_types.py
--rw-r--r--   0        0        0      990 2023-01-31 13:18:49.972409 fastapi-mlflow-0.4.0/fastapi_mlflow/applications.py
--rw-r--r--   0        0        0     3530 2023-01-31 13:18:49.975432 fastapi-mlflow-0.4.0/fastapi_mlflow/predictors.py
--rw-r--r--   0        0        0      785 2023-01-31 13:19:40.387328 fastapi-mlflow-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     3505 2023-01-31 13:26:19.763246 fastapi-mlflow-0.4.0/setup.py
--rw-r--r--   0        0        0     3438 2023-01-31 13:26:19.763437 fastapi-mlflow-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11352 2022-08-11 12:06:12.040233 fastapi_mlflow-0.4.1/LICENSE
+-rw-r--r--   0        0        0     2650 2023-01-06 15:26:32.995842 fastapi_mlflow-0.4.1/README.md
+-rw-r--r--   0        0        0       22 2022-08-10 14:33:30.741155 fastapi_mlflow-0.4.1/fastapi_mlflow/__init__.py
+-rw-r--r--   0        0        0     1475 2023-04-14 15:44:22.195832 fastapi_mlflow-0.4.1/fastapi_mlflow/_mlflow_types.py
+-rw-r--r--   0        0        0     1032 2023-04-17 13:06:21.593287 fastapi_mlflow-0.4.1/fastapi_mlflow/applications.py
+-rw-r--r--   0        0        0      513 2023-04-17 12:52:44.792281 fastapi_mlflow-0.4.1/fastapi_mlflow/exceptions.py
+-rw-r--r--   0        0        0     3326 2023-04-17 12:55:59.122998 fastapi_mlflow-0.4.1/fastapi_mlflow/predictors.py
+-rw-r--r--   0        0        0      788 2023-04-17 14:46:18.364081 fastapi_mlflow-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     3504 1970-01-01 00:00:00.000000 fastapi_mlflow-0.4.1/setup.py
+-rw-r--r--   0        0        0     3484 1970-01-01 00:00:00.000000 fastapi_mlflow-0.4.1/PKG-INFO
```

### Comparing `fastapi-mlflow-0.4.0/LICENSE` & `fastapi_mlflow-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi-mlflow-0.4.0/README.md` & `fastapi_mlflow-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `fastapi-mlflow-0.4.0/fastapi_mlflow/_mlflow_types.py` & `fastapi_mlflow-0.4.1/fastapi_mlflow/_mlflow_types.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,24 +14,34 @@
     "int32": int,
     "int64": int,
     "double": float,
     "float": float,
     "float32": float,
     "float64": float,
     "string": str,
+    "str": str,
+    "object": str,
     "binary": bytes,
     "datetime": Union[datetime, date],
 }
 
 
+class UnsupportedFieldTypeError(Exception):
+    pass
+
+
 def get_field(type_name: str, nullable: bool):
     """
     :param nullable (bool): Should field be nullable
     """
-    type_ = MLFLOW_SIGNATURE_TO_PYTHON_TYPE_MAP.get(type_name)
+    try:
+        type_ = MLFLOW_SIGNATURE_TO_PYTHON_TYPE_MAP[type_name]
+    except KeyError:
+        raise UnsupportedFieldTypeError(f"Field type not supported: {type_name}")
+
     if nullable:
         type_ = Optional[type_]
 
     field = (type_, ...)  # Ellipsis (...) because default value is unknown
     return field
```

### Comparing `fastapi-mlflow-0.4.0/fastapi_mlflow/applications.py` & `fastapi_mlflow-0.4.1/fastapi_mlflow/applications.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 from fastapi import (
     FastAPI,
     Request,
 )
 from fastapi.responses import JSONResponse
 
 from mlflow.pyfunc import PyFuncModel  # type: ignore
-from fastapi_mlflow.predictors import build_predictor, PyFuncModelPredictError
+
+from fastapi_mlflow.exceptions import DictSerialisableException
+from fastapi_mlflow.predictors import build_predictor
 
 
 def build_app(pyfunc_model: PyFuncModel) -> FastAPI:
     """Build and return a FastAPI app for the mlflow model."""
     app = FastAPI()
     predictor = build_predictor(pyfunc_model)
     response_model = signature(predictor).return_annotation
@@ -25,14 +27,14 @@
         "/predictions",
         predictor,
         response_model=response_model,
         methods=["POST"],
     )
 
     @app.exception_handler(Exception)
-    def handle_exception(_: Request, exc: PyFuncModelPredictError):
+    def handle_exception(_: Request, exc: DictSerialisableException):
         return JSONResponse(
             status_code=500,
             content=exc.to_dict(),
         )
 
     return app
```

### Comparing `fastapi-mlflow-0.4.0/fastapi_mlflow/predictors.py` & `fastapi_mlflow-0.4.1/fastapi_mlflow/predictors.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,24 +17,15 @@
 from mlflow.pyfunc import PyFuncModel  # type: ignore
 from pydantic import BaseModel, create_model
 
 from fastapi_mlflow._mlflow_types import (
     build_model_fields,
     MLFLOW_SIGNATURE_TO_PYTHON_TYPE_MAP,
 )
-
-
-class PyFuncModelPredictError(Exception):
-    def __init__(self, exc: Exception):
-        super().__init__()
-        self.error_type_name = exc.__class__.__name__
-        self.message = str(exc)
-
-    def to_dict(self):
-        return {"name": self.error_type_name, "message": self.message}
+from fastapi_mlflow.exceptions import DictSerialisableException
 
 
 @no_type_check  # Some types here are too dynamic for type checking
 def build_predictor(model: PyFuncModel) -> Callable[[BaseModel], Any]:
     """Build and return a function that wraps the mlflow model.
 
     Currently supports only the `pyfunc`_ flavour of mlflow.
@@ -76,19 +67,18 @@
                 )
 
         return df
 
     def predictor(request: Request) -> Response:
         try:
             predictions = model.predict(request_to_dataframe(request))
+            response_data = convert_predictions_to_python(predictions)
+            return Response(data=response_data)
         except Exception as exc:
-            raise PyFuncModelPredictError(exc) from exc
-
-        response_data = convert_predictions_to_python(predictions)
-        return Response(data=response_data)
+            raise DictSerialisableException.from_exception(exc) from exc
 
     return predictor  # type: ignore
 
 
 def convert_predictions_to_python(results) -> List[Dict[str, Any]]:
     """Convert and return predictions in native Python types."""
     try:
```

### Comparing `fastapi-mlflow-0.4.0/pyproject.toml` & `fastapi_mlflow-0.4.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "fastapi-mlflow"
-version = "0.4.0"
+version = "0.4.1"
 description = "Deploy mlflow models as JSON APIs with minimal new code."
 authors = ["John Harrison <john.harrison@autotrader.co.uk>"]
 readme = "README.md"
 repository = "https://github.com/autotraderuk/fastapi-mlflow"
 license = "Apache-2.0"
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = ">=3.8"
 mlflow = "^1.23.0"
 pydantic = "^1.9.0"
 fastapi = ">=0.73.0"
 
-[tool.poetry.dev-dependencies]
-black = "^21.12b0"
+[tool.poetry.group.dev.dependencies]
+black = ">=22"
 fastapi = {extras = ["all"], version = "^0.88.0"}
 flake8-bugbear = "^22.1.11"
 isort = "^5.10.1"
 pytest = "^6.2.5"
 pandas = "^1.2.0"
 pandas-stubs = "^1.2.0"
 numpy = "^1.22.1"
```

### Comparing `fastapi-mlflow-0.4.0/setup.py` & `fastapi_mlflow-0.4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 {'': ['*']}
 
 install_requires = \
 ['fastapi>=0.73.0', 'mlflow>=1.23.0,<2.0.0', 'pydantic>=1.9.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'fastapi-mlflow',
-    'version': '0.4.0',
+    'version': '0.4.1',
     'description': 'Deploy mlflow models as JSON APIs with minimal new code.',
     'long_description': '# fastapi mlflow\n\nDeploy [mlflow](https://www.mlflow.org/) models as JSON APIs using [FastAPI](https://fastapi.tiangolo.com) with minimal new code.\n\n## Installation\n\n```shell\npip install fastapi-mlflow\n```\n\nFor running the app in production, you will also need an ASGI server, such as [Uvicorn](https://www.uvicorn.org) or [Hypercorn](https://gitlab.com/pgjones/hypercorn).\n\n## Install on Apple Silicon (ARM / M1)\n\nIf you experience problems installing on a newer generation Apple silicon based device, [this solution from StackOverflow](https://stackoverflow.com/a/67586301) before retrying install has been found to help.\n\n```shell\nbrew install openblas gfortran\nexport OPENBLAS="$(brew --prefix openblas)"\n```\n\n## License\n\nCopyright © 2022-23 Auto Trader Group plc.\n\n[Apache-2.0](https://www.apache.org/licenses/LICENSE-2.0)\n\n## Examples\n\n### Simple\n\n#### Create\n\nCreate a file `main.py` containing:\n\n```python\nfrom fastapi_mlflow.applications import build_app\nfrom mlflow.pyfunc import load_model\n\nmodel = load_model("/Users/me/path/to/local/model")\napp = build_app(model)\n```\n\n#### Run\n\nRun the server with:\n\n```shell\nuvicorn main:app\n```\n\n#### Check\n\nOpen your browser at <http://127.0.0.1:8000/docs>\n\nYou should see the automatically generated docs for your model, and be able to test it out using the `Try it out` button in the UI.\n\n### Serve multiple models\n\nIt should be possible to host multiple models (assuming that they have compatible dependencies...) by leveraging [FastAPIs Sub Applications](https://fastapi.tiangolo.com/advanced/sub-applications/#sub-applications-mounts):\n\n```python\nfrom fastapi import FastAPI\nfrom fastapi_mlflow.applications import build_app\nfrom mlflow.pyfunc import load_model\n\napp = FastAPI()\n\nmodel1 = load_model("/Users/me/path/to/local/model1")\nmodel1_app = build_app(model1)\napp.mount("/model1", model1_app)\n\nmodel2 = load_model("/Users/me/path/to/local/model2")\nmodel2_app = build_app(model2)\napp.mount("/model2", model2_app)\n```\n\n[Run](#run) and [Check](#check) as above.\n\n### Custom routing\n\nIf you want more control over where and how the prediction end-point is mounted in your API, you can build the predictor function directly and use it as you need:\n\n```python\nfrom inspect import signature\n\nfrom fastapi import FastAPI\nfrom fastapi_mlflow.predictors import build_predictor\nfrom mlflow.pyfunc import load_model\n\nmodel = load_model("/Users/me/path/to/local/model")\npredictor = build_predictor(model)\napp = FastAPI()\napp.add_api_route(\n    "/classify",\n    predictor,\n    response_model=signature(predictor).return_annotation,\n    methods=["POST"],\n)\n```\n\n[Run](#run) and [Check](#check) as above.\n',
     'author': 'John Harrison',
     'author_email': 'john.harrison@autotrader.co.uk',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/autotraderuk/fastapi-mlflow',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
+    'python_requires': '>=3.8',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `fastapi-mlflow-0.4.0/PKG-INFO` & `fastapi_mlflow-0.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: fastapi-mlflow
-Version: 0.4.0
+Version: 0.4.1
 Summary: Deploy mlflow models as JSON APIs with minimal new code.
 Home-page: https://github.com/autotraderuk/fastapi-mlflow
 License: Apache-2.0
 Author: John Harrison
 Author-email: john.harrison@autotrader.co.uk
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fastapi (>=0.73.0)
 Requires-Dist: mlflow (>=1.23.0,<2.0.0)
 Requires-Dist: pydantic (>=1.9.0,<2.0.0)
 Project-URL: Repository, https://github.com/autotraderuk/fastapi-mlflow
 Description-Content-Type: text/markdown
 
 # fastapi mlflow
```

