# Comparing `tmp/magma_suite-1.2.0.tar.gz` & `tmp/magma_suite-1.2.2.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magma_suite-1.2.0.tar", max compression
+gzip compressed data, was "magma_suite-1.2.2.1b1.tar", max compression
```

## Comparing `magma_suite-1.2.0.tar` & `magma_suite-1.2.2.1b1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1083 2022-11-09 19:30:42.423429 magma_suite-1.2.0/LICENSE.txt
--rw-r--r--   0        0        0       96 2022-11-09 19:30:42.423678 magma_suite-1.2.0/README.md
--rw-r--r--   0        0        0        1 2022-11-09 19:30:42.427395 magma_suite-1.2.0/magma/__init__.py
--rw-r--r--   0        0        0     3444 2022-11-09 19:30:42.427982 magma_suite-1.2.0/magma/checkstatus.py
--rw-r--r--   0        0        0    12922 2022-11-09 19:30:42.429424 magma_suite-1.2.0/magma/inputgenerator.py
--rw-r--r--   0        0        0    15898 2022-11-09 19:30:42.430545 magma_suite-1.2.0/magma/metawfl.py
--rw-r--r--   0        0        0     8908 2022-11-09 19:30:42.431467 magma_suite-1.2.0/magma/metawflrun.py
--rw-r--r--   0        0        0     4087 2022-11-09 19:30:42.431804 magma_suite-1.2.0/magma/runupdate.py
--rw-r--r--   0        0        0        0 2022-11-09 19:30:42.432014 magma_suite-1.2.0/magma_ff/__init__.py
--rw-r--r--   0        0        0     2391 2022-11-09 19:30:42.432269 magma_suite-1.2.0/magma_ff/checkstatus.py
--rw-r--r--   0        0        0    44324 2022-11-09 19:30:42.432731 magma_suite-1.2.0/magma_ff/create_metawfr.py
--rw-r--r--   0        0        0     6670 2022-11-09 19:30:42.433164 magma_suite-1.2.0/magma_ff/import_metawfr.py
--rw-r--r--   0        0        0     5097 2022-11-09 19:30:42.433550 magma_suite-1.2.0/magma_ff/inputgenerator.py
--rw-r--r--   0        0        0      778 2022-11-09 19:30:42.433925 magma_suite-1.2.0/magma_ff/metawfl.py
--rw-r--r--   0        0        0     3162 2022-11-09 19:30:42.434158 magma_suite-1.2.0/magma_ff/metawflrun.py
--rw-r--r--   0        0        0     5032 2022-11-09 19:30:42.434762 magma_suite-1.2.0/magma_ff/parser.py
--rw-r--r--   0        0        0     6915 2022-11-09 19:30:42.435083 magma_suite-1.2.0/magma_ff/reset_metawfr.py
--rw-r--r--   0        0        0     2465 2022-11-09 19:30:42.435425 magma_suite-1.2.0/magma_ff/run_metawfr.py
--rw-r--r--   0        0        0       30 2022-11-09 19:30:42.435778 magma_suite-1.2.0/magma_ff/runupdate.py
--rw-r--r--   0        0        0     5650 2022-11-09 19:30:42.437062 magma_suite-1.2.0/magma_ff/status_metawfr.py
--rw-r--r--   0        0        0     1398 2022-11-09 19:30:42.437504 magma_suite-1.2.0/magma_ff/update_cost_metawfr.py
--rw-r--r--   0        0        0     3021 2022-11-09 19:30:42.437935 magma_suite-1.2.0/magma_ff/utils.py
--rw-r--r--   0        0        0     4066 2022-11-09 19:30:42.438285 magma_suite-1.2.0/magma_ff/wfrutils.py
--rw-r--r--   0        0        0      854 2022-11-17 18:43:34.674950 magma_suite-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      827 1970-01-01 00:00:00.000000 magma_suite-1.2.0/setup.py
--rw-r--r--   0        0        0      892 1970-01-01 00:00:00.000000 magma_suite-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-04-17 13:06:49.055030 magma_suite-1.2.2.1b1/LICENSE.txt
+-rw-r--r--   0        0        0       96 2023-04-17 13:06:49.055168 magma_suite-1.2.2.1b1/README.md
+-rw-r--r--   0        0        0        1 2023-04-17 13:06:49.056496 magma_suite-1.2.2.1b1/magma/__init__.py
+-rw-r--r--   0        0        0     3444 2023-04-17 13:06:49.056599 magma_suite-1.2.2.1b1/magma/checkstatus.py
+-rw-r--r--   0        0        0    12922 2023-04-17 13:06:49.056747 magma_suite-1.2.2.1b1/magma/inputgenerator.py
+-rw-r--r--   0        0        0    15898 2023-04-17 13:06:49.056890 magma_suite-1.2.2.1b1/magma/metawfl.py
+-rw-r--r--   0        0        0     8908 2023-04-17 13:06:49.057016 magma_suite-1.2.2.1b1/magma/metawflrun.py
+-rw-r--r--   0        0        0     4087 2023-04-17 13:06:49.057111 magma_suite-1.2.2.1b1/magma/runupdate.py
+-rw-r--r--   0        0        0        0 2023-04-17 13:06:49.057170 magma_suite-1.2.2.1b1/magma_ff/__init__.py
+-rw-r--r--   0        0        0     2391 2023-04-17 13:06:49.057253 magma_suite-1.2.2.1b1/magma_ff/checkstatus.py
+-rw-r--r--   0        0        0    45467 2023-04-17 13:06:49.057516 magma_suite-1.2.2.1b1/magma_ff/create_metawfr.py
+-rw-r--r--   0        0        0     6670 2023-04-17 13:06:49.057654 magma_suite-1.2.2.1b1/magma_ff/import_metawfr.py
+-rw-r--r--   0        0        0     5097 2023-04-17 13:06:49.057752 magma_suite-1.2.2.1b1/magma_ff/inputgenerator.py
+-rw-r--r--   0        0        0      778 2023-04-17 13:06:49.057830 magma_suite-1.2.2.1b1/magma_ff/metawfl.py
+-rw-r--r--   0        0        0     3162 2023-04-17 13:06:49.057893 magma_suite-1.2.2.1b1/magma_ff/metawflrun.py
+-rw-r--r--   0        0        0     5032 2023-04-17 13:06:49.058001 magma_suite-1.2.2.1b1/magma_ff/parser.py
+-rw-r--r--   0        0        0     6915 2023-04-17 13:06:49.058109 magma_suite-1.2.2.1b1/magma_ff/reset_metawfr.py
+-rw-r--r--   0        0        0     2465 2023-04-17 13:06:49.058190 magma_suite-1.2.2.1b1/magma_ff/run_metawfr.py
+-rw-r--r--   0        0        0       30 2023-04-17 13:06:49.058247 magma_suite-1.2.2.1b1/magma_ff/runupdate.py
+-rw-r--r--   0        0        0     5650 2023-04-17 13:06:49.058329 magma_suite-1.2.2.1b1/magma_ff/status_metawfr.py
+-rw-r--r--   0        0        0     1398 2023-04-17 13:06:49.058411 magma_suite-1.2.2.1b1/magma_ff/update_cost_metawfr.py
+-rw-r--r--   0        0        0     3021 2023-04-17 13:06:49.058499 magma_suite-1.2.2.1b1/magma_ff/utils.py
+-rw-r--r--   0        0        0     4066 2023-04-17 13:06:49.058584 magma_suite-1.2.2.1b1/magma_ff/wfrutils.py
+-rw-r--r--   0        0        0      858 2023-04-17 13:16:36.993579 magma_suite-1.2.2.1b1/pyproject.toml
+-rw-r--r--   0        0        0      831 1970-01-01 00:00:00.000000 magma_suite-1.2.2.1b1/setup.py
+-rw-r--r--   0        0        0      896 1970-01-01 00:00:00.000000 magma_suite-1.2.2.1b1/PKG-INFO
```

### Comparing `magma_suite-1.2.0/LICENSE.txt` & `magma_suite-1.2.2.1b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `magma_suite-1.2.0/magma/checkstatus.py` & `magma_suite-1.2.2.1b1/magma/checkstatus.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.2.0/magma/inputgenerator.py` & `magma_suite-1.2.2.1b1/magma/inputgenerator.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.2.0/magma/metawfl.py` & `magma_suite-1.2.2.1b1/magma/metawfl.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.2.0/magma/metawflrun.py` & `magma_suite-1.2.2.1b1/magma/metawflrun.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.2.0/magma/runupdate.py` & `magma_suite-1.2.2.1b1/magma/runupdate.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.2.0/magma_ff/checkstatus.py` & `magma_suite-1.2.2.1b1/magma_ff/checkstatus.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.2.0/magma_ff/create_metawfr.py` & `magma_suite-1.2.2.1b1/magma_ff/create_metawfr.py`

 * *Files 5% similar despite different names*

```diff
@@ -484,41 +484,56 @@
         :return: Structured file argument input
         :rtype: dict
         :raises MetaWorkflowRunCreationError: If expected dimensions
             could not be handled or an input of dimension 1 has more
             than 1 entry per sample (i.e. is 2 dimensional)
         """
         result = []
-        for input_idx, file_input in enumerate(file_input_value):
-            if input_dimensions == 1:
-                if len(file_input) > 1:
-                    raise MetaWorkflowRunCreationError(
-                        "Found multiple input files when only 1 was expected for"
-                        " parameter %s: %s" % (file_parameter, file_input)
-                    )
-                for file_uuid in file_input:
-                    dimension = str(input_idx)
+        if input_dimensions == 1:  # List of <= 1 list expected
+            if len(file_input_value) > 1:
+                raise MetaWorkflowRunCreationError(
+                    f"Input file dimensions were greater than expected for"
+                    f" parameter {file_parameter}. Expected input dimension"
+                    f" {input_dimensions} but received input: {file_input_value}."
+                )
+            for file_input_item in file_input_value:
+                for file_idx, file_uuid in enumerate(file_input_item):
+                    if not isinstance(file_uuid, str):
+                        raise MetaWorkflowRunCreationError(
+                            f"File input for parameter {file_parameter} was unexpected."
+                            f" Exected input file dimension {input_dimensions} but"
+                            f" received the following: {file_input_value}."
+                        )
+                    dimension = str(file_idx)
                     formatted_file_result = {
                         self.FILE: file_uuid,
                         self.DIMENSION: dimension,
                     }
                     result.append(formatted_file_result)
-            elif input_dimensions == 2:
-                for file_uuid_idx, file_uuid in enumerate(file_input):
-                    dimension = "%s,%s" % (input_idx, file_uuid_idx)
+        elif input_dimensions == 2:
+            for input_idx, file_input_item in enumerate(file_input_value):
+                if not isinstance(file_input_item, list):  # List of lists expected
+                    raise MetaWorkflowRunCreationError(
+                        f"Input file dimensions were greater than expected for"
+                        f" parameter {file_parameter}. Expected input dimension"
+                        f" {input_dimensions} but received input: {file_input_value}."
+                    )
+                for file_uuid_idx, file_uuid in enumerate(file_input_item):
+                    if not isinstance(file_uuid, str):
+                        raise MetaWorkflowRunCreationError(
+                            f"File input for parameter {file_parameter} was unexpected."
+                            f" Exected input file dimension {input_dimensions} but received"
+                            f" the following: {file_input_value}."
+                        )
+                    dimension = f"{input_idx},{file_uuid_idx}"
                     formatted_file_result = {
                         self.FILE: file_uuid,
                         self.DIMENSION: dimension,
                     }
                     result.append(formatted_file_result)
-            else:
-                raise MetaWorkflowRunCreationError(
-                    "Received an unexpected dimension number for parameter %s: %s"
-                    % (file_parameter, input_dimensions)
-                )
         return result
 
     def fetch_parameters(self, parameters_to_fetch):
         """Create non-file parameters for MetaWorkflowRun[json].
 
         :param parameters_to_fetch: Non-file input parameters from
             MetaWorkflow[json]
@@ -945,15 +960,15 @@
     def fastqs_r1(self):
         """FASTQ paired-end 1 file input."""
         return self.get_property_from_samples("fastqs_r1")
 
     @property
     def fastqs_r2(self):
         """FASTQ paired-end 2 file input."""
-        return self.get_property_from_samples("fastqs_r1")
+        return self.get_property_from_samples("fastqs_r2")
 
     @property
     def input_bams(self):
         """BAM file input."""
         return self.get_property_from_samples("input_bams")
 
     @property
```

### Comparing `magma_suite-1.2.0/magma_ff/import_metawfr.py` & `magma_suite-1.2.2.1b1/magma_ff/import_metawfr.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.2.0/magma_ff/inputgenerator.py` & `magma_suite-1.2.2.1b1/magma_ff/inputgenerator.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.2.0/magma_ff/metawfl.py` & `magma_suite-1.2.2.1b1/magma_ff/metawfl.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.2.0/magma_ff/metawflrun.py` & `magma_suite-1.2.2.1b1/magma_ff/metawflrun.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.2.0/magma_ff/parser.py` & `magma_suite-1.2.2.1b1/magma_ff/parser.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.2.0/magma_ff/reset_metawfr.py` & `magma_suite-1.2.2.1b1/magma_ff/reset_metawfr.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.2.0/magma_ff/run_metawfr.py` & `magma_suite-1.2.2.1b1/magma_ff/run_metawfr.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.2.0/magma_ff/status_metawfr.py` & `magma_suite-1.2.2.1b1/magma_ff/status_metawfr.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.2.0/magma_ff/update_cost_metawfr.py` & `magma_suite-1.2.2.1b1/magma_ff/update_cost_metawfr.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.2.0/magma_ff/utils.py` & `magma_suite-1.2.2.1b1/magma_ff/utils.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.2.0/magma_ff/wfrutils.py` & `magma_suite-1.2.2.1b1/magma_ff/wfrutils.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.2.0/pyproject.toml` & `magma_suite-1.2.2.1b1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "magma-suite"
-version = "1.2.0"
+version = "1.2.2.1b1"
 description = "Collection of tools to manage meta-workflows automation."
 authors = ["Michele Berselli <berselli.michele@gmail.com>", "Doug Rioux", "Soo Lee", "CGAP team"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/dbmi-bgm/magma"
 homepage = "https://github.com/dbmi-bgm/magma"
 classifiers = [
@@ -17,15 +17,15 @@
     { include="magma" },
     { include="magma_ff" }
 ]
 
 
 [tool.poetry.dependencies]
 python = ">=3.7,<3.9"
-dcicutils = "^6.0.0"
+dcicutils = "^7.0.0"
 tibanna-ff = "^1.0.0"
 
 
 [tool.poetry.dev-dependencies]
 mock = "*"
 pytest = "*"
```

### Comparing `magma_suite-1.2.0/setup.py` & `magma_suite-1.2.2.1b1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['magma', 'magma_ff']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['dcicutils>=6.0.0,<7.0.0', 'tibanna-ff>=1.0.0,<2.0.0']
+['dcicutils>=7.0.0,<8.0.0', 'tibanna-ff>=1.0.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'magma-suite',
-    'version': '1.2.0',
+    'version': '1.2.2.1b1',
     'description': 'Collection of tools to manage meta-workflows automation.',
     'long_description': '# magma\n\n[*Documentation*](https://magma-suite.readthedocs.io/en/latest/ "magma documentation")\n',
     'author': 'Michele Berselli',
     'author_email': 'berselli.michele@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/dbmi-bgm/magma',
```

### Comparing `magma_suite-1.2.0/PKG-INFO` & `magma_suite-1.2.2.1b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: magma-suite
-Version: 1.2.0
+Version: 1.2.2.1b1
 Summary: Collection of tools to manage meta-workflows automation.
 Home-page: https://github.com/dbmi-bgm/magma
 License: MIT
 Author: Michele Berselli
 Author-email: berselli.michele@gmail.com
 Requires-Python: >=3.7,<3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3
-Requires-Dist: dcicutils (>=6.0.0,<7.0.0)
+Requires-Dist: dcicutils (>=7.0.0,<8.0.0)
 Requires-Dist: tibanna-ff (>=1.0.0,<2.0.0)
 Project-URL: Repository, https://github.com/dbmi-bgm/magma
 Description-Content-Type: text/markdown
 
 # magma
 
 [*Documentation*](https://magma-suite.readthedocs.io/en/latest/ "magma documentation")
```

