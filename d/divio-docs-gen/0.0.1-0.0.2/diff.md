# Comparing `tmp/divio_docs_gen-0.0.1.tar.gz` & `tmp/divio_docs_gen-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "divio_docs_gen-0.0.1.tar", last modified: Mon Apr 17 10:20:37 2023, max compression
+gzip compressed data, was "divio_docs_gen-0.0.2.tar", last modified: Mon Apr 17 10:57:13 2023, max compression
```

## Comparing `divio_docs_gen-0.0.1.tar` & `divio_docs_gen-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 10:20:37.092321 divio_docs_gen-0.0.1/
--rw-r--r--   0 root         (0) root         (0)     1067 2023-04-17 10:20:26.000000 divio_docs_gen-0.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5366 2023-04-17 10:20:37.092321 divio_docs_gen-0.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4572 2023-04-17 10:20:26.000000 divio_docs_gen-0.0.1/README.md
--rw-r--r--   0 root         (0) root         (0)      849 2023-04-17 10:20:26.000000 divio_docs_gen-0.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 10:20:37.092321 divio_docs_gen-0.0.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 10:20:37.088321 divio_docs_gen-0.0.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 10:20:37.088321 divio_docs_gen-0.0.1/src/divio_docs_gen/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 10:20:26.000000 divio_docs_gen-0.0.1/src/divio_docs_gen/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4004 2023-04-17 10:20:26.000000 divio_docs_gen-0.0.1/src/divio_docs_gen/args.py
--rw-r--r--   0 root         (0) root         (0)      548 2023-04-17 10:20:26.000000 divio_docs_gen-0.0.1/src/divio_docs_gen/colourstring.py
--rw-r--r--   0 root         (0) root         (0)     4926 2023-04-17 10:20:26.000000 divio_docs_gen-0.0.1/src/divio_docs_gen/docsgen.py
--rw-r--r--   0 root         (0) root         (0)     7211 2023-04-17 10:20:26.000000 divio_docs_gen-0.0.1/src/divio_docs_gen/index.py
--rw-r--r--   0 root         (0) root         (0)     5529 2023-04-17 10:20:26.000000 divio_docs_gen-0.0.1/src/divio_docs_gen/repo.py
--rw-r--r--   0 root         (0) root         (0)     5410 2023-04-17 10:20:26.000000 divio_docs_gen-0.0.1/src/divio_docs_gen/sections.py
--rw-r--r--   0 root         (0) root         (0)      925 2023-04-17 10:20:26.000000 divio_docs_gen-0.0.1/src/divio_docs_gen/table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 10:20:37.092321 divio_docs_gen-0.0.1/src/divio_docs_gen.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5366 2023-04-17 10:20:37.000000 divio_docs_gen-0.0.1/src/divio_docs_gen.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      437 2023-04-17 10:20:37.000000 divio_docs_gen-0.0.1/src/divio_docs_gen.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 10:20:37.000000 divio_docs_gen-0.0.1/src/divio_docs_gen.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-04-17 10:20:37.000000 divio_docs_gen-0.0.1/src/divio_docs_gen.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 10:57:13.240103 divio_docs_gen-0.0.2/
+-rw-r--r--   0 root         (0) root         (0)     1067 2023-04-17 10:57:03.000000 divio_docs_gen-0.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5366 2023-04-17 10:57:13.240103 divio_docs_gen-0.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4572 2023-04-17 10:57:03.000000 divio_docs_gen-0.0.2/README.md
+-rw-r--r--   0 root         (0) root         (0)      907 2023-04-17 10:57:03.000000 divio_docs_gen-0.0.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 10:57:13.240103 divio_docs_gen-0.0.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 10:57:13.236103 divio_docs_gen-0.0.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 10:57:13.240103 divio_docs_gen-0.0.2/src/divio_docs_gen/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 10:57:03.000000 divio_docs_gen-0.0.2/src/divio_docs_gen/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4004 2023-04-17 10:57:03.000000 divio_docs_gen-0.0.2/src/divio_docs_gen/args.py
+-rw-r--r--   0 root         (0) root         (0)      548 2023-04-17 10:57:03.000000 divio_docs_gen-0.0.2/src/divio_docs_gen/colourstring.py
+-rw-r--r--   0 root         (0) root         (0)     4926 2023-04-17 10:57:03.000000 divio_docs_gen-0.0.2/src/divio_docs_gen/docsgen.py
+-rw-r--r--   0 root         (0) root         (0)     7252 2023-04-17 10:57:03.000000 divio_docs_gen-0.0.2/src/divio_docs_gen/index.py
+-rw-r--r--   0 root         (0) root         (0)     5529 2023-04-17 10:57:03.000000 divio_docs_gen-0.0.2/src/divio_docs_gen/repo.py
+-rw-r--r--   0 root         (0) root         (0)     5410 2023-04-17 10:57:03.000000 divio_docs_gen-0.0.2/src/divio_docs_gen/sections.py
+-rw-r--r--   0 root         (0) root         (0)      925 2023-04-17 10:57:03.000000 divio_docs_gen-0.0.2/src/divio_docs_gen/table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 10:57:13.240103 divio_docs_gen-0.0.2/src/divio_docs_gen.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5366 2023-04-17 10:57:13.000000 divio_docs_gen-0.0.2/src/divio_docs_gen.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      437 2023-04-17 10:57:13.000000 divio_docs_gen-0.0.2/src/divio_docs_gen.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 10:57:13.000000 divio_docs_gen-0.0.2/src/divio_docs_gen.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-04-17 10:57:13.000000 divio_docs_gen-0.0.2/src/divio_docs_gen.egg-info/top_level.txt
```

### Comparing `divio_docs_gen-0.0.1/LICENSE` & `divio_docs_gen-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.0.1/PKG-INFO` & `divio_docs_gen-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: divio_docs_gen
-Version: 0.0.1
+Version: 0.0.2
 Summary: Turn all the markdown files in your repos into one big, divio structrured documentation
 Author-email: Denperidge <denperidge@gmail.com>
 Project-URL: Homepage, https://github.com/Denperidge-Redpencil/divio-docs-gen
 Project-URL: Bug Tracker, https://github.com/Denperidge-Redpencil/divio-docs-gen/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Information Technology
```

### Comparing `divio_docs_gen-0.0.1/README.md` & `divio_docs_gen-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.0.1/pyproject.toml` & `divio_docs_gen-0.0.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "divio_docs_gen"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     { name="Denperidge", email="denperidge@gmail.com" },
 ]
 description = "Turn all the markdown files in your repos into one big, divio structrured documentation"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -17,10 +17,13 @@
     "Topic :: Software Development :: Documentation",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/Denperidge-Redpencil/divio-docs-gen"
 "Bug Tracker" = "https://github.com/Denperidge-Redpencil/divio-docs-gen/issues"
 
+[console_scripts]
+divio_docs_gen = "index:generate_docs"
+
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
```

### Comparing `divio_docs_gen-0.0.1/src/divio_docs_gen/args.py` & `divio_docs_gen-0.0.2/src/divio_docs_gen/args.py`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.0.1/src/divio_docs_gen/colourstring.py` & `divio_docs_gen-0.0.2/src/divio_docs_gen/colourstring.py`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.0.1/src/divio_docs_gen/docsgen.py` & `divio_docs_gen-0.0.2/src/divio_docs_gen/docsgen.py`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.0.1/src/divio_docs_gen/index.py` & `divio_docs_gen-0.0.2/src/divio_docs_gen/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 from sections import sections, RepoSection
 from table import setup_table, add_and_print, log_and_print, change_log_index
 from docsgen import filepath_in_exceptions, add_to_docs, add_sibling_nav_to_files, generate_docs_nav_file, clear_docs
 from args import args_repoconfigs, args_default_owner, args_generate_nav
 
 """Entrypoint for the application"""
 
-if __name__ == "__main__":
-    
-    # Get headers for CLI tale
+
+def generate_docs():    
+    # Get headers for CLI table
     headers = [
         "     repository     ", 
         sections['tutorials'].headertext, sections['howtos'].headertext,
         sections['explanations'].headertext, sections['references'].headertext]
 
     setup_table(headers)
 
@@ -170,7 +170,9 @@
     change_log_index(-1)
     log_and_print("... finished parsing repos")
 
     # Create a top level nav file
     generate_docs_nav_file("", 1, include_parent_nav=False)
 
 
+if __name__ == "__main__":
+    generate_docs()
```

### Comparing `divio_docs_gen-0.0.1/src/divio_docs_gen/repo.py` & `divio_docs_gen-0.0.2/src/divio_docs_gen/repo.py`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.0.1/src/divio_docs_gen/sections.py` & `divio_docs_gen-0.0.2/src/divio_docs_gen/sections.py`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.0.1/src/divio_docs_gen/table.py` & `divio_docs_gen-0.0.2/src/divio_docs_gen/table.py`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.0.1/src/divio_docs_gen.egg-info/PKG-INFO` & `divio_docs_gen-0.0.2/src/divio_docs_gen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: divio-docs-gen
-Version: 0.0.1
+Version: 0.0.2
 Summary: Turn all the markdown files in your repos into one big, divio structrured documentation
 Author-email: Denperidge <denperidge@gmail.com>
 Project-URL: Homepage, https://github.com/Denperidge-Redpencil/divio-docs-gen
 Project-URL: Bug Tracker, https://github.com/Denperidge-Redpencil/divio-docs-gen/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Information Technology
```

