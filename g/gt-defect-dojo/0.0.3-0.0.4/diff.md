# Comparing `tmp/gt_defect_dojo-0.0.3.tar.gz` & `tmp/gt_defect_dojo-0.0.4.tar.gz`

## Comparing `gt_defect_dojo-0.0.3.tar` & `gt_defect_dojo-0.0.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0  1384669 2020-02-02 00:00:00.000000 gt_defect_dojo-0.0.3/examples/dependency-check-report.xml
--rw-r--r--   0        0        0    17634 2020-02-02 00:00:00.000000 gt_defect_dojo-0.0.3/examples/upload-defectdojo.py
--rw-r--r--   0        0        0    51287 2020-02-02 00:00:00.000000 gt_defect_dojo-0.0.3/src/gt_defectdojo_api/__init__.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 gt_defect_dojo-0.0.3/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 gt_defect_dojo-0.0.3/LICENSE
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 gt_defect_dojo-0.0.3/README.md
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 gt_defect_dojo-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 gt_defect_dojo-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    51287 2020-02-02 00:00:00.000000 gt_defect_dojo-0.0.4/src/gt_defectdojo_api/__init__.py
+-rw-r--r--   0        0        0  1384669 2020-02-02 00:00:00.000000 gt_defect_dojo-0.0.4/tests/dependency-check-report.xml
+-rw-r--r--   0        0        0    17634 2020-02-02 00:00:00.000000 gt_defect_dojo-0.0.4/tests/upload-defectdojo.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 gt_defect_dojo-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 gt_defect_dojo-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 gt_defect_dojo-0.0.4/README.md
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 gt_defect_dojo-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 gt_defect_dojo-0.0.4/PKG-INFO
```

### Comparing `gt_defect_dojo-0.0.3/examples/dependency-check-report.xml` & `gt_defect_dojo-0.0.4/tests/dependency-check-report.xml`

 * *Files identical despite different names*

### Comparing `gt_defect_dojo-0.0.3/examples/upload-defectdojo.py` & `gt_defect_dojo-0.0.4/tests/upload-defectdojo.py`

 * *Files identical despite different names*

### Comparing `gt_defect_dojo-0.0.3/src/gt_defectdojo_api/__init__.py` & `gt_defect_dojo-0.0.4/src/gt_defectdojo_api/__init__.py`

 * *Files identical despite different names*

### Comparing `gt_defect_dojo-0.0.3/.gitignore` & `gt_defect_dojo-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `gt_defect_dojo-0.0.3/LICENSE` & `gt_defect_dojo-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gt_defect_dojo-0.0.3/README.md` & `gt_defect_dojo-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `gt_defect_dojo-0.0.3/pyproject.toml` & `gt_defect_dojo-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "gt-defect-dojo"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Raito", email="raito.yagami.9x@gmail.com" },
 ]
 description = "An API wrapper for DefectDojo."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `gt_defect_dojo-0.0.3/PKG-INFO` & `gt_defect_dojo-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gt-defect-dojo
-Version: 0.0.3
+Version: 0.0.4
 Summary: An API wrapper for DefectDojo.
 Project-URL: Homepage, https://github.com/gt-solutions/gt-defect-dojo
 Project-URL: Bug Tracker, https://github.com/gt-solutions/gt-defect-dojo/issues
 Author-email: Raito <raito.yagami.9x@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

