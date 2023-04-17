# Comparing `tmp/propertysync-0.3.0.tar.gz` & `tmp/propertysync-0.4.0.tar.gz`

## Comparing `propertysync-0.3.0.tar` & `propertysync-0.4.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 propertysync-0.3.0/CHANGELOG.md
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 propertysync-0.3.0/propertysync/__about__.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 propertysync-0.3.0/propertysync/__init__.py
--rw-r--r--   0        0        0    14818 2020-02-02 00:00:00.000000 propertysync-0.3.0/propertysync/api.py
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 propertysync-0.3.0/propertysync/batch.py
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 propertysync-0.3.0/propertysync/document.py
--rw-r--r--   0        0        0     5786 2020-02-02 00:00:00.000000 propertysync-0.3.0/propertysync/search.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 propertysync-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 propertysync-0.3.0/.gitignore
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 propertysync-0.3.0/LICENSE
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 propertysync-0.3.0/README.md
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 propertysync-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 propertysync-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 propertysync-0.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 propertysync-0.4.0/propertysync/__about__.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 propertysync-0.4.0/propertysync/__init__.py
+-rw-r--r--   0        0        0    14818 2020-02-02 00:00:00.000000 propertysync-0.4.0/propertysync/api.py
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 propertysync-0.4.0/propertysync/batch.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 propertysync-0.4.0/propertysync/document.py
+-rw-r--r--   0        0        0     5786 2020-02-02 00:00:00.000000 propertysync-0.4.0/propertysync/search.py
+-rw-r--r--   0        0        0    15625 2020-02-02 00:00:00.000000 propertysync-0.4.0/propertysync/titlesearch_batch.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 propertysync-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 propertysync-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 propertysync-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 propertysync-0.4.0/README.md
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 propertysync-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 propertysync-0.4.0/PKG-INFO
```

### Comparing `propertysync-0.3.0/CHANGELOG.md` & `propertysync-0.4.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,19 @@
 ## [Unreleased]
 
 ### Added
 ### Fixed
 ### Changed
 ### Removed
 
+## [0.4.0] - 2023-04-26
+
+### Added
+- Added TitleSearchBatch helper to convert from titlesearch format to batch format
+
 ## [0.3.0] - 2023-04-26
 
 ### Added
 - Added support to document and batch classes to support find and replace
 
 ## [0.2.1] - 2023-04-26
```

### Comparing `propertysync-0.3.0/propertysync/api.py` & `propertysync-0.4.0/propertysync/api.py`

 * *Files identical despite different names*

### Comparing `propertysync-0.3.0/propertysync/batch.py` & `propertysync-0.4.0/propertysync/batch.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 import json
+from .titlesearch_batch import TitleSearchBatch
 from .document import Document
 
 """
 This is a helper class for working with PropertySync batches.
 """
 
 class Batch:
     
     def __init__(self, json_string=None):
+        self.load(json_string)
+    
+    def load(self, json_string):  
         self.documents = []
-        self._json = json_string
+        self._json = {}
+
+        if json_string:
+            self._json = json_string
 
         if "id" in self._json:
             self.id = self._json["id"]
         else:
-            self.id = None        
+            self.id = None  
 
-        for doc in self._json["documents"]:
-            self.documents.append(Document(doc))
+        if "documents" in self._json:
+            for doc in self._json["documents"]:
+                self.documents.append(Document(doc))
 
     # serialize the doc to json
     def __str__(self):
         return json.dumps(self._json, indent=4)
     
     def __len__(self):
         return len(self.documents)
@@ -35,14 +43,19 @@
     def documents_without_tags(self, tags):
         return [doc for doc in self.documents if not set(tags).issubset(set(doc.tags))]
     
     # get documents with a specific instrumentType value
     def documents_with_instrument_type(self, instrument_type):
         return [doc for doc in self.documents if doc.instrumentType == instrument_type]
     
+    # load a batch from a titlesearch batch file
+    def load_from_titlesearch_batch(self, titlesearch_batch_file):
+        ts_batch = TitleSearchBatch(titlesearch_batch_file)
+        self.load(ts_batch.get_json())
+    
     # get all of the instrumentNumbers for a given instrumentType, or all instrumentNumbers if no instrumentType is specified
     def instrument_numbers(self, instrument_type_filter = None):
         if instrument_type_filter:
             return [doc.instrumentNumber for doc in self.documents if doc.instrumentType == instrument_type_filter]
         else:
             return [doc.instrumentNumber for doc in self.documents]
```

### Comparing `propertysync-0.3.0/propertysync/document.py` & `propertysync-0.4.0/propertysync/document.py`

 * *Files identical despite different names*

### Comparing `propertysync-0.3.0/propertysync/search.py` & `propertysync-0.4.0/propertysync/search.py`

 * *Files identical despite different names*

### Comparing `propertysync-0.3.0/LICENSE` & `propertysync-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `propertysync-0.3.0/README.md` & `propertysync-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `propertysync-0.3.0/pyproject.toml` & `propertysync-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `propertysync-0.3.0/PKG-INFO` & `propertysync-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propertysync
-Version: 0.3.0
+Version: 0.4.0
 Summary: A package for interacting with the PropertySync API.
 Project-URL: Documentation, https://developer.propertysync.com/python/index.html
 Author-email: Rob Martinson <rob@limelyte.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

