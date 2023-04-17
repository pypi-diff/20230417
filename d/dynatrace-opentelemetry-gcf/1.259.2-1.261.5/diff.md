# Comparing `tmp/dynatrace_opentelemetry_gcf-1.259.2-py3-none-any.whl.zip` & `tmp/dynatrace_opentelemetry_gcf-1.261.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 12112 bytes, number of entries: 10
+Zip file size: 12130 bytes, number of entries: 10
 -rw-r--r--  2.0 unx      675 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/gcf/__init__.py
 -rw-r--r--  2.0 unx     4834 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/gcf/_resource.py
--rw-r--r--  2.0 unx     6804 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/gcf/_trigger.py
+-rw-r--r--  2.0 unx     6846 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/gcf/_trigger.py
 -rw-r--r--  2.0 unx     1938 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/gcf/_wrapper.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/gcf/py.typed
 -rw-r--r--  2.0 unx       24 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/gcf/version.py
-?rw-r--r--  2.0 unx     1138 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_gcf-1.259.2.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_gcf-1.259.2.dist-info/WHEEL
-?rw-r--r--  2.0 unx    11342 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_gcf-1.259.2.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      959 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_gcf-1.259.2.dist-info/RECORD
-10 files, 27801 bytes uncompressed, 10430 bytes compressed:  62.5%
+?rw-r--r--  2.0 unx     1189 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_gcf-1.261.5.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_gcf-1.261.5.dist-info/WHEEL
+?rw-r--r--  2.0 unx    11342 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_gcf-1.261.5.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      959 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_gcf-1.261.5.dist-info/RECORD
+10 files, 27894 bytes uncompressed, 10448 bytes compressed:  62.5%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: dynatrace/opentelemetry/gcf/py.typed
 Comment: 
 
 Filename: dynatrace/opentelemetry/gcf/version.py
 Comment: 
 
-Filename: dynatrace_opentelemetry_gcf-1.259.2.dist-info/METADATA
+Filename: dynatrace_opentelemetry_gcf-1.261.5.dist-info/METADATA
 Comment: 
 
-Filename: dynatrace_opentelemetry_gcf-1.259.2.dist-info/WHEEL
+Filename: dynatrace_opentelemetry_gcf-1.261.5.dist-info/WHEEL
 Comment: 
 
-Filename: dynatrace_opentelemetry_gcf-1.259.2.dist-info/licenses/LICENSE
+Filename: dynatrace_opentelemetry_gcf-1.261.5.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: dynatrace_opentelemetry_gcf-1.259.2.dist-info/RECORD
+Filename: dynatrace_opentelemetry_gcf-1.261.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dynatrace/opentelemetry/gcf/_trigger.py

```diff
@@ -74,15 +74,15 @@
             parent_context,
             api_trace.SpanKind.SERVER,
             attributes=attrs,
             record_exception=False,
             set_status_on_exception=False,
             end_on_exit=True,
         )
-        span = activation.__enter__()
+        span = activation.__enter__()  # pylint:disable=unnecessary-dunder-call
         try:
             yield span
         except Exception as ex:  # pylint:disable=broad-except
             record_exception(span, ex)
             span.set_status(Status(StatusCode.ERROR))
             raise ex
         finally:
```

## dynatrace/opentelemetry/gcf/version.py

```diff
@@ -1 +1 @@
-__version__ = "1.259.2"
+__version__ = "1.261.5"
```

## Comparing `dynatrace_opentelemetry_gcf-1.259.2.dist-info/METADATA` & `dynatrace_opentelemetry_gcf-1.261.5.dist-info/METADATA`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: dynatrace-opentelemetry-gcf
-Version: 1.259.2
+Version: 1.261.5
 Summary: Dynatrace OpenTelemetry package for Google Cloud Functions
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
-Requires-Dist: dynatrace-opentelemetry-core==1.259.2
+Requires-Dist: dynatrace-opentelemetry-core==1.261.5
 Requires-Dist: flask<3.0,>=1.0
 Requires-Dist: opentelemetry-api~=1.3
 Provides-Extra: test
 Description-Content-Type: text/markdown
 
 # Dynatrace OpenTelemetry Tracing API For Python Google Cloud Functions
```

## Comparing `dynatrace_opentelemetry_gcf-1.259.2.dist-info/licenses/LICENSE` & `dynatrace_opentelemetry_gcf-1.261.5.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `dynatrace_opentelemetry_gcf-1.259.2.dist-info/RECORD` & `dynatrace_opentelemetry_gcf-1.261.5.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dynatrace/opentelemetry/gcf/__init__.py,sha256=pVCQ15ocBp7DACT2JC5wmLkyVRbeSqpF5nWkbypokL8,675
 dynatrace/opentelemetry/gcf/_resource.py,sha256=u2eY520ADxlgDir0OoapHkIf1Y9HdR-qSxxkcPkIV4I,4834
-dynatrace/opentelemetry/gcf/_trigger.py,sha256=3k0AL-4qKPK4na0Vp7tUU2ypxRmpBKW1kJpc1INXzRo,6804
+dynatrace/opentelemetry/gcf/_trigger.py,sha256=uDAF-PMwrexrfHGsM3v4yRMaj5OZRb5ClRzZ61f39AQ,6846
 dynatrace/opentelemetry/gcf/_wrapper.py,sha256=aigZlgBBlF2Sxsd04xmzSr5nm3-rM61B0y4ttk_3r0c,1938
 dynatrace/opentelemetry/gcf/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-dynatrace/opentelemetry/gcf/version.py,sha256=SBdDekiDRkI5T1WDPV4mAP6c_uyiSUP47xyIc9KwQ8E,24
-dynatrace_opentelemetry_gcf-1.259.2.dist-info/METADATA,sha256=fJL9rodstoSO4YYlMZzfzEyc3waLQko0OJfPpbS45kw,1138
-dynatrace_opentelemetry_gcf-1.259.2.dist-info/WHEEL,sha256=hKi7AIIx6qfnsRbr087vpeJnrVUuDokDHZacPPMW7-Y,87
-dynatrace_opentelemetry_gcf-1.259.2.dist-info/licenses/LICENSE,sha256=OUyLShRPZFGLXlxbnRr7Of_8mNYYQ_qda632uhGSIaY,11342
-dynatrace_opentelemetry_gcf-1.259.2.dist-info/RECORD,,
+dynatrace/opentelemetry/gcf/version.py,sha256=NQ0eAYSOBsMOXSK1dzrH_39hr_4a48telBH4Q9YPif4,24
+dynatrace_opentelemetry_gcf-1.261.5.dist-info/METADATA,sha256=S6WH3f6vLWPo8LyYYHn2plSgd4NwdSeJiZFx1jtgWvs,1189
+dynatrace_opentelemetry_gcf-1.261.5.dist-info/WHEEL,sha256=Fd6mP6ydyRguakwUJ05oBE7fh2IPxgtDN9IwHJ9OqJQ,87
+dynatrace_opentelemetry_gcf-1.261.5.dist-info/licenses/LICENSE,sha256=OUyLShRPZFGLXlxbnRr7Of_8mNYYQ_qda632uhGSIaY,11342
+dynatrace_opentelemetry_gcf-1.261.5.dist-info/RECORD,,
```

