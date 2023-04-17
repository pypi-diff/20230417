# Comparing `tmp/gt_defect_dojo-0.0.1.tar.gz` & `tmp/gt_defect_dojo-0.0.2.tar.gz`

## Comparing `gt_defect_dojo-0.0.1.tar` & `gt_defect_dojo-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0    18487 2020-02-02 00:00:00.000000 gt_defect_dojo-0.0.1/examples/upload-defectdojo.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 gt_defect_dojo-0.0.1/src/gt_defectdojo_api/__init__.py
--rw-r--r--   0        0        0    51285 2020-02-02 00:00:00.000000 gt_defect_dojo-0.0.1/src/gt_defectdojo_api/defectdojo_apiv2.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 gt_defect_dojo-0.0.1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 gt_defect_dojo-0.0.1/LICENSE
--rw-r--r--   0        0        0     2685 2020-02-02 00:00:00.000000 gt_defect_dojo-0.0.1/README.md
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 gt_defect_dojo-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     4440 2020-02-02 00:00:00.000000 gt_defect_dojo-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0  1384669 2020-02-02 00:00:00.000000 gt_defect_dojo-0.0.2/examples/dependency-check-report.xml
+-rw-r--r--   0        0        0    17616 2020-02-02 00:00:00.000000 gt_defect_dojo-0.0.2/examples/upload-defectdojo.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gt_defect_dojo-0.0.2/src/gt_defectdojo_api/__init__.py
+-rw-r--r--   0        0        0    51287 2020-02-02 00:00:00.000000 gt_defect_dojo-0.0.2/src/gt_defectdojo_api/defectdojo_apiv2.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 gt_defect_dojo-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 gt_defect_dojo-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 gt_defect_dojo-0.0.2/README.md
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 gt_defect_dojo-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 gt_defect_dojo-0.0.2/PKG-INFO
```

### Comparing `gt_defect_dojo-0.0.1/examples/upload-defectdojo.py` & `gt_defect_dojo-0.0.2/examples/upload-defectdojo.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/local/bin/python
 """
 Example written by Aaron Weaver <aaron.weaver@owasp.org>
 as part of the OWASP DefectDojo and OWASP AppSec Pipeline Security projects
 
 Description: CI/CD example for DefectDojo
 """
-from defectdojo_api import defectdojo_apiv2 as defectdojo
+import defectdojo_apiv2 as defectdojo
 from datetime import datetime, timedelta
 import os, sys
 import argparse
 import time
 
 import requests.packages.urllib3
 
@@ -56,15 +56,15 @@
         return user_id
     else:
         raise ValueError('user not found: ' + str(user_name))
 
 
 def get_product_id(dd, product_id, product_name):
     if product_id is not None:
-        product = dd.get_product(product_id)
+        dd.get_product(product_id)
         return product_id
     elif product_name is not None:
         # filtering on name was added at some point
         products_response = dd.list_products(name=product_name)
         prod_list = []
         for product in products_response.data["results"]:
             if product["name"] == product_name:
@@ -77,26 +77,22 @@
         print('\n'.join(map(str, prod_list)))
         raise ValueError('no product found with product_name ' + product_name)
     else:
         raise ValueError('product_id or product_name required')
 
 def get_engagement_id(dd, product_id, user_id, engagement_id, engagement_name, branch_name, build_id=None, build_url=None, commit_hash=None):
     if engagement_id != None:
-        engagement = dd.get_engagement(engagement_id = engagement_id)
+        dd.get_engagement(engagement_id = engagement_id)
         return engagement_id
     elif engagement_name != None:
-        engagement_name_plus_branch = engagement_name
-        if branch_name is not None:
-            # engagement_name_plus_branch = engagement_name + " (" + branch_name + ")"
-            # filtering on name was added at some point
-            engagements_reponse = dd.list_engagements(product_id=product_id, status="In Progress", name=engagement_name)
-            for engagement in engagements_reponse.data["results"]:
-                # print(engagement["name"])
-                if engagement["name"] == engagement_name:
-                    return engagement["id"]
+        engagements_reponse = dd.list_engagements(product_id=product_id, name=engagement_name)
+        for engagement in engagements_reponse.data["results"]:
+            print(engagement["name"])
+            if engagement["name"] == engagement_name:
+                return engagement["id"]
     else:
         raise ValueError('engagement id or name required')
 
 # no engagement found by id or by name, so create a new one
 
     # end_date == last upload
     start_date = datetime.now()
@@ -108,27 +104,17 @@
         engagement_description += " for " + build_url
 
     engagement_id = dd.create_engagement(engagement_name_plus_branch, product_id, str(user_id),
     "In Progress", start_date.strftime("%Y-%m-%d"), end_date.strftime("%Y-%m-%d"), branch_tag=branch_name, description=engagement_description, build_id=build_id, commit_hash=commit_hash)
     return str(engagement_id.data["id"])
 
 def get_test_id(dd, engagement_id, test_type):
-    # find latest test in engagement with the same scan_type / test_type
-    # TODO check ordering?
-    # TODO search by test_type (doesn't work for some reason currently)
-    # existing_tests = dd.list_tests(engagement_id, test_type, limit=5)
     existing_tests = dd.list_tests(engagement_id)
 
-
-    # print('existing_tests: ' + str(existing_tests))
-    # print('existing_tests.data: ' + str(existing_tests.data))
-    # print('existing_tests.data["count"]: ' + str(existing_tests.data['count']))
-    # print('existing_tests.data["results"]: ' + str(existing_tests.data['results']))
     for test in existing_tests.data["results"]:
-        print(test["test_type"])
         if test["test_type_name"] == test_type:
             return test["id"]
 
     return None
 
 
 def process_findings(dd, engagement_id, dir, build_id=None, auto_group_by=None):
@@ -375,14 +361,15 @@
             user_id=1
 
             product_id = get_product_id(dd, product_id, product_name)
             if debug:
                 print('product_id derived from paramaters: ', str(product_id))
 
             engagement_id = get_engagement_id(dd, product_id, user_id, engagement_id, engagement_name, branch_name, build_id=build_id, build_url=build_url, commit_hash=commit_hash)
+            
             if debug:
                 print('engagement_id derived from paramaters: ', str(engagement_id))
 
             test_ids = None
             if file is not None:
                 if scanner is not None:
                     test_ids = processFiles(dd, engagement_id, file, active, verified, close_old_findings, skip_duplicates, scanner=scanner, version=version, branch_tag=branch_name, commit_hash=commit_hash, build=build_id, auto_group_by=auto_group_by)
```

### Comparing `gt_defect_dojo-0.0.1/src/gt_defectdojo_api/defectdojo_apiv2.py` & `gt_defect_dojo-0.0.2/src/gt_defectdojo_api/defectdojo_apiv2.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,15 @@
             'username': username,
             'password': password
         }
         return self._request('POST', 'api-token-auth/', data=data)
 
 
     ###### Engagements API #######
-    def list_engagements(self, status=None, product_id=None, name_contains=None, name=None, limit=20, offset=0, related_fields=False):
+    def list_engagements(self, status=None, product_id=None, name_contains=None, name=None, limit=1000, offset=0, related_fields=False):
         """Retrieves all the engagements.
 
         :param product_in: List of product ids (1,2).
         :param name_contains: Engagement name
         :param limit: Number of records to return.
         :param offset: The initial index from which to return the result
```

### Comparing `gt_defect_dojo-0.0.1/.gitignore` & `gt_defect_dojo-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `gt_defect_dojo-0.0.1/LICENSE` & `gt_defect_dojo-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gt_defect_dojo-0.0.1/README.md` & `gt_defect_dojo-0.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-THIS API WRAPPER IS DEVELOPE BY ME
+THIS API WRAPPER IS DEVELOPE BY MEp
 ========
 
 See `clients and api wrappers in the docs <https://defectdojo.github.io/django-DefectDojo/integrations/api-v2-docs/#clients--api-wrappers>`_ for alternatives
 
 
 DefectDojo API
 ==============
```

### Comparing `gt_defect_dojo-0.0.1/pyproject.toml` & `gt_defect_dojo-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "gt-defect-dojo"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Raito", email="raito.yagami.9x@gmail.com" },
 ]
 description = "An API wrapper for DefectDojo."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `gt_defect_dojo-0.0.1/PKG-INFO` & `gt_defect_dojo-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gt-defect-dojo
-Version: 0.0.1
+Version: 0.0.2
 Summary: An API wrapper for DefectDojo.
 Project-URL: Homepage, https://github.com/gt-solutions/gt-defect-dojo
 Project-URL: Bug Tracker, https://github.com/gt-solutions/gt-defect-dojo/issues
 Author-email: Raito <raito.yagami.9x@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -27,15 +27,15 @@
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
-THIS API WRAPPER IS DEVELOPE BY ME
+THIS API WRAPPER IS DEVELOPE BY MEp
 ========
 
 See `clients and api wrappers in the docs <https://defectdojo.github.io/django-DefectDojo/integrations/api-v2-docs/#clients--api-wrappers>`_ for alternatives
 
 
 DefectDojo API
 ==============
```

