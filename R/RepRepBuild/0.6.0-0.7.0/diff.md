# Comparing `tmp/RepRepBuild-0.6.0.tar.gz` & `tmp/RepRepBuild-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RepRepBuild-0.6.0.tar", last modified: Wed Apr 12 08:22:49 2023, max compression
+gzip compressed data, was "RepRepBuild-0.7.0.tar", last modified: Mon Apr 17 08:03:13 2023, max compression
```

## Comparing `RepRepBuild-0.6.0.tar` & `RepRepBuild-0.7.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-04-12 08:22:49.956363 RepRepBuild-0.6.0/
--rw-r--r--   0 toon      (1000) toon      (1000)    35149 2017-09-30 07:16:26.000000 RepRepBuild-0.6.0/COPYING
--rw-r--r--   0 toon      (1000) toon      (1000)    43045 2023-04-12 08:22:49.956363 RepRepBuild-0.6.0/PKG-INFO
--rw-r--r--   0 toon      (1000) toon      (1000)     1392 2023-03-21 07:41:05.000000 RepRepBuild-0.6.0/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     1612 2023-04-12 08:21:27.000000 RepRepBuild-0.6.0/pyproject.toml
--rw-r--r--   0 toon      (1000) toon      (1000)       38 2023-04-12 08:22:49.956363 RepRepBuild-0.6.0/setup.cfg
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-04-12 08:22:49.952363 RepRepBuild-0.6.0/src/
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-04-12 08:22:49.953363 RepRepBuild-0.6.0/src/RepRepBuild.egg-info/
--rw-r--r--   0 toon      (1000) toon      (1000)    43045 2023-04-12 08:22:49.000000 RepRepBuild-0.6.0/src/RepRepBuild.egg-info/PKG-INFO
--rw-r--r--   0 toon      (1000) toon      (1000)      571 2023-04-12 08:22:49.000000 RepRepBuild-0.6.0/src/RepRepBuild.egg-info/SOURCES.txt
--rw-r--r--   0 toon      (1000) toon      (1000)        1 2023-04-12 08:22:49.000000 RepRepBuild-0.6.0/src/RepRepBuild.egg-info/dependency_links.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      362 2023-04-12 08:22:49.000000 RepRepBuild-0.6.0/src/RepRepBuild.egg-info/entry_points.txt
--rw-r--r--   0 toon      (1000) toon      (1000)       36 2023-04-12 08:22:49.000000 RepRepBuild-0.6.0/src/RepRepBuild.egg-info/requires.txt
--rw-r--r--   0 toon      (1000) toon      (1000)       12 2023-04-12 08:22:49.000000 RepRepBuild-0.6.0/src/RepRepBuild.egg-info/top_level.txt
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-04-12 08:22:49.956363 RepRepBuild-0.6.0/src/reprepbuild/
--rw-r--r--   0 toon      (1000) toon      (1000)      775 2023-03-14 11:47:22.000000 RepRepBuild-0.6.0/src/reprepbuild/__init__.py
--rw-r--r--   0 toon      (1000) toon      (1000)     9841 2023-04-12 01:15:07.000000 RepRepBuild-0.6.0/src/reprepbuild/__main__.py
--rw-r--r--   0 toon      (1000) toon      (1000)     1803 2023-03-25 09:41:44.000000 RepRepBuild-0.6.0/src/reprepbuild/articlezip.py
--rw-r--r--   0 toon      (1000) toon      (1000)     3517 2023-04-12 08:19:13.000000 RepRepBuild-0.6.0/src/reprepbuild/bibtex.py
--rw-r--r--   0 toon      (1000) toon      (1000)     3910 2023-03-25 09:41:50.000000 RepRepBuild-0.6.0/src/reprepbuild/latex.py
--rw-r--r--   0 toon      (1000) toon      (1000)     4434 2023-03-25 09:51:45.000000 RepRepBuild-0.6.0/src/reprepbuild/latexdep.py
--rw-r--r--   0 toon      (1000) toon      (1000)     1792 2023-03-25 09:42:18.000000 RepRepBuild-0.6.0/src/reprepbuild/normalizepdf.py
--rw-r--r--   0 toon      (1000) toon      (1000)     4087 2023-03-25 09:44:04.000000 RepRepBuild-0.6.0/src/reprepbuild/pythonscript.py
--rw-r--r--   0 toon      (1000) toon      (1000)     2856 2023-03-16 20:21:01.000000 RepRepBuild-0.6.0/src/reprepbuild/repeat.py
--rw-r--r--   0 toon      (1000) toon      (1000)     5006 2023-03-25 09:15:24.000000 RepRepBuild-0.6.0/src/reprepbuild/utils.py
--rw-r--r--   0 toon      (1000) toon      (1000)     2340 2023-03-28 14:48:56.000000 RepRepBuild-0.6.0/src/reprepbuild/zip.py
+drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-04-17 08:03:13.857958 RepRepBuild-0.7.0/
+-rw-r--r--   0 toon      (1000) toon      (1000)    35149 2017-09-30 07:16:26.000000 RepRepBuild-0.7.0/COPYING
+-rw-r--r--   0 toon      (1000) toon      (1000)    43045 2023-04-17 08:03:13.857958 RepRepBuild-0.7.0/PKG-INFO
+-rw-r--r--   0 toon      (1000) toon      (1000)     1392 2023-03-21 07:41:05.000000 RepRepBuild-0.7.0/README.md
+-rw-r--r--   0 toon      (1000) toon      (1000)     1612 2023-04-17 08:02:34.000000 RepRepBuild-0.7.0/pyproject.toml
+-rw-r--r--   0 toon      (1000) toon      (1000)       38 2023-04-17 08:03:13.857958 RepRepBuild-0.7.0/setup.cfg
+drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-04-17 08:03:13.844958 RepRepBuild-0.7.0/src/
+drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-04-17 08:03:13.845958 RepRepBuild-0.7.0/src/RepRepBuild.egg-info/
+-rw-r--r--   0 toon      (1000) toon      (1000)    43045 2023-04-17 08:03:13.000000 RepRepBuild-0.7.0/src/RepRepBuild.egg-info/PKG-INFO
+-rw-r--r--   0 toon      (1000) toon      (1000)      571 2023-04-17 08:03:13.000000 RepRepBuild-0.7.0/src/RepRepBuild.egg-info/SOURCES.txt
+-rw-r--r--   0 toon      (1000) toon      (1000)        1 2023-04-17 08:03:13.000000 RepRepBuild-0.7.0/src/RepRepBuild.egg-info/dependency_links.txt
+-rw-r--r--   0 toon      (1000) toon      (1000)      362 2023-04-17 08:03:13.000000 RepRepBuild-0.7.0/src/RepRepBuild.egg-info/entry_points.txt
+-rw-r--r--   0 toon      (1000) toon      (1000)       36 2023-04-17 08:03:13.000000 RepRepBuild-0.7.0/src/RepRepBuild.egg-info/requires.txt
+-rw-r--r--   0 toon      (1000) toon      (1000)       12 2023-04-17 08:03:13.000000 RepRepBuild-0.7.0/src/RepRepBuild.egg-info/top_level.txt
+drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-04-17 08:03:13.857958 RepRepBuild-0.7.0/src/reprepbuild/
+-rw-r--r--   0 toon      (1000) toon      (1000)      775 2023-03-14 11:47:22.000000 RepRepBuild-0.7.0/src/reprepbuild/__init__.py
+-rw-r--r--   0 toon      (1000) toon      (1000)    10101 2023-04-17 08:00:00.000000 RepRepBuild-0.7.0/src/reprepbuild/__main__.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     1803 2023-03-25 09:41:44.000000 RepRepBuild-0.7.0/src/reprepbuild/articlezip.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     3517 2023-04-12 08:19:13.000000 RepRepBuild-0.7.0/src/reprepbuild/bibtex.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     3910 2023-03-25 09:41:50.000000 RepRepBuild-0.7.0/src/reprepbuild/latex.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     4434 2023-03-25 09:51:45.000000 RepRepBuild-0.7.0/src/reprepbuild/latexdep.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     1792 2023-03-25 09:42:18.000000 RepRepBuild-0.7.0/src/reprepbuild/normalizepdf.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     4087 2023-03-25 09:44:04.000000 RepRepBuild-0.7.0/src/reprepbuild/pythonscript.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     2856 2023-03-16 20:21:01.000000 RepRepBuild-0.7.0/src/reprepbuild/repeat.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     5006 2023-03-25 09:15:24.000000 RepRepBuild-0.7.0/src/reprepbuild/utils.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     2340 2023-03-28 14:48:56.000000 RepRepBuild-0.7.0/src/reprepbuild/zip.py
```

### Comparing `RepRepBuild-0.6.0/COPYING` & `RepRepBuild-0.7.0/COPYING`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.6.0/PKG-INFO` & `RepRepBuild-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RepRepBuild
-Version: 0.6.0
+Version: 0.7.0
 Summary: Build tool for Reproducible Reporting
 Author-email: Toon Verstraelen <toon.verstraelen@ugent.be>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `RepRepBuild-0.6.0/README.md` & `RepRepBuild-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.6.0/pyproject.toml` & `RepRepBuild-0.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "RepRepBuild"
-version = "0.6.0"
+version = "0.7.0"
 authors = [
   { name="Toon Verstraelen", email="toon.verstraelen@ugent.be" },
 ]
 description = "Build tool for Reproducible Reporting"
 readme = "README.md"
 license = {file = "COPYING"}
 requires-python = ">=3.6"
```

### Comparing `RepRepBuild-0.6.0/src/RepRepBuild.egg-info/PKG-INFO` & `RepRepBuild-0.7.0/src/RepRepBuild.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RepRepBuild
-Version: 0.6.0
+Version: 0.7.0
 Summary: Build tool for Reproducible Reporting
 Author-email: Toon Verstraelen <toon.verstraelen@ugent.be>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `RepRepBuild-0.6.0/src/RepRepBuild.egg-info/SOURCES.txt` & `RepRepBuild-0.7.0/src/RepRepBuild.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.6.0/src/reprepbuild/__init__.py` & `RepRepBuild-0.7.0/src/reprepbuild/__init__.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.6.0/src/reprepbuild/__main__.py` & `RepRepBuild-0.7.0/src/reprepbuild/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,20 +38,33 @@
 from ninja.ninja_syntax import Writer
 
 from .utils import check_script_args, import_python_path
 
 __all__ = ("main",)
 
 
+LATEXDIFF_CONTEXT2CMD = ",".join(
+    [
+        "abstract",
+        "supplementary",
+        "dataavailability",
+        "funding",
+        "authorcontributions",
+        "conflictsofinterest",
+        "abbreviations",
+    ]
+)
+
+
 DEFAULT_RULES = {
     "latexdep": {"command": "rr-latexdep $in", "depfile": "$in.d"},
     "bibtex": {"command": "rr-bibtex $in", "depfile": "$in.d"},
     "latex": {"command": "rr-latex $in"},
     "copy": {"command": "cp $in $out"},
-    "latexdiff": {"command": "latexdiff --append-context2cmd=abstract $in > $out"},
+    "latexdiff": {"command": f"latexdiff --append-context2cmd={LATEXDIFF_CONTEXT2CMD} $in > $out"},
     "reprozip": {"command": "rr-zip $out $in"},
     "reproarticlezip": {"command": "rr-article-zip $out $in"},
     "svgtopdf": {
         "command": "inkscape $in --export-filename=$out --export-type=pdf; rr-normalize-pdf $out"
     },
     "pythonscript": {"command": "rr-python-script $in -- $args > $out", "depfile": "$in.d"},
 }
@@ -94,19 +107,19 @@
     }
     yield {
         "outputs": os.path.join("uploads", f"{prefix}.pdf"),
         "rule": "copy",
         "inputs": fixpath(f"{prefix}.pdf"),
         "default": True,
     }
-    if prefix == "article":
+    if prefix in ["article", "supp"]:
         yield {
-            "outputs": os.path.join("uploads", "article.zip"),
+            "outputs": os.path.join("uploads", f"{prefix}.zip"),
             "rule": "reproarticlezip",
-            "inputs": "latex-article/article.pdf",
+            "inputs": f"latex-{prefix}/{prefix}.pdf",
             "default": True,
         }
 
 
 def latexdiff_pattern(path):
     """Make ninja build commands to generate a latex diff."""
     result = re.match(r"latex-(?P<prefix>[a-z0-9-]+)/(?P=prefix)-old.(?P<ext>.*)$", path)
```

### Comparing `RepRepBuild-0.6.0/src/reprepbuild/articlezip.py` & `RepRepBuild-0.7.0/src/reprepbuild/articlezip.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.6.0/src/reprepbuild/bibtex.py` & `RepRepBuild-0.7.0/src/reprepbuild/bibtex.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.6.0/src/reprepbuild/latex.py` & `RepRepBuild-0.7.0/src/reprepbuild/latex.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.6.0/src/reprepbuild/latexdep.py` & `RepRepBuild-0.7.0/src/reprepbuild/latexdep.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.6.0/src/reprepbuild/normalizepdf.py` & `RepRepBuild-0.7.0/src/reprepbuild/normalizepdf.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.6.0/src/reprepbuild/pythonscript.py` & `RepRepBuild-0.7.0/src/reprepbuild/pythonscript.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.6.0/src/reprepbuild/repeat.py` & `RepRepBuild-0.7.0/src/reprepbuild/repeat.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.6.0/src/reprepbuild/utils.py` & `RepRepBuild-0.7.0/src/reprepbuild/utils.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.6.0/src/reprepbuild/zip.py` & `RepRepBuild-0.7.0/src/reprepbuild/zip.py`

 * *Files identical despite different names*

