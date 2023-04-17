# Comparing `tmp/itkwasm-1.0b93.tar.gz` & `tmp/itkwasm-1.0b94.tar.gz`

## Comparing `itkwasm-1.0b93.tar` & `itkwasm-1.0b94.tar`

### file list

```diff
@@ -1,46 +1,54 @@
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 itkwasm-1.0b93/itkwasm/__init__.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 itkwasm-1.0b93/itkwasm/binary_file.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 itkwasm-1.0b93/itkwasm/binary_stream.py
--rw-r--r--   0        0        0     3162 2020-02-02 00:00:00.000000 itkwasm-1.0b93/itkwasm/environment_dispatch.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 itkwasm-1.0b93/itkwasm/float_types.py
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 itkwasm-1.0b93/itkwasm/image.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 itkwasm-1.0b93/itkwasm/int_types.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 itkwasm-1.0b93/itkwasm/interface_types.py
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 itkwasm-1.0b93/itkwasm/mesh.py
--rw-r--r--   0        0        0    21137 2020-02-02 00:00:00.000000 itkwasm-1.0b93/itkwasm/pipeline.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 itkwasm-1.0b93/itkwasm/pipeline_input.py
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 itkwasm-1.0b93/itkwasm/pipeline_output.py
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 itkwasm-1.0b93/itkwasm/pixel_types.py
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 itkwasm-1.0b93/itkwasm/pointset.py
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 itkwasm-1.0b93/itkwasm/polydata.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 itkwasm-1.0b93/itkwasm/text_file.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 itkwasm-1.0b93/itkwasm/text_stream.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkwasm-1.0b93/itkwasm/transform.py
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 itkwasm-1.0b93/test/test_function_factory.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 itkwasm-1.0b93/test/test_image.py
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 itkwasm-1.0b93/test/test_mesh.py
--rw-r--r--   0        0        0     6973 2020-02-02 00:00:00.000000 itkwasm-1.0b93/test/test_pipeline.py
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 itkwasm-1.0b93/test/test_pointset.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 itkwasm-1.0b93/test/test_polydata.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkwasm-1.0b93/test/test_transform.py
--rw-r--r--   0        0        0    22130 2020-02-02 00:00:00.000000 itkwasm-1.0b93/test/baseline/test_pipeline_write_read_image.png
--rw-r--r--   0        0        0   143137 2020-02-02 00:00:00.000000 itkwasm-1.0b93/test/input/cow.vtk
--rw-r--r--   0        0        0    29353 2020-02-02 00:00:00.000000 itkwasm-1.0b93/test/input/cthead1.png
--rwxr-xr-x   0        0        0   620974 2020-02-02 00:00:00.000000 itkwasm-1.0b93/test/input/input-output-files-test.wasi.wasm
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 itkwasm-1.0b93/test/input/input.bin
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 itkwasm-1.0b93/test/input/input.txt
--rwxr-xr-x   0        0        0  1135160 2020-02-02 00:00:00.000000 itkwasm-1.0b93/test/input/median-filter-test.wasi.wasm
--rwxr-xr-x   0        0        0  1278174 2020-02-02 00:00:00.000000 itkwasm-1.0b93/test/input/mesh-read-write-test.wasi.wasm
--rwxr-xr-x   0        0        0  2174461 2020-02-02 00:00:00.000000 itkwasm-1.0b93/test/input/mesh-to-poly-data.wasi.wasm
--rwxr-xr-x   0        0        0  1287522 2020-02-02 00:00:00.000000 itkwasm-1.0b93/test/input/poly-data-to-mesh.wasi.wasm
--rwxr-xr-x   0        0        0   269115 2020-02-02 00:00:00.000000 itkwasm-1.0b93/test/input/stdout-stderr-test.wasi.wasm
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 itkwasm-1.0b93/test/test-accelerator/pyproject.toml
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 itkwasm-1.0b93/test/test-accelerator/test_accelerator/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm-1.0b93/test/test-accelerator/test_accelerator/faster_mod.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 itkwasm-1.0b93/test/test-accelerator/test_accelerator/fastest_mod.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm-1.0b93/test/test-accelerator/test_accelerator/slower_mod.py
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 itkwasm-1.0b93/.gitignore
--rw-r--r--   0        0        0    11360 2020-02-02 00:00:00.000000 itkwasm-1.0b93/LICENSE
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 itkwasm-1.0b93/README.md
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 itkwasm-1.0b93/pyproject.toml
--rw-r--r--   0        0        0    14437 2020-02-02 00:00:00.000000 itkwasm-1.0b93/PKG-INFO
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 itkwasm-1.0b94/docs/.gitignore
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 itkwasm-1.0b94/docs/Makefile
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 itkwasm-1.0b94/docs/conf.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 itkwasm-1.0b94/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 itkwasm-1.0b94/docs/make.bat
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 itkwasm-1.0b94/docs/requirements.txt
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 itkwasm-1.0b94/itkwasm/__init__.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 itkwasm-1.0b94/itkwasm/binary_file.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 itkwasm-1.0b94/itkwasm/binary_stream.py
+-rw-r--r--   0        0        0     3162 2020-02-02 00:00:00.000000 itkwasm-1.0b94/itkwasm/environment_dispatch.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 itkwasm-1.0b94/itkwasm/float_types.py
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 itkwasm-1.0b94/itkwasm/image.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 itkwasm-1.0b94/itkwasm/int_types.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 itkwasm-1.0b94/itkwasm/interface_types.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 itkwasm-1.0b94/itkwasm/js_package_config.py
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 itkwasm-1.0b94/itkwasm/mesh.py
+-rw-r--r--   0        0        0    21137 2020-02-02 00:00:00.000000 itkwasm-1.0b94/itkwasm/pipeline.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 itkwasm-1.0b94/itkwasm/pipeline_input.py
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 itkwasm-1.0b94/itkwasm/pipeline_output.py
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 itkwasm-1.0b94/itkwasm/pixel_types.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 itkwasm-1.0b94/itkwasm/pointset.py
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 itkwasm-1.0b94/itkwasm/polydata.py
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 itkwasm-1.0b94/itkwasm/text_file.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 itkwasm-1.0b94/itkwasm/text_stream.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkwasm-1.0b94/itkwasm/transform.py
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 itkwasm-1.0b94/test/test_function_factory.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 itkwasm-1.0b94/test/test_image.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 itkwasm-1.0b94/test/test_js_package_config.py
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 itkwasm-1.0b94/test/test_mesh.py
+-rw-r--r--   0        0        0     6973 2020-02-02 00:00:00.000000 itkwasm-1.0b94/test/test_pipeline.py
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 itkwasm-1.0b94/test/test_pointset.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 itkwasm-1.0b94/test/test_polydata.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkwasm-1.0b94/test/test_transform.py
+-rw-r--r--   0        0        0    22130 2020-02-02 00:00:00.000000 itkwasm-1.0b94/test/baseline/test_pipeline_write_read_image.png
+-rw-r--r--   0        0        0   143137 2020-02-02 00:00:00.000000 itkwasm-1.0b94/test/input/cow.vtk
+-rw-r--r--   0        0        0    29353 2020-02-02 00:00:00.000000 itkwasm-1.0b94/test/input/cthead1.png
+-rwxr-xr-x   0        0        0   620974 2020-02-02 00:00:00.000000 itkwasm-1.0b94/test/input/input-output-files-test.wasi.wasm
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 itkwasm-1.0b94/test/input/input.bin
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 itkwasm-1.0b94/test/input/input.txt
+-rwxr-xr-x   0        0        0  1135160 2020-02-02 00:00:00.000000 itkwasm-1.0b94/test/input/median-filter-test.wasi.wasm
+-rwxr-xr-x   0        0        0  1278174 2020-02-02 00:00:00.000000 itkwasm-1.0b94/test/input/mesh-read-write-test.wasi.wasm
+-rwxr-xr-x   0        0        0  2174461 2020-02-02 00:00:00.000000 itkwasm-1.0b94/test/input/mesh-to-poly-data.wasi.wasm
+-rwxr-xr-x   0        0        0  1287522 2020-02-02 00:00:00.000000 itkwasm-1.0b94/test/input/poly-data-to-mesh.wasi.wasm
+-rwxr-xr-x   0        0        0   269115 2020-02-02 00:00:00.000000 itkwasm-1.0b94/test/input/stdout-stderr-test.wasi.wasm
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 itkwasm-1.0b94/test/test-accelerator/pyproject.toml
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 itkwasm-1.0b94/test/test-accelerator/test_accelerator/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm-1.0b94/test/test-accelerator/test_accelerator/faster_mod.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 itkwasm-1.0b94/test/test-accelerator/test_accelerator/fastest_mod.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm-1.0b94/test/test-accelerator/test_accelerator/slower_mod.py
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 itkwasm-1.0b94/.gitignore
+-rw-r--r--   0        0        0    11360 2020-02-02 00:00:00.000000 itkwasm-1.0b94/LICENSE
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 itkwasm-1.0b94/README.md
+-rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 itkwasm-1.0b94/pyproject.toml
+-rw-r--r--   0        0        0    14379 2020-02-02 00:00:00.000000 itkwasm-1.0b94/PKG-INFO
```

### Comparing `itkwasm-1.0b93/itkwasm/__init__.py` & `itkwasm-1.0b94/itkwasm/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """itkwasm: Python interface to itk-wasm WebAssembly modules."""
 
-__version__ = "1.0b93"
+__version__ = "1.0b94"
 
 from .interface_types import InterfaceTypes
 from .image import Image, ImageType
 from .pointset import PointSet, PointSetType
 from .mesh import Mesh, MeshType
 from .polydata import PolyData, PolyDataType
 from .binary_file import BinaryFile
@@ -14,14 +14,15 @@
 from .pipeline import Pipeline
 from .pipeline_input import PipelineInput
 from .pipeline_output import PipelineOutput
 from .float_types import FloatTypes
 from .int_types import IntTypes
 from .pixel_types import PixelTypes
 from .environment_dispatch import environment_dispatch, function_factory
+from .js_package_config import JsPackageConfig
 
 __all__ = [
   "InterfaceTypes",
   "Pipeline",
   "PipelineInput",
   "PipelineOutput",
   "Image",
@@ -37,8 +38,9 @@
   "TextFile",
   "TextStream",
   "FloatTypes",
   "IntTypes",
   "PixelTypes",
   "environment_dispatch",
   "function_factory",
+  "JsPackageConfig",
 ]
```

### Comparing `itkwasm-1.0b93/itkwasm/environment_dispatch.py` & `itkwasm-1.0b94/itkwasm/environment_dispatch.py`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b93/itkwasm/image.py` & `itkwasm-1.0b94/itkwasm/image.py`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b93/itkwasm/mesh.py` & `itkwasm-1.0b94/itkwasm/mesh.py`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b93/itkwasm/pipeline.py` & `itkwasm-1.0b94/itkwasm/pipeline.py`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b93/itkwasm/pipeline_input.py` & `itkwasm-1.0b94/itkwasm/pipeline_input.py`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b93/itkwasm/pipeline_output.py` & `itkwasm-1.0b94/itkwasm/pipeline_output.py`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b93/itkwasm/pixel_types.py` & `itkwasm-1.0b94/itkwasm/pixel_types.py`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b93/itkwasm/pointset.py` & `itkwasm-1.0b94/itkwasm/pointset.py`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b93/itkwasm/polydata.py` & `itkwasm-1.0b94/itkwasm/polydata.py`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b93/test/test_function_factory.py` & `itkwasm-1.0b94/test/test_function_factory.py`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b93/test/test_image.py` & `itkwasm-1.0b94/test/test_image.py`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b93/test/test_mesh.py` & `itkwasm-1.0b94/test/test_mesh.py`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b93/test/test_pipeline.py` & `itkwasm-1.0b94/test/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b93/test/test_pointset.py` & `itkwasm-1.0b94/test/test_pointset.py`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b93/test/baseline/test_pipeline_write_read_image.png` & `itkwasm-1.0b94/test/baseline/test_pipeline_write_read_image.png`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b93/test/input/cow.vtk` & `itkwasm-1.0b94/test/input/cow.vtk`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b93/test/input/cthead1.png` & `itkwasm-1.0b94/test/input/cthead1.png`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b93/test/input/input-output-files-test.wasi.wasm` & `itkwasm-1.0b94/test/input/input-output-files-test.wasi.wasm`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b93/test/input/median-filter-test.wasi.wasm` & `itkwasm-1.0b94/test/input/median-filter-test.wasi.wasm`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b93/test/input/mesh-read-write-test.wasi.wasm` & `itkwasm-1.0b94/test/input/mesh-read-write-test.wasi.wasm`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b93/test/input/mesh-to-poly-data.wasi.wasm` & `itkwasm-1.0b94/test/input/mesh-to-poly-data.wasi.wasm`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b93/test/input/poly-data-to-mesh.wasi.wasm` & `itkwasm-1.0b94/test/input/poly-data-to-mesh.wasi.wasm`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b93/test/input/stdout-stderr-test.wasi.wasm` & `itkwasm-1.0b94/test/input/stdout-stderr-test.wasi.wasm`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b93/test/test-accelerator/pyproject.toml` & `itkwasm-1.0b94/test/test-accelerator/pyproject.toml`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b93/.gitignore` & `itkwasm-1.0b94/.gitignore`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b93/LICENSE` & `itkwasm-1.0b94/LICENSE`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b93/pyproject.toml` & `itkwasm-1.0b94/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -42,11 +42,19 @@
 Issues = "https://github.com/InsightSoftwareConsortium/itk-wasm/issues"
 
 [project.optional-dependencies]
 test = [
     "itk>=5.3.0",
     "pytest >=2.7.3",
 ]
-doc = ["sphinx"]
+
+[tool.hatch.envs.docs]
+dependencies = [
+  "sphinx",
+  "pydata-sphinx-theme",
+]
+
+[tool.hatch.envs.docs.scripts]
+html = "cd docs && make html"
 
 [tool.hatch.version]
 path = "itkwasm/__init__.py"
```

### Comparing `itkwasm-1.0b93/PKG-INFO` & `itkwasm-1.0b94/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itkwasm
-Version: 1.0b93
+Version: 1.0b94
 Summary: Python interface to itk-wasm WebAssembly (Wasm) modules.
 Project-URL: Home, https://wasm.itk.org/
 Project-URL: Source, https://github.com/InsightSoftwareConsortium/itk-wasm
 Project-URL: Issues, https://github.com/InsightSoftwareConsortium/itk-wasm/issues
 Author-email: Matt McCormick <matt.mccormick@kitware.com>
 License: 
                                          Apache License
@@ -222,16 +222,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Requires-Dist: importlib-metadata; python_version < '3.10'
 Requires-Dist: numpy
 Requires-Dist: typing-extensions
 Requires-Dist: wasmtime; sys_platform != 'emscripten'
-Provides-Extra: doc
-Requires-Dist: sphinx; extra == 'doc'
 Provides-Extra: test
 Requires-Dist: itk>=5.3.0; extra == 'test'
 Requires-Dist: pytest>=2.7.3; extra == 'test'
 Description-Content-Type: text/markdown
 
 # itkwasm
```

