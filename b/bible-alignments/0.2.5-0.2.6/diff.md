# Comparing `tmp/bible_alignments-0.2.5.tar.gz` & `tmp/bible_alignments-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bible_alignments-0.2.5.tar", max compression
+gzip compressed data, was "bible_alignments-0.2.6.tar", max compression
```

## Comparing `bible_alignments-0.2.5.tar` & `bible_alignments-0.2.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    20131 2023-02-22 04:20:29.147219 bible_alignments-0.2.5/LICENSE
--rw-r--r--   0        0        0      900 2023-03-01 18:19:16.168100 bible_alignments-0.2.5/README.md
--rw-r--r--   0        0        0     1705 2023-04-12 23:54:12.663470 bible_alignments-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      554 2023-02-22 04:20:29.528825 bible_alignments-0.2.5/src/.github/actions/run-checks/action.yml
--rw-r--r--   0        0        0     2033 2023-02-22 04:20:29.529037 bible_alignments-0.2.5/src/.github/actions/setup-poetry-env/action.yml
--rw-r--r--   0        0        0      975 2023-02-22 04:20:29.529246 bible_alignments-0.2.5/src/.github/workflows/on-merge-to-main.yml
--rw-r--r--   0        0        0      949 2023-02-22 04:20:29.529365 bible_alignments-0.2.5/src/.github/workflows/on-pull-request.yml
--rw-r--r--   0        0        0     1964 2023-02-22 04:20:29.529486 bible_alignments-0.2.5/src/.github/workflows/on-release-main.yml
--rw-r--r--   0        0        0      351 2023-02-22 04:20:29.529608 bible_alignments-0.2.5/src/.github/workflows/validate-codecov-config.yml
--rw-r--r--   0        0        0    16557 2023-02-28 20:36:24.715176 bible_alignments-0.2.5/src/01-Exploration.ipynb
--rw-r--r--   0        0        0        0 2023-02-24 04:25:37.140718 bible_alignments-0.2.5/src/__init__.py
--rw-r--r--   0        0        0     4810 2023-03-16 20:46:04.251808 bible_alignments-0.2.5/src/catalog.py
--rw-r--r--   0        0        0      247 2023-02-24 04:25:33.130530 bible_alignments-0.2.5/src/config.py
--rw-r--r--   0        0        0        0 2023-02-22 04:20:29.529807 bible_alignments-0.2.5/src/format/__init__.py
--rw-r--r--   0        0        0     5829 2023-02-22 04:20:29.529962 bible_alignments-0.2.5/src/format/grapecity.py
--rw-r--r--   0        0        0     2134 2023-04-12 01:30:26.702956 bible_alignments-0.2.5/src/gcsource.py
--rw-r--r--   0        0        0     2193 2023-04-12 01:30:54.463180 bible_alignments-0.2.5/src/gctarget.py
--rw-r--r--   0        0        0     4536 2023-04-12 23:47:40.528641 bible_alignments-0.2.5/src/grapecity.py
--rw-r--r--   0        0        0     2098 1970-01-01 00:00:00.000000 bible_alignments-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0    20131 2023-02-22 04:20:29.147219 bible_alignments-0.2.6/LICENSE
+-rw-r--r--   0        0        0      900 2023-03-01 18:19:16.168100 bible_alignments-0.2.6/README.md
+-rw-r--r--   0        0        0     1699 2023-04-17 20:24:58.984767 bible_alignments-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0      554 2023-02-22 04:20:29.528825 bible_alignments-0.2.6/src/.github/actions/run-checks/action.yml
+-rw-r--r--   0        0        0     2033 2023-02-22 04:20:29.529037 bible_alignments-0.2.6/src/.github/actions/setup-poetry-env/action.yml
+-rw-r--r--   0        0        0      975 2023-02-22 04:20:29.529247 bible_alignments-0.2.6/src/.github/workflows/on-merge-to-main.yml
+-rw-r--r--   0        0        0      949 2023-02-22 04:20:29.529364 bible_alignments-0.2.6/src/.github/workflows/on-pull-request.yml
+-rw-r--r--   0        0        0     1964 2023-02-22 04:20:29.529486 bible_alignments-0.2.6/src/.github/workflows/on-release-main.yml
+-rw-r--r--   0        0        0      351 2023-02-22 04:20:29.529608 bible_alignments-0.2.6/src/.github/workflows/validate-codecov-config.yml
+-rw-r--r--   0        0        0    16557 2023-02-28 20:36:24.715176 bible_alignments-0.2.6/src/01-Exploration.ipynb
+-rw-r--r--   0        0        0        0 2023-02-24 04:25:37.140718 bible_alignments-0.2.6/src/__init__.py
+-rw-r--r--   0        0        0     4810 2023-03-16 20:46:04.251808 bible_alignments-0.2.6/src/catalog.py
+-rw-r--r--   0        0        0      247 2023-02-24 04:25:33.130530 bible_alignments-0.2.6/src/config.py
+-rw-r--r--   0        0        0        0 2023-02-22 04:20:29.529807 bible_alignments-0.2.6/src/format/__init__.py
+-rw-r--r--   0        0        0     5829 2023-02-22 04:20:29.529962 bible_alignments-0.2.6/src/format/grapecity.py
+-rw-r--r--   0        0        0     2134 2023-04-12 01:30:26.702000 bible_alignments-0.2.6/src/gcsource.py
+-rw-r--r--   0        0        0     2193 2023-04-12 01:30:54.463000 bible_alignments-0.2.6/src/gctarget.py
+-rw-r--r--   0        0        0     4536 2023-04-12 23:47:40.528000 bible_alignments-0.2.6/src/grapecity.py
+-rw-r--r--   0        0        0     2086 1970-01-01 00:00:00.000000 bible_alignments-0.2.6/PKG-INFO
```

### Comparing `bible_alignments-0.2.5/LICENSE` & `bible_alignments-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.5/README.md` & `bible_alignments-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.5/pyproject.toml` & `bible_alignments-0.2.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "bible-alignments"
-version = "0.2.5"
+version = "0.2.6"
 description = "Word-level alignments for Bibles, including both automatic alignments and manually corrected alignments."
 authors = ["Sean Boisen <sean.boisen@clear.bible>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["Bible", "alignment", "Bible alignment"]
-repository = "https://github.com/Clear-Bible/bible-alignments"
+repository = "https://github.com/Clear-Bible/Alignments"
 #documentation = "https://sboisen.github.io/alignments/"
 packages = [
   {include = "src"}
 ]
 # need more here
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `bible_alignments-0.2.5/src/.github/actions/run-checks/action.yml` & `bible_alignments-0.2.6/src/.github/actions/run-checks/action.yml`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.5/src/.github/actions/setup-poetry-env/action.yml` & `bible_alignments-0.2.6/src/.github/actions/setup-poetry-env/action.yml`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.5/src/.github/workflows/on-merge-to-main.yml` & `bible_alignments-0.2.6/src/.github/workflows/on-merge-to-main.yml`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.5/src/.github/workflows/on-pull-request.yml` & `bible_alignments-0.2.6/src/.github/workflows/on-pull-request.yml`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.5/src/.github/workflows/on-release-main.yml` & `bible_alignments-0.2.6/src/.github/workflows/on-release-main.yml`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.5/src/01-Exploration.ipynb` & `bible_alignments-0.2.6/src/01-Exploration.ipynb`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.5/src/catalog.py` & `bible_alignments-0.2.6/src/catalog.py`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.5/src/format/grapecity.py` & `bible_alignments-0.2.6/src/format/grapecity.py`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.5/src/gcsource.py` & `bible_alignments-0.2.6/src/gcsource.py`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.5/src/gctarget.py` & `bible_alignments-0.2.6/src/gctarget.py`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.5/src/grapecity.py` & `bible_alignments-0.2.6/src/grapecity.py`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.5/PKG-INFO` & `bible_alignments-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: bible-alignments
-Version: 0.2.5
+Version: 0.2.6
 Summary: Word-level alignments for Bibles, including both automatic alignments and manually corrected alignments.
-Home-page: https://github.com/Clear-Bible/bible-alignments
+Home-page: https://github.com/Clear-Bible/Alignments
 License: MIT
 Keywords: Bible,alignment,Bible alignment
 Author: Sean Boisen
 Author-email: sean.boisen@clear.bible
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Religion
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Religion
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: jsonlines (>=3.1.0,<4.0.0)
 Requires-Dist: jupyterlab (>=3.6.1,<4.0.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
-Project-URL: Repository, https://github.com/Clear-Bible/bible-alignments
+Project-URL: Repository, https://github.com/Clear-Bible/Alignments
 Description-Content-Type: text/markdown
 
 
 
 # Alignments
 
 Word alignments for Bibles, including both automatic alignments and manually corrected alignments
```

