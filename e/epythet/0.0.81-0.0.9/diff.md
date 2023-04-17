# Comparing `tmp/epythet-0.0.81.tar.gz` & `tmp/epythet-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epythet-0.0.81.tar", last modified: Mon Apr 17 18:26:22 2023, max compression
+gzip compressed data, was "dist/epythet-0.0.9.tar", last modified: Wed Oct  7 19:34:38 2020, max compression
```

## Comparing `epythet-0.0.81.tar` & `epythet-0.0.9.tar`

### file list

```diff
@@ -1,34 +1,18 @@
-drwxr-xr-x   0 vferon   (1311931687) staff       (20)        0 2023-04-17 18:26:22.426588 epythet-0.0.81/
--rw-r--r--   0 vferon   (1311931687) staff       (20)    11357 2022-06-08 22:47:41.000000 epythet-0.0.81/LICENSE
--rw-r--r--   0 vferon   (1311931687) staff       (20)      177 2022-06-08 22:47:41.000000 epythet-0.0.81/MANIFEST.in
--rw-r--r--   0 vferon   (1311931687) staff       (20)     2163 2023-04-17 18:26:22.426778 epythet-0.0.81/PKG-INFO
--rw-r--r--   0 vferon   (1311931687) staff       (20)     1821 2023-03-20 22:48:43.000000 epythet-0.0.81/README.md
-drwxr-xr-x   0 vferon   (1311931687) staff       (20)        0 2023-04-17 18:26:22.410899 epythet-0.0.81/epythet/
--rw-r--r--   0 vferon   (1311931687) staff       (20)     3533 2022-06-08 22:47:42.000000 epythet-0.0.81/epythet/__init__.py
-drwxr-xr-x   0 vferon   (1311931687) staff       (20)        0 2023-04-17 18:26:22.402971 epythet-0.0.81/epythet/_static/
-drwxr-xr-x   0 vferon   (1311931687) staff       (20)        0 2023-04-17 18:26:22.418385 epythet-0.0.81/epythet/_static/docsrc/
--rw-r--r--   0 vferon   (1311931687) staff       (20)        8 2022-06-08 22:47:42.000000 epythet-0.0.81/epythet/_static/docsrc/.gitignore
--rw-r--r--   0 vferon   (1311931687) staff       (20)      897 2022-06-08 22:47:42.000000 epythet-0.0.81/epythet/_static/docsrc/Makefile
--rw-r--r--   0 vferon   (1311931687) staff       (20)     3033 2022-06-08 22:47:42.000000 epythet-0.0.81/epythet/_static/docsrc/conf.py
--rw-r--r--   0 vferon   (1311931687) staff       (20)      795 2022-06-08 22:47:42.000000 epythet-0.0.81/epythet/_static/docsrc/make.bat
--rw-r--r--   0 vferon   (1311931687) staff       (20)     5032 2022-06-08 22:47:42.000000 epythet-0.0.81/epythet/autogen.py
--rw-r--r--   0 vferon   (1311931687) staff       (20)      446 2022-06-08 22:47:42.000000 epythet-0.0.81/epythet/call_make.py
--rw-r--r--   0 vferon   (1311931687) staff       (20)     1141 2022-06-08 22:47:42.000000 epythet-0.0.81/epythet/cli.py
--rw-r--r--   0 vferon   (1311931687) staff       (20)     1013 2022-06-08 22:47:42.000000 epythet-0.0.81/epythet/config_parser.py
--rw-r--r--   0 vferon   (1311931687) staff       (20)      156 2022-06-08 22:47:42.000000 epythet-0.0.81/epythet/docs_gen.py
--rw-r--r--   0 vferon   (1311931687) staff       (20)     1829 2022-06-08 22:47:42.000000 epythet-0.0.81/epythet/setup_docsrc.py
--rw-r--r--   0 vferon   (1311931687) staff       (20)     2971 2022-06-08 22:47:42.000000 epythet-0.0.81/epythet/templates.py
-drwxr-xr-x   0 vferon   (1311931687) staff       (20)        0 2023-04-17 18:26:22.426034 epythet-0.0.81/epythet/tools/
--rw-r--r--   0 vferon   (1311931687) staff       (20)     3770 2022-06-08 22:47:42.000000 epythet-0.0.81/epythet/tools/__init__.py
--rw-r--r--   0 vferon   (1311931687) staff       (20)    12021 2022-06-08 22:47:42.000000 epythet-0.0.81/epythet/tools/docstring_diagnosis.py
--rw-r--r--   0 vferon   (1311931687) staff       (20)     4584 2022-06-08 22:47:42.000000 epythet-0.0.81/epythet/tools/published_docs.py
-drwxr-xr-x   0 vferon   (1311931687) staff       (20)        0 2023-04-17 18:26:22.415566 epythet-0.0.81/epythet.egg-info/
--rw-r--r--   0 vferon   (1311931687) staff       (20)     2163 2023-04-17 18:26:22.000000 epythet-0.0.81/epythet.egg-info/PKG-INFO
--rw-r--r--   0 vferon   (1311931687) staff       (20)      655 2023-04-17 18:26:22.000000 epythet-0.0.81/epythet.egg-info/SOURCES.txt
--rw-r--r--   0 vferon   (1311931687) staff       (20)        1 2023-04-17 18:26:22.000000 epythet-0.0.81/epythet.egg-info/dependency_links.txt
--rw-r--r--   0 vferon   (1311931687) staff       (20)       52 2023-04-17 18:26:22.000000 epythet-0.0.81/epythet.egg-info/entry_points.txt
--rw-r--r--   0 vferon   (1311931687) staff       (20)        1 2023-04-17 18:21:13.000000 epythet-0.0.81/epythet.egg-info/not-zip-safe
--rw-r--r--   0 vferon   (1311931687) staff       (20)      141 2023-04-17 18:26:22.000000 epythet-0.0.81/epythet.egg-info/requires.txt
--rw-r--r--   0 vferon   (1311931687) staff       (20)        8 2023-04-17 18:26:22.000000 epythet-0.0.81/epythet.egg-info/top_level.txt
--rw-r--r--   0 vferon   (1311931687) staff       (20)      875 2023-04-17 18:26:22.427898 epythet-0.0.81/setup.cfg
--rw-r--r--   0 vferon   (1311931687) staff       (20)       91 2022-06-08 22:47:42.000000 epythet-0.0.81/setup.py
+drwxr-xr-x   0 twhalen    (502) staff       (20)        0 2020-10-07 19:34:38.277929 epythet-0.0.9/
+-rw-r--r--   0 twhalen    (502) staff       (20)       82 2020-09-30 23:55:15.000000 epythet-0.0.9/MANIFEST.in
+-rw-r--r--   0 twhalen    (502) staff       (20)      450 2020-10-07 19:34:38.278145 epythet-0.0.9/PKG-INFO
+-rw-r--r--   0 twhalen    (502) staff       (20)      102 2020-08-22 01:19:00.000000 epythet-0.0.9/README.md
+drwxr-xr-x   0 twhalen    (502) staff       (20)        0 2020-10-07 19:34:38.267713 epythet-0.0.9/epythet/
+drwxr-xr-x   0 twhalen    (502) staff       (20)        0 2020-10-07 19:34:38.267815 epythet-0.0.9/epythet/docs_gen/
+drwxr-xr-x   0 twhalen    (502) staff       (20)        0 2020-10-07 19:34:38.267920 epythet-0.0.9/epythet/docs_gen/_static/
+drwxr-xr-x   0 twhalen    (502) staff       (20)        0 2020-10-07 19:34:38.277206 epythet-0.0.9/epythet/docs_gen/_static/docsrc/
+-rw-r--r--   0 twhalen    (502) staff       (20)      897 2020-09-30 23:55:15.000000 epythet-0.0.9/epythet/docs_gen/_static/docsrc/Makefile
+-rw-r--r--   0 twhalen    (502) staff       (20)     2688 2020-09-30 23:55:15.000000 epythet-0.0.9/epythet/docs_gen/_static/docsrc/conf.py
+-rw-r--r--   0 twhalen    (502) staff       (20)      795 2020-09-30 23:55:15.000000 epythet-0.0.9/epythet/docs_gen/_static/docsrc/make.bat
+drwxr-xr-x   0 twhalen    (502) staff       (20)        0 2020-10-07 19:34:38.273784 epythet-0.0.9/epythet.egg-info/
+-rw-r--r--   0 twhalen    (502) staff       (20)      450 2020-10-07 19:34:38.000000 epythet-0.0.9/epythet.egg-info/PKG-INFO
+-rw-r--r--   0 twhalen    (502) staff       (20)      286 2020-10-07 19:34:38.000000 epythet-0.0.9/epythet.egg-info/SOURCES.txt
+-rw-r--r--   0 twhalen    (502) staff       (20)        1 2020-10-07 19:34:38.000000 epythet-0.0.9/epythet.egg-info/dependency_links.txt
+-rw-r--r--   0 twhalen    (502) staff       (20)        1 2020-10-07 19:34:38.000000 epythet-0.0.9/epythet.egg-info/top_level.txt
+-rw-r--r--   0 twhalen    (502) staff       (20)      544 2020-10-07 19:34:38.279224 epythet-0.0.9/setup.cfg
+-rw-r--r--   0 twhalen    (502) staff       (20)      327 2020-10-06 21:46:19.000000 epythet-0.0.9/setup.py
```

### Comparing `epythet-0.0.81/epythet/_static/docsrc/Makefile` & `epythet-0.0.9/epythet/docs_gen/_static/docsrc/Makefile`

 * *Files identical despite different names*

### Comparing `epythet-0.0.81/epythet/_static/docsrc/conf.py` & `epythet-0.0.9/epythet/docs_gen/_static/docsrc/conf.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,37 +12,42 @@
 
 import os
 import sys
 
 sys.path.insert(0, os.path.abspath('..'))
 
 # -- Project information -----------------------------------------------------
-from epythet.config_parser import parse_config
+from configparser import ConfigParser
 from pathlib import Path
 
-project, copyright, author, release, display_name = parse_config(
-    Path(__file__).absolute().parent.parent / 'setup.cfg'
-)
+config_file = Path(__file__).absolute().parent.parent / 'setup.cfg'  # same folder as setup.py
+config = ConfigParser()
+config.read_file(open(config_file, 'r'))
+
+project = config['metadata']['name']
+copyright = config['metadata']['copyright']
+author = config['metadata']['author']
+
+# The full version, including alpha/beta/rc tags
+release = config['metadata']['version']
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
-    'sphinx_toggleprompt',
-    'sphinx_copybutton',
     'sphinx.ext.autodoc',  # Include documentation from docstrings
     'sphinx.ext.doctest',  # Test snippets in the documentation
     'sphinx.ext.githubpages',  # This extension creates .nojekyll file
     'sphinx.ext.graphviz',  # Add Graphviz graphs
     'sphinx.ext.napoleon',  # Support for NumPy and Google style docstrings
     'sphinx.ext.todo',  # Support for todo items
     'sphinx.ext.viewcode',  # Add links to highlighted source code
-    'myst_parser',  # Parse .md files
+    'recommonmark',  # Parse .md files
 ]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
@@ -50,33 +55,13 @@
 exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = 'sphinx_rtd_theme'
+html_theme = 'alabaster'
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ['_static']
-
-
-# -- Options for Markdown support -------------------------------------------
-# TODO: fix md support so that it doesn't interfere with rst docs
-# import commonmark
-#
-#
-# def docstring(app, what, name, obj, options, lines):
-#     md = '\n'.join(lines)
-#     ast = commonmark.Parser().parse(md)
-#     rst = commonmark.ReStructuredTextRenderer().render(ast)
-#     lines.clear()
-#     lines += rst.splitlines()
-#
-#
-# def setup(app):
-#     app.connect('autodoc-process-docstring', docstring)
-
-
-toggleprompt_offset_right = 30
```

### Comparing `epythet-0.0.81/epythet/_static/docsrc/make.bat` & `epythet-0.0.9/epythet/docs_gen/_static/docsrc/make.bat`

 * *Files identical despite different names*

