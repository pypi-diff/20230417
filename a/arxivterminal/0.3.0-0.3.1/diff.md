# Comparing `tmp/arxivterminal-0.3.0.tar.gz` & `tmp/arxivterminal-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arxivterminal-0.3.0.tar", max compression
+gzip compressed data, was "arxivterminal-0.3.1.tar", max compression
```

## Comparing `arxivterminal-0.3.0.tar` & `arxivterminal-0.3.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    35149 2023-04-15 01:36:31.930555 arxivterminal-0.3.0/LICENSE
--rw-r--r--   0        0        0     3528 2023-04-16 05:33:02.049937 arxivterminal-0.3.0/README.md
--rw-r--r--   0        0        0        0 2023-04-15 06:44:50.310227 arxivterminal-0.3.0/arxivterminal/__init__.py
--rw-r--r--   0        0        0     3255 2023-04-16 05:33:02.050319 arxivterminal-0.3.0/arxivterminal/cli.py
--rw-r--r--   0        0        0      349 2023-04-15 07:14:41.406231 arxivterminal-0.3.0/arxivterminal/constants.py
--rw-r--r--   0        0        0    10279 2023-04-16 05:33:02.050586 arxivterminal-0.3.0/arxivterminal/db.py
--rw-r--r--   0        0        0     1049 2023-04-16 05:33:02.050891 arxivterminal-0.3.0/arxivterminal/download.py
--rw-r--r--   0        0        0     2197 2023-04-16 05:33:02.051247 arxivterminal-0.3.0/arxivterminal/fetch.py
--rw-r--r--   0        0        0     5222 2023-04-15 07:14:41.406823 arxivterminal-0.3.0/arxivterminal/ml.py
--rw-r--r--   0        0        0      339 2023-04-16 05:33:02.051527 arxivterminal-0.3.0/arxivterminal/models.py
--rw-r--r--   0        0        0     4656 2023-04-16 05:33:02.051793 arxivterminal-0.3.0/arxivterminal/output.py
--rw-r--r--   0        0        0      772 2023-04-16 05:33:02.052023 arxivterminal-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4512 1970-01-01 00:00:00.000000 arxivterminal-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-15 01:36:31.930555 arxivterminal-0.3.1/LICENSE
+-rw-r--r--   0        0        0     3588 2023-04-17 05:13:23.511960 arxivterminal-0.3.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-15 06:44:50.310227 arxivterminal-0.3.1/arxivterminal/__init__.py
+-rw-r--r--   0        0        0     3255 2023-04-16 05:33:02.050319 arxivterminal-0.3.1/arxivterminal/cli.py
+-rw-r--r--   0        0        0      349 2023-04-15 07:14:41.406231 arxivterminal-0.3.1/arxivterminal/constants.py
+-rw-r--r--   0        0        0    10279 2023-04-16 05:33:02.050586 arxivterminal-0.3.1/arxivterminal/db.py
+-rw-r--r--   0        0        0     1049 2023-04-16 05:33:02.050891 arxivterminal-0.3.1/arxivterminal/download.py
+-rw-r--r--   0        0        0     2197 2023-04-16 05:33:02.051247 arxivterminal-0.3.1/arxivterminal/fetch.py
+-rw-r--r--   0        0        0     5222 2023-04-15 07:14:41.406823 arxivterminal-0.3.1/arxivterminal/ml.py
+-rw-r--r--   0        0        0      339 2023-04-16 05:33:02.051527 arxivterminal-0.3.1/arxivterminal/models.py
+-rw-r--r--   0        0        0     4656 2023-04-16 05:33:02.051793 arxivterminal-0.3.1/arxivterminal/output.py
+-rw-r--r--   0        0        0      779 2023-04-17 05:43:37.545900 arxivterminal-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     4552 1970-01-01 00:00:00.000000 arxivterminal-0.3.1/PKG-INFO
```

### Comparing `arxivterminal-0.3.0/LICENSE` & `arxivterminal-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `arxivterminal-0.3.0/README.md` & `arxivterminal-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # Arxiv Terminal
 ![Tests](https://github.com/jbencina/arxivterminal/actions/workflows/main.yaml/badge.svg)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/arxivterminal)](https://pypi.org/project/arxivterminal)
+![PyPI](https://img.shields.io/pypi/v/arxivterminal)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/arxivterminal)
 
 Arxiv Terminal is a command-line interface (CLI) tool for fetching, searching, and displaying papers from the [arXiv](https://arxiv.org/) preprint repository. The tool allows you to fetch papers from specified categories, search the fetched papers, and display their statistics.
 
 ## Features
 
 - Fetch paper abstracts from specified categories and save them in a local sqllite database.
 - Show fetched papers and interatively open for more detailed abstracts
 - Search fetched papers based on a query (Currently supports pattern + LSA semantic search)
 - Download papers locally as PDF
 
-![Demo](static/demo.gif)
+![Demo](https://raw.githubusercontent.com/jbencina/arxivterminal/main/static/demo.gif)
 
 ## Contributors
 A special call out to ChatGPT (v4) which helped write and modify various code and documentation in this repository.
 
 ## Installation
 
 ```bash
```

### Comparing `arxivterminal-0.3.0/arxivterminal/cli.py` & `arxivterminal-0.3.1/arxivterminal/cli.py`

 * *Files identical despite different names*

### Comparing `arxivterminal-0.3.0/arxivterminal/db.py` & `arxivterminal-0.3.1/arxivterminal/db.py`

 * *Files identical despite different names*

### Comparing `arxivterminal-0.3.0/arxivterminal/download.py` & `arxivterminal-0.3.1/arxivterminal/download.py`

 * *Files identical despite different names*

### Comparing `arxivterminal-0.3.0/arxivterminal/fetch.py` & `arxivterminal-0.3.1/arxivterminal/fetch.py`

 * *Files identical despite different names*

### Comparing `arxivterminal-0.3.0/arxivterminal/ml.py` & `arxivterminal-0.3.1/arxivterminal/ml.py`

 * *Files identical despite different names*

### Comparing `arxivterminal-0.3.0/arxivterminal/output.py` & `arxivterminal-0.3.1/arxivterminal/output.py`

 * *Files identical despite different names*

### Comparing `arxivterminal-0.3.0/pyproject.toml` & `arxivterminal-0.3.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 [tool.poetry]
 name = "arxivterminal"
-version = "0.3.0"
+version = "0.3.1"
 description = "An application for summarizing Arxiv results within the terminal"
 authors = ["John Bencina <jbencina@users.noreply.github.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
+repository = "https://github.com/jbencina/arxivterminal"
+keywords = ["arxiv"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-requests = "^2.28.2"
-bs4 = "^0.0.1"
-openai = "^0.27.4"
-lxml = "^4.9.2"
 pydantic = "^1.10.7"
 arxiv = "^1.4.3"
 click = "^8.1.3"
 termcolor = "^2.2.0"
 appdirs = "^1.4.4"
 scikit-learn = "^1.2.2"
```

### Comparing `arxivterminal-0.3.0/PKG-INFO` & `arxivterminal-0.3.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 Metadata-Version: 2.1
 Name: arxivterminal
-Version: 0.3.0
+Version: 0.3.1
 Summary: An application for summarizing Arxiv results within the terminal
+Home-page: https://github.com/jbencina/arxivterminal
 License: GPL-3.0-or-later
+Keywords: arxiv
 Author: John Bencina
 Author-email: jbencina@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
 Requires-Dist: arxiv (>=1.4.3,<2.0.0)
-Requires-Dist: bs4 (>=0.0.1,<0.0.2)
 Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: lxml (>=4.9.2,<5.0.0)
-Requires-Dist: openai (>=0.27.4,<0.28.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
-Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
 Requires-Dist: termcolor (>=2.2.0,<3.0.0)
+Project-URL: Repository, https://github.com/jbencina/arxivterminal
 Description-Content-Type: text/markdown
 
 # Arxiv Terminal
 ![Tests](https://github.com/jbencina/arxivterminal/actions/workflows/main.yaml/badge.svg)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/arxivterminal)](https://pypi.org/project/arxivterminal)
+![PyPI](https://img.shields.io/pypi/v/arxivterminal)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/arxivterminal)
 
 Arxiv Terminal is a command-line interface (CLI) tool for fetching, searching, and displaying papers from the [arXiv](https://arxiv.org/) preprint repository. The tool allows you to fetch papers from specified categories, search the fetched papers, and display their statistics.
 
 ## Features
 
 - Fetch paper abstracts from specified categories and save them in a local sqllite database.
 - Show fetched papers and interatively open for more detailed abstracts
 - Search fetched papers based on a query (Currently supports pattern + LSA semantic search)
 - Download papers locally as PDF
 
-![Demo](static/demo.gif)
+![Demo](https://raw.githubusercontent.com/jbencina/arxivterminal/main/static/demo.gif)
 
 ## Contributors
 A special call out to ChatGPT (v4) which helped write and modify various code and documentation in this repository.
 
 ## Installation
 
 ```bash
```

