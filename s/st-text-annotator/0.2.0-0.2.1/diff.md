# Comparing `tmp/st_text_annotator-0.2.0.tar.gz` & `tmp/st_text_annotator-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_text_annotator-0.2.0.tar", max compression
+gzip compressed data, was "st_text_annotator-0.2.1.tar", max compression
```

## Comparing `st_text_annotator-0.2.0.tar` & `st_text_annotator-0.2.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1075 2023-04-14 18:30:17.965925 st_text_annotator-0.2.0/LICENSE
--rw-r--r--   0        0        0      968 2023-04-16 19:02:59.836508 st_text_annotator-0.2.0/README.md
--rw-r--r--   0        0        0      713 2023-04-17 18:50:45.551995 st_text_annotator-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2308 2023-04-16 18:16:49.394296 st_text_annotator-0.2.0/src/st_text_annotator/__init__.py
--rw-r--r--   0        0        0      180 2023-04-14 17:24:02.791373 st_text_annotator-0.2.0/src/st_text_annotator/frontend/.env
--rw-r--r--   0        0        0       67 2023-04-14 17:24:02.792164 st_text_annotator-0.2.0/src/st_text_annotator/frontend/.prettierrc
--rw-r--r--   0        0        0      961 2023-04-16 18:17:20.106557 st_text_annotator-0.2.0/src/st_text_annotator/frontend/build/asset-manifest.json
--rw-r--r--   0        0        0   197459 2023-04-16 18:17:00.578609 st_text_annotator-0.2.0/src/st_text_annotator/frontend/build/bootstrap.min.css
--rw-r--r--   0        0        0     2097 2023-04-16 18:17:20.106481 st_text_annotator-0.2.0/src/st_text_annotator/frontend/build/index.html
--rw-r--r--   0        0        0      685 2023-04-16 18:17:20.106175 st_text_annotator-0.2.0/src/st_text_annotator/frontend/build/precache-manifest.b83f8cda23e89b45d1bce2e70668eace.js
--rw-r--r--   0        0        0     1183 2023-04-16 18:17:20.106326 st_text_annotator-0.2.0/src/st_text_annotator/frontend/build/service-worker.js
--rw-r--r--   0        0        0   594301 2023-04-16 18:17:20.115612 st_text_annotator-0.2.0/src/st_text_annotator/frontend/build/static/js/2.0d16c425.chunk.js
--rw-r--r--   0        0        0     1803 2023-04-16 18:17:20.113847 st_text_annotator-0.2.0/src/st_text_annotator/frontend/build/static/js/2.0d16c425.chunk.js.LICENSE.txt
--rw-r--r--   0        0        0  1813945 2023-04-16 18:17:20.114381 st_text_annotator-0.2.0/src/st_text_annotator/frontend/build/static/js/2.0d16c425.chunk.js.map
--rw-r--r--   0        0        0    11817 2023-04-16 18:17:20.107357 st_text_annotator-0.2.0/src/st_text_annotator/frontend/build/static/js/main.185866dc.chunk.js
--rw-r--r--   0        0        0      149 2023-04-16 18:17:20.113813 st_text_annotator-0.2.0/src/st_text_annotator/frontend/build/static/js/main.185866dc.chunk.js.LICENSE.txt
--rw-r--r--   0        0        0    22913 2023-04-16 18:17:20.114480 st_text_annotator-0.2.0/src/st_text_annotator/frontend/build/static/js/main.185866dc.chunk.js.map
--rw-r--r--   0        0        0     1594 2023-04-16 18:17:20.113768 st_text_annotator-0.2.0/src/st_text_annotator/frontend/build/static/js/runtime-main.d5954658.js
--rw-r--r--   0        0        0     8307 2023-04-16 18:17:20.115460 st_text_annotator-0.2.0/src/st_text_annotator/frontend/build/static/js/runtime-main.d5954658.js.map
--rw-r--r--   0        0        0      846 2023-04-16 18:09:54.163942 st_text_annotator-0.2.0/src/st_text_annotator/frontend/package.json
--rw-r--r--   0        0        0   197459 2023-04-14 17:24:02.785648 st_text_annotator-0.2.0/src/st_text_annotator/frontend/public/bootstrap.min.css
--rw-r--r--   0        0        0      894 2023-04-14 17:24:02.786098 st_text_annotator-0.2.0/src/st_text_annotator/frontend/public/index.html
--rw-r--r--   0        0        0     7490 2023-04-14 21:49:47.302144 st_text_annotator-0.2.0/src/st_text_annotator/frontend/src/Annotation.tsx
--rw-r--r--   0        0        0     7490 2023-04-15 21:14:06.072822 st_text_annotator-0.2.0/src/st_text_annotator/frontend/src/AnnotationNew.tsx
--rw-r--r--   0        0        0      219 2023-04-15 21:23:26.959735 st_text_annotator-0.2.0/src/st_text_annotator/frontend/src/index.tsx
--rw-r--r--   0        0        0       40 2023-04-14 17:24:02.814143 st_text_annotator-0.2.0/src/st_text_annotator/frontend/src/react-app-env.d.ts
--rw-r--r--   0        0        0      459 2023-04-14 17:24:02.792820 st_text_annotator-0.2.0/src/st_text_annotator/frontend/tsconfig.json
--rw-r--r--   0        0        0     1558 1970-01-01 00:00:00.000000 st_text_annotator-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-04-14 18:30:17.965925 st_text_annotator-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1951 2023-04-17 19:03:03.350393 st_text_annotator-0.2.1/README.md
+-rw-r--r--   0        0        0      713 2023-04-17 19:10:04.090049 st_text_annotator-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2919 2023-04-17 19:03:13.656762 st_text_annotator-0.2.1/src/st_text_annotator/__init__.py
+-rw-r--r--   0        0        0      180 2023-04-14 17:24:02.791373 st_text_annotator-0.2.1/src/st_text_annotator/frontend/.env
+-rw-r--r--   0        0        0       67 2023-04-14 17:24:02.792164 st_text_annotator-0.2.1/src/st_text_annotator/frontend/.prettierrc
+-rw-r--r--   0        0        0      961 2023-04-16 18:17:20.106557 st_text_annotator-0.2.1/src/st_text_annotator/frontend/build/asset-manifest.json
+-rw-r--r--   0        0        0   197459 2023-04-16 18:17:00.578609 st_text_annotator-0.2.1/src/st_text_annotator/frontend/build/bootstrap.min.css
+-rw-r--r--   0        0        0     2097 2023-04-16 18:17:20.106481 st_text_annotator-0.2.1/src/st_text_annotator/frontend/build/index.html
+-rw-r--r--   0        0        0      685 2023-04-16 18:17:20.106175 st_text_annotator-0.2.1/src/st_text_annotator/frontend/build/precache-manifest.b83f8cda23e89b45d1bce2e70668eace.js
+-rw-r--r--   0        0        0     1183 2023-04-16 18:17:20.106326 st_text_annotator-0.2.1/src/st_text_annotator/frontend/build/service-worker.js
+-rw-r--r--   0        0        0   594301 2023-04-16 18:17:20.115612 st_text_annotator-0.2.1/src/st_text_annotator/frontend/build/static/js/2.0d16c425.chunk.js
+-rw-r--r--   0        0        0     1803 2023-04-16 18:17:20.113847 st_text_annotator-0.2.1/src/st_text_annotator/frontend/build/static/js/2.0d16c425.chunk.js.LICENSE.txt
+-rw-r--r--   0        0        0  1813945 2023-04-16 18:17:20.114381 st_text_annotator-0.2.1/src/st_text_annotator/frontend/build/static/js/2.0d16c425.chunk.js.map
+-rw-r--r--   0        0        0    11817 2023-04-16 18:17:20.107357 st_text_annotator-0.2.1/src/st_text_annotator/frontend/build/static/js/main.185866dc.chunk.js
+-rw-r--r--   0        0        0      149 2023-04-16 18:17:20.113813 st_text_annotator-0.2.1/src/st_text_annotator/frontend/build/static/js/main.185866dc.chunk.js.LICENSE.txt
+-rw-r--r--   0        0        0    22913 2023-04-16 18:17:20.114480 st_text_annotator-0.2.1/src/st_text_annotator/frontend/build/static/js/main.185866dc.chunk.js.map
+-rw-r--r--   0        0        0     1594 2023-04-16 18:17:20.113768 st_text_annotator-0.2.1/src/st_text_annotator/frontend/build/static/js/runtime-main.d5954658.js
+-rw-r--r--   0        0        0     8307 2023-04-16 18:17:20.115460 st_text_annotator-0.2.1/src/st_text_annotator/frontend/build/static/js/runtime-main.d5954658.js.map
+-rw-r--r--   0        0        0      846 2023-04-16 18:09:54.163942 st_text_annotator-0.2.1/src/st_text_annotator/frontend/package.json
+-rw-r--r--   0        0        0   197459 2023-04-14 17:24:02.785648 st_text_annotator-0.2.1/src/st_text_annotator/frontend/public/bootstrap.min.css
+-rw-r--r--   0        0        0      894 2023-04-14 17:24:02.786098 st_text_annotator-0.2.1/src/st_text_annotator/frontend/public/index.html
+-rw-r--r--   0        0        0     7490 2023-04-14 21:49:47.302144 st_text_annotator-0.2.1/src/st_text_annotator/frontend/src/Annotation.tsx
+-rw-r--r--   0        0        0     7490 2023-04-15 21:14:06.072822 st_text_annotator-0.2.1/src/st_text_annotator/frontend/src/AnnotationNew.tsx
+-rw-r--r--   0        0        0      219 2023-04-15 21:23:26.959735 st_text_annotator-0.2.1/src/st_text_annotator/frontend/src/index.tsx
+-rw-r--r--   0        0        0       40 2023-04-14 17:24:02.814143 st_text_annotator-0.2.1/src/st_text_annotator/frontend/src/react-app-env.d.ts
+-rw-r--r--   0        0        0      459 2023-04-14 17:24:02.792820 st_text_annotator-0.2.1/src/st_text_annotator/frontend/tsconfig.json
+-rw-r--r--   0        0        0     2541 1970-01-01 00:00:00.000000 st_text_annotator-0.2.1/PKG-INFO
```

### Comparing `st_text_annotator-0.2.0/LICENSE` & `st_text_annotator-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `st_text_annotator-0.2.0/pyproject.toml` & `st_text_annotator-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "st-text-annotator"
-version = "0.2.0"
+version = "0.2.1"
 description = "Component for annotating text for NLP resolution"
 classifiers = ["Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent"]
 authors = ["Robin Marquet <robin.marquet@epitech.eu>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["streamlit", "text", "annotation", "nlp"]
 include = ["./src/st_text_annotator/frontend/build/**/*"]
```

### Comparing `st_text_annotator-0.2.0/src/st_text_annotator/frontend/build/asset-manifest.json` & `st_text_annotator-0.2.1/src/st_text_annotator/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `st_text_annotator-0.2.0/src/st_text_annotator/frontend/build/bootstrap.min.css` & `st_text_annotator-0.2.1/src/st_text_annotator/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `st_text_annotator-0.2.0/src/st_text_annotator/frontend/build/index.html` & `st_text_annotator-0.2.1/src/st_text_annotator/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `st_text_annotator-0.2.0/src/st_text_annotator/frontend/build/precache-manifest.b83f8cda23e89b45d1bce2e70668eace.js` & `st_text_annotator-0.2.1/src/st_text_annotator/frontend/build/precache-manifest.b83f8cda23e89b45d1bce2e70668eace.js`

 * *Files identical despite different names*

### Comparing `st_text_annotator-0.2.0/src/st_text_annotator/frontend/build/service-worker.js` & `st_text_annotator-0.2.1/src/st_text_annotator/frontend/build/service-worker.js`

 * *Files identical despite different names*

### Comparing `st_text_annotator-0.2.0/src/st_text_annotator/frontend/build/static/js/2.0d16c425.chunk.js` & `st_text_annotator-0.2.1/src/st_text_annotator/frontend/build/static/js/2.0d16c425.chunk.js`

 * *Files identical despite different names*

### Comparing `st_text_annotator-0.2.0/src/st_text_annotator/frontend/build/static/js/2.0d16c425.chunk.js.LICENSE.txt` & `st_text_annotator-0.2.1/src/st_text_annotator/frontend/build/static/js/2.0d16c425.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `st_text_annotator-0.2.0/src/st_text_annotator/frontend/build/static/js/2.0d16c425.chunk.js.map` & `st_text_annotator-0.2.1/src/st_text_annotator/frontend/build/static/js/2.0d16c425.chunk.js.map`

 * *Files identical despite different names*

### Comparing `st_text_annotator-0.2.0/src/st_text_annotator/frontend/build/static/js/main.185866dc.chunk.js` & `st_text_annotator-0.2.1/src/st_text_annotator/frontend/build/static/js/main.185866dc.chunk.js`

 * *Files identical despite different names*

### Comparing `st_text_annotator-0.2.0/src/st_text_annotator/frontend/build/static/js/main.185866dc.chunk.js.map` & `st_text_annotator-0.2.1/src/st_text_annotator/frontend/build/static/js/main.185866dc.chunk.js.map`

 * *Files identical despite different names*

### Comparing `st_text_annotator-0.2.0/src/st_text_annotator/frontend/build/static/js/runtime-main.d5954658.js` & `st_text_annotator-0.2.1/src/st_text_annotator/frontend/build/static/js/runtime-main.d5954658.js`

 * *Files identical despite different names*

### Comparing `st_text_annotator-0.2.0/src/st_text_annotator/frontend/build/static/js/runtime-main.d5954658.js.map` & `st_text_annotator-0.2.1/src/st_text_annotator/frontend/build/static/js/runtime-main.d5954658.js.map`

 * *Files identical despite different names*

### Comparing `st_text_annotator-0.2.0/src/st_text_annotator/frontend/package.json` & `st_text_annotator-0.2.1/src/st_text_annotator/frontend/package.json`

 * *Files identical despite different names*

### Comparing `st_text_annotator-0.2.0/src/st_text_annotator/frontend/public/bootstrap.min.css` & `st_text_annotator-0.2.1/src/st_text_annotator/frontend/public/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `st_text_annotator-0.2.0/src/st_text_annotator/frontend/public/index.html` & `st_text_annotator-0.2.1/src/st_text_annotator/frontend/public/index.html`

 * *Files identical despite different names*

### Comparing `st_text_annotator-0.2.0/src/st_text_annotator/frontend/src/Annotation.tsx` & `st_text_annotator-0.2.1/src/st_text_annotator/frontend/src/Annotation.tsx`

 * *Files identical despite different names*

### Comparing `st_text_annotator-0.2.0/src/st_text_annotator/frontend/src/AnnotationNew.tsx` & `st_text_annotator-0.2.1/src/st_text_annotator/frontend/src/AnnotationNew.tsx`

 * *Files identical despite different names*

### Comparing `st_text_annotator-0.2.0/PKG-INFO` & `st_text_annotator-0.2.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,28 @@
-Metadata-Version: 2.1
-Name: st-text-annotator
-Version: 0.2.0
-Summary: Component for annotating text for NLP resolution
-License: MIT
-Keywords: streamlit,text,annotation,nlp
-Author: Robin Marquet
-Author-email: robin.marquet@epitech.eu
-Requires-Python: >=3.8,<3.9
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3
-Requires-Dist: streamlit (>=1.21.0,<2.0.0)
-Description-Content-Type: text/markdown
-
 <h1> streamlit-annotation </h1>
 
 - [Install](#install)
 - [Quick Use](#quick-use)
 - [Development](#development)
   - [Install](#install-1)
   - [Run](#run)
 - [License](#license)
 - [Author](#author)
 - [Contributors](#contributors)
 
+# Streamlit Text Annotator
+
+[![PyPI version](https://badge.fury.io/py/st-text-annotator.svg)](https://badge.fury.io/py/st-text-annotator)
+[![Downloads](https://pepy.tech/badge/st-text-annotator)](https://pepy.tech/project/st-text-annotator)
+[![Downloads](https://pepy.tech/badge/st-text-annotator/month)](https://pepy.tech/project/st-text-annotator)
+[![Downloads](https://pepy.tech/badge/st-text-annotator/week)](https://pepy.tech/project/st-text-annotator)
+
+Streamlit Text Annotator is a Streamlit component that allows you to annotate text.
+
+![](docs/example.gif)
 
 # Install
 
 ```
 pip install st-text-annotator
 ```
 
@@ -47,14 +40,45 @@
 
 Run:
 
 ```
 streamlit run example.py
 ```
 
+Output:
+
+```json
+{
+  "annotations": [
+    [
+      {
+        "start": 0,
+        "end": 5,
+        "label": "Lorem"
+      },
+      {
+        "start": 12,
+        "end": 26,
+        "label": "dolor sit amet"
+      },
+      {
+        "start": 130,
+        "end": 148,
+        "label": "Curabitur lobortis"
+      },
+      {
+        "start": 309,
+        "end": 319,
+        "label": "nec turpis"
+      }
+    ]
+  ]
+}
+```
+
 # Development
 
 ## Install
 
 ```
 git clone git@github.com:rmarquet21/streamlit-text-annotator.git
 cd streamlit-text-annotator
@@ -75,8 +99,7 @@
 
 Robin Marquet
 
 # Contributors
 
 - [Robin Marquet](robin.marquet3@gmail.com)
 
-
```

