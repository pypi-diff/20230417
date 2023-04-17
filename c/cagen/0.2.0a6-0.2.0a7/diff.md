# Comparing `tmp/cagen-0.2.0a6.tar.gz` & `tmp/cagen-0.2.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cagen-0.2.0a6.tar", last modified: Mon Apr 17 08:08:57 2023, max compression
+gzip compressed data, was "cagen-0.2.0a7.tar", last modified: Mon Apr 17 08:52:05 2023, max compression
```

## Comparing `cagen-0.2.0a6.tar` & `cagen-0.2.0a7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-17 08:08:57.940003 cagen-0.2.0a6/
--rw-r--r--   0 xan       (1000) xan       (1000)      177 2023-03-28 18:54:19.000000 cagen-0.2.0a6/MANIFEST.in
--rw-r--r--   0 xan       (1000) xan       (1000)     4049 2023-04-17 08:08:57.940003 cagen-0.2.0a6/PKG-INFO
--rw-r--r--   0 xan       (1000) xan       (1000)     3314 2023-04-16 10:42:06.000000 cagen-0.2.0a6/README.md
--rw-r--r--   0 xan       (1000) xan       (1000)     1160 2023-04-17 08:07:55.000000 cagen-0.2.0a6/pyproject.toml
--rw-r--r--   0 xan       (1000) xan       (1000)       38 2023-04-17 08:08:57.943336 cagen-0.2.0a6/setup.cfg
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-17 08:08:57.940003 cagen-0.2.0a6/src/
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-17 08:08:57.940003 cagen-0.2.0a6/src/cagen/
--rw-r--r--   0 xan       (1000) xan       (1000)      112 2023-03-28 18:54:41.000000 cagen-0.2.0a6/src/cagen/__init__.py
--rw-r--r--   0 xan       (1000) xan       (1000)     4773 2023-04-16 21:18:58.000000 cagen-0.2.0a6/src/cagen/cmd.py
--rw-r--r--   0 xan       (1000) xan       (1000)     8259 2023-04-17 08:07:21.000000 cagen-0.2.0a6/src/cagen/libcagen.py
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-17 08:08:57.940003 cagen-0.2.0a6/src/cagen/templates/
--rw-r--r--   0 xan       (1000) xan       (1000)      381 2023-02-09 11:33:44.000000 cagen-0.2.0a6/src/cagen/templates/list.md.tmpl
--rw-r--r--   0 xan       (1000) xan       (1000)      107 2023-03-28 18:55:41.000000 cagen-0.2.0a6/src/cagen/templates/list.md.tmpl.license
--rw-r--r--   0 xan       (1000) xan       (1000)     1754 2023-01-21 12:38:41.000000 cagen-0.2.0a6/src/cagen/templates/schema.tmpl
--rw-r--r--   0 xan       (1000) xan       (1000)      107 2023-03-28 18:55:48.000000 cagen-0.2.0a6/src/cagen/templates/schema.tmpl.license
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-17 08:08:57.940003 cagen-0.2.0a6/src/cagen.egg-info/
--rw-r--r--   0 xan       (1000) xan       (1000)     4049 2023-04-17 08:08:57.000000 cagen-0.2.0a6/src/cagen.egg-info/PKG-INFO
--rw-r--r--   0 xan       (1000) xan       (1000)      443 2023-04-17 08:08:57.000000 cagen-0.2.0a6/src/cagen.egg-info/SOURCES.txt
--rw-r--r--   0 xan       (1000) xan       (1000)        1 2023-04-17 08:08:57.000000 cagen-0.2.0a6/src/cagen.egg-info/dependency_links.txt
--rw-r--r--   0 xan       (1000) xan       (1000)      114 2023-04-17 08:08:57.000000 cagen-0.2.0a6/src/cagen.egg-info/entry_points.txt
--rw-r--r--   0 xan       (1000) xan       (1000)       53 2023-04-17 08:08:57.000000 cagen-0.2.0a6/src/cagen.egg-info/requires.txt
--rw-r--r--   0 xan       (1000) xan       (1000)        6 2023-04-17 08:08:57.000000 cagen-0.2.0a6/src/cagen.egg-info/top_level.txt
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-17 08:52:05.616749 cagen-0.2.0a7/
+-rw-r--r--   0 xan       (1000) xan       (1000)      177 2023-03-28 18:54:19.000000 cagen-0.2.0a7/MANIFEST.in
+-rw-r--r--   0 xan       (1000) xan       (1000)     4049 2023-04-17 08:52:05.616749 cagen-0.2.0a7/PKG-INFO
+-rw-r--r--   0 xan       (1000) xan       (1000)     3314 2023-04-16 10:42:06.000000 cagen-0.2.0a7/README.md
+-rw-r--r--   0 xan       (1000) xan       (1000)     1160 2023-04-17 08:51:52.000000 cagen-0.2.0a7/pyproject.toml
+-rw-r--r--   0 xan       (1000) xan       (1000)       38 2023-04-17 08:52:05.616749 cagen-0.2.0a7/setup.cfg
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-17 08:52:05.616749 cagen-0.2.0a7/src/
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-17 08:52:05.616749 cagen-0.2.0a7/src/cagen/
+-rw-r--r--   0 xan       (1000) xan       (1000)      112 2023-03-28 18:54:41.000000 cagen-0.2.0a7/src/cagen/__init__.py
+-rw-r--r--   0 xan       (1000) xan       (1000)     4773 2023-04-16 21:18:58.000000 cagen-0.2.0a7/src/cagen/cmd.py
+-rw-r--r--   0 xan       (1000) xan       (1000)     8236 2023-04-17 08:48:25.000000 cagen-0.2.0a7/src/cagen/libcagen.py
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-17 08:52:05.616749 cagen-0.2.0a7/src/cagen/templates/
+-rw-r--r--   0 xan       (1000) xan       (1000)      381 2023-02-09 11:33:44.000000 cagen-0.2.0a7/src/cagen/templates/list.md.tmpl
+-rw-r--r--   0 xan       (1000) xan       (1000)      107 2023-03-28 18:55:41.000000 cagen-0.2.0a7/src/cagen/templates/list.md.tmpl.license
+-rw-r--r--   0 xan       (1000) xan       (1000)     1754 2023-01-21 12:38:41.000000 cagen-0.2.0a7/src/cagen/templates/schema.tmpl
+-rw-r--r--   0 xan       (1000) xan       (1000)      107 2023-03-28 18:55:48.000000 cagen-0.2.0a7/src/cagen/templates/schema.tmpl.license
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-17 08:52:05.616749 cagen-0.2.0a7/src/cagen.egg-info/
+-rw-r--r--   0 xan       (1000) xan       (1000)     4049 2023-04-17 08:52:05.000000 cagen-0.2.0a7/src/cagen.egg-info/PKG-INFO
+-rw-r--r--   0 xan       (1000) xan       (1000)      443 2023-04-17 08:52:05.000000 cagen-0.2.0a7/src/cagen.egg-info/SOURCES.txt
+-rw-r--r--   0 xan       (1000) xan       (1000)        1 2023-04-17 08:52:05.000000 cagen-0.2.0a7/src/cagen.egg-info/dependency_links.txt
+-rw-r--r--   0 xan       (1000) xan       (1000)      114 2023-04-17 08:52:05.000000 cagen-0.2.0a7/src/cagen.egg-info/entry_points.txt
+-rw-r--r--   0 xan       (1000) xan       (1000)       53 2023-04-17 08:52:05.000000 cagen-0.2.0a7/src/cagen.egg-info/requires.txt
+-rw-r--r--   0 xan       (1000) xan       (1000)        6 2023-04-17 08:52:05.000000 cagen-0.2.0a7/src/cagen.egg-info/top_level.txt
```

### Comparing `cagen-0.2.0a6/PKG-INFO` & `cagen-0.2.0a7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cagen
-Version: 0.2.0a6
+Version: 0.2.0a7
 Summary: A static site generator for cmpalgorithms project
 Author: Xavier B.
 Project-URL: Homepage, https://repo.or.cz/cagen.git
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `cagen-0.2.0a6/README.md` & `cagen-0.2.0a7/README.md`

 * *Files identical despite different names*

### Comparing `cagen-0.2.0a6/pyproject.toml` & `cagen-0.2.0a7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 [project.scripts]
 cagen = "cagen.cmd:cagen_cli"
 cagen-list = "cagen.cmd:cagen_list"
 cagen-make = "cagen.cmd:cagen_make"
 
 [project]
 name = "cagen"
-version = "0.2.0.alpha-6"
+version = "0.2.0.alpha-7"
 authors = [{'name'="Xavier B."}]
 description = "A static site generator for cmpalgorithms project"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
         'Development Status :: 3 - Alpha',
         'Environment :: Console',
```

### Comparing `cagen-0.2.0a6/src/cagen/cmd.py` & `cagen-0.2.0a7/src/cagen/cmd.py`

 * *Files identical despite different names*

### Comparing `cagen-0.2.0a6/src/cagen/libcagen.py` & `cagen-0.2.0a7/src/cagen/libcagen.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,15 +123,15 @@
         """
 
         mysearchlist = self.to_dict
         mysearchlist['conversion'] = self.pandoc_convert(destsyntax)
 
         # Merging two dictionaries using |= method
         mysearchlist |= additionalsearchlist
-        tmp = Template(filename=mytemplatepath, strict_undefined=True)
+        tmp = Template(filename=mytemplatepath)
         return tmp.render(**mysearchlist)
 
 
 
 class Collection:
     """A collection of `Entry` instances"""
```

### Comparing `cagen-0.2.0a6/src/cagen/templates/schema.tmpl` & `cagen-0.2.0a7/src/cagen/templates/schema.tmpl`

 * *Files identical despite different names*

### Comparing `cagen-0.2.0a6/src/cagen.egg-info/PKG-INFO` & `cagen-0.2.0a7/src/cagen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cagen
-Version: 0.2.0a6
+Version: 0.2.0a7
 Summary: A static site generator for cmpalgorithms project
 Author: Xavier B.
 Project-URL: Homepage, https://repo.or.cz/cagen.git
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

