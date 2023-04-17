# Comparing `tmp/cylc-sphinx-extensions-1.4.1.tar.gz` & `tmp/cylc-sphinx-extensions-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cylc-sphinx-extensions-1.4.1.tar", last modified: Wed Jul 27 11:00:46 2022, max compression
+gzip compressed data, was "dist/cylc-sphinx-extensions-1.4.2.tar", last modified: Mon Apr 17 09:46:01 2023, max compression
```

## Comparing `cylc-sphinx-extensions-1.4.1.tar` & `cylc-sphinx-extensions-1.4.2.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 11:00:46.000000 cylc-sphinx-extensions-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (121)     2615 2022-07-27 11:00:46.000000 cylc-sphinx-extensions-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2328 2022-07-27 10:59:54.000000 cylc-sphinx-extensions-1.4.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 11:00:46.000000 cylc-sphinx-extensions-1.4.1/cylc/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 11:00:46.000000 cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/
--rw-r--r--   0 runner    (1001) docker     (121)     3466 2022-07-27 10:59:54.000000 cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 11:00:46.000000 cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/cylc_lang/
--rw-r--r--   0 runner    (1001) docker     (121)     5285 2022-07-27 10:59:54.000000 cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/cylc_lang/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9219 2022-07-27 10:59:54.000000 cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/cylc_lang/autodocumenters.py
--rw-r--r--   0 runner    (1001) docker     (121)    21012 2022-07-27 10:59:54.000000 cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/cylc_lang/domains.py
--rw-r--r--   0 runner    (1001) docker     (121)    10290 2022-07-27 10:59:54.000000 cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/cylc_lang/lexers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 11:00:46.000000 cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/cylc_lang/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     6674 2022-07-27 10:59:54.000000 cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/cylc_lang/tests/test_autodocumenters.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 11:00:46.000000 cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/diff_selection/
--rw-r--r--   0 runner    (1001) docker     (121)      744 2022-07-27 10:59:54.000000 cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/diff_selection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 11:00:46.000000 cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/diff_selection/_static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 11:00:46.000000 cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/diff_selection/_static/css/
--rw-r--r--   0 runner    (1001) docker     (121)     1424 2022-07-27 10:59:54.000000 cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/diff_selection/_static/css/diff_selector.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 11:00:46.000000 cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/diff_selection/_static/js/
--rw-r--r--   0 runner    (1001) docker     (121)     4785 2022-07-27 10:59:54.000000 cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/diff_selection/_static/js/diff_selector.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 11:00:46.000000 cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/grid_table/
--rw-r--r--   0 runner    (1001) docker     (121)      743 2022-07-27 10:59:54.000000 cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/grid_table/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 11:00:46.000000 cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/grid_table/_static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 11:00:46.000000 cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/grid_table/_static/css/
--rw-r--r--   0 runner    (1001) docker     (121)     1785 2022-07-27 10:59:54.000000 cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/grid_table/_static/css/grid_table.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 11:00:46.000000 cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/hieroglyph_addons/
--rw-r--r--   0 runner    (1001) docker     (121)     1005 2022-07-27 10:59:54.000000 cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/hieroglyph_addons/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 11:00:46.000000 cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/hieroglyph_addons/_static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 11:00:46.000000 cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/hieroglyph_addons/_static/css/
--rw-r--r--   0 runner    (1001) docker     (121)      690 2022-07-27 10:59:54.000000 cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/hieroglyph_addons/_static/css/hieroglyph_theme_addons.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 11:00:46.000000 cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/literal_sub_include/
--rw-r--r--   0 runner    (1001) docker     (121)     2196 2022-07-27 10:59:54.000000 cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/literal_sub_include/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-07-27 10:59:54.000000 cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/literal_sub_include/directives.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 11:00:46.000000 cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/minicylc/
--rw-r--r--   0 runner    (1001) docker     (121)     3126 2022-07-27 10:59:54.000000 cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/minicylc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 11:00:46.000000 cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/minicylc/_static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 11:00:46.000000 cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/minicylc/_static/js/
--rw-r--r--   0 runner    (1001) docker     (121)     9783 2022-07-27 10:59:54.000000 cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/minicylc/_static/js/minicylc.js
--rw-r--r--   0 runner    (1001) docker     (121)     8775 2022-07-27 10:59:54.000000 cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/minicylc/minicylc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 11:00:46.000000 cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/practical/
--rw-r--r--   0 runner    (1001) docker     (121)     2884 2022-07-27 10:59:54.000000 cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/practical/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 11:00:46.000000 cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/practical/_static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 11:00:46.000000 cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/practical/_static/css/
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-07-27 10:59:54.000000 cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/practical/_static/css/tutorial.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 11:00:46.000000 cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/practical/_static/js/
--rw-r--r--   0 runner    (1001) docker     (121)     2313 2022-07-27 10:59:54.000000 cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/practical/_static/js/spoiler.js
--rw-r--r--   0 runner    (1001) docker     (121)     3117 2022-07-27 10:59:54.000000 cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/practical/admonitions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 11:00:46.000000 cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/rst_example/
--rw-r--r--   0 runner    (1001) docker     (121)     1425 2022-07-27 10:59:54.000000 cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/rst_example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1682 2022-07-27 10:59:54.000000 cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/rst_example/directives.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 11:00:46.000000 cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/rtd_theme_addons/
--rw-r--r--   0 runner    (1001) docker     (121)     1505 2022-07-27 10:59:54.000000 cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/rtd_theme_addons/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 11:00:46.000000 cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/rtd_theme_addons/_static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 11:00:46.000000 cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/rtd_theme_addons/_static/css/
--rw-r--r--   0 runner    (1001) docker     (121)     3628 2022-07-27 10:59:54.000000 cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/rtd_theme_addons/_static/css/addons.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 11:00:46.000000 cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/rtd_theme_addons/_static/js/
--rw-r--r--   0 runner    (1001) docker     (121)     1299 2022-07-27 10:59:54.000000 cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/rtd_theme_addons/_static/js/addons.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 11:00:46.000000 cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/sub_lang/
--rw-r--r--   0 runner    (1001) docker     (121)     1451 2022-07-27 10:59:54.000000 cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/sub_lang/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1395 2022-07-27 10:59:54.000000 cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/sub_lang/lexer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 11:00:46.000000 cylc-sphinx-extensions-1.4.1/cylc_sphinx_extensions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2615 2022-07-27 11:00:46.000000 cylc-sphinx-extensions-1.4.1/cylc_sphinx_extensions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1570 2022-07-27 11:00:46.000000 cylc-sphinx-extensions-1.4.1/cylc_sphinx_extensions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-27 11:00:46.000000 cylc-sphinx-extensions-1.4.1/cylc_sphinx_extensions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      227 2022-07-27 11:00:46.000000 cylc-sphinx-extensions-1.4.1/cylc_sphinx_extensions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-07-27 11:00:46.000000 cylc-sphinx-extensions-1.4.1/cylc_sphinx_extensions.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-27 11:00:46.000000 cylc-sphinx-extensions-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2232 2022-07-27 10:59:54.000000 cylc-sphinx-extensions-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:46:01.000000 cylc-sphinx-extensions-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-04-17 09:46:01.000000 cylc-sphinx-extensions-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-04-17 09:45:28.000000 cylc-sphinx-extensions-1.4.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:46:01.000000 cylc-sphinx-extensions-1.4.2/cylc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:46:01.000000 cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-04-17 09:45:28.000000 cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:46:01.000000 cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/cylc_lang/
+-rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-04-17 09:45:28.000000 cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/cylc_lang/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9219 2023-04-17 09:45:28.000000 cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/cylc_lang/autodocumenters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21020 2023-04-17 09:45:28.000000 cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/cylc_lang/domains.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10290 2023-04-17 09:45:28.000000 cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/cylc_lang/lexers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:46:01.000000 cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/cylc_lang/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-04-17 09:45:28.000000 cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/cylc_lang/tests/test_autodocumenters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:46:01.000000 cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/diff_selection/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-17 09:45:28.000000 cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/diff_selection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:46:01.000000 cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/diff_selection/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:46:01.000000 cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/diff_selection/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-04-17 09:45:28.000000 cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/diff_selection/_static/css/diff_selector.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:46:01.000000 cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/diff_selection/_static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-04-17 09:45:28.000000 cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/diff_selection/_static/js/diff_selector.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:46:01.000000 cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/grid_table/
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-17 09:45:28.000000 cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/grid_table/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:46:01.000000 cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/grid_table/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:46:01.000000 cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/grid_table/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-04-17 09:45:28.000000 cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/grid_table/_static/css/grid_table.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:46:01.000000 cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/hieroglyph_addons/
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-17 09:45:28.000000 cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/hieroglyph_addons/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:46:01.000000 cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/hieroglyph_addons/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:46:01.000000 cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/hieroglyph_addons/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-17 09:45:28.000000 cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/hieroglyph_addons/_static/css/hieroglyph_theme_addons.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:46:01.000000 cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/literal_sub_include/
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-17 09:45:28.000000 cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/literal_sub_include/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-04-17 09:45:28.000000 cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/literal_sub_include/directives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:46:01.000000 cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/minicylc/
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-04-17 09:45:28.000000 cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/minicylc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:46:01.000000 cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/minicylc/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:46:01.000000 cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/minicylc/_static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    10921 2023-04-17 09:45:28.000000 cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/minicylc/_static/js/minicylc.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8775 2023-04-17 09:45:28.000000 cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/minicylc/minicylc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:46:01.000000 cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/practical/
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-04-17 09:45:28.000000 cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/practical/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:46:01.000000 cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/practical/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:46:01.000000 cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/practical/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-17 09:45:28.000000 cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/practical/_static/css/tutorial.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:46:01.000000 cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/practical/_static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-04-17 09:45:28.000000 cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/practical/_static/js/spoiler.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-04-17 09:45:28.000000 cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/practical/admonitions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:46:01.000000 cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/rst_example/
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-17 09:45:28.000000 cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/rst_example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-04-17 09:45:28.000000 cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/rst_example/directives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:46:01.000000 cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/rtd_theme_addons/
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-17 09:45:28.000000 cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/rtd_theme_addons/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:46:01.000000 cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/rtd_theme_addons/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:46:01.000000 cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/rtd_theme_addons/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-04-17 09:45:28.000000 cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/rtd_theme_addons/_static/css/addons.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:46:01.000000 cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/rtd_theme_addons/_static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-04-17 09:45:28.000000 cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/rtd_theme_addons/_static/js/addons.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:46:01.000000 cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/sub_lang/
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-17 09:45:28.000000 cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/sub_lang/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-17 09:45:28.000000 cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/sub_lang/lexer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:46:01.000000 cylc-sphinx-extensions-1.4.2/cylc_sphinx_extensions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-04-17 09:46:01.000000 cylc-sphinx-extensions-1.4.2/cylc_sphinx_extensions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-04-17 09:46:01.000000 cylc-sphinx-extensions-1.4.2/cylc_sphinx_extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 09:46:01.000000 cylc-sphinx-extensions-1.4.2/cylc_sphinx_extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-17 09:46:01.000000 cylc-sphinx-extensions-1.4.2/cylc_sphinx_extensions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-17 09:46:01.000000 cylc-sphinx-extensions-1.4.2/cylc_sphinx_extensions.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 09:46:01.000000 cylc-sphinx-extensions-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-17 09:45:28.000000 cylc-sphinx-extensions-1.4.2/setup.py
```

### Comparing `cylc-sphinx-extensions-1.4.1/PKG-INFO` & `cylc-sphinx-extensions-1.4.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cylc-sphinx-extensions
-Version: 1.4.1
+Version: 1.4.2
 Summary: Sphinx extensions for documenting Cylc
 License: GPL
 Provides-Extra: cylc_lang
 Provides-Extra: hieroglyph_addons
 Provides-Extra: rtd_theme_addons
 Provides-Extra: sub_lang
 Provides-Extra: test
@@ -78,15 +78,15 @@
    $ pycodestyle .  # python
    $ eslint cylc/   # javascript
 
 
 Copyright and Terms of Use
 --------------------------
 
-Copyright (C) 2008-2022 NIWA & British Crown (Met Office) & Contributors.
+Copyright (C) 2008-2023 NIWA & British Crown (Met Office) & Contributors.
 
 Cylc is free software: you can redistribute it and/or modify it under the terms
 of the GNU General Public License as published by the Free Software Foundation,
 either version 3 of the License, or (at your option) any later version.
 
 Cylc is distributed in the hope that it will be useful, but WITHOUT ANY
 WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
```

### Comparing `cylc-sphinx-extensions-1.4.1/README.rst` & `cylc-sphinx-extensions-1.4.2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
    $ pycodestyle .  # python
    $ eslint cylc/   # javascript
 
 
 Copyright and Terms of Use
 --------------------------
 
-Copyright (C) 2008-2022 NIWA & British Crown (Met Office) & Contributors.
+Copyright (C) 2008-2023 NIWA & British Crown (Met Office) & Contributors.
 
 Cylc is free software: you can redistribute it and/or modify it under the terms
 of the GNU General Public License as published by the Free Software Foundation,
 either version 3 of the License, or (at your option) any later version.
 
 Cylc is distributed in the hope that it will be useful, but WITHOUT ANY
 WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
```

### Comparing `cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/__init__.py` & `cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 
 from pathlib import Path
 import os
 from shutil import copyfile
 
 
-__version__ = '1.4.1'
+__version__ = '1.4.2'
 
 
 # map sub directory name to the name of the sphinx registration function
 # which should be called to include the static resource
 STATIC_BINDINGS = [
     # (sub_dir, name_of_registration_function)
     ('css', 'add_css_file'),
```

### Comparing `cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/cylc_lang/__init__.py` & `cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/cylc_lang/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/cylc_lang/autodocumenters.py` & `cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/cylc_lang/autodocumenters.py`

 * *Files identical despite different names*

### Comparing `cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/cylc_lang/domains.py` & `cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/cylc_lang/domains.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from sphinx.util.nodes import make_refnode
 
 
 DEFAULT_SCOPE = 'flow.cylc'
 
 KEYS = {
     'conf': lambda s: f'{s}',
-    'section': lambda l: ''.join(f'[{s}]' for s in l),
+    'section': lambda part: ''.join(f'[{s}]' for s in part),
     'setting': lambda s: s,
     'value': lambda s: f'={s}'
 }
 
 # NOTE we allow `<...>` because this is used for custom sections
 # (i.e. for `__MANY__` items)
 CYLC_WORD = r'''
@@ -550,15 +550,15 @@
             name = detokenise(tokens)
             dispname = name
             for type_ in reversed(list(KEYS)):
                 if type_ in tokens and tokens[type_]:
                     break
             anchor = name
             priority = 1
-            yield(
+            yield (
                 name,
                 dispname,
                 type_,
                 docname,
                 anchor,
                 priority
             )
@@ -699,15 +699,15 @@
 
     def get_objects(self):
         for tokens, docname in self.data['objects'].items():
             name = tokens[-1]
             dispname = name
             anchor = name
             priority = 1
-            yield(
+            yield (
                 name,
                 dispname,
                 'type',
                 docname,
                 anchor,
                 priority
             )
```

### Comparing `cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/cylc_lang/lexers.py` & `cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/cylc_lang/lexers.py`

 * *Files identical despite different names*

### Comparing `cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/cylc_lang/tests/test_autodocumenters.py` & `cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/cylc_lang/tests/test_autodocumenters.py`

 * *Files identical despite different names*

### Comparing `cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/diff_selection/__init__.py` & `cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/diff_selection/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/diff_selection/_static/css/diff_selector.css` & `cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/diff_selection/_static/css/diff_selector.css`

 * *Files identical despite different names*

### Comparing `cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/diff_selection/_static/js/diff_selector.js` & `cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/diff_selection/_static/js/diff_selector.js`

 * *Files identical despite different names*

### Comparing `cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/grid_table/__init__.py` & `cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/grid_table/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/grid_table/_static/css/grid_table.css` & `cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/grid_table/_static/css/grid_table.css`

 * *Files identical despite different names*

### Comparing `cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/hieroglyph_addons/__init__.py` & `cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/hieroglyph_addons/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/hieroglyph_addons/_static/css/hieroglyph_theme_addons.css` & `cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/hieroglyph_addons/_static/css/hieroglyph_theme_addons.css`

 * *Files identical despite different names*

### Comparing `cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/literal_sub_include/__init__.py` & `cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/literal_sub_include/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/literal_sub_include/directives.py` & `cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/literal_sub_include/directives.py`

 * *Files identical despite different names*

### Comparing `cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/minicylc/__init__.py` & `cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/minicylc/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/minicylc/_static/js/minicylc.js` & `cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/minicylc/_static/js/minicylc.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -17,14 +17,24 @@
  * ------------------------------------------------------------------------- */
 
 /*eslint no-console: off*/
 
 // Default Cylc colour theme.
 var minicylc_default_theme = {
     'waiting_fill': 'none',
+    'waiting_stroke': 'black',
+    'running_fill': '#55c3e5ff',
+    'running_stroke': 'black',
+    'succeed_fill': '#64c77eff',
+    'succeed_stroke': 'black'
+}
+
+// Old Cylc 7 theme.
+var minicylc_cylc7_theme = {
+    'waiting_fill': 'none',
     'waiting_stroke': '#88c6ff',
     'running_fill': '#00c410',
     'running_stroke': 'black',
     'succeed_fill': '#ada5a5',
     'succeed_stroke': 'black'
 }
 
@@ -47,36 +57,70 @@
      */
 
     constructor(div) {
         /**
          * Initiate the object.
          * @param div The <div> element containing the SVG.
          * */
+        this.div = div;
+        this.load();
+    }
+
+    load() {
+        /**
+         * Obtain nodes and edges from svg.
+         *
+         * This function calls itself recursively until the SVG is loaded.
+         *
+         * This function starts the animation when finished.
+         */
+        const svg = ($(this.div).find('object:first')[0]).contentDocument;
+        const self = this;
+
+        if (!svg) {
+            console.log('Wait for SVG load: Gecko');
+            // this retry loop works for Firefox, etc
+            setTimeout(function() {
+                self.load();
+            }, 500)
+            return;
+        }
+        var eles = $(svg).find('g');
+        if (!eles.length) {
+            console.log('Wait for SVG load: Blink');
+            // this retry loop works for Chrome, etc
+            setTimeout(function() {
+                self.load();
+            }, 500)
+            return;
+        }
 
-        // Obtain nodes and edges from svg.
-        var svg = ($(div).find('object:first')[0]).contentDocument;
         this._find_svg_elements(svg);
 
         // Parse dependencies.
-        var deps = this._get_dependencies_from_graph(div);
+        var deps = this._get_dependencies_from_graph(this.div);
         this._construct_dependency_map(deps);
 
         // Process colour theme.
-        this.setup_colours($(div).data('theme'));
+        this.setup_colours($(this.div).data('theme'));
+
+        this.run()
     }
 
     setup_colours(theme) {
         /**
          * Set the colour theme.
          * @param theme The name of a colour theme as a string.
          */
         if (!theme || theme == 'default') {
             this.theme = minicylc_default_theme;
         } else if (theme == 'demo') {
             this.theme = minicylc_demo_theme;
+        } else if (theme == 'cylc7') {
+            this.theme = minicylc_cylc7_theme;
         } else {
             console.log('Warning: Invalid theme detected "' + theme +
                 '", defaulting to black.');
             this.theme = {};
         }
     }
 
@@ -85,15 +129,15 @@
          * Associate task/dependency names with SVG nodes.
          *
          * Associations stored as dictionaries this.nodes and this.edges.
          * @param svg The <svg> element containing the workflow.
          */
         var nodes = {};
         var edges = {};
-        $(svg).find('.graph g').each(function() {
+        $(svg).find('g').each(function() {
             var node = $(this)[0];
             var node_class = $(node).attr('class');
             if (node_class == 'node') {
                 nodes[node.textContent.trim().split('\n')[0]] = node;
             } else if (node_class == 'edge') {
                 edges[node.textContent.trim().split('\n')[0]] = node;
             }
@@ -113,15 +157,15 @@
         var parts;
         for (let dep of $(div).data('dependencies').split('//')) {
             parts = dep.split('=>');
             if (parts.length == 0) {
                 continue; // Graph line does not contain a dependency => skip.
             }
             for (ind = 0; ind < parts.length - 1; ind++) {
-                deps.push([parts[ind], parts[ind + 1]]); // [left, right].
+                deps.push([parts[ind].trim(), parts[ind + 1].trim()]); // [left, right].
             }
         }
 
         return deps;
     }
 
     _construct_dependency_map(deps) {
@@ -301,10 +345,10 @@
 }
 
 
 // Activate minicylc.
 $(document).ready(function() {
     $('.minicylc').each(function() {
         var obj = this;
-        new MiniCylc(obj).run();
+        new MiniCylc(obj);
     });
 });
```

### Comparing `cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/minicylc/minicylc.py` & `cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/minicylc/minicylc.py`

 * *Files identical despite different names*

### Comparing `cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/practical/__init__.py` & `cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/practical/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/practical/_static/js/spoiler.js` & `cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/practical/_static/js/spoiler.js`

 * *Files identical despite different names*

### Comparing `cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/practical/admonitions.py` & `cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/practical/admonitions.py`

 * *Files identical despite different names*

### Comparing `cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/rst_example/__init__.py` & `cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/rst_example/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/rst_example/directives.py` & `cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/rst_example/directives.py`

 * *Files identical despite different names*

### Comparing `cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/rtd_theme_addons/__init__.py` & `cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/rtd_theme_addons/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/rtd_theme_addons/_static/css/addons.css` & `cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/rtd_theme_addons/_static/css/addons.css`

 * *Files identical despite different names*

### Comparing `cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/rtd_theme_addons/_static/js/addons.js` & `cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/rtd_theme_addons/_static/js/addons.js`

 * *Files identical despite different names*

### Comparing `cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/sub_lang/__init__.py` & `cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/sub_lang/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-sphinx-extensions-1.4.1/cylc/sphinx_ext/sub_lang/lexer.py` & `cylc-sphinx-extensions-1.4.2/cylc/sphinx_ext/sub_lang/lexer.py`

 * *Files identical despite different names*

### Comparing `cylc-sphinx-extensions-1.4.1/cylc_sphinx_extensions.egg-info/PKG-INFO` & `cylc-sphinx-extensions-1.4.2/cylc_sphinx_extensions.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cylc-sphinx-extensions
-Version: 1.4.1
+Version: 1.4.2
 Summary: Sphinx extensions for documenting Cylc
 License: GPL
 Provides-Extra: cylc_lang
 Provides-Extra: hieroglyph_addons
 Provides-Extra: rtd_theme_addons
 Provides-Extra: sub_lang
 Provides-Extra: test
@@ -78,15 +78,15 @@
    $ pycodestyle .  # python
    $ eslint cylc/   # javascript
 
 
 Copyright and Terms of Use
 --------------------------
 
-Copyright (C) 2008-2022 NIWA & British Crown (Met Office) & Contributors.
+Copyright (C) 2008-2023 NIWA & British Crown (Met Office) & Contributors.
 
 Cylc is free software: you can redistribute it and/or modify it under the terms
 of the GNU General Public License as published by the Free Software Foundation,
 either version 3 of the License, or (at your option) any later version.
 
 Cylc is distributed in the hope that it will be useful, but WITHOUT ANY
 WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
```

### Comparing `cylc-sphinx-extensions-1.4.1/cylc_sphinx_extensions.egg-info/SOURCES.txt` & `cylc-sphinx-extensions-1.4.2/cylc_sphinx_extensions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cylc-sphinx-extensions-1.4.1/setup.py` & `cylc-sphinx-extensions-1.4.2/setup.py`

 * *Files identical despite different names*

