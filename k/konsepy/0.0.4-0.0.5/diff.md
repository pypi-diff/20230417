# Comparing `tmp/konsepy-0.0.4.tar.gz` & `tmp/konsepy-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "konsepy-0.0.4.tar", last modified: Fri Apr 14 18:07:27 2023, max compression
+gzip compressed data, was "konsepy-0.0.5.tar", last modified: Mon Apr 17 20:39:17 2023, max compression
```

## Comparing `konsepy-0.0.4.tar` & `konsepy-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0      996 2023-04-14 18:07:23.814765 konsepy-0.0.4/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0       41 2023-04-14 18:07:23.814765 konsepy-0.0.4/.gitignore
--rw-r--r--   0        0        0      335 2023-04-14 18:07:23.814765 konsepy-0.0.4/README.md
--rw-r--r--   0        0        0      905 2023-04-14 18:07:23.814765 konsepy-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      110 2023-04-14 18:07:23.814765 konsepy-0.0.4/src/konsepy/__init__.py
--rw-r--r--   0        0        0     4077 2023-04-14 18:07:23.814765 konsepy-0.0.4/src/konsepy/bio_tag.py
--rw-r--r--   0        0        0     2899 2023-04-14 18:07:23.814765 konsepy-0.0.4/src/konsepy/cli.py
--rw-r--r--   0        0        0      104 2023-04-14 18:07:23.814765 konsepy-0.0.4/src/konsepy/constants.py
--rw-r--r--   0        0        0     4249 2023-04-14 18:07:23.814765 konsepy-0.0.4/src/konsepy/get_text_snippets.py
--rw-r--r--   0        0        0     1564 2023-04-14 18:07:23.814765 konsepy-0.0.4/src/konsepy/importer.py
--rw-r--r--   0        0        0     5284 2023-04-14 18:07:23.814765 konsepy-0.0.4/src/konsepy/regex.py
--rw-r--r--   0        0        0     2390 2023-04-14 18:07:23.814765 konsepy-0.0.4/src/konsepy/run_all.py
--rw-r--r--   0        0        0      654 2023-04-14 18:07:23.814765 konsepy-0.0.4/src/konsepy/rxutils.py
--rw-r--r--   0        0        0     3738 2023-04-14 18:07:23.814765 konsepy-0.0.4/src/konsepy/textio.py
--rw-r--r--   0        0        0      202 2023-04-14 18:07:23.814765 konsepy-0.0.4/src/konsepy/types.py
--rw-r--r--   0        0        0     1212 1970-01-01 00:00:00.000000 konsepy-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      996 2023-04-17 20:39:09.203511 konsepy-0.0.5/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0       41 2023-04-17 20:39:09.203511 konsepy-0.0.5/.gitignore
+-rw-r--r--   0        0        0      607 2023-04-17 20:39:09.203511 konsepy-0.0.5/CHANGELOG.md
+-rw-r--r--   0        0        0      335 2023-04-17 20:39:09.203511 konsepy-0.0.5/README.md
+-rw-r--r--   0        0        0      905 2023-04-17 20:39:09.203511 konsepy-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      110 2023-04-17 20:39:09.203511 konsepy-0.0.5/src/konsepy/__init__.py
+-rw-r--r--   0        0        0     4077 2023-04-17 20:39:09.203511 konsepy-0.0.5/src/konsepy/bio_tag.py
+-rw-r--r--   0        0        0     2888 2023-04-17 20:39:09.203511 konsepy-0.0.5/src/konsepy/cli.py
+-rw-r--r--   0        0        0      104 2023-04-17 20:39:09.203511 konsepy-0.0.5/src/konsepy/constants.py
+-rw-r--r--   0        0        0     4249 2023-04-17 20:39:09.203511 konsepy-0.0.5/src/konsepy/get_text_snippets.py
+-rw-r--r--   0        0        0     1564 2023-04-17 20:39:09.203511 konsepy-0.0.5/src/konsepy/importer.py
+-rw-r--r--   0        0        0     5284 2023-04-17 20:39:09.203511 konsepy-0.0.5/src/konsepy/regex.py
+-rw-r--r--   0        0        0     2390 2023-04-17 20:39:09.203511 konsepy-0.0.5/src/konsepy/run_all.py
+-rw-r--r--   0        0        0      654 2023-04-17 20:39:09.203511 konsepy-0.0.5/src/konsepy/rxutils.py
+-rw-r--r--   0        0        0     3738 2023-04-17 20:39:09.203511 konsepy-0.0.5/src/konsepy/textio.py
+-rw-r--r--   0        0        0      202 2023-04-17 20:39:09.203511 konsepy-0.0.5/src/konsepy/types.py
+-rw-r--r--   0        0        0     1212 1970-01-01 00:00:00.000000 konsepy-0.0.5/PKG-INFO
```

### Comparing `konsepy-0.0.4/.github/workflows/publish-to-pypi.yml` & `konsepy-0.0.5/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `konsepy-0.0.4/pyproject.toml` & `konsepy-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `konsepy-0.0.4/src/konsepy/bio_tag.py` & `konsepy-0.0.5/src/konsepy/bio_tag.py`

 * *Files identical despite different names*

### Comparing `konsepy-0.0.4/src/konsepy/cli.py` & `konsepy-0.0.5/src/konsepy/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,13 +44,13 @@
     parser.add_argument('--outdir', type=Path, default=Path('.'),
                         help='Directory to place output files.')
     parser.add_argument('--input-files', nargs='+', type=str, default=list(),
                         help='Input CSV or SAS file(s) to read.')
     parser.add_argument('--id-label', default=ID_LABEL,
                         help='Column label for individual id')
     parser.add_argument('--noteid-label', default=NOTEID_LABEL,
-                        help='Column label for individual id')
+                        help='Column label for note id')
     parser.add_argument('--notedate-label', default=NOTEDATE_LABEL,
-                        help='Column label for individual id')
+                        help='Column label for date of note')
     parser.add_argument('--notetext-label', default=NOTETEXT_LABEL,
-                        help='Column label for individual id')
+                        help='Column label for note text')
     return parser
```

### Comparing `konsepy-0.0.4/src/konsepy/get_text_snippets.py` & `konsepy-0.0.5/src/konsepy/get_text_snippets.py`

 * *Files identical despite different names*

### Comparing `konsepy-0.0.4/src/konsepy/importer.py` & `konsepy-0.0.5/src/konsepy/importer.py`

 * *Files identical despite different names*

### Comparing `konsepy-0.0.4/src/konsepy/regex.py` & `konsepy-0.0.5/src/konsepy/regex.py`

 * *Files identical despite different names*

### Comparing `konsepy-0.0.4/src/konsepy/run_all.py` & `konsepy-0.0.5/src/konsepy/run_all.py`

 * *Files identical despite different names*

### Comparing `konsepy-0.0.4/src/konsepy/rxutils.py` & `konsepy-0.0.5/src/konsepy/rxutils.py`

 * *Files identical despite different names*

### Comparing `konsepy-0.0.4/src/konsepy/textio.py` & `konsepy-0.0.5/src/konsepy/textio.py`

 * *Files identical despite different names*

### Comparing `konsepy-0.0.4/PKG-INFO` & `konsepy-0.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: konsepy
-Version: 0.0.4
+Version: 0.0.5
 Summary: Framework for build NLP information extraction systems using regular expressions.
 Keywords: nlp
 Author-email: dcronkite <dcronkite+pypi@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

