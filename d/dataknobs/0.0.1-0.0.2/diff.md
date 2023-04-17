# Comparing `tmp/dataknobs-0.0.1.tar.gz` & `tmp/dataknobs-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataknobs-0.0.1.tar", max compression
+gzip compressed data, was "dataknobs-0.0.2.tar", max compression
```

## Comparing `dataknobs-0.0.1.tar` & `dataknobs-0.0.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1065 2023-02-10 14:57:51.288106 dataknobs-0.0.1/LICENSE
--rw-r--r--   0        0        0     2189 2023-04-07 01:34:46.742693 dataknobs-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-02-10 14:59:17.454505 dataknobs-0.0.1/dataknobs/__init__.py
--rw-r--r--   0        0        0        0 2023-02-10 14:59:17.448758 dataknobs-0.0.1/dataknobs/structures/__init__.py
--rw-r--r--   0        0        0     1984 2023-02-10 14:59:17.453600 dataknobs-0.0.1/dataknobs/structures/conditional_dict.py
--rw-r--r--   0        0        0     2244 2023-02-21 14:43:49.731060 dataknobs-0.0.1/dataknobs/structures/document.py
--rw-r--r--   0        0        0    16152 2023-02-21 14:43:49.732221 dataknobs-0.0.1/dataknobs/structures/tree.py
--rw-r--r--   0        0        0        0 2023-02-10 14:59:17.460301 dataknobs-0.0.1/dataknobs/utils/__init__.py
--rw-r--r--   0        0        0    10016 2023-03-19 14:30:33.649398 dataknobs-0.0.1/dataknobs/utils/elasticsearch_utils.py
--rw-r--r--   0        0        0     8677 2023-02-10 14:59:17.470241 dataknobs-0.0.1/dataknobs/utils/emoji_utils.py
--rw-r--r--   0        0        0     1971 2023-04-07 01:30:02.990153 dataknobs-0.0.1/dataknobs/utils/file_utils.py
--rw-r--r--   0        0        0    17695 2023-03-10 01:33:33.971598 dataknobs-0.0.1/dataknobs/utils/json_paths.py.002
--rw-r--r--   0        0        0    17767 2023-03-11 21:00:19.316119 dataknobs-0.0.1/dataknobs/utils/json_paths.py.del
--rw-r--r--   0        0        0    39879 2023-03-22 16:43:44.020177 dataknobs-0.0.1/dataknobs/utils/json_utils.py
--rw-r--r--   0        0        0    20296 2023-02-18 17:25:48.681883 dataknobs-0.0.1/dataknobs/utils/json_utils.py.000
--rw-r--r--   0        0        0    56727 2023-03-08 20:22:00.908582 dataknobs-0.0.1/dataknobs/utils/json_utils.py.001
--rw-r--r--   0        0        0    56710 2023-03-09 18:53:43.696089 dataknobs-0.0.1/dataknobs/utils/json_utils.py.002
--rw-r--r--   0        0        0    38844 2023-03-12 02:44:32.369267 dataknobs-0.0.1/dataknobs/utils/json_utils.py.003
--rw-r--r--   0        0        0    39879 2023-03-22 16:43:44.020177 dataknobs-0.0.1/dataknobs/utils/json_utils.py.004
--rw-r--r--   0        0        0    14351 2023-02-10 14:59:17.456062 dataknobs-0.0.1/dataknobs/utils/pandas_utils.py
--rw-r--r--   0        0        0     9134 2023-03-13 17:34:48.816244 dataknobs-0.0.1/dataknobs/utils/path_group.py.no-add
--rw-r--r--   0        0        0    11853 2023-03-11 22:32:17.644075 dataknobs-0.0.1/dataknobs/utils/path_sorter.py.del
--rw-r--r--   0        0        0    13283 2023-02-10 14:59:17.466209 dataknobs-0.0.1/dataknobs/utils/requests_utils.py
--rw-r--r--   0        0        0     3782 2023-02-10 14:59:17.458516 dataknobs-0.0.1/dataknobs/utils/resource_utils.py
--rw-r--r--   0        0        0    13186 2023-02-10 14:59:17.469429 dataknobs-0.0.1/dataknobs/utils/sql_utils.py
--rw-r--r--   0        0        0    23161 2023-04-06 13:26:19.246705 dataknobs-0.0.1/dataknobs/utils/stats_utils.py
--rw-r--r--   0        0        0     1425 2023-04-07 01:30:29.212977 dataknobs-0.0.1/dataknobs/utils/subprocess_utils.py
--rw-r--r--   0        0        0     3104 2023-02-10 14:59:17.468140 dataknobs-0.0.1/dataknobs/utils/xml_utils.py
--rw-r--r--   0        0        0     2878 2023-02-10 14:59:17.477011 dataknobs-0.0.1/dataknobs/xization/0.readme.txt
--rw-r--r--   0        0        0        0 2023-02-10 14:59:17.477662 dataknobs-0.0.1/dataknobs/xization/__init__.py
--rw-r--r--   0        0        0    23741 2023-02-21 14:43:49.735671 dataknobs-0.0.1/dataknobs/xization/annotations.py
--rw-r--r--   0        0        0    32223 2023-02-21 14:43:49.736547 dataknobs-0.0.1/dataknobs/xization/authorities.py
--rw-r--r--   0        0        0    24670 2023-04-07 01:28:30.505818 dataknobs-0.0.1/dataknobs/xization/lexicon.py
--rw-r--r--   0        0        0    27391 2023-02-21 14:43:49.738081 dataknobs-0.0.1/dataknobs/xization/masking_tokenizer.py
--rw-r--r--   0        0        0    14226 2023-02-10 14:59:17.476141 dataknobs-0.0.1/dataknobs/xization/normalize.py
--rw-r--r--   0        0        0      834 2023-04-06 13:44:01.838973 dataknobs-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3313 1970-01-01 00:00:00.000000 dataknobs-0.0.1/setup.py
--rw-r--r--   0        0        0     3138 1970-01-01 00:00:00.000000 dataknobs-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-02-10 14:57:51.288106 dataknobs-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2189 2023-04-07 02:48:31.052502 dataknobs-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-02-10 14:59:17.454505 dataknobs-0.0.2/dataknobs/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-10 14:59:17.448758 dataknobs-0.0.2/dataknobs/structures/__init__.py
+-rw-r--r--   0        0        0     1984 2023-02-10 14:59:17.453600 dataknobs-0.0.2/dataknobs/structures/conditional_dict.py
+-rw-r--r--   0        0        0     2244 2023-04-07 02:48:31.054139 dataknobs-0.0.2/dataknobs/structures/document.py
+-rw-r--r--   0        0        0    16152 2023-04-07 02:48:31.055468 dataknobs-0.0.2/dataknobs/structures/tree.py
+-rw-r--r--   0        0        0        0 2023-02-10 14:59:17.460301 dataknobs-0.0.2/dataknobs/utils/__init__.py
+-rw-r--r--   0        0        0    10016 2023-04-07 02:48:31.055899 dataknobs-0.0.2/dataknobs/utils/elasticsearch_utils.py
+-rw-r--r--   0        0        0     8677 2023-02-10 14:59:17.470241 dataknobs-0.0.2/dataknobs/utils/emoji_utils.py
+-rw-r--r--   0        0        0     2317 2023-04-17 02:32:55.436615 dataknobs-0.0.2/dataknobs/utils/file_utils.py
+-rw-r--r--   0        0        0    17695 2023-03-10 01:33:33.971598 dataknobs-0.0.2/dataknobs/utils/json_paths.py.002
+-rw-r--r--   0        0        0    17767 2023-03-11 21:00:19.316119 dataknobs-0.0.2/dataknobs/utils/json_paths.py.del
+-rw-r--r--   0        0        0    39879 2023-04-07 02:48:31.056635 dataknobs-0.0.2/dataknobs/utils/json_utils.py
+-rw-r--r--   0        0        0    20296 2023-02-18 17:25:48.681883 dataknobs-0.0.2/dataknobs/utils/json_utils.py.000
+-rw-r--r--   0        0        0    56727 2023-03-08 20:22:00.908582 dataknobs-0.0.2/dataknobs/utils/json_utils.py.001
+-rw-r--r--   0        0        0    56710 2023-03-09 18:53:43.696089 dataknobs-0.0.2/dataknobs/utils/json_utils.py.002
+-rw-r--r--   0        0        0    38844 2023-03-12 02:44:32.369267 dataknobs-0.0.2/dataknobs/utils/json_utils.py.003
+-rw-r--r--   0        0        0    39879 2023-03-22 16:43:44.020177 dataknobs-0.0.2/dataknobs/utils/json_utils.py.004
+-rw-r--r--   0        0        0    14351 2023-02-10 14:59:17.456062 dataknobs-0.0.2/dataknobs/utils/pandas_utils.py
+-rw-r--r--   0        0        0     9134 2023-03-13 17:34:48.816244 dataknobs-0.0.2/dataknobs/utils/path_group.py.no-add
+-rw-r--r--   0        0        0    11853 2023-03-11 22:32:17.644075 dataknobs-0.0.2/dataknobs/utils/path_sorter.py.del
+-rw-r--r--   0        0        0    13283 2023-02-10 14:59:17.466209 dataknobs-0.0.2/dataknobs/utils/requests_utils.py
+-rw-r--r--   0        0        0     3782 2023-02-10 14:59:17.458516 dataknobs-0.0.2/dataknobs/utils/resource_utils.py
+-rw-r--r--   0        0        0    13186 2023-02-10 14:59:17.469429 dataknobs-0.0.2/dataknobs/utils/sql_utils.py
+-rw-r--r--   0        0        0    23161 2023-04-07 02:48:31.057009 dataknobs-0.0.2/dataknobs/utils/stats_utils.py
+-rw-r--r--   0        0        0     1425 2023-04-07 02:48:31.057298 dataknobs-0.0.2/dataknobs/utils/subprocess_utils.py
+-rw-r--r--   0        0        0     3104 2023-02-10 14:59:17.468140 dataknobs-0.0.2/dataknobs/utils/xml_utils.py
+-rw-r--r--   0        0        0     2878 2023-02-10 14:59:17.477011 dataknobs-0.0.2/dataknobs/xization/0.readme.txt
+-rw-r--r--   0        0        0        0 2023-02-10 14:59:17.477662 dataknobs-0.0.2/dataknobs/xization/__init__.py
+-rw-r--r--   0        0        0    23741 2023-04-07 02:48:31.058125 dataknobs-0.0.2/dataknobs/xization/annotations.py
+-rw-r--r--   0        0        0    32223 2023-04-07 02:48:31.059013 dataknobs-0.0.2/dataknobs/xization/authorities.py
+-rw-r--r--   0        0        0    24670 2023-04-07 02:48:31.059440 dataknobs-0.0.2/dataknobs/xization/lexicon.py
+-rw-r--r--   0        0        0    27391 2023-04-07 02:48:31.060348 dataknobs-0.0.2/dataknobs/xization/masking_tokenizer.py
+-rw-r--r--   0        0        0    14226 2023-02-10 14:59:17.476141 dataknobs-0.0.2/dataknobs/xization/normalize.py
+-rw-r--r--   0        0        0      834 2023-04-17 02:57:56.300566 dataknobs-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3313 1970-01-01 00:00:00.000000 dataknobs-0.0.2/setup.py
+-rw-r--r--   0        0        0     3138 1970-01-01 00:00:00.000000 dataknobs-0.0.2/PKG-INFO
```

### Comparing `dataknobs-0.0.1/LICENSE` & `dataknobs-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.1/README.md` & `dataknobs-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.1/dataknobs/structures/conditional_dict.py` & `dataknobs-0.0.2/dataknobs/structures/conditional_dict.py`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.1/dataknobs/structures/document.py` & `dataknobs-0.0.2/dataknobs/structures/document.py`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.1/dataknobs/structures/tree.py` & `dataknobs-0.0.2/dataknobs/structures/tree.py`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.1/dataknobs/utils/elasticsearch_utils.py` & `dataknobs-0.0.2/dataknobs/utils/elasticsearch_utils.py`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.1/dataknobs/utils/emoji_utils.py` & `dataknobs-0.0.2/dataknobs/utils/emoji_utils.py`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.1/dataknobs/utils/file_utils.py` & `dataknobs-0.0.2/dataknobs/utils/file_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,39 +2,44 @@
 import os
 from typing import Set
 
 
 def filepath_generator(
         rootpath: str,
         descend: bool = True,
-        seen: Set[str] = None
+        seen: Set[str] = None,
+        files_only: bool = True,
 ):  # yields -> str
     '''
     Generate all filepaths under the root path.
 
     :param rootpath: The root path under which to find files.
     :param descend: True to descend into subdirectories
     :param seen: Set of filepaths and/or directories to ignore
+    :param files_only: True to generate only paths to files; False to
+        include paths to directories.
     :yield: Each file path
     '''
     if seen is None:
         seen = set()
     seen.add(rootpath)
     for root, dirs, files in os.walk(rootpath, topdown=True):
+        if not descend and root != rootpath and root in seen:
+            break
         for name in files:
             fpath = os.path.join(root, name)
             if fpath not in seen:
                 seen.add(fpath)
                 yield fpath
-        if descend:
+        if not descend or not files_only:
             for name in dirs:
                 next_root = os.path.join(root, name)
                 if next_root not in seen:
                     seen.add(next_root)
-                    filepath_generator(next_root, descend=True, seen=seen)
+                    yield next_root
 
 
 def fileline_generator(filename: str, rootdir: str = None):
     '''
     Generate lines from the file.
     :param filename: The name of the file.
     :param rootdir: (optional) The directory of the file.
@@ -57,10 +62,16 @@
     '''
     Write the lines to the file.
     :param outfile: The name of the file.
     :param rootdir: (optional) The directory of the file.
     '''
     if rootdir is not None:
         outfile = os.path.join(rootdir, outfile)
-    with open(outfile, 'w', encoding='utf-8') as f:
+    if outfile.endswith('.gz'):
+        open_fn = gzip.open
+        mode = 'wt'
+    else:
+        open_fn = open
+        mode = 'w'
+    with open_fn(outfile, mode=mode, encoding='utf-8') as f:
         for line in sorted(lines):
             print(line, file=f)
```

### Comparing `dataknobs-0.0.1/dataknobs/utils/json_paths.py.002` & `dataknobs-0.0.2/dataknobs/utils/json_paths.py.002`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.1/dataknobs/utils/json_paths.py.del` & `dataknobs-0.0.2/dataknobs/utils/json_paths.py.del`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.1/dataknobs/utils/json_utils.py` & `dataknobs-0.0.2/dataknobs/utils/json_utils.py`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.1/dataknobs/utils/json_utils.py.000` & `dataknobs-0.0.2/dataknobs/utils/json_utils.py.000`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.1/dataknobs/utils/json_utils.py.001` & `dataknobs-0.0.2/dataknobs/utils/json_utils.py.001`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.1/dataknobs/utils/json_utils.py.002` & `dataknobs-0.0.2/dataknobs/utils/json_utils.py.002`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.1/dataknobs/utils/json_utils.py.003` & `dataknobs-0.0.2/dataknobs/utils/json_utils.py.003`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.1/dataknobs/utils/json_utils.py.004` & `dataknobs-0.0.2/dataknobs/utils/json_utils.py.004`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.1/dataknobs/utils/pandas_utils.py` & `dataknobs-0.0.2/dataknobs/utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.1/dataknobs/utils/path_group.py.no-add` & `dataknobs-0.0.2/dataknobs/utils/path_group.py.no-add`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.1/dataknobs/utils/path_sorter.py.del` & `dataknobs-0.0.2/dataknobs/utils/path_sorter.py.del`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.1/dataknobs/utils/requests_utils.py` & `dataknobs-0.0.2/dataknobs/utils/requests_utils.py`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.1/dataknobs/utils/resource_utils.py` & `dataknobs-0.0.2/dataknobs/utils/resource_utils.py`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.1/dataknobs/utils/sql_utils.py` & `dataknobs-0.0.2/dataknobs/utils/sql_utils.py`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.1/dataknobs/utils/stats_utils.py` & `dataknobs-0.0.2/dataknobs/utils/stats_utils.py`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.1/dataknobs/utils/subprocess_utils.py` & `dataknobs-0.0.2/dataknobs/utils/subprocess_utils.py`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.1/dataknobs/utils/xml_utils.py` & `dataknobs-0.0.2/dataknobs/utils/xml_utils.py`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.1/dataknobs/xization/0.readme.txt` & `dataknobs-0.0.2/dataknobs/xization/0.readme.txt`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.1/dataknobs/xization/annotations.py` & `dataknobs-0.0.2/dataknobs/xization/annotations.py`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.1/dataknobs/xization/authorities.py` & `dataknobs-0.0.2/dataknobs/xization/authorities.py`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.1/dataknobs/xization/lexicon.py` & `dataknobs-0.0.2/dataknobs/xization/lexicon.py`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.1/dataknobs/xization/masking_tokenizer.py` & `dataknobs-0.0.2/dataknobs/xization/masking_tokenizer.py`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.1/dataknobs/xization/normalize.py` & `dataknobs-0.0.2/dataknobs/xization/normalize.py`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.1/pyproject.toml` & `dataknobs-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dataknobs"
-version = "0.0.1"
+version = "0.0.2"
 description = "Useful implementations of data structures and design patterns for AI knowledge bases."
 authors = ["Spence Koehler <KoehlerSB747@gmail.com>"]
 readme = "README.md"
 packages = [{include = "dataknobs"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `dataknobs-0.0.1/setup.py` & `dataknobs-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  'psycopg2-binary>=2.9.3,<3.0.0',
  'python-dotenv>=0.21.0,<0.22.0',
  'requests>=2.28.1,<3.0.0',
  'scikit-learn>=1.2.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'dataknobs',
-    'version': '0.0.1',
+    'version': '0.0.2',
     'description': 'Useful implementations of data structures and design patterns for AI knowledge bases.',
     'long_description': 'DataKnobs\n=============================\n\n## Description\n\nUseful implementations of data structures and design patterns for knowledge bases and AI, or the knobs and levers for fine-tuning and leveraging your data.\n\nThis repo also serves as a template or sandbox for development, experimentation, and testing of general data structures, algorithms, and utilities for DS, AI, ML, and NLP.\n\nProvides connectors for other popular text and data processing packages like:\n  * numpy and pandas\n  * nltk\n  * wordnet\n  * postgres\n  * elasticsearch\n\n## General project information\n\nThe purpose of this project is:\n\n  * To provide dependable implementations of useful data structures.\n  * To show examples of design patterns and ways to apply AI concepts.\n  * To prototype tools for delivering a robust DS/AI/ML/NLP utilities library package.\n  * To facilitate interactive development, demonstration, visualization, and testing of the library components via jupter notebooks and/or scripts.\n\n## Installation and Usage\n\n```bash/python\n% pip install dataknobs\n% python\n>>> import dataknobs as dk\n>>> ...\n```\n\n\n## Development\n\n### Development machine prerequisites\n\nThe following minimum configuration should exist for development:\n\n  * tox\n  * pyenv\n     * pyenv install 3.9\n  * poetry\n\nWith optional:\n\n  * docker\n  * bash\n\nBy convention, a data directory can be leveraged for development that is mounted as a shared volumne in Docker as /data. This has the default of $HOME/data, but can be overridden with the DATADIR environment variable.\n\n\n### Development quickstart guide\n\n  * In a terminal, clone the repo and cd into the project directory.\n\n#### Testing\n\n  * Tests and Lint: "tox"\n  * Just unit tests: "tox -e tests"\n  * Just lint: "tox -e lint"\n\n#### Using docker\n\n  * Development:\n```\n% tox -e dev\n# poetry shell\n# python\n```\n\n  * Notebook:\n    * execute "tox -e nb"\n      * copy/paste url into browser\n\n#### Using virtual environments\n\n  * Development:\n    * Manual: source ".project_vars", poetry install, poetry shell\n    * Automated: execute "bin/start_dev.sh"  (requires "/bin/bash" on your machine)\n\n  * Notebook:\n    * execute "bin/start_notebook.sh"\n      * copy/paste url into browser\n',
     'author': 'Spence Koehler',
     'author_email': 'KoehlerSB747@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `dataknobs-0.0.1/PKG-INFO` & `dataknobs-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataknobs
-Version: 0.0.1
+Version: 0.0.2
 Summary: Useful implementations of data structures and design patterns for AI knowledge bases.
 Author: Spence Koehler
 Author-email: KoehlerSB747@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

