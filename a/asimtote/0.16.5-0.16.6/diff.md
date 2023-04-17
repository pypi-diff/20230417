# Comparing `tmp/asimtote-0.16.5.tar.gz` & `tmp/asimtote-0.16.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asimtote-0.16.5.tar", last modified: Mon Apr 17 14:15:27 2023, max compression
+gzip compressed data, was "asimtote-0.16.6.tar", last modified: Mon Apr 17 14:16:03 2023, max compression
```

## Comparing `asimtote-0.16.5.tar` & `asimtote-0.16.6.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-04-17 14:15:27.042190 asimtote-0.16.5/
--rw-r--r--   0 rcf34      (503) staff       (20)     1334 2023-02-01 17:57:38.000000 asimtote-0.16.5/.gitignore
--rw-r--r--   0 rcf34      (503) staff       (20)     1101 2023-02-01 17:57:38.000000 asimtote-0.16.5/LICENSE
--rw-r--r--   0 rcf34      (503) staff       (20)      297 2023-04-14 17:08:48.000000 asimtote-0.16.5/Makefile
--rw-r--r--   0 rcf34      (503) staff       (20)     3483 2023-04-17 14:15:27.042032 asimtote-0.16.5/PKG-INFO
--rw-r--r--   0 rcf34      (503) staff       (20)     3016 2023-04-14 17:08:48.000000 asimtote-0.16.5/README.md
-drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-04-17 14:15:27.035780 asimtote-0.16.5/asimtote/
--rw-r--r--   0 rcf34      (503) staff       (20)       45 2023-04-17 14:15:22.000000 asimtote-0.16.5/asimtote/__init__.py
--rw-r--r--   0 rcf34      (503) staff       (20)    13909 2023-04-14 17:08:48.000000 asimtote-0.16.5/asimtote/__main__.py
--rw-r--r--   0 rcf34      (503) staff       (20)    16544 2023-04-14 17:08:48.000000 asimtote-0.16.5/asimtote/config.py
--rw-r--r--   0 rcf34      (503) staff       (20)    74811 2023-04-17 14:15:22.000000 asimtote-0.16.5/asimtote/diff.py
-drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-04-17 14:15:27.037158 asimtote-0.16.5/asimtote/ios/
--rw-r--r--   0 rcf34      (503) staff       (20)      188 2023-04-14 17:08:48.000000 asimtote-0.16.5/asimtote/ios/__init__.py
-drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-04-17 14:15:27.038038 asimtote-0.16.5/asimtote/ios/commands/
--rw-r--r--   0 rcf34      (503) staff       (20)      719 2023-04-14 17:08:48.000000 asimtote-0.16.5/asimtote/ios/commands/__init__.py
--rw-r--r--   0 rcf34      (503) staff       (20)    18303 2023-04-14 17:08:48.000000 asimtote-0.16.5/asimtote/ios/commands/interface.py
--rw-r--r--   0 rcf34      (503) staff       (20)     5931 2023-04-14 17:08:48.000000 asimtote-0.16.5/asimtote/ios/commands/lists.py
--rw-r--r--   0 rcf34      (503) staff       (20)     8074 2023-04-14 17:08:48.000000 asimtote-0.16.5/asimtote/ios/commands/other.py
--rw-r--r--   0 rcf34      (503) staff       (20)    26719 2023-04-14 17:08:48.000000 asimtote-0.16.5/asimtote/ios/commands/router.py
--rw-r--r--   0 rcf34      (503) staff       (20)     6134 2023-04-14 17:08:48.000000 asimtote-0.16.5/asimtote/ios/config.py
-drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-04-17 14:15:27.038740 asimtote-0.16.5/asimtote/ios/converters/
--rw-r--r--   0 rcf34      (503) staff       (20)      741 2023-04-17 14:15:22.000000 asimtote-0.16.5/asimtote/ios/converters/__init__.py
--rw-r--r--   0 rcf34      (503) staff       (20)    28594 2023-04-17 14:15:22.000000 asimtote-0.16.5/asimtote/ios/converters/interface.py
--rw-r--r--   0 rcf34      (503) staff       (20)     3469 2023-04-17 14:15:22.000000 asimtote-0.16.5/asimtote/ios/converters/lists.py
--rw-r--r--   0 rcf34      (503) staff       (20)     7828 2023-04-17 14:15:22.000000 asimtote-0.16.5/asimtote/ios/converters/other.py
--rw-r--r--   0 rcf34      (503) staff       (20)    41940 2023-04-17 14:15:22.000000 asimtote-0.16.5/asimtote/ios/converters/router.py
--rw-r--r--   0 rcf34      (503) staff       (20)     4753 2023-04-14 17:08:48.000000 asimtote-0.16.5/asimtote/ios/diff.py
--rw-r--r--   0 rcf34      (503) staff       (20)    22009 2023-04-14 17:08:48.000000 asimtote-0.16.5/asimtote/ios/utils.py
--rw-r--r--   0 rcf34      (503) staff       (20)     1492 2023-04-14 17:08:48.000000 asimtote-0.16.5/asimtote/misc.py
-drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-04-17 14:15:27.036491 asimtote-0.16.5/asimtote.egg-info/
--rw-r--r--   0 rcf34      (503) staff       (20)     3483 2023-04-17 14:15:26.000000 asimtote-0.16.5/asimtote.egg-info/PKG-INFO
--rw-r--r--   0 rcf34      (503) staff       (20)     1230 2023-04-17 14:15:27.000000 asimtote-0.16.5/asimtote.egg-info/SOURCES.txt
--rw-r--r--   0 rcf34      (503) staff       (20)        1 2023-04-17 14:15:26.000000 asimtote-0.16.5/asimtote.egg-info/dependency_links.txt
--rw-r--r--   0 rcf34      (503) staff       (20)       23 2023-04-17 14:15:26.000000 asimtote-0.16.5/asimtote.egg-info/requires.txt
--rw-r--r--   0 rcf34      (503) staff       (20)        9 2023-04-17 14:15:26.000000 asimtote-0.16.5/asimtote.egg-info/top_level.txt
--rw-r--r--   0 rcf34      (503) staff       (20)       38 2023-04-17 14:15:27.042231 asimtote-0.16.5/setup.cfg
--rwxr-xr-x   0 rcf34      (503) staff       (20)      807 2023-04-14 17:08:48.000000 asimtote-0.16.5/setup.py
-drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-04-17 14:15:27.038889 asimtote-0.16.5/test_asimtote/
--rw-r--r--   0 rcf34      (503) staff       (20)      149 2023-04-14 17:08:48.000000 asimtote-0.16.5/test_asimtote/__main__.py
-drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-04-17 14:15:27.039300 asimtote-0.16.5/test_asimtote/ios/
--rw-r--r--   0 rcf34      (503) staff       (20)      143 2023-04-14 17:08:48.000000 asimtote-0.16.5/test_asimtote/ios/__init__.py
-drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-04-17 14:15:27.040290 asimtote-0.16.5/test_asimtote/ios/config/
--rw-r--r--   0 rcf34      (503) staff       (20)      328 2023-04-14 17:08:48.000000 asimtote-0.16.5/test_asimtote/ios/config/__init__.py
--rw-r--r--   0 rcf34      (503) staff       (20)    34207 2023-04-14 17:08:48.000000 asimtote-0.16.5/test_asimtote/ios/config/interface.py
--rw-r--r--   0 rcf34      (503) staff       (20)    14804 2023-04-14 17:08:48.000000 asimtote-0.16.5/test_asimtote/ios/config/lists.py
--rw-r--r--   0 rcf34      (503) staff       (20)     9991 2023-04-14 17:08:48.000000 asimtote-0.16.5/test_asimtote/ios/config/other.py
--rw-r--r--   0 rcf34      (503) staff       (20)    60416 2023-04-14 17:08:48.000000 asimtote-0.16.5/test_asimtote/ios/config/router.py
-drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-04-17 14:15:27.041525 asimtote-0.16.5/test_asimtote/ios/converters/
--rw-r--r--   0 rcf34      (503) staff       (20)      336 2023-04-14 17:08:48.000000 asimtote-0.16.5/test_asimtote/ios/converters/__init__.py
--rw-r--r--   0 rcf34      (503) staff       (20)     2646 2023-04-14 17:08:48.000000 asimtote-0.16.5/test_asimtote/ios/converters/cvtunittest.py
--rw-r--r--   0 rcf34      (503) staff       (20)    95324 2023-04-14 17:08:48.000000 asimtote-0.16.5/test_asimtote/ios/converters/interface.py
--rw-r--r--   0 rcf34      (503) staff       (20)    13090 2023-04-14 17:08:48.000000 asimtote-0.16.5/test_asimtote/ios/converters/lists.py
--rw-r--r--   0 rcf34      (503) staff       (20)    24061 2023-04-14 17:08:48.000000 asimtote-0.16.5/test_asimtote/ios/converters/other.py
--rw-r--r--   0 rcf34      (503) staff       (20)   152946 2023-04-14 17:08:48.000000 asimtote-0.16.5/test_asimtote/ios/converters/router.py
--rw-r--r--   0 rcf34      (503) staff       (20)     2220 2023-04-14 17:08:48.000000 asimtote-0.16.5/test_asimtote/ios/utils.py
+drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-04-17 14:16:03.085910 asimtote-0.16.6/
+-rw-r--r--   0 rcf34      (503) staff       (20)     1334 2023-02-01 17:57:38.000000 asimtote-0.16.6/.gitignore
+-rw-r--r--   0 rcf34      (503) staff       (20)     1101 2023-02-01 17:57:38.000000 asimtote-0.16.6/LICENSE
+-rw-r--r--   0 rcf34      (503) staff       (20)      297 2023-04-14 17:08:48.000000 asimtote-0.16.6/Makefile
+-rw-r--r--   0 rcf34      (503) staff       (20)     3483 2023-04-17 14:16:03.085778 asimtote-0.16.6/PKG-INFO
+-rw-r--r--   0 rcf34      (503) staff       (20)     3016 2023-04-14 17:08:48.000000 asimtote-0.16.6/README.md
+drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-04-17 14:16:03.079585 asimtote-0.16.6/asimtote/
+-rw-r--r--   0 rcf34      (503) staff       (20)       45 2023-04-17 14:15:37.000000 asimtote-0.16.6/asimtote/__init__.py
+-rw-r--r--   0 rcf34      (503) staff       (20)    13909 2023-04-14 17:08:48.000000 asimtote-0.16.6/asimtote/__main__.py
+-rw-r--r--   0 rcf34      (503) staff       (20)    16544 2023-04-14 17:08:48.000000 asimtote-0.16.6/asimtote/config.py
+-rw-r--r--   0 rcf34      (503) staff       (20)    74793 2023-04-17 14:15:37.000000 asimtote-0.16.6/asimtote/diff.py
+drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-04-17 14:16:03.081388 asimtote-0.16.6/asimtote/ios/
+-rw-r--r--   0 rcf34      (503) staff       (20)      188 2023-04-14 17:08:48.000000 asimtote-0.16.6/asimtote/ios/__init__.py
+drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-04-17 14:16:03.082221 asimtote-0.16.6/asimtote/ios/commands/
+-rw-r--r--   0 rcf34      (503) staff       (20)      719 2023-04-14 17:08:48.000000 asimtote-0.16.6/asimtote/ios/commands/__init__.py
+-rw-r--r--   0 rcf34      (503) staff       (20)    18303 2023-04-14 17:08:48.000000 asimtote-0.16.6/asimtote/ios/commands/interface.py
+-rw-r--r--   0 rcf34      (503) staff       (20)     5931 2023-04-14 17:08:48.000000 asimtote-0.16.6/asimtote/ios/commands/lists.py
+-rw-r--r--   0 rcf34      (503) staff       (20)     8074 2023-04-14 17:08:48.000000 asimtote-0.16.6/asimtote/ios/commands/other.py
+-rw-r--r--   0 rcf34      (503) staff       (20)    26719 2023-04-14 17:08:48.000000 asimtote-0.16.6/asimtote/ios/commands/router.py
+-rw-r--r--   0 rcf34      (503) staff       (20)     6134 2023-04-14 17:08:48.000000 asimtote-0.16.6/asimtote/ios/config.py
+drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-04-17 14:16:03.082970 asimtote-0.16.6/asimtote/ios/converters/
+-rw-r--r--   0 rcf34      (503) staff       (20)      733 2023-04-17 14:15:37.000000 asimtote-0.16.6/asimtote/ios/converters/__init__.py
+-rw-r--r--   0 rcf34      (503) staff       (20)    28322 2023-04-17 14:15:37.000000 asimtote-0.16.6/asimtote/ios/converters/interface.py
+-rw-r--r--   0 rcf34      (503) staff       (20)     3441 2023-04-17 14:15:37.000000 asimtote-0.16.6/asimtote/ios/converters/lists.py
+-rw-r--r--   0 rcf34      (503) staff       (20)     7726 2023-04-17 14:15:37.000000 asimtote-0.16.6/asimtote/ios/converters/other.py
+-rw-r--r--   0 rcf34      (503) staff       (20)    41819 2023-04-17 14:15:37.000000 asimtote-0.16.6/asimtote/ios/converters/router.py
+-rw-r--r--   0 rcf34      (503) staff       (20)     4753 2023-04-14 17:08:48.000000 asimtote-0.16.6/asimtote/ios/diff.py
+-rw-r--r--   0 rcf34      (503) staff       (20)    22009 2023-04-14 17:08:48.000000 asimtote-0.16.6/asimtote/ios/utils.py
+-rw-r--r--   0 rcf34      (503) staff       (20)     1492 2023-04-14 17:08:48.000000 asimtote-0.16.6/asimtote/misc.py
+drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-04-17 14:16:03.080411 asimtote-0.16.6/asimtote.egg-info/
+-rw-r--r--   0 rcf34      (503) staff       (20)     3483 2023-04-17 14:16:03.000000 asimtote-0.16.6/asimtote.egg-info/PKG-INFO
+-rw-r--r--   0 rcf34      (503) staff       (20)     1230 2023-04-17 14:16:03.000000 asimtote-0.16.6/asimtote.egg-info/SOURCES.txt
+-rw-r--r--   0 rcf34      (503) staff       (20)        1 2023-04-17 14:16:03.000000 asimtote-0.16.6/asimtote.egg-info/dependency_links.txt
+-rw-r--r--   0 rcf34      (503) staff       (20)       23 2023-04-17 14:16:03.000000 asimtote-0.16.6/asimtote.egg-info/requires.txt
+-rw-r--r--   0 rcf34      (503) staff       (20)        9 2023-04-17 14:16:03.000000 asimtote-0.16.6/asimtote.egg-info/top_level.txt
+-rw-r--r--   0 rcf34      (503) staff       (20)       38 2023-04-17 14:16:03.085945 asimtote-0.16.6/setup.cfg
+-rwxr-xr-x   0 rcf34      (503) staff       (20)      807 2023-04-14 17:08:48.000000 asimtote-0.16.6/setup.py
+drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-04-17 14:16:03.083166 asimtote-0.16.6/test_asimtote/
+-rw-r--r--   0 rcf34      (503) staff       (20)      149 2023-04-14 17:08:48.000000 asimtote-0.16.6/test_asimtote/__main__.py
+drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-04-17 14:16:03.083425 asimtote-0.16.6/test_asimtote/ios/
+-rw-r--r--   0 rcf34      (503) staff       (20)      143 2023-04-14 17:08:48.000000 asimtote-0.16.6/test_asimtote/ios/__init__.py
+drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-04-17 14:16:03.084262 asimtote-0.16.6/test_asimtote/ios/config/
+-rw-r--r--   0 rcf34      (503) staff       (20)      328 2023-04-14 17:08:48.000000 asimtote-0.16.6/test_asimtote/ios/config/__init__.py
+-rw-r--r--   0 rcf34      (503) staff       (20)    34207 2023-04-14 17:08:48.000000 asimtote-0.16.6/test_asimtote/ios/config/interface.py
+-rw-r--r--   0 rcf34      (503) staff       (20)    14804 2023-04-14 17:08:48.000000 asimtote-0.16.6/test_asimtote/ios/config/lists.py
+-rw-r--r--   0 rcf34      (503) staff       (20)     9991 2023-04-14 17:08:48.000000 asimtote-0.16.6/test_asimtote/ios/config/other.py
+-rw-r--r--   0 rcf34      (503) staff       (20)    60416 2023-04-14 17:08:48.000000 asimtote-0.16.6/test_asimtote/ios/config/router.py
+drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-04-17 14:16:03.085299 asimtote-0.16.6/test_asimtote/ios/converters/
+-rw-r--r--   0 rcf34      (503) staff       (20)      336 2023-04-14 17:08:48.000000 asimtote-0.16.6/test_asimtote/ios/converters/__init__.py
+-rw-r--r--   0 rcf34      (503) staff       (20)     2646 2023-04-14 17:08:48.000000 asimtote-0.16.6/test_asimtote/ios/converters/cvtunittest.py
+-rw-r--r--   0 rcf34      (503) staff       (20)    95324 2023-04-14 17:08:48.000000 asimtote-0.16.6/test_asimtote/ios/converters/interface.py
+-rw-r--r--   0 rcf34      (503) staff       (20)    13090 2023-04-14 17:08:48.000000 asimtote-0.16.6/test_asimtote/ios/converters/lists.py
+-rw-r--r--   0 rcf34      (503) staff       (20)    24061 2023-04-14 17:08:48.000000 asimtote-0.16.6/test_asimtote/ios/converters/other.py
+-rw-r--r--   0 rcf34      (503) staff       (20)   152946 2023-04-14 17:08:48.000000 asimtote-0.16.6/test_asimtote/ios/converters/router.py
+-rw-r--r--   0 rcf34      (503) staff       (20)     2220 2023-04-14 17:08:48.000000 asimtote-0.16.6/test_asimtote/ios/utils.py
```

### Comparing `asimtote-0.16.5/.gitignore` & `asimtote-0.16.6/.gitignore`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.5/LICENSE` & `asimtote-0.16.6/LICENSE`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.5/PKG-INFO` & `asimtote-0.16.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asimtote
-Version: 0.16.5
+Version: 0.16.6
 Summary: Compare network device configuration files using contextual structures
 Home-page: https://gitlab.developers.cam.ac.uk/uis/netsys/udn/asimtote
 Author: Robert Franklin
 Author-email: rcf34@cam.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `asimtote-0.16.5/README.md` & `asimtote-0.16.6/README.md`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.5/asimtote/__main__.py` & `asimtote-0.16.6/asimtote/__main__.py`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.5/asimtote/config.py` & `asimtote-0.16.6/asimtote/config.py`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.5/asimtote/diff.py` & `asimtote-0.16.6/asimtote/diff.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
 
 
 # --- classes ---
 
 
 
-class DiffConvert:
+class Convert:
     """This abstract class handles converting the difference between an
     old ('from') configuration item to the corresponding new ('to')
     configuration item.
 
     The main difference process will use deepops.deepdiff() to work out
     what has been removed and what updated (added/changed) between the
     two configurations.
@@ -350,16 +350,16 @@
 
         return self._path_matches(d, tuple(context) + self.cmd + self.ext)
 
 
     def context_removed(self, d, match):
         """This method takes a remove dictionary, as returned by
         deepdiff(), and a specific match into it (which must be from
-        the same DiffConvert object as the method is called on) and
-        returns True iff the context for this converter is either:
+        the same Convert object as the method is called on) and returns
+        True iff the context for this converter is either:
 
         1.  In the remove dictionary entirely and exactly (i.e. it is
         empty at the end of the match path), or
 
         2.  The dictionary does not contain the match path but the match
         path runs out at a point in the dictionary where it is empty
         (indicating everything below this is removed).
@@ -853,15 +853,15 @@
         adds the converter block sequence with _add_blocks() and
         individual converters using _add_converters().  It also stores
         some settings controlling the level of information describing
         the conversion process, based on the command line arguments:
 
         init_explain=False -- include comments in the output
         configuration changes that explain the differences being matched
-        by the DiffConvert objects (if available).
+        by the Convert objects (if available).
 
         init_dump_config=False -- dump the old and new configurations
         (after excludes).
 
         init_dump_diff=False -- dump the differences (remove and update
         configurations).
 
@@ -917,16 +917,16 @@
         as they require.
         """
 
         pass
 
 
     def _add_converter(self, cvt):
-        """Add an individual converter object, a child of the
-        DiffConverter class, to the list of converters for its block.
+        """Add an individual converter object, a child of the Convert
+        class, to the list of converters for its block.
 
         If the block used in the converter does not exist, a KeyError
         will be raised.
         """
 
         block = cvt.block
```

### Comparing `asimtote-0.16.5/asimtote/ios/commands/__init__.py` & `asimtote-0.16.6/asimtote/ios/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.5/asimtote/ios/commands/interface.py` & `asimtote-0.16.6/asimtote/ios/commands/interface.py`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.5/asimtote/ios/commands/lists.py` & `asimtote-0.16.6/asimtote/ios/commands/lists.py`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.5/asimtote/ios/commands/other.py` & `asimtote-0.16.6/asimtote/ios/commands/other.py`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.5/asimtote/ios/commands/router.py` & `asimtote-0.16.6/asimtote/ios/commands/router.py`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.5/asimtote/ios/config.py` & `asimtote-0.16.6/asimtote/ios/config.py`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.5/asimtote/ios/converters/__init__.py` & `asimtote-0.16.6/asimtote/ios/converters/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 from .other import *
 from .router import *
 
 from ...misc import get_all_subclasses
 
 
 
-# the converters are all subclasses of DiffConvert which have the 'cmd'
+# the converters are all subclasses of Convert which have the 'cmd'
 # attribute defined, stored as a set - the order is not important as we
 # sort the list later
 #
 # CiscoIOSDiffConfig._add_converters() adds these into the list of
 # converter classes
 
 converters = {
-    c for c in get_all_subclasses(DiffConvert) if c.cmd is not None  }
+    c for c in get_all_subclasses(Convert) if c.cmd is not None  }
```

### Comparing `asimtote-0.16.5/asimtote/ios/converters/interface.py` & `asimtote-0.16.6/asimtote/ios/converters/interface.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 
 # --- imports ---
 
 
 
 from ..utils import is_int_physical
 
-from ...diff import DiffConvert
+from ...diff import Convert
 
 
 
 # --- converter classes ---
 
 
 
-class Cvt_Int(DiffConvert):
+class Cvt_Int(Convert):
     cmd = "interface", None
 
     def remove(self, old, c, int_name):
          # if the interface is physical, we can't delete it ...
         if is_int_physical(int_name):
             # ... but, if there was something in the old configuration
             # other than just it being shut down, we 'default' it
@@ -38,15 +38,15 @@
     def add(self, new, c, int_name):
         # physical interfaces don't need creating (it doesn't hurt but
         # it's not necessary and makes the unit tests more cumbersome)
         if not is_int_physical(int_name):
             return "interface " + int_name
 
 
-class DiffConvert_Int(DiffConvert):
+class Context_Int(Convert):
     context = Cvt_Int.cmd
 
     def enter(self, int_name):
         return ["interface " + int_name]
 
 
 
@@ -55,15 +55,15 @@
 # =============================================================================
 
 
 
 # we put the 'interface / shutdown' at the start to shut it down before
 # we do any [re]configuration
 
-class Cvt_Int_Shutdown(DiffConvert_Int):
+class Cvt_Int_Shutdown(Context_Int):
     cmd = "shutdown",
     block = "int-shutdown"
 
     def update(self, old, upd, new, c):
         # we only 'shutdown' if we are disabling the port ('no shutdown'
         # happens at the end of interface configuration)
         if new:
@@ -76,93 +76,93 @@
 # =============================================================================
 
 
 
 # converter to detect a VRF change and fire a trigger to make changes
 # required before it is actually changed
 
-class Cvt_VRFTrgr_VRFFwd(DiffConvert_Int):
+class Cvt_VRFTrgr_VRFFwd(Context_Int):
     cmd = "vrf-forwarding",
     block = "int-vrf-trigger"
     trigger_blocks = { "int-vrf-pre" }
     empty_trigger = True
 
 
 # we do VRF changes on an interface before we do any IP address
 # configuration, otherwise the IP configuration will be removed
 
-class Cvt_Int_VRFFwd(DiffConvert_Int):
+class Cvt_Int_VRFFwd(Context_Int):
     cmd = "vrf-forwarding",
     block = "int-vrf"
     trigger_blocks = { "int-vrf-post" }
 
     def remove(self, old, c):
         return self.enter(*c) + [" no vrf forwarding"]
 
     def update(self, old, upd, new, c):
         return self.enter(*c) + [" vrf forwarding " + new]
 
 
-class Cvt_Int_ARPTime(DiffConvert_Int):
+class Cvt_Int_ARPTime(Context_Int):
     cmd = "arp-timeout",
 
     def remove(self, old, c):
         return self.enter(*c) + [" no arp timeout"]
 
     def update(self, old, upd, new, c):
         return self.enter(*c) + [" arp timeout " + str(new)]
 
 
-class Cvt_Int_CDPEna(DiffConvert_Int):
+class Cvt_Int_CDPEna(Context_Int):
     cmd = "cdp-enable",
 
     def remove(self, old, c):
         # if the 'cdp enable' option is not present, that just means
         # it's reverted to the default setting of enabled - if it wasn't
         # previously enabled, we do that
         if not old:
             return self.enter(*c) + [" cdp enable"]
 
     def update(self, old, upd, new, c):
         return self.enter(*c) + [ " " + ("" if upd else "no ") + "cdp enable"]
 
 
-class Cvt_Int_ChnGrp(DiffConvert_Int):
+class Cvt_Int_ChnGrp(Context_Int):
     cmd = "channel-group",
 
     def remove(self, old, c):
         return self.enter(*c) + [" no channel-group"]
 
     def update(self, old, upd, new, c):
         id_, mode = new
         return self.enter(*c) + [
                    " channel-group %d%s" % (id_, mode if mode else "")]
 
 
-class Cvt_Int_Desc(DiffConvert_Int):
+class Cvt_Int_Desc(Context_Int):
     cmd = "description",
 
     def remove(self, old, c):
         return self.enter(*c) + [" no description"]
 
     def update(self, old, upd, new, c):
         return self.enter(*c) + [" description " + new]
 
 
-class Cvt_Int_Encap(DiffConvert_Int):
+class Cvt_Int_Encap(Context_Int):
     cmd = "encapsulation",
 
     def remove(self, old, c):
         return self.enter(*c) + [" no encapsulation " + old]
 
     def update(self, old, upd, new, c):
         return self.enter(*c) + [" encapsulation " + new]
 
 
-class Cvt_Int_IPAccGrp(DiffConvert_Int):
+class Cvt_Int_IPAccGrp(Context_Int):
     cmd = "ip-access-group", None
 
     def remove(self, old, c, dir_):
         return self.enter(*c) + [" no ip access-group " + dir_]
 
     def update(self, old, upd, new, c, dir_):
         return self.enter(*c) + [" ip access-group %s %s" % (new, dir_)]
@@ -171,26 +171,26 @@
 
 # =============================================================================
 # ip address ...
 # =============================================================================
 
 
 
-class Cvt_Int_IPAddr(DiffConvert_Int):
+class Cvt_Int_IPAddr(Context_Int):
     cmd = "ip-address",
     block = "int-vrf-post"
 
     def remove(self, old, c):
         return self.enter(*c) + [" no ip address"]
 
     def update(self, old, upd, new, c):
         return self.enter(*c) + [" ip address " + new]
 
 
-class Cvt_Int_IPAddrSec(DiffConvert_Int):
+class Cvt_Int_IPAddrSec(Context_Int):
     cmd = "ip-address-secondary", None
     block = "int-vrf-post"
 
     def remove(self, old, c, addr):
         return self.enter(*c) + [" no ip address %s secondary" % addr]
 
     def update(self, old, upd, new, c, addr):
@@ -200,15 +200,15 @@
 
 # =============================================================================
 # ...
 # =============================================================================
 
 
 
-class Cvt_Int_IPFlowMon(DiffConvert_Int):
+class Cvt_Int_IPFlowMon(Context_Int):
     cmd = "ip-flow-monitor", None
 
     def remove(self, old, c, dir_):
         return self.enter(*c) + [ " no ip flow monitor %s %s" % (old, dir_)]
 
     def update(self, old, upd, new, c, dir_):
         l = self.enter(*c)
@@ -236,27 +236,27 @@
 # VRF-NAME ADDR'.
 #
 # To handle this, we remove the helper address before the VRF change and
 # then re-add it after changing it.  This is achieved through blocks and
 # triggers.
 
 
-class DiffConvert_Int_IPHlprAddr(DiffConvert_Int):
+class _AbsCvt_Int_IPHlprAddr(Context_Int):
     "Abstract class for 'ip helper-address'."
 
     cmd = "ip-helper-address", None
 
     def _cmd(self, helper):
         return ("ip helper-address"
                 + (" global" if "global" in helper else "")
                 + (" vrf " + helper["vrf"] if "vrf" in helper else "")
                 + " " + helper["addr"])
 
 
-class Cvt_VRFPre_IPHlprAddr(DiffConvert_Int_IPHlprAddr):
+class Cvt_VRFPre_IPHlprAddr(_AbsCvt_Int_IPHlprAddr):
     """Class to handle removing 'ip helper-address' commands prior to a
     VRF change.
     """
 
     block = "int-vrf-pre"
 
     def remove(self, old, c, helper):
@@ -265,15 +265,15 @@
 
     def trigger(self, new, c, helper):
         # if we're not changing the helper address, we remove it prior
         # to changing VRF (to be re-added after the VRF change)
         return self.remove(new, c, helper)
 
 
-class Cvt_VRFPost_Int_IPHlprAddr(DiffConvert_Int_IPHlprAddr):
+class Cvt_VRFPost_Int_IPHlprAddr(_AbsCvt_Int_IPHlprAddr):
     """Class to handle adding (or re-adding, post a VRF change) 'ip
     helper-address' commands.
     """
 
     block = "int-vrf-post"
 
     # removing helper addresses is done before the VRF changes
@@ -285,25 +285,25 @@
 
 # =============================================================================
 # ...
 # =============================================================================
 
 
 
-class Cvt_Int_IPIGMPVer(DiffConvert_Int):
+class Cvt_Int_IPIGMPVer(Context_Int):
     cmd = "ip-igmp-version",
 
     def remove(self, old, c):
         return self.enter(*c) + [" no ip igmp version"]
 
     def update(self, old, upd, new, c):
         return self.enter(*c) + [" ip igmp version %d" % new]
 
 
-class Cvt_Int_IPMcastBdry(DiffConvert_Int):
+class Cvt_Int_IPMcastBdry(Context_Int):
     cmd = "ip-multicast-boundary",
 
     def remove(self, old, c):
         return self.enter(*c) + [" no ip multicast boundary"]
 
     def update(self, old, upd, new, c):
         return self.enter(*c) + [" ip multicast boundary " + new]
@@ -312,79 +312,79 @@
 
 # =============================================================================
 # ip ospf ...
 # =============================================================================
 
 
 
-class Cvt_Int_IPOSPFArea(DiffConvert_Int):
+class Cvt_Int_IPOSPFArea(Context_Int):
     cmd = "ip-ospf", "area"
 
     def remove(self, old, c):
         return self.enter(*c) + [
                    " no ip ospf %d area %s" % (old["process"], old["id"])]
 
     def update(self, old, upd, new, c):
         return self.enter(*c) + [
                    " ip ospf %d area %s" % (new["process"], new["id"])]
 
 
-class Cvt_Int_IPOSPFAuth(DiffConvert_Int):
+class Cvt_Int_IPOSPFAuth(Context_Int):
     cmd = "ip-ospf", "authentication"
 
     def remove(self, old, c):
         return self.enter(*c) + [" no ip ospf authentication"]
 
     def update(self, old, upd, new, c):
         return self.enter(*c) + [" ip ospf authentication " + new]
 
 
-class Cvt_Int_IPOSPFCost(DiffConvert_Int):
+class Cvt_Int_IPOSPFCost(Context_Int):
     cmd = "ip-ospf", "cost"
 
     def remove(self, old, c):
         return self.enter(*c) + [" no ip ospf cost"]
 
     def update(self, old, upd, new, c):
         return self.enter(*c) + [" ip ospf cost " + str(new)]
 
 
-class Cvt_Int_IPOSPFDeadIvl(DiffConvert_Int):
+class Cvt_Int_IPOSPFDeadIvl(Context_Int):
     cmd = "ip-ospf", "dead-interval"
 
     def remove(self, old, c):
         return self.enter(*c) + [" no ip ospf dead-interval"]
 
     def update(self, old, upd, new, c):
         return self.enter(*c) + [" ip ospf dead-interval " + str(new)]
 
 
-class Cvt_Int_IPOSPFHelloIvl(DiffConvert_Int):
+class Cvt_Int_IPOSPFHelloIvl(Context_Int):
     cmd = "ip-ospf", "hello-interval"
 
     def remove(self, old, c):
         return self.enter(*c) + [" no ip ospf hello-interval"]
 
     def update(self, old, upd, new, c):
         return self.enter(*c) + [" ip ospf hello-interval " + str(new)]
 
 
-class Cvt_Int_IPOSPFMsgDigKey(DiffConvert_Int):
+class Cvt_Int_IPOSPFMsgDigKey(Context_Int):
     cmd = "ip-ospf", "message-digest-key", None
 
     def remove(self, old, c, id_):
         return self.enter(*c) + [
                    " no ip ospf message-digest-key " + str(id_)]
 
     def update(self, old, upd, new, c, id_):
         return self.enter(*c) + [
                    " ip ospf message-digest-key %d md5 %s" % (id_, new)]
 
 
-class Cvt_Int_IPOSPFNet(DiffConvert_Int):
+class Cvt_Int_IPOSPFNet(Context_Int):
     cmd = "ip-ospf", "network"
 
     def remove(self, old, c):
         return self.enter(*c) + [" no ip ospf network"]
 
     def update(self, old, upd, new, c):
         return self.enter(*c) + [" ip ospf network " + new]
@@ -393,25 +393,25 @@
 
 # =============================================================================
 # ip pim ...
 # =============================================================================
 
 
 
-class Cvt_Int_IPPIMMode(DiffConvert_Int):
+class Cvt_Int_IPPIMMode(Context_Int):
     cmd = "ip-pim", "mode"
 
     def remove(self, old, c):
         return self.enter(*c) + [" no ip pim %s-mode" % old]
 
     def update(self, old, upd, new, c):
         return self.enter(*c) + [" ip pim %s-mode" % new]
 
 
-class Cvt_Int_IPPIMBSRBdr(DiffConvert_Int):
+class Cvt_Int_IPPIMBSRBdr(Context_Int):
     cmd = "ip-pim", "bsr-border"
     block = "int-vrf-post"
 
     def remove(self, old, c):
         return self.enter(*c) + [" no ip pim bsr-border"]
 
     def update(self, old, upd, new, c):
@@ -421,39 +421,39 @@
 
 # =============================================================================
 # ip (other) ...
 # =============================================================================
 
 
 
-class Cvt_Int_IPPolicyRtMap(DiffConvert_Int):
+class Cvt_Int_IPPolicyRtMap(Context_Int):
     cmd = "ip-policy-route-map",
 
     def remove(self, old, c):
         return self.enter(*c) + [" no ip policy route-map"]
 
     def update(self, old, upd, new, c):
         return self.enter(*c) + [" ip policy route-map " + new]
 
 
-class Cvt_Int_IPProxyARP(DiffConvert_Int):
+class Cvt_Int_IPProxyARP(Context_Int):
     cmd = "ip-proxy-arp",
 
     def remove(self, old, c):
         # if proxy ARP was disabled and we remove it, we're reverting to
         # the default of enabled
         if not old:
             return self.enter(*c) + [" ip proxy-arp"]
 
     def update(self, old, upd, new, c):
         return self.enter(*c) + [
                    " " + ("" if new else "no ") + "ip proxy-arp"]
 
 
-class Cvt_Int_IPVerifyUni(DiffConvert_Int):
+class Cvt_Int_IPVerifyUni(Context_Int):
     cmd = "ip-verify-unicast",
 
     def remove(self, old, c):
         return self.enter(*c) + [" no ip verify unicast"]
 
     def update(self, old, upd, new, c):
         return self.enter(*c) + [" ip verify unicast " + new]
@@ -462,36 +462,36 @@
 
 # =============================================================================
 # ipv6 ...
 # =============================================================================
 
 
 
-class Cvt_Int_IPv6Addr(DiffConvert_Int):
+class Cvt_Int_IPv6Addr(Context_Int):
     cmd = "ipv6-address", None
     block = "int-vrf-post"
 
     def remove(self, old, c, addr):
         return self.enter(*c) + [" no ipv6 address " + addr]
 
     def update(self, old, upd, new, c, addr):
         return self.enter(*c) + [" ipv6 address " + addr]
 
 
-class Cvt_Int_IPv6MultBdry(DiffConvert_Int):
+class Cvt_Int_IPv6MultBdry(Context_Int):
     cmd = "ipv6-multicast-boundary-scope",
 
     def remove(self, old, c):
         return self.enter(*c) + [" no ipv6 multicast boundary scope"]
 
     def update(self, old, upd, new, c):
         return self.enter(*c) + [ " ipv6 multicast boundary scope %d" % new]
 
 
-class Cvt_Int_IPv6NDPfx(DiffConvert_Int):
+class Cvt_Int_IPv6NDPfx(Context_Int):
     cmd = "ipv6-nd-prefix", None
     block = "int-vrf-post"
 
     def remove(self, old, c, pfx):
         return self.enter(*c) + [" no ipv6 nd prefix " + pfx]
 
     def update(self, old, upd, new, c, pfx):
@@ -500,46 +500,46 @@
             e = "%d %d" % (new["valid-lifetime"], new["preferred-lifetime"])
         else:
             # we're using absolute 'until' date/time
             e = "at %s %s" % (new["valid-until"], new["preferred-until"])
         return self.enter(*c) + [" ipv6 nd prefix %s %s" % (pfx, e)]
 
 
-class Cvt_Int_IPv6PIMBSRBdr(DiffConvert_Int):
+class Cvt_Int_IPv6PIMBSRBdr(Context_Int):
     cmd = "ipv6-pim", "bsr-border"
     block = "int-vrf-post"
 
     def remove(self, old, c):
         return self.enter(*c) + [" no ipv6 pim bsr border"]
 
     def update(self, old, upd, new, c):
         return self.enter(*c) + [" ipv6 pim bsr border"]
 
 
-class Cvt_Int_IPv6PolicyRtMap(DiffConvert_Int):
+class Cvt_Int_IPv6PolicyRtMap(Context_Int):
     cmd = "ipv6-policy-route-map",
 
     def remove(self, old, c):
         return self.enter(*c) + [" no ipv6 policy route-map"]
 
     def update(self, old, upd, new, c):
         return self.enter(*c) + [" ipv6 policy route-map " + new]
 
 
-class Cvt_Int_IPv6TrafFilt(DiffConvert_Int):
+class Cvt_Int_IPv6TrafFilt(Context_Int):
     cmd = "ipv6-traffic-filter", None
 
     def remove(self, old, c, dir_):
         return self.enter(*c) + [" no ipv6 traffic-filter " + dir_]
 
     def update(self, old, upd, new, c, dir_):
         return self.enter(*c) + [ " ipv6 traffic-filter %s %s" % (new, dir_)]
 
 
-class Cvt_Int_IPv6VerifyUni(DiffConvert_Int):
+class Cvt_Int_IPv6VerifyUni(Context_Int):
     cmd = "ipv6-verify-unicast",
 
     def remove(self, old, c):
         return self.enter(*c) + [" no ipv6 verify unicast"]
 
     def update(self, old, upd, new, c):
         return self.enter(*c) + [" ipv6 verify unicast " + new]
@@ -548,15 +548,15 @@
 
 # =============================================================================
 # mpls ...
 # =============================================================================
 
 
 
-class Cvt_Int_MPLSIP(DiffConvert_Int):
+class Cvt_Int_MPLSIP(Context_Int):
     cmd = "mpls-ip",
 
     def remove(self, old, c):
         return self.enter(*c) + [" no mpls ip"]
 
     def update(self, old, upd, new, c):
         return self.enter(*c) + [" mpls ip"]
@@ -565,15 +565,15 @@
 
 # =============================================================================
 # mtu ...
 # =============================================================================
 
 
 
-class Cvt_Int_MTU(DiffConvert_Int):
+class Cvt_Int_MTU(Context_Int):
     cmd = tuple()
     ext = "mtu",
 
     def remove(self, old, c):
         # if interface is in a port-channel, the MTU is set in the
         # port-channel interface
         if "channel-group" in old:
@@ -592,59 +592,59 @@
 
 # =============================================================================
 # ospfv3 ...
 # =============================================================================
 
 
 
-class Cvt_Int_OSPFv3Area(DiffConvert_Int):
+class Cvt_Int_OSPFv3Area(Context_Int):
     cmd = "ospfv3", "area", None
 
     def remove(self, old, c, proto):
         return self.enter(*c) + [
                    " no ospfv3 %d %s area %s"
                        % (old["process"], proto, old["id"])]
 
     def update(self, old, upd, new, c, proto):
         return self.enter(*c) + [
                    " ospfv3 %d %s area %s"
                        % (new["process"], proto, new["id"])]
 
 
-class Cvt_Int_OSPFv3Cost(DiffConvert_Int):
+class Cvt_Int_OSPFv3Cost(Context_Int):
     cmd = "ospfv3", "cost"
 
     def remove(self, old, c):
         return self.enter(*c) + [" no ospfv3 cost"]
 
     def update(self, old, upd, new, c):
         return self.enter(*c) + [" ospfv3 cost " + str(new)]
 
 
-class Cvt_Int_OSPFv3DeadIvl(DiffConvert_Int):
+class Cvt_Int_OSPFv3DeadIvl(Context_Int):
     cmd = "ospfv3", "dead-interval"
 
     def remove(self, old, c):
         return self.enter(*c) + [" no ospfv3 dead-interval"]
 
     def update(self, old, upd, new, c):
         return self.enter(*c) + [" ospfv3 dead-interval " + str(new)]
 
 
-class Cvt_Int_OSPFv3HelloIvl(DiffConvert_Int):
+class Cvt_Int_OSPFv3HelloIvl(Context_Int):
     cmd = "ospfv3", "hello-interval"
 
     def remove(self, old, c):
         return self.enter(*c) + [" no ospfv3 hello-interval"]
 
     def update(self, old, upd, new, c):
         return self.enter(*c) + [" ospfv3 hello-interval " + str(new)]
 
 
-class Cvt_Int_OSPFv3Net(DiffConvert_Int):
+class Cvt_Int_OSPFv3Net(Context_Int):
     cmd = "ospfv3", "network"
 
     def remove(self, old, c):
         return self.enter(*c) + [" no ospfv3 network"]
 
     def update(self, old, upd, new, c):
         return self.enter(*c) + [" ospfv3 network " + new]
@@ -653,15 +653,15 @@
 
 # =============================================================================
 # ...
 # =============================================================================
 
 
 
-class Cvt_Int_ServPol(DiffConvert_Int):
+class Cvt_Int_ServPol(Context_Int):
     cmd = "service-policy", None, None
 
     def _cmd(self, type_, dir_, name):
         return ("service-policy"
                 + ((" type " + type_) if type_ else "")
                 + " " + dir_ + " " + name)
 
@@ -684,112 +684,112 @@
 
 # =============================================================================
 # standby ...
 # =============================================================================
 
 
 
-class Cvt_Int_NoStandbyIPSec(DiffConvert_Int):
+class Cvt_Int_NoStandbyIPSec(Context_Int):
     cmd = "standby", "group", None, "ip-secondary", None
     block = "int-vrf-pre"
 
     def remove(self, old, c, grp, addr):
         return self.enter(*c) + [
                    " no standby %d ip %s secondary" % (grp, addr)]
 
 
-class Cvt_Int_StandbyIP(DiffConvert_Int):
+class Cvt_Int_StandbyIP(Context_Int):
     cmd = "standby", "group", None, "ip"
     block = "int-vrf-post"
 
     def remove(self, old, c, grp):
         return self.enter(*c) + [" no standby %d ip" % grp]
 
     def update(self, old, upd, new, c, grp):
         return self.enter(*c) + [" standby %d ip %s" % (grp, new)]
 
 
-class Cvt_Int_StandbyIPSec(DiffConvert_Int):
+class Cvt_Int_StandbyIPSec(Context_Int):
     cmd = "standby", "group", None, "ip-secondary", None
     block = "int-vrf-post"
 
     def update(self, old, upd, new, c, grp, addr):
         return self.enter(*c) + [
                    " standby %d ip %s secondary" % (grp, addr)]
 
 
-class Cvt_Int_StandbyIPv6(DiffConvert_Int):
+class Cvt_Int_StandbyIPv6(Context_Int):
     cmd = "standby", "group", None, "ipv6", None
     block = "int-vrf-post"
 
     def remove(self, old, c, grp, addr):
         return self.enter(*c) + [" no standby %d ipv6 %s" % (grp, addr)]
 
     def update(self, old, upd, new, c, grp, addr):
         return self.enter(*c) + [" standby %d ipv6 %s" % (grp, addr)]
 
 
-class Cvt_Int_StandbyPreempt(DiffConvert_Int):
+class Cvt_Int_StandbyPreempt(Context_Int):
     cmd = "standby", "group", None, "preempt"
 
     def remove(self, old, c, grp):
         return self.enter(*c) + [" no standby %d preempt" % grp]
 
     def update(self, old, upd, new, c, grp):
         return self.enter(*c) + [" standby %d preempt" % grp]
 
 
-class Cvt_Int_StandbyPri(DiffConvert_Int):
+class Cvt_Int_StandbyPri(Context_Int):
     cmd = "standby", "group", None, "priority"
 
     def remove(self, old, c, grp):
         return self.enter(*c) + [" no standby %d priority" % grp]
 
     def update(self, old, upd, new, c, grp):
         return self.enter(*c) + [" standby %d priority %d" % (grp, new)]
 
 
-class Cvt_Int_StandbyTimers(DiffConvert_Int):
+class Cvt_Int_StandbyTimers(Context_Int):
     cmd = "standby", "group", None, "timers"
 
     def remove(self, old, c, grp):
         return self.enter(*c) + [" no standby %d timers" % grp]
 
     def update(self, old, upd, new, c, grp):
         return self.enter(*c) + [" standby %d timers %s" % (grp, new)]
 
 
-class Cvt_Int_StandbyTrk(DiffConvert_Int):
+class Cvt_Int_StandbyTrk(Context_Int):
     cmd = "standby", "group", None, "track", None
 
     def remove(self, old, c, grp, obj):
         return self.enter(*c) + [" no standby %d track %s" % (grp, obj)]
 
     def update(self, old, upd, new, c, grp, obj):
         return self.enter(*c) + [
                    " standby %d track %s%s"
                        % (grp, obj, (" " + new) if new else "")]
 
 
-class Cvt_Int_StandbyVer(DiffConvert_Int):
+class Cvt_Int_StandbyVer(Context_Int):
     cmd = "standby", "version"
     block = "int-pre"
 
     def update(self, old, upd, new, c):
         # only set this here if we're switching to version >= 2 (so we
         # can potentially use any high-numbered groups)
         #
         # version 1 is the default so is effectively removing 'standby
         # version' in the Cvt_Int_NoStandbyVer class
         if new < 2:
             return
         return self.enter(*c) + [" standby version " + str(new)]
 
 
-class Cvt_Int_NoStandbyVer(DiffConvert_Int):
+class Cvt_Int_NoStandbyVer(Context_Int):
     cmd = "standby", "version"
     block = "int-post"
 
     def remove(self, old, c):
         return self.enter(*c) + [" no standby version"]
 
     def update(self, old, upd, new, c):
@@ -803,15 +803,15 @@
 
 # =============================================================================
 # ...
 # =============================================================================
 
 
 
-class Cvt_Int_StormCtrl(DiffConvert_Int):
+class Cvt_Int_StormCtrl(Context_Int):
     cmd = "storm-control", None
 
     def remove(self, old, c, traffic):
         return self.enter(*c) + [" no storm-control %s level" % traffic]
 
     def update(self, old, upd, new, c, traffic):
         return self.enter(*c) + [
@@ -821,15 +821,15 @@
 
 # =============================================================================
 # switchport ...
 # =============================================================================
 
 
 
-class Cvt_Int_SwPort(DiffConvert_Int):
+class Cvt_Int_SwPort(Context_Int):
     cmd = "switchport",
 
     def remove(self, old, c):
         # if the 'switchport' option is not present, that doesn't mean
         # it's disabled but just that it's not specified, so we assume
         # the default is for it to be disabled
         #
@@ -839,35 +839,35 @@
         return self.enter(*c) + [" no switchport"]
 
     def update(self, old, upd, new, c):
         return self.enter(*c) + [
                    " " + ("" if upd else "no ") + "switchport"]
 
 
-class Cvt_Int_SwPortMode(DiffConvert_Int):
+class Cvt_Int_SwPortMode(Context_Int):
     cmd = "switchport-mode",
 
     def remove(self, old, c):
         return self.enter(*c) + [" no switchport mode"]
 
     def update(self, old, upd, new, c):
         return self.enter(*c) + [" switchport mode " + new]
 
 
-class Cvt_Int_SwPortNoNeg(DiffConvert_Int):
+class Cvt_Int_SwPortNoNeg(Context_Int):
     cmd = "switchport-nonegotiate",
 
     def remove(self, old, c):
         return self.enter(*c) + [" no switchport nonegotiate"]
 
     def update(self, old, upd, new, c):
         return self.enter(*c) + [" switchport nonegotiate"]
 
 
-class Cvt_Int_SwPortTrkNtv(DiffConvert_Int):
+class Cvt_Int_SwPortTrkNtv(Context_Int):
     # we just match the interface as we need to look inside it to see if
     # the interface is part of a channel group
     cmd = tuple()
     ext = "switchport-trunk-native",
 
     def remove(self, old, c):
         # if this interface is in a port-channel, we do all changes
@@ -883,15 +883,15 @@
         if "channel-group" in new:
             return None
 
         return self.enter(*c) + [
                    " switchport trunk native vlan " + str(self.get_ext(new))]
 
 
-class Cvt_Int_SwPortTrkAlw(DiffConvert_Int):
+class Cvt_Int_SwPortTrkAlw(Context_Int):
     # we just match the interface as we need to look inside it to see if
     # the interface is part of a channel group
     cmd = tuple()
     ext = "switchport-trunk-allow",
 
     def remove(self, old, c):
         # if this interface is in a port-channel, we do all changes
@@ -937,25 +937,25 @@
 
 # =============================================================================
 # ...
 # =============================================================================
 
 
 
-class Cvt_Int_PcMinLinks(DiffConvert_Int):
+class Cvt_Int_PcMinLinks(Context_Int):
     cmd = "port-channel-min-links",
 
     def remove(self, old, c):
         return self.enter(*c) + [" no port-channel min-links"]
 
     def update(self, old, upd, new, c):
         return self.enter(*c) + [" port-channel min-links " + str(new)]
 
 
-class Cvt_Int_XConn(DiffConvert_Int):
+class Cvt_Int_XConn(Context_Int):
     cmd = "xconnect",
 
     def remove(self, old, c):
         return self.enter(*c) + [" no xconnect"]
 
     def update(self, old, upd, new, c):
         return self.enter(*c) + [" xconnect " + new]
@@ -967,15 +967,15 @@
 # =============================================================================
 
 
 
 # we put the 'interface / no shutdown' at the end to only enable the
 # interface once it's been correctly [re]configured
 
-class Cvt_Int_NoShutdown(DiffConvert_Int):
+class Cvt_Int_NoShutdown(Context_Int):
     cmd = "shutdown",
     block = "int-noshutdown"
 
     def update(self, old, upd, new, c):
         # we only 'no shutdown' if we are enabling the port ('shutdown'
         # happens at the start of interface configuration)
         if not new:
```

### Comparing `asimtote-0.16.5/asimtote/ios/converters/lists.py` & `asimtote-0.16.6/asimtote/ios/converters/lists.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,59 +6,59 @@
 
 # --- imports ---
 
 
 
 from ..utils import explain_diffs
 
-from ...diff import DiffConvert
+from ...diff import Convert
 
 
 
 # --- converter classes ---
 
 
 
 # =============================================================================
 # ip[v6] access-list ...
 # =============================================================================
 
 
 
-class Cvt_IPACL_Std(DiffConvert):
+class Cvt_IPACL_Std(Convert):
     cmd = "ip-access-list-standard", None
 
     def remove(self, old, _, acl_name):
         return "no ip access-list standard " + acl_name
 
     def update(self, old, upd, new, _, acl_name):
         r = []
         if old:
             r.append("no ip access-list standard " + acl_name)
         r.append("ip access-list standard " + acl_name)
         r.extend(explain_diffs(old, new, indent=" "))
         return r
 
 
-class Cvt_IPACL_Ext(DiffConvert):
+class Cvt_IPACL_Ext(Convert):
     cmd = "ip-access-list-extended", None
 
     def remove(self, old, _, acl_name):
         return "no ip access-list extended " + acl_name
 
     def update(self, old, upd, new, _, acl_name):
         r = []
         if old:
             r.append("no ip access-list extended " + acl_name)
         r.append("ip access-list extended " + acl_name)
         r.extend(explain_diffs(old, new, indent=" "))
         return r
 
 
-class Cvt_IPv6ACL(DiffConvert):
+class Cvt_IPv6ACL(Convert):
     cmd = "ipv6-access-list", None
 
     def remove(self, old, _, acl_name):
         return "no ipv6 access-list " + acl_name
 
     def update(self, old, upd, new, _, acl_name):
         r = []
@@ -72,15 +72,15 @@
 
 # =============================================================================
 # ip as-path access-list ...
 # =============================================================================
 
 
 
-class Cvt_IPASPathACL(DiffConvert):
+class Cvt_IPASPathACL(Convert):
     cmd = "ip-as-path-access-list", None
 
     def to_str(self, rule):
         action, re = rule
         return action + " " + re
 
     def remove(self, old, _, num):
@@ -98,30 +98,30 @@
 
 # =============================================================================
 # ip[v6] prefix-list ...
 # =============================================================================
 
 
 
-class Cvt_IPPfxList(DiffConvert):
+class Cvt_IPPfxList(Convert):
     cmd = "ip-prefix-list", None
 
     def remove(self, old, _, pfx_name):
         return "no ip prefix-list " + pfx_name
 
     def update(self, old, upd, new, _, pfx_name):
         r = []
         if old:
             r.append("no ip prefix-list " + pfx_name)
         r.extend(explain_diffs(
                      old, new, prefix="ip prefix-list %s " % pfx_name))
         return r
 
 
-class Cvt_IPv6PfxList(DiffConvert):
+class Cvt_IPv6PfxList(Convert):
     cmd = "ipv6-prefix-list", None
 
     def remove(self, old, _, pfx_name):
         return "no ipv6 prefix-list " + pfx_name
 
     def update(self, old, upd, new, _, pfx_name):
         r = []
```

### Comparing `asimtote-0.16.5/asimtote/ios/converters/other.py` & `asimtote-0.16.6/asimtote/ios/converters/other.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,29 +4,29 @@
 
 
 
 # --- imports ---
 
 
 
-from ...diff import DiffConvert
+from ...diff import Convert
 
 
 
 # --- converter classes ---
 
 
 
 # =============================================================================
 # hostname ...
 # =============================================================================
 
 
 
-class Cvt_Hostname(DiffConvert):
+class Cvt_Hostname(Convert):
     cmd = "hostname",
 
     def remove(self, old, c):
         return "no hostname"
 
     def update(self, old, upd, new, c):
         return "hostname " + new
@@ -35,27 +35,27 @@
 
 # =============================================================================
 # [no] spanning-tree ...
 # =============================================================================
 
 
 
-class Cvt_NoSTP(DiffConvert):
+class Cvt_NoSTP(Convert):
     cmd = "no-spanning-tree-vlan", None
 
     def remove(self, old, c, tag):
         # removing 'no spanning-tree' enables spanning-tree
         return "spanning-tree vlan %d" % tag
 
     def update(self, old, upd, new, c, tag):
         # adding 'no spanning-tree' disables spanning-tree
         return "no spanning-tree vlan %d" % tag
 
 
-class Cvt_STPPri(DiffConvert):
+class Cvt_STPPri(Convert):
     cmd = "spanning-tree-vlan-priority", None
 
     def remove(self, old, c, tag):
         return "no spanning-tree vlan %d priority" % tag
 
     def update(self, old, upd, new, c, tag):
         return "spanning-tree vlan %d priority %d" % (tag, new)
@@ -73,80 +73,80 @@
 # destroyed and created anew
 #
 # the parameters of the type of track can, however, be changed, e.g. the
 # specific interface or route that's being tracked
 
 
 
-class Cvt_Track(DiffConvert):
+class Cvt_Track(Convert):
     cmd = "track", None
 
     def remove(self, old, c, obj_num):
         return "no track %d" % obj_num
 
 
-class Cvt_TrackUpdate(DiffConvert):
+class Cvt_TrackUpdate(Convert):
     cmd = "track", None
     ext = "type",
 
     # when the type of a tracking object is changed, it must be deleted
     # and the new type created - this does not need to happen when a new
     # one is added, though
 
     def add(self, new, c, obj_num):
         pass
 
     def update(self, old, upd, new, c, obj_num):
         return "no track " + str(obj_num)
 
 
-class DiffConvert_TrackCreate(DiffConvert):
+class Context_TrackCreate(Convert):
     context = "track", None
     block = "track-create"
     trigger_blocks = { "track-sub" }
 
 
-class Cvt_TrackInterface(DiffConvert_TrackCreate):
+class Cvt_TrackInterface(Context_TrackCreate):
     cmd = "interface",
 
     def update(self, old, upd, new, c):
         obj_num, = c
         return ["track %d interface %s %s"
                     % (obj_num, new["interface"], new["capability"])]
 
 
-class Cvt_TrackList(DiffConvert_TrackCreate):
+class Cvt_TrackList(Context_TrackCreate):
     cmd = "list",
 
     def update(self, old, upd, new, c):
         obj_num, = c
         if new["type"] == "boolean":
             return ["track %d list boolean %s" % (obj_num, new["op"])]
 
         return ValueError("unhandled track list type:" + l["type"])
 
 
-class Cvt_TrackRoute(DiffConvert_TrackCreate):
+class Cvt_TrackRoute(Context_TrackCreate):
     cmd = "route",
 
     def update(self, old, upd, new, c):
         obj_num, = c
         return ["track %d %s route %s %s"
                     % (obj_num, new["proto"], new["net"], new["measure"])]
 
 
-class DiffConvert_TrackSub(DiffConvert):
+class Context_TrackSub(Convert):
     context = Cvt_Track.cmd
     block = "track-sub"
 
     def enter(self, obj_num):
         return ["track %d" % obj_num]
 
 
-class Cvt_Track_Delay(DiffConvert_TrackSub):
+class Cvt_Track_Delay(Context_TrackSub):
     cmd = "delay",
 
     def truncate(self, old, rem, new, c):
         # delays cannot individually be removed from a tracking object;
         # only all delays at the same time
         #
         # to remove a delay, we have to clear them all and re-add the
@@ -163,35 +163,35 @@
     def update(self, old, upd, new, c):
         c = self.enter(*c)
         for dir_ in sorted(upd):
             c.append(" delay %s %d" % (dir_, new[dir_]))
         return c
 
 
-class Cvt_Track_IPVRF(DiffConvert_TrackSub):
+class Cvt_Track_IPVRF(Context_TrackSub):
     cmd = "ip-vrf",
 
     def remove(self, old, c):
         return self.enter(*c) + [" no ip vrf"]
 
     def update(self, old, upd, new, c):
         return self.enter(*c) + [" ip vrf " + new]
 
 
-class Cvt_Track_IPv6VRF(DiffConvert_TrackSub):
+class Cvt_Track_IPv6VRF(Context_TrackSub):
     cmd = "ipv6-vrf",
 
     def remove(self, old, c):
         return self.enter(*c) + [" no ipv6 vrf"]
 
     def update(self, old, upd, new, c):
         return self.enter(*c) + [" ipv6 vrf " + new]
 
 
-class Cvt_Track_ListObj(DiffConvert_TrackSub):
+class Cvt_Track_ListObj(Context_TrackSub):
     cmd = "object", None
 
     def remove(self, old, c, sub_obj_num):
         return self.enter(*c) + [" no object " + str(sub_obj_num)]
 
     def update(self, old, upd, new, c, sub_obj_num):
         return self.enter(*c) + [" object " + str(sub_obj_num)]
@@ -200,30 +200,30 @@
 
 # =============================================================================
 # vlan ...
 # =============================================================================
 
 
 
-class Cvt_VLAN(DiffConvert):
+class Cvt_VLAN(Convert):
     cmd = "vlan", None
 
     def remove(self, old, c, tag):
         return "no vlan %d" % tag
 
     def add(self, new, c, tag):
         return "vlan %d" % tag
 
 
-class DiffConvert_VLAN(DiffConvert):
+class Context_VLAN(Convert):
     def enter(self, tag):
         return ["vlan %d" % tag]
 
 
-class Cvt_VLAN_Name(DiffConvert_VLAN):
+class Cvt_VLAN_Name(Context_VLAN):
     context = Cvt_VLAN.cmd
     cmd = "name",
 
     def remove(self, old, c):
         return self.enter(*c) + [" no name"]
 
     def update(self, old, upd, new, c):
@@ -233,73 +233,74 @@
 
 # =============================================================================
 # vrf definition ...
 # =============================================================================
 
 
 
-class Cvt_VRF(DiffConvert):
+class Cvt_VRF(Convert):
     cmd = "vrf", None
 
     def remove(self, old, c, name):
         return "no vrf definition " + name
 
     def add(self, new,  c, name):
         return "vrf definition " + name
 
 
-class DiffConvert_VRF(DiffConvert):
+class Context_VRF(Convert):
     context = Cvt_VRF.cmd
 
     def enter(self, vrf_name):
         return ["vrf definition " + vrf_name]
 
 
-class Cvt_VRF_RD(DiffConvert_VRF):
+class Cvt_VRF_RD(Context_VRF):
     cmd = "rd",
 
     def remove(self, old, c):
         return self.enter(*c) + [" no rd " + old]
 
     def update(self, old, upd, new, c):
-        l = list(super().enter(*c))
+        l = self.enter(*c)
         if old:
             l.append(" no rd " + old)
         l.append(" rd " + new)
         return l
 
 
-class Cvt_VRF_RT(DiffConvert_VRF):
+class Cvt_VRF_RT(Context_VRF):
     cmd = "route-target", None, None
 
     def truncate(self, old, rem, new, c, dir_, rt):
         return self.enter(*c) + [" no route-target %s %s" % (dir_, rt)]
 
     def update(self, old, upd, new, c, dir_, rt):
         return self.enter(*c) + [" route-target %s %s" % (dir_, rt)]
 
 
-class Cvt_VRF_AF(DiffConvert_VRF):
+class Cvt_VRF_AF(Context_VRF):
     cmd = "address-family", None
 
     def remove(self, old, c, af):
         return self.enter(*c) + [" no address-family " + af]
 
     def add(self, new, c, af):
         return self.enter(*c) + [" address-family " + af]
 
 
-class DiffConvert_VRF_AF(DiffConvert_VRF):
-    context = DiffConvert_VRF.context + Cvt_VRF_AF.cmd
+class Context_VRF_AF(Context_VRF):
+    context = Context_VRF.context + Cvt_VRF_AF.cmd
 
-    def enter(self, vrf_name, af):
-        return [*super().enter(vrf_name), " address-family " + af]
+    def enter(self, *c):
+        c_super, (af, ) = c[:-1], c[-1:]
+        return super().enter(*c_super) + [" address-family " + af]
 
 
-class Cvt_VRF_AF_RT(DiffConvert_VRF_AF):
+class Cvt_VRF_AF_RT(Context_VRF_AF):
     cmd = "route-target", None, None
 
     def truncate(self, old, rem, new, c, dir_, rt):
         return self.enter(*c) + ["  no route-target %s %s" % (dir_, rt)]
 
     def update(self, old, upd, new, c, dir_, rt):
         return self.enter(*c) + ["  route-target %s %s" % (dir_, rt)]
```

### Comparing `asimtote-0.16.5/asimtote/ios/converters/router.py` & `asimtote-0.16.6/asimtote/ios/converters/router.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,30 +8,30 @@
 
 
 
 import netaddr
 
 from deepops import deepget
 
-from ...diff import DiffConvert
+from ...diff import Convert
 from ..utils import VRF_GLOBAL
 
 
 
 # --- converter classes ---
 
 
 
 # =============================================================================
 # ip[v6] route ...
 # =============================================================================
 
 
 
-class Cvt_IPRoute(DiffConvert):
+class Cvt_IPRoute(Convert):
     cmd = "ip-route", None, None, None
 
     def _cmd(self, vrf, net, r):
         n = netaddr.IPNetwork(net)
 
         return ("ip route"
                 + ((" vrf " + vrf) if vrf else "")
@@ -44,15 +44,15 @@
     def remove(self, old, c, vrf, net, id):
         return "no " + self._cmd(vrf, net, old)
 
     def update(self, old, upd, new, c, vrf, net, id):
         return self._cmd(vrf, net, new)
 
 
-class Cvt_IPv6Route(DiffConvert):
+class Cvt_IPv6Route(Convert):
     cmd = "ipv6-route", None, None, None
 
     def _cmd(self, vrf, net, r):
         return ("ipv6 route"
                 + ((" vrf " + vrf) if vrf else "")
                 + " " + net
                 + ((" " + r["interface"]) if "interface" in r else "")
@@ -70,81 +70,84 @@
 
 # =============================================================================
 # route-map ...
 # =============================================================================
 
 
 
-class Cvt_RtMap(DiffConvert):
+class Cvt_RtMap(Convert):
     cmd = "route-map", None
     block = "rtmap-del"
 
     def remove(self, old, c, rtmap_name):
         return "no route-map " + rtmap_name
 
 
-class DiffConvert_RtMap(DiffConvert):
+class Context_RtMap(Convert):
     context = Cvt_RtMap.cmd
 
 
-class Cvt_RtMap_Entry(DiffConvert_RtMap):
+class Cvt_RtMap_Entry(Context_RtMap):
     cmd = None,
     block = "rtmap-del"
 
     def remove(self, old, c, seq):
         rtmap_name, = c
         return "no route-map %s %d" % (rtmap_name, seq)
 
 
-class Cvt_RtMap_Entry_Action(DiffConvert_RtMap):
+class Cvt_RtMap_Entry_Action(Context_RtMap):
     cmd = None, "action"
     block = "rtmap-add"
 
     def update(self, old, upd, new, c, seq):
         rtmap_name, = c
         return "route-map %s %s %d" % (rtmap_name, new, seq)
 
 
-class DiffConvert_RtMap_Entry(DiffConvert_RtMap):
-    context = DiffConvert_RtMap.context + Cvt_RtMap_Entry.cmd
+class Context_RtMap_Entry(Context_RtMap):
+    context = Context_RtMap.context + Cvt_RtMap_Entry.cmd
 
+    # route-map entries require you to know the action type ('permit' or
+    # 'deny') when modifying them, which are in the dictionary element
+    # underneath, in our configuration model
     def enter(self, rtmap_name, seq, rtmap_dict):
         return ["route-map %s %s %d" % (rtmap_name, rtmap_dict["action"], seq)]
 
 
-class Cvt_RtMap_MatchCmty_DelExact(DiffConvert_RtMap_Entry):
+class Cvt_RtMap_MatchCmty_Exact_del(Context_RtMap_Entry):
     cmd = tuple()
     ext = "match", "community", "exact-match"
     block = "rtmap-del"
     trigger_blocks = { "rtmap-add-cmty" }
 
     # if removing the exact-match option, we need to clear the list and
     # recreate it without it
     def remove(self, old, c):
         if self.get_ext(old):
             l = self.enter(*c, old)
             l.append(" no match community")
             return l
 
 
-class DiffConvert_RtMap_MatchCmty(DiffConvert_RtMap_Entry):
+class _AbsCvt_RtMap_MatchCmty(Context_RtMap_Entry):
     cmd = tuple()
     ext = "match", "community", "communities", None
 
 
-class Cvt_RtMap_MatchCmty_Del(DiffConvert_RtMap_MatchCmty):
+class Cvt_RtMap_MatchCmty_del(_AbsCvt_RtMap_MatchCmty):
     block = "rtmap-del"
 
     def truncate(self, old, rem, new, c, cmty):
         l = self.enter(*c, old)
         l.append(" no match community " + cmty)
         return l
 
 
-class Cvt_RtMap_MatchCmty_add(DiffConvert_RtMap_MatchCmty):
+class Cvt_RtMap_MatchCmty_add(_AbsCvt_RtMap_MatchCmty):
     block = "rtmap-add-cmty"
 
     def update(self, old, upd, new, c, cmty):
         # TODO: need to handle applying 'exact-match' when list is the
         # same; will rework these to use context_offset to see if that
         # makes it easier (as we need the action from a higher context
         # but would like to set a lower context)
@@ -154,180 +157,180 @@
                      % (cmty, " exact-match" if exact_match else ""))
         return l
 
     def trigger(self, new, c, *args):
         return self.update(None, new, new, c, *args)
 
 
-class Cvt_RtMap_MatchIPAddr(DiffConvert_RtMap_Entry):
+class _AbsCvt_RtMap_MatchIPAddr(Context_RtMap_Entry):
     cmd = tuple()
     ext = "match", "ip-address"
 
-class Cvt_RtMap_MatchIPAddr_Del(Cvt_RtMap_MatchIPAddr):
+class Cvt_RtMap_MatchIPAddr_del(_AbsCvt_RtMap_MatchIPAddr):
     block = "rtmap-del"
 
     def truncate(self, old, rem, new, c):
         l = self.enter(*c, old)
         for addr in sorted(self.get_ext(rem)):
             l.append(" no match ip address " + addr)
         return l
 
-class Cvt_RtMap_MatchIPAddr_Add(Cvt_RtMap_MatchIPAddr):
+class Cvt_RtMap_MatchIPAddr_add(_AbsCvt_RtMap_MatchIPAddr):
     block = "rtmap-add"
 
     def update(self, old, upd, new, c):
         l = self.enter(*c, new)
         for addr in sorted(self.get_ext(upd)):
             l.append(" match ip address " + addr)
         return l
 
 
-class Cvt_RtMap_MatchIPPfxLst(DiffConvert_RtMap_Entry):
+class _AbsCvt_RtMap_MatchIPPfxLst(Context_RtMap_Entry):
     cmd = tuple()
     ext = "match", "ip-prefix-list"
 
-class Cvt_RtMap_MatchIPPfxLst_Del(Cvt_RtMap_MatchIPPfxLst):
+class Cvt_RtMap_MatchIPPfxLst_del(_AbsCvt_RtMap_MatchIPPfxLst):
     block = "rtmap-del"
 
     def truncate(self, old, rem, new, c):
         l = self.enter(*c, old)
         for pfx in sorted(self.get_ext(rem)):
             l.append(" no match ip address prefix-list " + pfx)
         return l
 
-class Cvt_RtMap_MatchIPPfxLst_Add(Cvt_RtMap_MatchIPPfxLst):
+class Cvt_RtMap_MatchIPPfxLst_add(_AbsCvt_RtMap_MatchIPPfxLst):
     block = "rtmap-add"
 
     def update(self, old, upd, new, c):
         l = self.enter(*c, new)
         for pfx in sorted(self.get_ext(upd)):
             l.append(" match ip address prefix-list " + pfx)
         return l
 
 
-class Cvt_RtMap_MatchIPv6Addr(DiffConvert_RtMap_Entry):
+class _AbsCvt_RtMap_MatchIPv6Addr(Context_RtMap_Entry):
     cmd = tuple()
     ext = "match", "ipv6-address"
 
-class Cvt_RtMap_MatchIPv6Addr_Del(Cvt_RtMap_MatchIPv6Addr):
+class Cvt_RtMap_MatchIPv6Addr_del(_AbsCvt_RtMap_MatchIPv6Addr):
     block = "rtmap-del"
 
     def truncate(self, old, rem, new, c):
         l = self.enter(*c, old)
         for addr in sorted(self.get_ext(rem)):
             l.append(" no match ipv6 address " + addr)
         return l
 
-class Cvt_RtMap_MatchIPv6Addr_Add(Cvt_RtMap_MatchIPv6Addr):
+class Cvt_RtMap_MatchIPv6Addr_add(_AbsCvt_RtMap_MatchIPv6Addr):
     block = "rtmap-add"
 
     def update(self, old, upd, new, c):
         l = self.enter(*c, new)
         for addr in sorted(self.get_ext(upd)):
             l.append(" match ipv6 address " + addr)
         return l
 
 
-class Cvt_RtMap_MatchIPv6PfxLst(DiffConvert_RtMap_Entry):
+class _AbsCvt_RtMap_MatchIPv6PfxLst(Context_RtMap_Entry):
     cmd = tuple()
     ext = "match", "ipv6-prefix-list"
 
-class Cvt_RtMap_MatchIPv6PfxLst_Del(Cvt_RtMap_MatchIPv6PfxLst):
+class Cvt_RtMap_MatchIPv6PfxLst_del(_AbsCvt_RtMap_MatchIPv6PfxLst):
     block = "rtmap-del"
 
     def truncate(self, old, rem, new, c):
         l = self.enter(*c, old)
         for pfx in sorted(self.get_ext(rem)):
             l.append(" no match ipv6 address prefix-list " + pfx)
         return l
 
-class Cvt_RtMap_MatchIPv6PfxLst_Add(Cvt_RtMap_MatchIPv6PfxLst):
+class Cvt_RtMap_MatchIPv6PfxLst_add(_AbsCvt_RtMap_MatchIPv6PfxLst):
     block = "rtmap-add"
 
     def update(self, old, upd, new, c):
         l = self.enter(*c, new)
         for pfx in sorted(self.get_ext(upd)):
             l.append(" match ipv6 address prefix-list " + pfx)
         return l
 
 
-class Cvt_RtMap_MatchTag(DiffConvert_RtMap_Entry):
+class _AbsCvt_RtMap_MatchTag(Context_RtMap_Entry):
     cmd = tuple()
     ext = "match", "tag"
 
-class Cvt_RtMap_MatchTag_Del(Cvt_RtMap_MatchTag):
+class Cvt_RtMap_MatchTag_del(_AbsCvt_RtMap_MatchTag):
     block = "rtmap-del"
 
     def truncate(self, old, rem, new, c):
         l = self.enter(*c, old)
         for tag in sorted(self.get_ext(rem)):
             l.append(" no match tag " + str(tag))
         return l
 
-class Cvt_RtMap_MatchTag_Add(Cvt_RtMap_MatchTag):
+class Cvt_RtMap_MatchTag_add(_AbsCvt_RtMap_MatchTag):
     block = "rtmap-add"
 
     def update(self, old, upd, new, c):
         l = self.enter(*c, new)
         for tag in sorted(self.get_ext(upd)):
             l.append(" match tag " + str(tag))
         return l
 
 
-class Cvt_RtMap_SetCmty(DiffConvert_RtMap_Entry):
+class _AbsCvt_RtMap_SetCmty(Context_RtMap_Entry):
     cmd = tuple()
     ext = "set", "community", "communities"
 
-class Cvt_RtMap_SetCmty_Del(Cvt_RtMap_SetCmty):
+class Cvt_RtMap_SetCmty_del(_AbsCvt_RtMap_SetCmty):
     block = "rtmap-del"
 
     def truncate(self, old, rem, new, c):
         l = self.enter(*c, old)
         for cmty in sorted(self.get_ext(rem)):
             l.append(" no set community " + cmty)
         return l
 
-class Cvt_RtMap_SetCmty_Add(Cvt_RtMap_SetCmty):
+class Cvt_RtMap_SetCmty_add(_AbsCvt_RtMap_SetCmty):
     block = "rtmap-add"
 
     # TODO: need to handle case where list is the same but 'additive'
     # is only addition or removal
     def update(self, old, upd, new, c):
         l = self.enter(*c, new)
         for cmty in sorted(self.get_ext(upd)):
             l.append(" set community "
                      + cmty
                      + (" additive" if "additive" in new["set"]["community"]
                             else ""))
         return l
 
 
-class Cvt_RtMap_SetIPNxtHop(DiffConvert_RtMap_Entry):
+class _AbsCvt_RtMap_SetIPNxtHop(Context_RtMap_Entry):
     cmd = tuple()
     ext = "set", "ip-next-hop"
 
     def _cmd(self, nexthop):
         addr = nexthop["addr"]
         vrf = None
         if "vrf" in nexthop:
             vrf = ("vrf " + nexthop["vrf"]) if nexthop["vrf"] else "global"
 
         return "set ip" + ((" " + vrf) if vrf else "") + " next-hop " + addr
 
-class Cvt_RtMap_SetIPNxtHop_Del(Cvt_RtMap_SetIPNxtHop):
+class Cvt_RtMap_SetIPNxtHop_del(_AbsCvt_RtMap_SetIPNxtHop):
     block = "rtmap-del"
 
     def remove(self, old, c):
         # we must remove all the 'set ip next-hop' commands individually
         l = self.enter(*c, old)
         for nexthop in self.get_ext(old):
             l.append(" no " + self._cmd(nexthop))
         return l
 
-class Cvt_RtMap_SetIPNxtHop_Add(Cvt_RtMap_SetIPNxtHop):
+class Cvt_RtMap_SetIPNxtHop_add(_AbsCvt_RtMap_SetIPNxtHop):
     block = "rtmap-add"
 
     def update(self, old, upd, new, c):
         # the 'set ip ... next-hop' commands are an ordered list and, if
         # anything has changed, we need to destroy the old one and
         # create the new one from scratch
         l = self.enter(*c, new)
@@ -335,78 +338,79 @@
             for old_nexthop in self.get_ext(old):
                 l.append(" no " + self._cmd(old_nexthop))
         for new_nexthop in self.get_ext(new):
             l.append(" " + self._cmd(new_nexthop))
         return l
 
 
-class Cvt_RtMap_SetIPNxtHopVrfy(DiffConvert_RtMap_Entry):
+class Cvt_RtMap_SetIPNxtHopVrfy(Context_RtMap_Entry):
     cmd = tuple()
     ext = "set", "ip-next-hop-verify-availability"
 
     def remove(self, old, c):
         l = self.enter(*c, old)
         l.append(" no set ip next-hop verify-availability")
         return l
 
     def update(self, old, upd, new, c):
         l = self.enter(*c, new)
         l.append(" set ip next-hop verify-availability")
         return l
 
-class Cvt_RtMap_SetIPNxtHopVrfyTrk(DiffConvert_RtMap_Entry):
+
+class _AbsCvt_RtMap_SetIPNxtHopVrfyTrk(Context_RtMap_Entry):
     cmd = tuple()
     ext = "set", "ip-next-hop-verify-availability-track", None
 
     def _cmd(self, seq, nexthop):
         return ("set ip next-hop verify-availability %s %s track %d"
                      % (nexthop["addr"], seq, nexthop["track-obj"]))
 
-class Cvt_RtMap_SetIPNxtHopVrfy_Del(Cvt_RtMap_SetIPNxtHopVrfyTrk):
+class Cvt_RtMap_SetIPNxtHopVrfy_del(_AbsCvt_RtMap_SetIPNxtHopVrfyTrk):
     block = "rtmap-del"
 
     def remove(self, old, c, nexthop_seq):
         return self.enter(*c, old) + [
                    " no "
                        + self._cmd(nexthop_seq,
                                    self.get_ext(old, nexthop_seq))]
 
-class Cvt_RtMap_SetIPNxtHopVrfy_Add(Cvt_RtMap_SetIPNxtHopVrfyTrk):
+class Cvt_RtMap_SetIPNxtHopVrfy_add(_AbsCvt_RtMap_SetIPNxtHopVrfyTrk):
     block = "rtmap-add"
 
     def update(self, old, upd, new, c, nexthop_seq):
         # individual entries (ordered by sequence number) can be replaced but
         # the old entry must be removed first, before the new one added
         l = self.enter(*c, new)
         if old:
             l.append(" no "
                      + self._cmd(nexthop_seq, self.get_ext(old, nexthop_seq)))
         l.append(" " + self._cmd(nexthop_seq, self.get_ext(new, nexthop_seq)))
         return l
 
 
-class Cvt_RtMap_SetIPv6NxtHop(DiffConvert_RtMap_Entry):
+class _AbsCvt_RtMap_SetIPv6NxtHop(Context_RtMap_Entry):
     cmd = tuple()
     ext = "set", "ipv6-next-hop"
 
     def _cmd(self, nexthop):
         addr = nexthop["addr"]
         return "set ipv6 next-hop " + addr
 
-class Cvt_RtMap_SetIPv6NxtHop_Del(Cvt_RtMap_SetIPv6NxtHop):
+class Cvt_RtMap_SetIPv6NxtHop_del(_AbsCvt_RtMap_SetIPv6NxtHop):
     block = "rtmap-del"
 
     def remove(self, old, c):
         # we must remove all the 'set ipv6 next-hop' commands individually
         l = self.enter(*c, old)
         for nexthop in self.get_ext(old):
             l.append(" no " + self._cmd(nexthop))
         return l
 
-class Cvt_RtMap_SetIPv6NxtHop_Add(Cvt_RtMap_SetIPv6NxtHop):
+class Cvt_RtMap_SetIPv6NxtHop_add(_AbsCvt_RtMap_SetIPv6NxtHop):
     block = "rtmap-add"
 
     def update(self, old, upd, new, c):
         # the 'set ip ... next-hop' commands are an ordered list and, if
         # anything has changed, we need to destroy the old one and
         # create the new one from scratch
         l = self.enter(*c, new)
@@ -414,48 +418,48 @@
             for old_nexthop in self.get_ext(old):
                 l.append(" no " + self._cmd(old_nexthop))
         for new_nexthop in self.get_ext(new):
             l.append(" " + self._cmd(new_nexthop))
         return l
 
 
-class Cvt_RtMap_SetLocalPref(DiffConvert_RtMap_Entry):
+class _AbsCvt_RtMap_SetLocalPref(Context_RtMap_Entry):
     cmd = tuple()
     ext = "set", "local-preference"
 
-class Cvt_RtMap_SetLocalPref_Del(Cvt_RtMap_SetLocalPref):
+class Cvt_RtMap_SetLocalPref_del(_AbsCvt_RtMap_SetLocalPref):
     block = "rtmap-del"
 
     def remove(self, old, c):
         return self.enter(*c, old) + [" no set local-preference"]
 
-class Cvt_RtMap_SetLocalPref_Add(Cvt_RtMap_SetLocalPref):
+class Cvt_RtMap_SetLocalPref_add(_AbsCvt_RtMap_SetLocalPref):
     block = "rtmap-add"
 
     def update(self, old, upd, new, c):
         return self.enter(*c, new) + [
                    " set local-preference " + str(self.get_ext(new))]
 
 
-class Cvt_RtMap_SetVRF(DiffConvert_RtMap_Entry):
+class _AbsCvt_RtMap_SetVRF(Context_RtMap_Entry):
     # this handles both 'set global' and 'set vrf ...'
     cmd = tuple()
     ext = "set", "vrf"
 
     def _cmd(self, entry):
         vrf = self.get_ext(entry)
         return "set " + (("vrf " + vrf) if vrf else "global")
 
-class Cvt_RtMap_SetVRF_Del(Cvt_RtMap_SetVRF):
+class Cvt_RtMap_SetVRF_del(_AbsCvt_RtMap_SetVRF):
     block = "rtmap-del"
 
     def remove(self, old, c):
         return self.enter(*c, old) + [" no " + self._cmd(old)]
 
-class Cvt_RtMap_SetVRF_Add(Cvt_RtMap_SetVRF):
+class Cvt_RtMap_SetVRF_add(_AbsCvt_RtMap_SetVRF):
     block = "rtmap-add"
 
     def update(self, old, upd, new, c):
         l = self.enter(*c, new)
 
         # if there's a previous setting, and we're changing from global
         # to a VRF, or vice-versa, we need to clear the old setting
@@ -470,42 +474,42 @@
 
 # =============================================================================
 # router bgp ...
 # =============================================================================
 
 
 
-class Cvt_RtrBGP(DiffConvert):
+class Cvt_RtrBGP(Convert):
     cmd = "router", "bgp", None
 
     def remove(self, old, c, asn):
         return "no router bgp " + asn
 
     def add(self, new, c, asn):
         return "router bgp " + asn
 
 
-class DiffConvert_RtrBGP(DiffConvert):
+class Context_RtrBGP(Convert):
     context = "router", "bgp", None
 
     def enter(self, asn):
         return ["router bgp " + asn]
 
 
-class Cvt_RtrBGP_BGPRtrID(DiffConvert_RtrBGP):
+class Cvt_RtrBGP_BGPRtrID(Context_RtrBGP):
     cmd = "router-id",
 
     def remove(self, old, c):
         return self.enter(*c) + [" no bgp router-id"]
 
     def update(self, old, upd, new, c):
         return self.enter(*c) + [" bgp router-id " + new]
 
 
-class Cvt_RtrBGP_Nbr(DiffConvert_RtrBGP):
+class Cvt_RtrBGP_Nbr(Context_RtrBGP):
     cmd = "neighbor", None
 
     def remove(self, old, c, nbr):
         # when removing a neighbor that is a peer-group, we need to
         # state that
         return self.enter(*c) + [
                    "  no neighbor "
@@ -518,57 +522,57 @@
         # (normally, a neighbor is created implicitly by configuring
         # settings for it, starting by putting it in a peer-group or
         # its remote-as)
         if new.get("type") == "peer-group":
             return self.enter(*c) + ["  neighbor %s peer-group" % nbr]
 
 
-class DiffConvert_RtrBGP_Nbr(DiffConvert_RtrBGP):
-    context = DiffConvert_RtrBGP.context + Cvt_RtrBGP_Nbr.cmd
+class Context_RtrBGP_Nbr(Context_RtrBGP):
+    context = Context_RtrBGP.context + Cvt_RtrBGP_Nbr.cmd
 
     # we're going to use these classes directly under the 'router,bgp,
     # ASN,neighbor,NBR' context and the 'router,bgp,ASN,vrf,VRF,
     # address-family,AF,neighbor,NBR' context but we also need access to
     # the NBR parameter for the commands (since they start 'neighbor
     # NBR ...')
     #
     # setting context_offset to -1 causes the neighbor to be supplied as
     # a local argument to the converter and gives a variable length
     # context, depending on whether the configuration is at the global
     # or address-family level
     context_offset = -1
 
 
-class Cvt_RtrBGP_Nbr_FallOver(DiffConvert_RtrBGP_Nbr):
+class Cvt_RtrBGP_Nbr_FallOver(Context_RtrBGP_Nbr):
     cmd = "fall-over",
 
     def remove(self, old, c, nbr):
         return self.enter(*c) + [" no neighbor %s fall-over" % nbr]
 
     def update(self, old, upd, new, c, nbr):
         return self.enter(*c) + [
                    " neighbor %s fall-over %s"
                        % (nbr,
                           ("bfd " + new["bfd"]) if "bfd" in new
                                else "route-map " + new["route-map"])]
 
 
-class Cvt_RtrBGP_Nbr_Pwd(DiffConvert_RtrBGP_Nbr):
+class Cvt_RtrBGP_Nbr_Pwd(Context_RtrBGP_Nbr):
     cmd = "password",
 
     def remove(self, old, c, nbr):
         return self.enter(*c) + [" no neighbor %s password" % nbr]
 
     def update(self, old, upd, new, c, nbr):
         return self.enter(*c) + [
                    " neighbor %s password %d %s"
                        % (nbr, new["encryption"], new["password"])]
 
 
-class Cvt_RtrBGP_Nbr_PrGrpMbr(DiffConvert_RtrBGP_Nbr):
+class Cvt_RtrBGP_Nbr_PrGrpMbr(Context_RtrBGP_Nbr):
     # this converter is used to add or remove a neighbor to/from a
     # peer-group
     cmd = "peer-group",
     trigger_blocks = { "bgp-nbr-activate" }
 
     def remove(self, old, c, nbr):
         return self.enter(*c) + ["  no neighbor %s peer-group %s" % (nbr, old)]
@@ -578,25 +582,25 @@
 
     def update(self, old, upd, new, c, nbr):
         return self.enter(*c) + [
                    "  no neighbor %s peer-group %s" % (nbr, old),
                    "  neighbor %s peer-group %s" % (nbr, new)]
 
 
-class Cvt_RtrBGP_Nbr_RemAS(DiffConvert_RtrBGP_Nbr):
+class Cvt_RtrBGP_Nbr_RemAS(Context_RtrBGP_Nbr):
     cmd = "remote-as",
 
     # removing a remote AS actually removes the neighbor, so we deal
     # with that in the context, above - we just handle add/update here
 
     def update(self, old, upd, new, c, nbr):
         return self.enter(*c) + [" neighbor %s remote-as %s" % (nbr, new)]
 
 
-class Cvt_RtrBGP_Nbr_UpdSrc(DiffConvert_RtrBGP_Nbr):
+class Cvt_RtrBGP_Nbr_UpdSrc(Context_RtrBGP_Nbr):
     cmd = "update-source",
 
     def remove(self, old, c, nbr):
         return self.enter(*c) + [" no neighbor %s update-source" % nbr]
 
     def update(self, old, upd,new, c, nbr):
         return self.enter(*c) + [" neighbor %s update-source %s" % (nbr, new)]
@@ -604,53 +608,52 @@
 
 # router bgp ... address-family ... [vrf ...]
 
 
 # working out the address-family line is complicated and we do it in
 # several places, so separate it into a function
 
-def _RtrBGP_AF(vrf, af):
+def _RtrBGP_AF_cmd(vrf, af):
     # address families in the global routing table as in a VRF called
     # VRF_GLOBAL as a special case so everything lines up at the same
     # level in the inventory
     return (" address-family "
             + af
             + ((" vrf " + vrf) if vrf != VRF_GLOBAL else ""))
 
 
-class Cvt_RtrBGP_AF(DiffConvert_RtrBGP):
+class Cvt_RtrBGP_AF(Context_RtrBGP):
     cmd = "vrf", None, "address-family", None
 
     def remove(self, old, c, vrf, af):
-        return self.enter(*c) + [" no" + _RtrBGP_AF(vrf, af)]
+        return self.enter(*c) + [" no" + _RtrBGP_AF_cmd(vrf, af)]
 
     def add(self, new, c, vrf, af):
-        return self.enter(*c) + [_RtrBGP_AF(vrf, af)]
+        return self.enter(*c) + [_RtrBGP_AF_cmd(vrf, af)]
 
 
-class DiffConvert_RtrBGP_AF(DiffConvert_RtrBGP):
-    context = DiffConvert_RtrBGP.context + Cvt_RtrBGP_AF.cmd
+class Context_RtrBGP_AF(Context_RtrBGP):
+    context = Context_RtrBGP.context + Cvt_RtrBGP_AF.cmd
 
     def enter(self, *c):
-        c_super = c[:-2]
-        vrf, af = c[-2:]
-        return super().enter(*c_super) + [_RtrBGP_AF(vrf, af)]
+        c_super, (vrf, af) = c[:-2], c[-2:]
+        return super().enter(*c_super) + [_RtrBGP_AF_cmd(vrf, af)]
 
 
-class Cvt_RtrBGP_AF_MaxPaths(DiffConvert_RtrBGP_AF):
+class Cvt_RtrBGP_AF_MaxPaths(Context_RtrBGP_AF):
     cmd = "maximum-paths",
 
     def remove(self, old, c):
         return self.enter(*c) + ["  no maximum-paths %d" % old]
 
     def update(self, old, upd, new, c):
         return self.enter(*c) + ["  maximum-paths %d" % new]
 
 
-class Cvt_RtrBGP_AF_MaxPathsIBGP(DiffConvert_RtrBGP_AF):
+class Cvt_RtrBGP_AF_MaxPathsIBGP(Context_RtrBGP_AF):
     cmd = "maximum-paths-ibgp",
 
     def remove(self, old, c):
         return self.enter(*c) + ["  no maximum-paths ibgp %d" % old]
 
     def update(self, old, upd, new, c):
         return self.enter(*c) + ["  maximum-paths ibgp %d" % new]
@@ -670,25 +673,25 @@
 # 'no redistribute ... route-map/metric' will turn them off, but leave
 # redistribution itself on
 
 
 # classes to cover the redistribution contexts
 
 
-class Cvt_RtrBGP_AF_Redist_Simple(DiffConvert_RtrBGP_AF):
+class Cvt_RtrBGP_AF_Redist_Simple(Context_RtrBGP_AF):
     cmd = "redistribute", { "static", "connected" }
 
     def remove(self, old, c, proto):
         return self.enter(*c) + ["  no redistribute " + proto]
 
     def add(self, new, c, proto):
         return self.enter(*c) + ["  redistribute " + proto]
 
 
-class Cvt_RtrBGP_AF_Redist_OSPF(DiffConvert_RtrBGP_AF):
+class Cvt_RtrBGP_AF_Redist_OSPF(Context_RtrBGP_AF):
     cmd = "redistribute", { "ospf", "ospfv3" }, None
 
     def remove(self, old, c, proto, proc):
         return self.enter(*c) + ["  no redistribute %s %d" % (proto, proc)]
 
     def add(self, new, c, proto, proc):
         return self.enter(*c) + ["  redistribute %s %d" % (proto, proc)]
@@ -697,51 +700,49 @@
 # context versions of above
 #
 # the parameter classes will be subclasses of these and use a variable
 # length context because the 'simple' protocols have no additional
 # arguments but the OSPF one has a process number
 
 
-class DiffConvert_RtrBGP_AF_Redist_Simple(DiffConvert_RtrBGP_AF):
-    context = (
-        DiffConvert_RtrBGP_AF.context + Cvt_RtrBGP_AF_Redist_Simple.cmd)
+class Context_RtrBGP_AF_Redist_Simple(Context_RtrBGP_AF):
+    context = Context_RtrBGP_AF.context + Cvt_RtrBGP_AF_Redist_Simple.cmd
 
     # also get the protocol from the context
     context_offset = -1
 
     def _redist(self, proto):
         return "redistribute " + proto
 
 
-class DiffConvert_RtrBGP_AF_Redist_OSPF(DiffConvert_RtrBGP_AF):
-    context = (
-        DiffConvert_RtrBGP_AF.context + Cvt_RtrBGP_AF_Redist_OSPF.cmd)
+class Context_RtrBGP_AF_Redist_OSPF(Context_RtrBGP_AF):
+    context = Context_RtrBGP_AF.context + Cvt_RtrBGP_AF_Redist_OSPF.cmd
 
     # also get the protocol and process number from the context
     context_offset = -2
 
     def _redist(self, proto, proc):
         return "redistribute %s %d" % (proto, proc)
 
 
 # redistribution parameter classes
 
 
-class Cvt_RtrBGP_AF_Redist_Simple_Metric(DiffConvert_RtrBGP_AF_Redist_Simple):
+class Cvt_RtrBGP_AF_Redist_Simple_Metric(Context_RtrBGP_AF_Redist_Simple):
     cmd = "metric",
 
     def remove(self, old, c, *redist):
         return self.enter(*c) + ["  no %s metric" % self._redist(*redist)]
 
     def update(self, old, upd, new, c, *redist):
         return self.enter(*c) + [
                    "  %s metric %d" % (self._redist(*redist), new)]
 
 
-class Cvt_RtrBGP_AF_Redist_Simple_RtMap(DiffConvert_RtrBGP_AF_Redist_Simple):
+class Cvt_RtrBGP_AF_Redist_Simple_RtMap(Context_RtrBGP_AF_Redist_Simple):
     cmd = "route-map",
 
     def remove(self, old, c, redist):
         return self.enter(*c) + [
                    "  no %s route-map %s" % (self._redist(redist), old)]
 
     def update(self, old, upd, new, c, redist):
@@ -750,46 +751,46 @@
 
 
 # OSPF version of the above parameter classes - these inherit from the
 # OSPF context class, instead of the simple context class
 
 
 class Cvt_RtrBGP_AF_Redist_OSPF_Metric(
-    DiffConvert_RtrBGP_AF_Redist_OSPF, Cvt_RtrBGP_AF_Redist_Simple_Metric):
+    Context_RtrBGP_AF_Redist_OSPF, Cvt_RtrBGP_AF_Redist_Simple_Metric):
 
     pass
 
 
 class Cvt_RtrBGP_AF_Redist_OSPF_RtMap(
-    DiffConvert_RtrBGP_AF_Redist_OSPF, Cvt_RtrBGP_AF_Redist_Simple_RtMap):
+    Context_RtrBGP_AF_Redist_OSPF, Cvt_RtrBGP_AF_Redist_Simple_RtMap):
 
     pass
 
 
 # adding and removing entire neighbors as a context is only done in the
 # non-global VRF (in the global VRF, neighbors are configured at the
 # parent, 'router bgp' level and then only address-family specific
 # parameters at that level; for VRFs, the whole neighbor, including the
 # remote-as, is configured at the address-family level)
 
-class Cvt_RtrBGP_AF_vrf_Nbr(DiffConvert_RtrBGP_AF, Cvt_RtrBGP_Nbr):
+class Cvt_RtrBGP_AF_vrf_Nbr(Context_RtrBGP_AF, Cvt_RtrBGP_Nbr):
     def filter(self, c, *_):
         asn, vrf, af = c
         return vrf != VRF_GLOBAL
 
 
 
 # this abstract class and the two that follow are used to create two
 # versions of each command class below by inheriting from each
 # separately - one for the global VRF and one for a different VRF
 #
 # this class modifies the path during construction in two different
 # ways
 
-class _DiffConvert_RtrBGP_AF_Nbr(DiffConvert_RtrBGP_AF):
+class _AbsCvt_RtrBGP_AF_Nbr(Context_RtrBGP_AF):
     def __init__(self):
         self.add_nbr_path()
         super().__init__()
 
     def add_nbr_path(self):
         pass
 
@@ -798,15 +799,15 @@
 # 'neighbor ...' but still operate in the [global] address-family
 # context - as such, this just appends that to the 'cmd' attribute
 #
 # this is because commands in the global address-family do not add or
 # delete entire neighbors (that's done at the 'router bgp' level), but
 # just configured parameters about them
 
-class DiffConvert_RtrBGP_AF_global_Nbr(_DiffConvert_RtrBGP_AF_Nbr):
+class _AbsCvt_RtrBGP_AF_global_Nbr(_AbsCvt_RtrBGP_AF_Nbr):
     def add_nbr_path(self):
         self.cmd = ("neighbor", None) + self.cmd
 
     def filter(self, c, *_):
         asn, vrf, af = c
         return vrf == VRF_GLOBAL
 
@@ -817,28 +818,28 @@
 # 'neighbor ...' onto it
 #
 # this is because, in a non-global VRF, neighbors are separate from
 # those at the global level and must be created and can also be removed
 # by removing the context, with 'no neighbor ...', rather than the
 # individual parameters
 
-class DiffConvert_RtrBGP_AF_vrf_Nbr(_DiffConvert_RtrBGP_AF_Nbr):
+class _AbsCvt_RtrBGP_AF_vrf_Nbr(_AbsCvt_RtrBGP_AF_Nbr):
     context_offset = -1
 
     def add_nbr_path(self):
         self.context = self.context + ("neighbor", None)
 
     def filter(self, c, *_):
         asn, vrf, af = c
         return vrf != VRF_GLOBAL
 
 
 # this is the global VRF version of 'neighbor ... activate'
 
-class Cvt_RtrBGP_AF_global_Nbr_Act(DiffConvert_RtrBGP_AF_global_Nbr):
+class Cvt_RtrBGP_AF_global_Nbr_Act(_AbsCvt_RtrBGP_AF_global_Nbr):
     cmd = "activate",
     block = "bgp-nbr-activate"
 
     def remove(self, old, c, nbr):
         return self.enter(*c) + ["  no neighbor %s activate" % nbr]
 
     def update(self, old, upd, new, c, nbr):
@@ -847,20 +848,20 @@
 
 # this creates the non-global VRF version of 'neighbor ... activate'
 #
 # this pattern continues for all commands below that exist in both the
 # global or non-global VRF
 
 class Cvt_RtrBGP_AF_vrf_Nbr_Act(
-    DiffConvert_RtrBGP_AF_vrf_Nbr, Cvt_RtrBGP_AF_global_Nbr_Act):
+    _AbsCvt_RtrBGP_AF_vrf_Nbr, Cvt_RtrBGP_AF_global_Nbr_Act):
 
     pass
 
 
-class Cvt_RtrBGP_AF_global_Nbr_AddPath(DiffConvert_RtrBGP_AF_global_Nbr):
+class Cvt_RtrBGP_AF_global_Nbr_AddPath(_AbsCvt_RtrBGP_AF_global_Nbr):
     cmd = "additional-paths",
 
     def _add_paths(self, p):
         return (
             " ".join([a for a in [ "send", "receive", "disable" ] if a in p]))
 
     def remove(self, old, c, nbr):
@@ -874,15 +875,15 @@
 
     def update(self, old, upd, new, c, nbr):
         return self.enter(*c) + [
                    "  neighbor %s additional-paths %s"
                        % (nbr, self._add_paths(new))]
 
 
-class Cvt_RtrBGP_AF_global_Nbr_AdvAddPath(DiffConvert_RtrBGP_AF_global_Nbr):
+class Cvt_RtrBGP_AF_global_Nbr_AdvAddPath(_AbsCvt_RtrBGP_AF_global_Nbr):
     cmd = "advertise-additional-paths", None
 
     def remove(self, old, c, nbr, adv):
         # we can just remove any type and don't need to give the number
         # when removing 'best n'
         return self.enter(*c) + [
                    "  no neighbor %s advertise additional-paths %s"
@@ -894,15 +895,15 @@
                        % (nbr, ("best %d" % new) if adv == "best" else adv)]
 
 
 # Cvt_RtrBGP_AF_vrf _Nbr_AdvAddPath
 # does not exist - there is no non-global VRF version of this
 
 
-class Cvt_RtrBGP_AF_global_Nbr_AlwAS(DiffConvert_RtrBGP_AF_global_Nbr):
+class Cvt_RtrBGP_AF_global_Nbr_AlwAS(_AbsCvt_RtrBGP_AF_global_Nbr):
     cmd = "allowas-in",
 
     def truncate(self, old, rem, new, c, nbr):
         # if we're truncating, we must be removing the 'max'
         return self.enter(*c) + [
                    "  neighbor %s allowas-in" % nbr]
 
@@ -915,49 +916,49 @@
         # either changing the 'max' or adding a plain form
         return self.enter(*c) + [
                    "  neighbor %s allowas-in%s"
                        % (nbr, (" %d" % new["max"]) if "max" in new else "")]
 
 
 class Cvt_RtrBGP_AF_vrf_Nbr_AlwAS(
-    DiffConvert_RtrBGP_AF_vrf_Nbr, Cvt_RtrBGP_AF_global_Nbr_AlwAS):
+    _AbsCvt_RtrBGP_AF_vrf_Nbr, Cvt_RtrBGP_AF_global_Nbr_AlwAS):
 
     pass
 
 
 # Cvt_RtrBGP_AF_global_Nbr_FallOver
 # does not exist - there is no global VRF version of this (done at the
 # 'router bgp' level)
 
 
 class Cvt_RtrBGP_AF_vrf_Nbr_FallOver(
-    DiffConvert_RtrBGP_AF_vrf_Nbr, Cvt_RtrBGP_Nbr_FallOver):
+    _AbsCvt_RtrBGP_AF_vrf_Nbr, Cvt_RtrBGP_Nbr_FallOver):
 
     pass
 
 
-class Cvt_RtrBGP_AF_global_Nbr_FltLst(DiffConvert_RtrBGP_AF_global_Nbr):
+class Cvt_RtrBGP_AF_global_Nbr_FltLst(_AbsCvt_RtrBGP_AF_global_Nbr):
     cmd = "filter-list", None
 
     def remove(self, old, c, nbr, dir_):
         return self.enter(*c) + [
                    "  no neighbor %s filter-list %d %s" % (nbr, old, dir_)]
 
     def update(self, old, upd, new, c, nbr, dir_):
         return self.enter(*c) + [
                    "  neighbor %s filter-list %d %s" % (nbr, new, dir_)]
 
 
 class Cvt_RtrBGP_AF_vrf_Nbr_FltLst(
-    DiffConvert_RtrBGP_AF_vrf_Nbr, Cvt_RtrBGP_AF_global_Nbr_FltLst):
+    _AbsCvt_RtrBGP_AF_vrf_Nbr, Cvt_RtrBGP_AF_global_Nbr_FltLst):
 
     pass
 
 
-class Cvt_RtrBGP_AF_global_Nbr_MaxPfx(DiffConvert_RtrBGP_AF_global_Nbr):
+class Cvt_RtrBGP_AF_global_Nbr_MaxPfx(_AbsCvt_RtrBGP_AF_global_Nbr):
     cmd = "maximum-prefix",
 
     def remove(self, old, c, nbr):
         # oddly, when removing, the old maximum must be spefified but
         # not the threshold
         return self.enter(*c) + [
                    "  no neighbor %s maximum-prefix %d" % (nbr, old["max"])]
@@ -968,20 +969,20 @@
                        % (nbr,
                           new["max"],
                           (" %d" % new["threshold"]) if "threshold" in new
                                else "")]
 
 
 class Cvt_RtrBGP_AF_vrf_Nbr_MaxPfx(
-    DiffConvert_RtrBGP_AF_vrf_Nbr, Cvt_RtrBGP_AF_global_Nbr_MaxPfx):
+    _AbsCvt_RtrBGP_AF_vrf_Nbr, Cvt_RtrBGP_AF_global_Nbr_MaxPfx):
 
     pass
 
 
-class Cvt_RtrBGP_AF_global_Nbr_NHSelf(DiffConvert_RtrBGP_AF_global_Nbr):
+class Cvt_RtrBGP_AF_global_Nbr_NHSelf(_AbsCvt_RtrBGP_AF_global_Nbr):
     cmd = "next-hop-self",
 
     def truncate(self, old, rem, new, c, nbr):
         # if we're truncating, we must be changing to the plain form
         return self.enter(*c) + [
                    "  neighbor %s next-hop-self" % nbr]
 
@@ -994,73 +995,71 @@
         # either updatring to 'all' or adding a plain form
         return self.enter(*c) + [
                    "  neighbor %s next-hop-self%s"
                        % (nbr, " all" if new.get("all") else "")]
 
 
 class Cvt_RtrBGP_AF_vrf_Nbr_NHSelf(
-    DiffConvert_RtrBGP_AF_vrf_Nbr, Cvt_RtrBGP_AF_global_Nbr_NHSelf):
+    _AbsCvt_RtrBGP_AF_vrf_Nbr, Cvt_RtrBGP_AF_global_Nbr_NHSelf):
 
     pass
 
 
 # Cvt_RtrBGP_AF_global_Nbr_Pwd
 # does not exist - there is no global VRF version of this (done at the
 # 'router bgp' level)
 
 
-class Cvt_RtrBGP_AF_vrf_Nbr_Pwd(
-    DiffConvert_RtrBGP_AF_vrf_Nbr, Cvt_RtrBGP_Nbr_Pwd):
-
+class Cvt_RtrBGP_AF_vrf_Nbr_Pwd(_AbsCvt_RtrBGP_AF_vrf_Nbr, Cvt_RtrBGP_Nbr_Pwd):
     pass
 
 
 # Cvt_RtrBGP_AF_global_Nbr_PrGrpMbr
 # does not exist - there is no global VRF version of this (done at the
 # 'router bgp' level)
 
 
 class Cvt_RtrBGP_AF_vrf_Nbr_PrGrpMbr(
-    DiffConvert_RtrBGP_AF_vrf_Nbr, Cvt_RtrBGP_Nbr_PrGrpMbr):
+    _AbsCvt_RtrBGP_AF_vrf_Nbr, Cvt_RtrBGP_Nbr_PrGrpMbr):
 
     pass
 
 
-class Cvt_RtrBGP_AF_global_Nbr_PfxLst(DiffConvert_RtrBGP_AF_global_Nbr):
+class Cvt_RtrBGP_AF_global_Nbr_PfxLst(_AbsCvt_RtrBGP_AF_global_Nbr):
     cmd = "prefix-list", None
 
     def remove(self, old, c, nbr, dir_):
         return self.enter(*c) + [
                    "  no neighbor %s prefix-list %s %s" % (nbr, old, dir_)]
 
     def update(self, old, upd, new, c, nbr, dir_):
         return self.enter(*c) + [
                    "  neighbor %s prefix-list %s %s" % (nbr, new, dir_)]
 
 
 class Cvt_RtrBGP_AF_vrf_Nbr_PfxLst(
-    DiffConvert_RtrBGP_AF_vrf_Nbr, Cvt_RtrBGP_AF_global_Nbr_PfxLst):
+    _AbsCvt_RtrBGP_AF_vrf_Nbr, Cvt_RtrBGP_AF_global_Nbr_PfxLst):
 
     pass
 
 
-class Cvt_RtrBGP_AF_vrf_Nbr_RemAS(DiffConvert_RtrBGP_AF_vrf_Nbr):
+class Cvt_RtrBGP_AF_vrf_Nbr_RemAS(_AbsCvt_RtrBGP_AF_vrf_Nbr):
     cmd = "remote-as",
     sort_key = "0_remote-as",
 
     def remove(self, old, c, nbr):
         return self.enter(*c) + [
                    "  no neighbor %s remote-as" % nbr]
 
     def update(self, old, upd, new, c, nbr):
         return self.enter(*c) + [
                    "  neighbor %s remote-as %s" % (nbr, new)]
 
 
-class Cvt_RtrBGP_AF_global_Nbr_RemPrivAS(DiffConvert_RtrBGP_AF_global_Nbr):
+class Cvt_RtrBGP_AF_global_Nbr_RemPrivAS(_AbsCvt_RtrBGP_AF_global_Nbr):
     cmd = "remove-private-as",
 
     def truncate(self, old, rem, new, c, nbr):
         # if we're truncating, we must be changing to the plain form
         return self.enter(*c) + [
                    "  neighbor %s remove-private-as" % nbr]
 
@@ -1075,38 +1074,38 @@
         # either updatring to 'all' or adding a plain form
         return self.enter(*c) + [
                    "  neighbor %s remove-private-as%s"
                        % (nbr, " all" if new.get("all") else "")]
 
 
 class Cvt_RtrBGP_AF_vrf_Nbr_RemPrivAS(
-    DiffConvert_RtrBGP_AF_vrf_Nbr, Cvt_RtrBGP_AF_global_Nbr_RemPrivAS):
+    _AbsCvt_RtrBGP_AF_vrf_Nbr, Cvt_RtrBGP_AF_global_Nbr_RemPrivAS):
 
     pass
 
 
-class Cvt_RtrBGP_AF_global_Nbr_RtMap(DiffConvert_RtrBGP_AF_global_Nbr):
+class Cvt_RtrBGP_AF_global_Nbr_RtMap(_AbsCvt_RtrBGP_AF_global_Nbr):
     cmd = "route-map", None
 
     def remove(self, old, c, nbr, dir_):
         return self.enter(*c) + [
                    "  no neighbor %s route-map %s %s" % (nbr, old, dir_)]
 
     def update(self, old, upd, new, c, nbr, dir_):
         return self.enter(*c) + [
                    "  neighbor %s route-map %s %s" % (nbr, new, dir_)]
 
 
 class Cvt_RtrBGP_AF_vrf_Nbr_RtMap(
-    DiffConvert_RtrBGP_AF_vrf_Nbr, Cvt_RtrBGP_AF_global_Nbr_RtMap):
+    _AbsCvt_RtrBGP_AF_vrf_Nbr, Cvt_RtrBGP_AF_global_Nbr_RtMap):
 
     pass
 
 
-class Cvt_RtrBGP_AF_global_Nbr_SndCmty(DiffConvert_RtrBGP_AF_global_Nbr):
+class Cvt_RtrBGP_AF_global_Nbr_SndCmty(_AbsCvt_RtrBGP_AF_global_Nbr):
     cmd = "send-community", None
 
     # the 'neighbor ... send-community' command is odd in that the
     # 'standard', 'extended' and 'both' options don't replace the
     # current setting but add or remove those communities to it
     #
     # the configuration is expressed as a set containing none, one or
@@ -1118,72 +1117,72 @@
 
     def update(self, old, upd, new, c, nbr, cmty):
         return self.enter(*c) + [
                    "  neighbor %s send-community %s" % (nbr, cmty)]
 
 
 class Cvt_RtrBGP_AF_vrf_Nbr_SndCmty(
-    DiffConvert_RtrBGP_AF_vrf_Nbr, Cvt_RtrBGP_AF_global_Nbr_SndCmty):
+    _AbsCvt_RtrBGP_AF_vrf_Nbr, Cvt_RtrBGP_AF_global_Nbr_SndCmty):
 
     pass
 
 
-class Cvt_RtrBGP_AF_global_Nbr_SoftRecfg(DiffConvert_RtrBGP_AF_global_Nbr):
+class Cvt_RtrBGP_AF_global_Nbr_SoftRecfg(_AbsCvt_RtrBGP_AF_global_Nbr):
     cmd = "soft-reconfiguration",
 
     def remove(self, old, c, nbr):
         return self.enter(*c) + [
                    "  no neighbor %s soft-reconfiguration %s" % (nbr, old)]
 
     def update(self, old, upd, new, c, nbr):
         return self.enter(*c) + [
                    "  neighbor %s soft-reconfiguration %s" % (nbr, new)]
 
 
 class Cvt_RtrBGP_AF_vrf_Nbr_SoftRecfg(
-    DiffConvert_RtrBGP_AF_vrf_Nbr, Cvt_RtrBGP_AF_global_Nbr_SoftRecfg):
+    _AbsCvt_RtrBGP_AF_vrf_Nbr, Cvt_RtrBGP_AF_global_Nbr_SoftRecfg):
 
     pass
 
 
 
 # =============================================================================
 # router ospf ...
 # =============================================================================
 
 
 
-class Cvt_RtrOSPF(DiffConvert):
+class Cvt_RtrOSPF(Convert):
     cmd = "router", "ospf", None
 
     def remove(self, old, proc):
         return "no router ospf " + str(proc)
 
     def add(self, new, proc):
         return "router ospf " + str(proc)
 
 
-class DiffConvert_RtrOSPF(DiffConvert):
-    context = "router", "ospf", None
+class Context_RtrOSPF(Convert):
+    context = Cvt_RtrOSPF.cmd
 
     def enter(self, proc):
         return ["router ospf " + str(proc)]
 
 
-class Cvt_RtrOSPF_Id(DiffConvert_RtrOSPF):
+class Cvt_RtrOSPF_Id(Context_RtrOSPF):
     cmd = "id",
 
     def remove(self, old, c):
         return self.enter(*c) + [" no router-id"]
 
     def update(self, old, upd, new, c):
         return self.enter(*c) + [" router-id " + new]
 
 
-class Cvt_RtrOSPF_AreaNSSA(DiffConvert_RtrOSPF):
+class Cvt_RtrOSPF_AreaNSSA(Context_RtrOSPF):
     cmd = "area", None, "nssa"
 
     def remove(self, old, c, area):
         return self.enter(*c) + [" no area %s nssa" % area]
 
     def truncate(self, old, upd, new, c, area):
         # if we're truncating, we're removing options and we do that by
@@ -1198,43 +1197,43 @@
 
 
 # passive-interface configuration is slightly odd as the default mode is
 # stored (assuming it's not the default) and then a list of exceptions
 # is maintained and it can go either way
 
 
-class Cvt_RtrOSPF_PasvInt_Dflt(DiffConvert_RtrOSPF):
+class Cvt_RtrOSPF_PasvInt_Dflt(Context_RtrOSPF):
     cmd = "passive-interface", "default"
 
     def remove(self, old, c):
         return self.enter(*c) + [" no passive-interface default"]
 
     def update(self, old, upd, new, c):
         return self.enter(*c) + [" passive-interface default"]
 
 
 # ... the exception interface lists must execute after changing the
 # default mode, which they will do as 'default' comes before 'interface'
 # and 'no-interface'
 
-class Cvt_RtrOSPF_PasvInt_Int(DiffConvert_RtrOSPF):
+class Cvt_RtrOSPF_PasvInt_Int(Context_RtrOSPF):
     cmd = "passive-interface",
     ext = "interface", None
 
     def delete(self, old, rem, new, c, int_name):
         # if we're changing the default mode, the old list of exceptions
         # will be removed by that, so we don't need to do it
         if (old or {}).get("default") == (new or {}).get("default"):
             return self.enter(*c) + [" no passive-interface " + int_name]
 
     def update(self, old, upd, new, c, int_name):
         return self.enter(*c) + [" passive-interface " + int_name]
 
 
-class Cvt_RtrOSPF_PasvInt_NoInt(DiffConvert_RtrOSPF):
+class Cvt_RtrOSPF_PasvInt_NoInt(Context_RtrOSPF):
     cmd = "passive-interface",
     ext = "no-interface", None
 
     def delete(self, old, rem, new, c, int_name):
         # if we're changing the default mode, the old list of exceptions
         # will be removed by that, so we don't need to do it
         if (old or {}).get("default") == (new or {}).get("default"):
@@ -1247,42 +1246,42 @@
 
 # =============================================================================
 # router ospfv3 ...
 # =============================================================================
 
 
 
-class Cvt_RtrOSPFv3(DiffConvert):
+class Cvt_RtrOSPFv3(Convert):
     cmd = "router", "ospfv3", None
 
     def remove(self, old, c, proc):
         return "no router ospfv3 " + str(proc)
 
     def add(self, new, c, proc):
         return "router ospfv3 " + str(proc)
 
 
-class DiffConvert_RtrOSPFv3(DiffConvert):
-    context = "router", "ospfv3", None
+class Context_RtrOSPFv3(Convert):
+    context = Cvt_RtrOSPFv3.cmd
 
     def enter(self, proc):
         return ["router ospfv3 " + str(proc)]
 
 
-class Cvt_RtrOSPFv3_Id(DiffConvert_RtrOSPFv3):
+class Cvt_RtrOSPFv3_Id(Context_RtrOSPFv3):
     cmd = "id",
 
     def remove(self, old, c):
         return self.enter(*c) + [" no router-id"]
 
     def update(self, old, upd, new, c):
         return self.enter(*c) + [" router-id " + new]
 
 
-class Cvt_RtrOSPFv3_AreaNSSA(DiffConvert_RtrOSPFv3):
+class Cvt_RtrOSPFv3_AreaNSSA(Context_RtrOSPFv3):
     cmd = "area", None, "nssa"
 
     def remove(self, old, c, area):
         return self.enter(*c) + [" no area %s nssa" % area]
 
     def truncate(self, old, upd, new, c, area):
         # if we're truncating, we're removing options and we do that by
@@ -1292,58 +1291,59 @@
     def update(self, old, upd, new, c, area):
         s = ""
         if "no-redistribution" in new: s += " no-redistribution"
         if "no-summary" in new: s += " no-summary"
         return self.enter(*c) + [" area %s nssa%s" % (area, s)]
 
 
-class Cvt_RtrOSPFv3_AF(DiffConvert_RtrOSPFv3):
+class Cvt_RtrOSPFv3_AF(Context_RtrOSPFv3):
     cmd = "address-family", None
 
     def remove(self, old, c, af):
         return self.enter(*c) + [" no address-family " + af]
 
     def add(self, new, c, af):
         return self.enter(*c) + [" address-family " + af]
 
 
-class DiffConvert_RtrOSPFv3_AF(DiffConvert_RtrOSPFv3):
-    context = DiffConvert_RtrOSPFv3.context + Cvt_RtrOSPFv3_AF.cmd
+class Context_RtrOSPFv3_AF(Context_RtrOSPFv3):
+    context = Context_RtrOSPFv3.context + Cvt_RtrOSPFv3_AF.cmd
 
-    def enter(self, proc, af):
-        return super().enter(proc) + [" address-family " + af]
+    def enter(self, *c):
+        c_super, (af, ) = c[:-1], c[-1:]
+        return super().enter(*c_super) + [" address-family " + af]
 
 
 # see the Cvt_RtrOSPF_... versions above for the explanation of how
 # these converters work
 
 
-class Cvt_RtrOSPFv3_AF_PasvInt_Dflt(DiffConvert_RtrOSPFv3_AF):
+class Cvt_RtrOSPFv3_AF_PasvInt_Dflt(Context_RtrOSPFv3_AF):
     cmd = "passive-interface", "default"
 
     def remove(self, old, c):
         return self.enter(*c) + [" no passive-interface default"]
 
     def update(self, old, upd, new, c):
         return self.enter(*c) + [" passive-interface default"]
 
 
-class Cvt_RtrOSPFv3_AF_PasvInt_Int(DiffConvert_RtrOSPFv3_AF):
+class Cvt_RtrOSPFv3_AF_PasvInt_Int(Context_RtrOSPFv3_AF):
     cmd = "passive-interface",
     ext = "interface", None
 
     def delete(self, old, rem, new, c, int_name):
         if (old or {}).get("default") == (new or {}).get("default"):
             return self.enter(*c) + [" no passive-interface " + int_name]
 
     def update(self, old, upd, new, c, int_name):
         return self.enter(*c) + [" passive-interface " + int_name]
 
 
-class Cvt_RtrOSPFv3_AF_PasvInt_NoInt(DiffConvert_RtrOSPFv3_AF):
+class Cvt_RtrOSPFv3_AF_PasvInt_NoInt(Context_RtrOSPFv3_AF):
     cmd = "passive-interface",
     ext = "no-interface", None
 
     def delete(self, old, rem, new, c, int_name):
         if (old or {}).get("default") == (new or {}).get("default"):
             return self.enter(*c) + [" passive-interface " + int_name]
```

### Comparing `asimtote-0.16.5/asimtote/ios/diff.py` & `asimtote-0.16.6/asimtote/ios/diff.py`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.5/asimtote/ios/utils.py` & `asimtote-0.16.6/asimtote/ios/utils.py`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.5/asimtote/misc.py` & `asimtote-0.16.6/asimtote/misc.py`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.5/asimtote.egg-info/PKG-INFO` & `asimtote-0.16.6/asimtote.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asimtote
-Version: 0.16.5
+Version: 0.16.6
 Summary: Compare network device configuration files using contextual structures
 Home-page: https://gitlab.developers.cam.ac.uk/uis/netsys/udn/asimtote
 Author: Robert Franklin
 Author-email: rcf34@cam.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `asimtote-0.16.5/asimtote.egg-info/SOURCES.txt` & `asimtote-0.16.6/asimtote.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.5/setup.py` & `asimtote-0.16.6/setup.py`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.5/test_asimtote/ios/config/interface.py` & `asimtote-0.16.6/test_asimtote/ios/config/interface.py`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.5/test_asimtote/ios/config/lists.py` & `asimtote-0.16.6/test_asimtote/ios/config/lists.py`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.5/test_asimtote/ios/config/other.py` & `asimtote-0.16.6/test_asimtote/ios/config/other.py`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.5/test_asimtote/ios/config/router.py` & `asimtote-0.16.6/test_asimtote/ios/config/router.py`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.5/test_asimtote/ios/converters/cvtunittest.py` & `asimtote-0.16.6/test_asimtote/ios/converters/cvtunittest.py`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.5/test_asimtote/ios/converters/interface.py` & `asimtote-0.16.6/test_asimtote/ios/converters/interface.py`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.5/test_asimtote/ios/converters/lists.py` & `asimtote-0.16.6/test_asimtote/ios/converters/lists.py`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.5/test_asimtote/ios/converters/other.py` & `asimtote-0.16.6/test_asimtote/ios/converters/other.py`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.5/test_asimtote/ios/converters/router.py` & `asimtote-0.16.6/test_asimtote/ios/converters/router.py`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.5/test_asimtote/ios/utils.py` & `asimtote-0.16.6/test_asimtote/ios/utils.py`

 * *Files identical despite different names*

