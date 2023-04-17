# Comparing `tmp/fig2sketch-0.2.3.tar.gz` & `tmp/fig2sketch-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fig2sketch-0.2.3.tar", last modified: Fri Feb 24 09:57:07 2023, max compression
+gzip compressed data, was "fig2sketch-0.2.4.tar", last modified: Mon Apr 17 09:36:10 2023, max compression
```

## Comparing `fig2sketch-0.2.3.tar` & `fig2sketch-0.2.4.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 09:57:07.293820 fig2sketch-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-02-24 09:56:58.000000 fig2sketch-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-02-24 09:57:07.293820 fig2sketch-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-02-24 09:56:58.000000 fig2sketch-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-02-24 09:56:58.000000 fig2sketch-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-24 09:57:07.293820 fig2sketch-0.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 09:57:07.285820 fig2sketch-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 09:57:07.289820 fig2sketch-0.2.3/src/converter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 09:56:58.000000 fig2sketch-0.2.3/src/converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-02-24 09:56:58.000000 fig2sketch-0.2.3/src/converter/artboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-02-24 09:56:58.000000 fig2sketch-0.2.3/src/converter/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-02-24 09:56:58.000000 fig2sketch-0.2.3/src/converter/component.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-02-24 09:56:58.000000 fig2sketch-0.2.3/src/converter/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-02-24 09:56:58.000000 fig2sketch-0.2.3/src/converter/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-02-24 09:56:58.000000 fig2sketch-0.2.3/src/converter/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-02-24 09:56:58.000000 fig2sketch-0.2.3/src/converter/document.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-02-24 09:56:58.000000 fig2sketch-0.2.3/src/converter/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-02-24 09:56:58.000000 fig2sketch-0.2.3/src/converter/font.py
--rw-r--r--   0 runner    (1001) docker     (123)    34002 2023-02-24 09:56:58.000000 fig2sketch-0.2.3/src/converter/font_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-02-24 09:56:58.000000 fig2sketch-0.2.3/src/converter/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    10554 2023-02-24 09:56:58.000000 fig2sketch-0.2.3/src/converter/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-02-24 09:56:58.000000 fig2sketch-0.2.3/src/converter/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-02-24 09:56:58.000000 fig2sketch-0.2.3/src/converter/page.py
--rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-02-24 09:56:58.000000 fig2sketch-0.2.3/src/converter/positioning.py
--rw-r--r--   0 runner    (1001) docker     (123)     6693 2023-02-24 09:56:58.000000 fig2sketch-0.2.3/src/converter/prototype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-02-24 09:56:58.000000 fig2sketch-0.2.3/src/converter/rectangle.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-02-24 09:56:58.000000 fig2sketch-0.2.3/src/converter/shape.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-02-24 09:56:58.000000 fig2sketch-0.2.3/src/converter/shape_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    12579 2023-02-24 09:56:58.000000 fig2sketch-0.2.3/src/converter/shape_path.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-02-24 09:56:58.000000 fig2sketch-0.2.3/src/converter/slice.py
--rw-r--r--   0 runner    (1001) docker     (123)    10101 2023-02-24 09:56:58.000000 fig2sketch-0.2.3/src/converter/style.py
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-02-24 09:56:58.000000 fig2sketch-0.2.3/src/converter/symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)    12602 2023-02-24 09:56:58.000000 fig2sketch-0.2.3/src/converter/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-02-24 09:56:58.000000 fig2sketch-0.2.3/src/converter/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-02-24 09:56:58.000000 fig2sketch-0.2.3/src/converter/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-02-24 09:56:58.000000 fig2sketch-0.2.3/src/converter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 09:57:07.289820 fig2sketch-0.2.3/src/fig2sketch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-02-24 09:57:07.000000 fig2sketch-0.2.3/src/fig2sketch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-02-24 09:57:07.000000 fig2sketch-0.2.3/src/fig2sketch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 09:57:07.000000 fig2sketch-0.2.3/src/fig2sketch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-02-24 09:57:07.000000 fig2sketch-0.2.3/src/fig2sketch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-02-24 09:57:07.000000 fig2sketch-0.2.3/src/fig2sketch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-02-24 09:57:07.000000 fig2sketch-0.2.3/src/fig2sketch.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     3382 2023-02-24 09:56:58.000000 fig2sketch-0.2.3/src/fig2sketch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 09:57:07.289820 fig2sketch-0.2.3/src/figformat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 09:56:58.000000 fig2sketch-0.2.3/src/figformat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-02-24 09:56:58.000000 fig2sketch-0.2.3/src/figformat/decodefig.py
--rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-02-24 09:56:58.000000 fig2sketch-0.2.3/src/figformat/fig2tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-02-24 09:56:58.000000 fig2sketch-0.2.3/src/figformat/kiwi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-02-24 09:56:58.000000 fig2sketch-0.2.3/src/figformat/vector_network.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 09:57:07.293820 fig2sketch-0.2.3/src/sketchformat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 09:56:58.000000 fig2sketch-0.2.3/src/sketchformat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-02-24 09:56:58.000000 fig2sketch-0.2.3/src/sketchformat/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-02-24 09:56:58.000000 fig2sketch-0.2.3/src/sketchformat/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-02-24 09:56:58.000000 fig2sketch-0.2.3/src/sketchformat/layer_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-02-24 09:56:58.000000 fig2sketch-0.2.3/src/sketchformat/layer_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-02-24 09:56:58.000000 fig2sketch-0.2.3/src/sketchformat/layer_shape.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-02-24 09:56:58.000000 fig2sketch-0.2.3/src/sketchformat/prototype.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 09:57:07.293820 fig2sketch-0.2.3/src/sketchformat/serialize/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-02-24 09:56:58.000000 fig2sketch-0.2.3/src/sketchformat/serialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-02-24 09:56:58.000000 fig2sketch-0.2.3/src/sketchformat/serialize/json.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-02-24 09:56:58.000000 fig2sketch-0.2.3/src/sketchformat/serialize/orjson.py
--rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-02-24 09:56:58.000000 fig2sketch-0.2.3/src/sketchformat/style.py
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-02-24 09:56:58.000000 fig2sketch-0.2.3/src/sketchformat/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:36:10.313639 fig2sketch-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-04-17 09:36:10.313639 fig2sketch-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 09:36:10.313639 fig2sketch-0.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:36:10.305639 fig2sketch-0.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:36:10.309639 fig2sketch-0.2.4/src/converter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/converter/artboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/converter/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/converter/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/converter/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/converter/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/converter/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/converter/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/converter/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/converter/font.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34002 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/converter/font_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/converter/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10554 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/converter/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/converter/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/converter/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/converter/positioning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6693 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/converter/prototype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/converter/rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/converter/shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/converter/shape_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12579 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/converter/shape_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/converter/slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10115 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/converter/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/converter/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12602 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/converter/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/converter/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/converter/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/converter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:36:10.309639 fig2sketch-0.2.4/src/fig2sketch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-04-17 09:36:10.000000 fig2sketch-0.2.4/src/fig2sketch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-17 09:36:10.000000 fig2sketch-0.2.4/src/fig2sketch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 09:36:10.000000 fig2sketch-0.2.4/src/fig2sketch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-17 09:36:10.000000 fig2sketch-0.2.4/src/fig2sketch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-17 09:36:10.000000 fig2sketch-0.2.4/src/fig2sketch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-17 09:36:10.000000 fig2sketch-0.2.4/src/fig2sketch.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3382 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/fig2sketch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:36:10.309639 fig2sketch-0.2.4/src/figformat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/figformat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/figformat/decodefig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/figformat/fig2tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/figformat/kiwi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/figformat/vector_network.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:36:10.313639 fig2sketch-0.2.4/src/sketchformat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/sketchformat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/sketchformat/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/sketchformat/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/sketchformat/layer_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/sketchformat/layer_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/sketchformat/layer_shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/sketchformat/prototype.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:36:10.313639 fig2sketch-0.2.4/src/sketchformat/serialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/sketchformat/serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/sketchformat/serialize/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/sketchformat/serialize/orjson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/sketchformat/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-04-17 09:36:01.000000 fig2sketch-0.2.4/src/sketchformat/text.py
```

### Comparing `fig2sketch-0.2.3/LICENSE` & `fig2sketch-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.3/PKG-INFO` & `fig2sketch-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fig2sketch
-Version: 0.2.3
+Version: 0.2.4
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: fast
 Provides-Extra: dev
 License-File: LICENSE
 
 # .fig to Sketch converter
```

### Comparing `fig2sketch-0.2.3/README.md` & `fig2sketch-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.3/pyproject.toml` & `fig2sketch-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.3/src/converter/artboard.py` & `fig2sketch-0.2.4/src/converter/artboard.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.3/src/converter/base.py` & `fig2sketch-0.2.4/src/converter/base.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.3/src/converter/component.py` & `fig2sketch-0.2.4/src/converter/component.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.3/src/converter/context.py` & `fig2sketch-0.2.4/src/converter/context.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.3/src/converter/convert.py` & `fig2sketch-0.2.4/src/converter/convert.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.3/src/converter/document.py` & `fig2sketch-0.2.4/src/converter/document.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.3/src/converter/font.py` & `fig2sketch-0.2.4/src/converter/font.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.3/src/converter/font_features.py` & `fig2sketch-0.2.4/src/converter/font_features.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.3/src/converter/group.py` & `fig2sketch-0.2.4/src/converter/group.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.3/src/converter/instance.py` & `fig2sketch-0.2.4/src/converter/instance.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.3/src/converter/meta.py` & `fig2sketch-0.2.4/src/converter/meta.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.3/src/converter/page.py` & `fig2sketch-0.2.4/src/converter/page.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.3/src/converter/positioning.py` & `fig2sketch-0.2.4/src/converter/positioning.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.3/src/converter/prototype.py` & `fig2sketch-0.2.4/src/converter/prototype.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.3/src/converter/rectangle.py` & `fig2sketch-0.2.4/src/converter/rectangle.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.3/src/converter/shape_group.py` & `fig2sketch-0.2.4/src/converter/shape_group.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.3/src/converter/shape_path.py` & `fig2sketch-0.2.4/src/converter/shape_path.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.3/src/converter/style.py` & `fig2sketch-0.2.4/src/converter/style.py`

 * *Files 1% similar despite different names*

```diff
@@ -241,26 +241,26 @@
     for e in fig_node.get("effects", []):
         if e["type"] == "INNER_SHADOW":
             sketch["innerShadows"].append(
                 InnerShadow(
                     blurRadius=e["radius"],
                     offsetX=e["offset"]["x"],
                     offsetY=e["offset"]["y"],
-                    spread=e["spread"],
+                    spread=e.get("spread", 0),
                     color=convert_color(e["color"]),
                 )
             )
 
         elif e["type"] == "DROP_SHADOW":
             sketch["shadows"].append(
                 Shadow(
                     blurRadius=e["radius"],
                     offsetX=e["offset"]["x"],
                     offsetY=e["offset"]["y"],
-                    spread=e["spread"],
+                    spread=e.get("spread", 0),
                     color=convert_color(e["color"]),
                 )
             )
 
         elif e["type"] == "FOREGROUND_BLUR":
             if sketch["blur"].isEnabled:
                 utils.log_conversion_warning("STY001", fig_node)
```

### Comparing `fig2sketch-0.2.3/src/converter/symbol.py` & `fig2sketch-0.2.4/src/converter/symbol.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.3/src/converter/text.py` & `fig2sketch-0.2.4/src/converter/text.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.3/src/converter/tree.py` & `fig2sketch-0.2.4/src/converter/tree.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.3/src/converter/user.py` & `fig2sketch-0.2.4/src/converter/user.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.3/src/converter/utils.py` & `fig2sketch-0.2.4/src/converter/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,14 +91,15 @@
     "GRD005": "has a row layout with a set height which is not supported by Sketch. It will be converted to a layout grid taking the whole height of the artboard",
     "GRD006": "has a row layout with an offset that is not supported. The offset will be ignored",
     "GRD007": "has a row layout with non-integer ratio between gutter and row size. The row layout will not be converted",
     "GRD008": "has a row and column layout. The rows will only be as wide as the columns (instead of taking the entire width of the artboard)",
     "IMG001": "appears to be corrupted in the .fig file, it will not be converted. Try passing --force-convert-images to try to convert it anyway",
     "IMG002": "appears to be corrupted in the .fig file, it will not be converted",
     "IMG003": "is missing from the .fig file, it will not be converted",
+    "IMG004": "appears to be corrupted in the .fig file ({error}), it will not be converted",
 }
 
 
 def log_conversion_warning(warning_code: str, fig_node: dict, **kw: list) -> None:
     if fig_node["guid"] not in issued_warnings:
         issued_warnings[fig_node["guid"]] = [warning_code]
     elif warning_code not in issued_warnings[fig_node["guid"]]:
```

### Comparing `fig2sketch-0.2.3/src/fig2sketch.egg-info/PKG-INFO` & `fig2sketch-0.2.4/src/fig2sketch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fig2sketch
-Version: 0.2.3
+Version: 0.2.4
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: fast
 Provides-Extra: dev
 License-File: LICENSE
 
 # .fig to Sketch converter
```

### Comparing `fig2sketch-0.2.3/src/fig2sketch.egg-info/SOURCES.txt` & `fig2sketch-0.2.4/src/fig2sketch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.3/src/fig2sketch.py` & `fig2sketch-0.2.4/src/fig2sketch.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.3/src/figformat/decodefig.py` & `fig2sketch-0.2.4/src/figformat/decodefig.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.3/src/figformat/fig2tree.py` & `fig2sketch-0.2.4/src/figformat/fig2tree.py`

 * *Files 4% similar despite different names*

```diff
@@ -127,7 +127,13 @@
         else:
             utils.log_conversion_warning("IMG001", {"type": "Image", "guid": fname, "name": fname})
 
         return "f2s_corrupted"
     except KeyError:
         utils.log_conversion_warning("IMG003", {"type": "Image", "guid": fname, "name": fname})
         return "f2s_missing"
+    except Exception as e:
+        utils.log_conversion_warning(
+            "IMG004", {"type": "Image", "guid": fname, "name": fname}, error=str(e)
+        )
+
+        return "f2s_corrupted"
```

### Comparing `fig2sketch-0.2.3/src/figformat/kiwi.py` & `fig2sketch-0.2.4/src/figformat/kiwi.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import codecs
 import ctypes
 from collections import OrderedDict
 import zlib
 import struct
 import io
+import logging
 
 
 class KiwiReader:
     def __init__(self, reader):
         self._reader = reader
 
     def byte(self):
@@ -138,21 +139,26 @@
                 case 2:
                     return self._decode_message(kw, type)
                 case other:
                     raise "Unknown"
 
 
 def decode(reader, type_converters):
-    SUPPORTED_VERSIONS = [15, 20]
+    MIN_SUPPORTED_VERSIONS = 15
+    MAX_SUPPORTED_VERSION = 25
 
     header = reader.read(12)
     fig_version = struct.unpack("<I", header[8:12])[0]
-    if fig_version not in SUPPORTED_VERSIONS:
+    if fig_version < MIN_SUPPORTED_VERSIONS:
         raise Exception(
-            f"Unsupported .fig version. File = {fig_version} / Supported = {SUPPORTED_VERSIONS}"
+            f"[FIG002] The .fig file has version {fig_version} which is older than the minimum supported ({MIN_SUPPORTED_VERSIONS}). Cannot convert"
+        )
+    elif fig_version > MAX_SUPPORTED_VERSION:
+        logging.info(
+            f"[FIG001] The .fig file has version {fig_version} which is newer than the maximum supported ({MAX_SUPPORTED_VERSION}). Some new properties may not be correctly converted"
         )
 
     segment_header = reader.read(4)
     size = struct.unpack("<I", segment_header)[0]
     data = io.BytesIO(zlib.decompress(reader.read(size), wbits=-15))
     schema = KiwiSchema(data)
```

### Comparing `fig2sketch-0.2.3/src/figformat/vector_network.py` & `fig2sketch-0.2.4/src/figformat/vector_network.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.3/src/sketchformat/common.py` & `fig2sketch-0.2.4/src/sketchformat/common.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.3/src/sketchformat/document.py` & `fig2sketch-0.2.4/src/sketchformat/document.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.3/src/sketchformat/layer_common.py` & `fig2sketch-0.2.4/src/sketchformat/layer_common.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.3/src/sketchformat/layer_group.py` & `fig2sketch-0.2.4/src/sketchformat/layer_group.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.3/src/sketchformat/layer_shape.py` & `fig2sketch-0.2.4/src/sketchformat/layer_shape.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.3/src/sketchformat/prototype.py` & `fig2sketch-0.2.4/src/sketchformat/prototype.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.3/src/sketchformat/serialize/json.py` & `fig2sketch-0.2.4/src/sketchformat/serialize/json.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.3/src/sketchformat/serialize/orjson.py` & `fig2sketch-0.2.4/src/sketchformat/serialize/orjson.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.3/src/sketchformat/style.py` & `fig2sketch-0.2.4/src/sketchformat/style.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.3/src/sketchformat/text.py` & `fig2sketch-0.2.4/src/sketchformat/text.py`

 * *Files identical despite different names*

