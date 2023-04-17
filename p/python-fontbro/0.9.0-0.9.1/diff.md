# Comparing `tmp/python-fontbro-0.9.0.tar.gz` & `tmp/python-fontbro-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-fontbro-0.9.0.tar", last modified: Tue Jun  7 10:17:51 2022, max compression
+gzip compressed data, was "python-fontbro-0.9.1.tar", last modified: Tue Jun  7 12:39:39 2022, max compression
```

## Comparing `python-fontbro-0.9.0.tar` & `python-fontbro-0.9.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2022-06-07 10:17:51.043233 python-fontbro-0.9.0/
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     1078 2021-10-18 10:03:11.000000 python-fontbro-0.9.0/LICENSE.txt
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)      114 2021-10-18 10:19:39.000000 python-fontbro-0.9.0/MANIFEST.in
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)    18824 2022-06-07 10:17:51.043431 python-fontbro-0.9.0/PKG-INFO
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)    17157 2022-05-11 09:35:02.000000 python-fontbro-0.9.0/README.md
-drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2022-06-07 10:17:51.040518 python-fontbro-0.9.0/fontbro/
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)      369 2022-03-24 13:13:04.000000 python-fontbro-0.9.0/fontbro/__init__.py
-drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2022-06-07 10:17:51.041482 python-fontbro-0.9.0/fontbro/data/
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)    17152 2022-01-18 11:14:21.000000 python-fontbro-0.9.0/fontbro/data/features.json
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)    25636 2022-06-07 10:11:13.000000 python-fontbro-0.9.0/fontbro/data/unicode-blocks.json
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)    15535 2022-06-07 10:11:13.000000 python-fontbro-0.9.0/fontbro/data/unicode-scripts.json
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)      605 2022-01-12 21:42:11.000000 python-fontbro-0.9.0/fontbro/flags.py
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)    43883 2022-06-07 10:08:49.000000 python-fontbro-0.9.0/fontbro/font.py
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)      288 2022-06-07 10:11:34.000000 python-fontbro-0.9.0/fontbro/metadata.py
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)      848 2022-01-26 17:11:08.000000 python-fontbro-0.9.0/fontbro/subset.py
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)      194 2022-04-28 21:27:33.000000 python-fontbro-0.9.0/fontbro/utils.py
-drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2022-06-07 10:17:51.042971 python-fontbro-0.9.0/python_fontbro.egg-info/
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)    18824 2022-06-07 10:17:50.000000 python-fontbro-0.9.0/python_fontbro.egg-info/PKG-INFO
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)      443 2022-06-07 10:17:51.000000 python-fontbro-0.9.0/python_fontbro.egg-info/SOURCES.txt
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)        1 2022-06-07 10:17:50.000000 python-fontbro-0.9.0/python_fontbro.egg-info/dependency_links.txt
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)      119 2022-06-07 10:17:50.000000 python-fontbro-0.9.0/python_fontbro.egg-info/requires.txt
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)        8 2022-06-07 10:17:50.000000 python-fontbro-0.9.0/python_fontbro.egg-info/top_level.txt
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)      195 2022-06-07 10:17:51.044128 python-fontbro-0.9.0/setup.cfg
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     2928 2022-05-04 10:57:20.000000 python-fontbro-0.9.0/setup.py
+drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2022-06-07 12:39:39.826686 python-fontbro-0.9.1/
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     1078 2021-10-18 10:03:11.000000 python-fontbro-0.9.1/LICENSE.txt
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)      114 2021-10-18 10:19:39.000000 python-fontbro-0.9.1/MANIFEST.in
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)    18824 2022-06-07 12:39:39.826833 python-fontbro-0.9.1/PKG-INFO
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)    17157 2022-05-11 09:35:02.000000 python-fontbro-0.9.1/README.md
+drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2022-06-07 12:39:39.823944 python-fontbro-0.9.1/fontbro/
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)      369 2022-03-24 13:13:04.000000 python-fontbro-0.9.1/fontbro/__init__.py
+drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2022-06-07 12:39:39.825027 python-fontbro-0.9.1/fontbro/data/
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)    17152 2022-01-18 11:14:21.000000 python-fontbro-0.9.1/fontbro/data/features.json
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)    25636 2022-06-07 12:34:29.000000 python-fontbro-0.9.1/fontbro/data/unicode-blocks.json
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)    15535 2022-06-07 12:34:29.000000 python-fontbro-0.9.1/fontbro/data/unicode-scripts.json
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)      605 2022-01-12 21:42:11.000000 python-fontbro-0.9.1/fontbro/flags.py
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)    44049 2022-06-07 12:33:50.000000 python-fontbro-0.9.1/fontbro/font.py
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)      288 2022-06-07 12:38:16.000000 python-fontbro-0.9.1/fontbro/metadata.py
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)      848 2022-01-26 17:11:08.000000 python-fontbro-0.9.1/fontbro/subset.py
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)      194 2022-04-28 21:27:33.000000 python-fontbro-0.9.1/fontbro/utils.py
+drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2022-06-07 12:39:39.826480 python-fontbro-0.9.1/python_fontbro.egg-info/
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)    18824 2022-06-07 12:39:39.000000 python-fontbro-0.9.1/python_fontbro.egg-info/PKG-INFO
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)      443 2022-06-07 12:39:39.000000 python-fontbro-0.9.1/python_fontbro.egg-info/SOURCES.txt
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)        1 2022-06-07 12:39:39.000000 python-fontbro-0.9.1/python_fontbro.egg-info/dependency_links.txt
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)      119 2022-06-07 12:39:39.000000 python-fontbro-0.9.1/python_fontbro.egg-info/requires.txt
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)        8 2022-06-07 12:39:39.000000 python-fontbro-0.9.1/python_fontbro.egg-info/top_level.txt
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)      195 2022-06-07 12:39:39.827257 python-fontbro-0.9.1/setup.cfg
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     2928 2022-05-04 10:57:20.000000 python-fontbro-0.9.1/setup.py
```

### Comparing `python-fontbro-0.9.0/LICENSE.txt` & `python-fontbro-0.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python-fontbro-0.9.0/PKG-INFO` & `python-fontbro-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: python-fontbro
-Version: 0.9.0
+Version: 0.9.1
 Summary: friendly font operations on top of fontTools.
 Home-page: https://github.com/fabiocaccamo/python-fontbro
 Author: Fabio Caccamo
 Author-email: fabio.caccamo@gmail.com
 License: MIT
-Download-URL: https://github.com/fabiocaccamo/python-fontbro/archive/0.9.0.tar.gz
+Download-URL: https://github.com/fabiocaccamo/python-fontbro/archive/0.9.1.tar.gz
 Project-URL: Documentation, https://github.com/fabiocaccamo/python-fontbro#readme
 Project-URL: Issues, https://github.com/fabiocaccamo/python-fontbro/issues
 Project-URL: Funding, https://github.com/sponsors/fabiocaccamo/
 Project-URL: Twitter, https://twitter.com/fabiocaccamo
 Keywords: font,fonttools,languages,opentype,otf,python,scripts,slicing,subset,subsetting ,ttf,unicode,utility,variable,variations,woff,woff2,wrapper,writing-systems
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `python-fontbro-0.9.0/README.md` & `python-fontbro-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `python-fontbro-0.9.0/fontbro/data/features.json` & `python-fontbro-0.9.1/fontbro/data/features.json`

 * *Files identical despite different names*

### Comparing `python-fontbro-0.9.0/fontbro/data/unicode-blocks.json` & `python-fontbro-0.9.1/fontbro/data/unicode-blocks.json`

 * *Files identical despite different names*

### Comparing `python-fontbro-0.9.0/fontbro/data/unicode-scripts.json` & `python-fontbro-0.9.1/fontbro/data/unicode-scripts.json`

 * *Files identical despite different names*

### Comparing `python-fontbro-0.9.0/fontbro/flags.py` & `python-fontbro-0.9.1/fontbro/flags.py`

 * *Files identical despite different names*

### Comparing `python-fontbro-0.9.0/fontbro/font.py` & `python-fontbro-0.9.1/fontbro/font.py`

 * *Files 1% similar despite different names*

```diff
@@ -1078,14 +1078,17 @@
         font = self.get_ttfont()
         if not any([unicodes, glyphs, text]):
             raise ValueError(
                 "Subsetting requires at least one of the following args: unicode,"
                 " glyphs, text."
             )
         unicodes = parse_unicodes(unicodes)
+        options.setdefault("glyph_names", True)
+        options.setdefault("ignore_missing_glyphs", True)
+        options.setdefault("ignore_missing_unicodes", True)
         options.setdefault("layout_features", ["*"])
         options.setdefault("name_IDs", "*")
         options.setdefault("notdef_outline", True)
         subs_args = {"unicodes": unicodes, "glyphs": glyphs, "text": text}
         # https://github.com/fonttools/fonttools/blob/main/Lib/fontTools/subset/__init__.py
         subs_options = SubsetterOptions(**options)
         subs = Subsetter(options=subs_options)
```

### Comparing `python-fontbro-0.9.0/fontbro/subset.py` & `python-fontbro-0.9.1/fontbro/subset.py`

 * *Files identical despite different names*

### Comparing `python-fontbro-0.9.0/python_fontbro.egg-info/PKG-INFO` & `python-fontbro-0.9.1/python_fontbro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: python-fontbro
-Version: 0.9.0
+Version: 0.9.1
 Summary: friendly font operations on top of fontTools.
 Home-page: https://github.com/fabiocaccamo/python-fontbro
 Author: Fabio Caccamo
 Author-email: fabio.caccamo@gmail.com
 License: MIT
-Download-URL: https://github.com/fabiocaccamo/python-fontbro/archive/0.9.0.tar.gz
+Download-URL: https://github.com/fabiocaccamo/python-fontbro/archive/0.9.1.tar.gz
 Project-URL: Documentation, https://github.com/fabiocaccamo/python-fontbro#readme
 Project-URL: Issues, https://github.com/fabiocaccamo/python-fontbro/issues
 Project-URL: Funding, https://github.com/sponsors/fabiocaccamo/
 Project-URL: Twitter, https://twitter.com/fabiocaccamo
 Keywords: font,fonttools,languages,opentype,otf,python,scripts,slicing,subset,subsetting ,ttf,unicode,utility,variable,variations,woff,woff2,wrapper,writing-systems
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `python-fontbro-0.9.0/setup.py` & `python-fontbro-0.9.1/setup.py`

 * *Files identical despite different names*

