# Comparing `tmp/dynatrace_opentelemetry_azure_functions-1.259.2-py3-none-any.whl.zip` & `tmp/dynatrace_opentelemetry_azure_functions-1.261.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 15104 bytes, number of entries: 11
+Zip file size: 15107 bytes, number of entries: 11
 -rw-r--r--  2.0 unx      687 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/azure/functions/__init__.py
 -rw-r--r--  2.0 unx     3948 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/azure/functions/_bindings.py
 -rw-r--r--  2.0 unx     3563 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/azure/functions/_resource.py
 -rw-r--r--  2.0 unx     6768 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/azure/functions/_triggers.py
 -rw-r--r--  2.0 unx     8183 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/azure/functions/_wrapper.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/azure/functions/py.typed
 -rw-r--r--  2.0 unx       24 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/azure/functions/version.py
-?rw-r--r--  2.0 unx     1171 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_azure_functions-1.259.2.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_azure_functions-1.259.2.dist-info/WHEEL
-?rw-r--r--  2.0 unx    11342 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_azure_functions-1.259.2.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx     1189 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_azure_functions-1.259.2.dist-info/RECORD
-11 files, 36962 bytes uncompressed, 13000 bytes compressed:  64.8%
+?rw-r--r--  2.0 unx     1222 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_azure_functions-1.261.5.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_azure_functions-1.261.5.dist-info/WHEEL
+?rw-r--r--  2.0 unx    11342 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_azure_functions-1.261.5.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx     1189 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_azure_functions-1.261.5.dist-info/RECORD
+11 files, 37013 bytes uncompressed, 13003 bytes compressed:  64.9%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: dynatrace/opentelemetry/azure/functions/py.typed
 Comment: 
 
 Filename: dynatrace/opentelemetry/azure/functions/version.py
 Comment: 
 
-Filename: dynatrace_opentelemetry_azure_functions-1.259.2.dist-info/METADATA
+Filename: dynatrace_opentelemetry_azure_functions-1.261.5.dist-info/METADATA
 Comment: 
 
-Filename: dynatrace_opentelemetry_azure_functions-1.259.2.dist-info/WHEEL
+Filename: dynatrace_opentelemetry_azure_functions-1.261.5.dist-info/WHEEL
 Comment: 
 
-Filename: dynatrace_opentelemetry_azure_functions-1.259.2.dist-info/licenses/LICENSE
+Filename: dynatrace_opentelemetry_azure_functions-1.261.5.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: dynatrace_opentelemetry_azure_functions-1.259.2.dist-info/RECORD
+Filename: dynatrace_opentelemetry_azure_functions-1.261.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dynatrace/opentelemetry/azure/functions/version.py

```diff
@@ -1 +1 @@
-__version__ = "1.259.2"
+__version__ = "1.261.5"
```

## Comparing `dynatrace_opentelemetry_azure_functions-1.259.2.dist-info/METADATA` & `dynatrace_opentelemetry_azure_functions-1.261.5.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: dynatrace-opentelemetry-azure-functions
-Version: 1.259.2
+Version: 1.261.5
 Summary: Dynatrace OpenTelemetry package for Azure Functions
 Project-URL: Homepage, https://www.dynatrace.com/technologies/python-monitoring/
 Author: Dynatrace
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Requires-Dist: azure-functions>=1.0
-Requires-Dist: dynatrace-opentelemetry-core==1.259.2
+Requires-Dist: dynatrace-opentelemetry-core==1.261.5
 Requires-Dist: opentelemetry-api~=1.3
 Requires-Dist: wrapt<2,>=1.10
 Provides-Extra: test
 Description-Content-Type: text/markdown
 
 # Dynatrace OpenTelemetry Tracing API For Python Azure Functions
```

## Comparing `dynatrace_opentelemetry_azure_functions-1.259.2.dist-info/licenses/LICENSE` & `dynatrace_opentelemetry_azure_functions-1.261.5.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

