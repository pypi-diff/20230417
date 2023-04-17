# Comparing `tmp/apis_highlighter-1.0.2.tar.gz` & `tmp/apis_highlighter-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apis_highlighter-1.0.2.tar", max compression
+gzip compressed data, was "apis_highlighter-1.0.3.tar", max compression
```

## Comparing `apis_highlighter-1.0.2.tar` & `apis_highlighter-1.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1141 2023-04-04 12:32:39.440886 apis_highlighter-1.0.2/LICENSE
--rw-r--r--   0        0        0       22 2023-04-04 12:33:12.536939 apis_highlighter-1.0.2/apis_highlighter/__init__.py
--rw-r--r--   0        0        0     2454 2023-04-04 12:32:39.440886 apis_highlighter-1.0.2/apis_highlighter/active_learning.py
--rw-r--r--   0        0        0      253 2023-04-04 12:32:39.440886 apis_highlighter-1.0.2/apis_highlighter/admin.py
--rw-r--r--   0        0        0     6847 2023-04-04 12:32:39.440886 apis_highlighter-1.0.2/apis_highlighter/api_views.py
--rw-r--r--   0        0        0      106 2023-04-04 12:32:39.440886 apis_highlighter-1.0.2/apis_highlighter/apps.py
--rw-r--r--   0        0        0    13732 2023-04-04 12:32:39.440886 apis_highlighter-1.0.2/apis_highlighter/forms.py
--rw-r--r--   0        0        0     9432 2023-04-04 12:32:39.440886 apis_highlighter-1.0.2/apis_highlighter/highlighter.py
--rw-r--r--   0        0        0     5943 2023-04-04 12:32:39.440886 apis_highlighter-1.0.2/apis_highlighter/migrations/0001_initial.py
--rw-r--r--   0        0        0     1589 2023-04-04 12:32:39.440886 apis_highlighter-1.0.2/apis_highlighter/migrations/0002_auto_20200121_1227.py
--rw-r--r--   0        0        0      411 2023-04-04 12:32:39.440886 apis_highlighter-1.0.2/apis_highlighter/migrations/0003_annotationproject_published.py
--rw-r--r--   0        0        0      768 2023-04-04 12:32:39.440886 apis_highlighter-1.0.2/apis_highlighter/migrations/0004_auto_20210623_2124.py
--rw-r--r--   0        0        0      347 2023-04-04 12:32:39.440886 apis_highlighter-1.0.2/apis_highlighter/migrations/0005_remove_annotation_entity_link.py
--rw-r--r--   0        0        0      444 2023-04-04 12:32:39.440886 apis_highlighter-1.0.2/apis_highlighter/migrations/0006_auto_20221012_1446.py
--rw-r--r--   0        0        0        0 2023-04-04 12:32:39.440886 apis_highlighter-1.0.2/apis_highlighter/migrations/__init__.py
--rw-r--r--   0        0        0    13807 2023-04-04 12:32:39.440886 apis_highlighter-1.0.2/apis_highlighter/models.py
--rw-r--r--   0        0        0     2779 2023-04-04 12:32:39.440886 apis_highlighter-1.0.2/apis_highlighter/serializer.py
--rw-r--r--   0        0        0     2060 2023-04-04 12:32:39.440886 apis_highlighter-1.0.2/apis_highlighter/static/apis_highlighter/apis_highlighter.css
--rw-r--r--   0        0        0    16734 2023-04-04 12:32:39.440886 apis_highlighter-1.0.2/apis_highlighter/static/apis_highlighter/apis_highlighter.js
--rw-r--r--   0        0        0      687 2023-04-04 12:32:39.440886 apis_highlighter-1.0.2/apis_highlighter/templates/apis_highlighter/calculate_agreement.html
--rw-r--r--   0        0        0    47602 2023-04-04 12:32:39.440886 apis_highlighter-1.0.2/apis_highlighter/tests.py
--rw-r--r--   0        0        0      333 2023-04-04 12:32:39.440886 apis_highlighter-1.0.2/apis_highlighter/urls.py
--rw-r--r--   0        0        0     2857 2023-04-04 12:32:39.440886 apis_highlighter-1.0.2/apis_highlighter/views.py
--rw-r--r--   0        0        0      365 2023-04-04 12:33:12.448939 apis_highlighter-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      561 1970-01-01 00:00:00.000000 apis_highlighter-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1141 2023-04-17 10:41:20.579160 apis_highlighter-1.0.3/LICENSE
+-rw-r--r--   0        0        0       22 2023-04-17 10:41:49.703935 apis_highlighter-1.0.3/apis_highlighter/__init__.py
+-rw-r--r--   0        0        0     2454 2023-04-17 10:41:20.579160 apis_highlighter-1.0.3/apis_highlighter/active_learning.py
+-rw-r--r--   0        0        0      253 2023-04-17 10:41:20.579160 apis_highlighter-1.0.3/apis_highlighter/admin.py
+-rw-r--r--   0        0        0     6847 2023-04-17 10:41:20.579160 apis_highlighter-1.0.3/apis_highlighter/api_views.py
+-rw-r--r--   0        0        0      106 2023-04-17 10:41:20.579160 apis_highlighter-1.0.3/apis_highlighter/apps.py
+-rw-r--r--   0        0        0    13732 2023-04-17 10:41:20.579160 apis_highlighter-1.0.3/apis_highlighter/forms.py
+-rw-r--r--   0        0        0     9432 2023-04-17 10:41:20.579160 apis_highlighter-1.0.3/apis_highlighter/highlighter.py
+-rw-r--r--   0        0        0     5943 2023-04-17 10:41:20.579160 apis_highlighter-1.0.3/apis_highlighter/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1589 2023-04-17 10:41:20.579160 apis_highlighter-1.0.3/apis_highlighter/migrations/0002_auto_20200121_1227.py
+-rw-r--r--   0        0        0      411 2023-04-17 10:41:20.579160 apis_highlighter-1.0.3/apis_highlighter/migrations/0003_annotationproject_published.py
+-rw-r--r--   0        0        0      768 2023-04-17 10:41:20.579160 apis_highlighter-1.0.3/apis_highlighter/migrations/0004_auto_20210623_2124.py
+-rw-r--r--   0        0        0      347 2023-04-17 10:41:20.579160 apis_highlighter-1.0.3/apis_highlighter/migrations/0005_remove_annotation_entity_link.py
+-rw-r--r--   0        0        0      444 2023-04-17 10:41:20.579160 apis_highlighter-1.0.3/apis_highlighter/migrations/0006_auto_20221012_1446.py
+-rw-r--r--   0        0        0        0 2023-04-17 10:41:20.579160 apis_highlighter-1.0.3/apis_highlighter/migrations/__init__.py
+-rw-r--r--   0        0        0    13807 2023-04-17 10:41:20.579160 apis_highlighter-1.0.3/apis_highlighter/models.py
+-rw-r--r--   0        0        0     2779 2023-04-17 10:41:20.579160 apis_highlighter-1.0.3/apis_highlighter/serializer.py
+-rw-r--r--   0        0        0     2060 2023-04-17 10:41:20.579160 apis_highlighter-1.0.3/apis_highlighter/static/apis_highlighter/apis_highlighter.css
+-rw-r--r--   0        0        0    16734 2023-04-17 10:41:20.579160 apis_highlighter-1.0.3/apis_highlighter/static/apis_highlighter/apis_highlighter.js
+-rw-r--r--   0        0        0      687 2023-04-17 10:41:20.579160 apis_highlighter-1.0.3/apis_highlighter/templates/apis_highlighter/calculate_agreement.html
+-rw-r--r--   0        0        0    47602 2023-04-17 10:41:20.579160 apis_highlighter-1.0.3/apis_highlighter/tests.py
+-rw-r--r--   0        0        0      330 2023-04-17 10:41:20.579160 apis_highlighter-1.0.3/apis_highlighter/urls.py
+-rw-r--r--   0        0        0     2857 2023-04-17 10:41:20.583160 apis_highlighter-1.0.3/apis_highlighter/views.py
+-rw-r--r--   0        0        0      342 2023-04-17 10:41:49.643934 apis_highlighter-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0      576 1970-01-01 00:00:00.000000 apis_highlighter-1.0.3/PKG-INFO
```

### Comparing `apis_highlighter-1.0.2/LICENSE` & `apis_highlighter-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `apis_highlighter-1.0.2/apis_highlighter/active_learning.py` & `apis_highlighter-1.0.3/apis_highlighter/active_learning.py`

 * *Files identical despite different names*

### Comparing `apis_highlighter-1.0.2/apis_highlighter/api_views.py` & `apis_highlighter-1.0.3/apis_highlighter/api_views.py`

 * *Files identical despite different names*

### Comparing `apis_highlighter-1.0.2/apis_highlighter/forms.py` & `apis_highlighter-1.0.3/apis_highlighter/forms.py`

 * *Files identical despite different names*

### Comparing `apis_highlighter-1.0.2/apis_highlighter/highlighter.py` & `apis_highlighter-1.0.3/apis_highlighter/highlighter.py`

 * *Files identical despite different names*

### Comparing `apis_highlighter-1.0.2/apis_highlighter/migrations/0001_initial.py` & `apis_highlighter-1.0.3/apis_highlighter/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `apis_highlighter-1.0.2/apis_highlighter/migrations/0002_auto_20200121_1227.py` & `apis_highlighter-1.0.3/apis_highlighter/migrations/0002_auto_20200121_1227.py`

 * *Files identical despite different names*

### Comparing `apis_highlighter-1.0.2/apis_highlighter/migrations/0004_auto_20210623_2124.py` & `apis_highlighter-1.0.3/apis_highlighter/migrations/0004_auto_20210623_2124.py`

 * *Files identical despite different names*

### Comparing `apis_highlighter-1.0.2/apis_highlighter/models.py` & `apis_highlighter-1.0.3/apis_highlighter/models.py`

 * *Files identical despite different names*

### Comparing `apis_highlighter-1.0.2/apis_highlighter/serializer.py` & `apis_highlighter-1.0.3/apis_highlighter/serializer.py`

 * *Files identical despite different names*

### Comparing `apis_highlighter-1.0.2/apis_highlighter/static/apis_highlighter/apis_highlighter.css` & `apis_highlighter-1.0.3/apis_highlighter/static/apis_highlighter/apis_highlighter.css`

 * *Files identical despite different names*

### Comparing `apis_highlighter-1.0.2/apis_highlighter/static/apis_highlighter/apis_highlighter.js` & `apis_highlighter-1.0.3/apis_highlighter/static/apis_highlighter/apis_highlighter.js`

 * *Files identical despite different names*

### Comparing `apis_highlighter-1.0.2/apis_highlighter/templates/apis_highlighter/calculate_agreement.html` & `apis_highlighter-1.0.3/apis_highlighter/templates/apis_highlighter/calculate_agreement.html`

 * *Files identical despite different names*

### Comparing `apis_highlighter-1.0.2/apis_highlighter/tests.py` & `apis_highlighter-1.0.3/apis_highlighter/tests.py`

 * *Files identical despite different names*

### Comparing `apis_highlighter-1.0.2/apis_highlighter/views.py` & `apis_highlighter-1.0.3/apis_highlighter/views.py`

 * *Files identical despite different names*

### Comparing `apis_highlighter-1.0.2/PKG-INFO` & `apis_highlighter-1.0.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: apis-highlighter
-Version: 1.0.2
+Version: 1.0.3
 Summary: Highlighter module for annotations in APIS framework
 License: MIT
 Author: Matthias Schlögl
 Author-email: m.schloegl@gmail.com
-Requires-Python: >=3.7,<3.11
+Requires-Python: >=3.7,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: apis-core (>=0.16.0)
+Classifier: Programming Language :: Python :: 3.11
```

