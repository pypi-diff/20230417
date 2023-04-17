# Comparing `tmp/japyconjugator-1.0.0.tar.gz` & `tmp/japyconjugator-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "japyconjugator-1.0.0.tar", last modified: Mon Apr 17 12:18:33 2023, max compression
+gzip compressed data, was "japyconjugator-1.0.2.tar", last modified: Mon Apr 17 13:16:48 2023, max compression
```

## Comparing `japyconjugator-1.0.0.tar` & `japyconjugator-1.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 12:18:33.762912 japyconjugator-1.0.0/
--rw-rw-rw-   0        0        0     1090 2023-04-15 11:42:39.000000 japyconjugator-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     1166 2023-04-17 12:18:33.762912 japyconjugator-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      607 2023-04-17 12:10:42.000000 japyconjugator-1.0.0/README.md
--rw-rw-rw-   0        0        0      547 2023-04-16 20:17:45.000000 japyconjugator-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-17 12:18:33.762912 japyconjugator-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-17 12:18:33.712910 japyconjugator-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-17 12:18:33.722911 japyconjugator-1.0.0/src/japyconjugator/
--rw-rw-rw-   0        0        0        0 2023-04-16 20:34:22.000000 japyconjugator-1.0.0/src/japyconjugator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 12:18:33.742911 japyconjugator-1.0.0/src/japyconjugator/adjectives/
--rw-rw-rw-   0        0        0       24 2023-04-17 11:21:39.000000 japyconjugator-1.0.0/src/japyconjugator/adjectives/__init__.py
--rw-rw-rw-   0        0        0      625 2023-04-17 12:09:44.000000 japyconjugator-1.0.0/src/japyconjugator/adjectives/conjugate.py
--rw-rw-rw-   0        0        0      911 2023-04-17 11:57:32.000000 japyconjugator-1.0.0/src/japyconjugator/adjectives/conjugation_helpers.py
--rw-rw-rw-   0        0        0     1239 2023-04-17 11:57:25.000000 japyconjugator-1.0.0/src/japyconjugator/adjectives/conjugators.py
--rw-rw-rw-   0        0        0      235 2023-04-17 11:57:47.000000 japyconjugator-1.0.0/src/japyconjugator/adjectives/defs.py
--rw-rw-rw-   0        0        0      103 2023-04-16 20:43:39.000000 japyconjugator-1.0.0/src/japyconjugator/defs.py
-drwxrwxrwx   0        0        0        0 2023-04-17 12:18:33.762912 japyconjugator-1.0.0/src/japyconjugator/verbs/
--rw-rw-rw-   0        0        0       24 2023-04-16 20:34:11.000000 japyconjugator-1.0.0/src/japyconjugator/verbs/__init__.py
--rw-rw-rw-   0        0        0      635 2023-04-17 11:15:36.000000 japyconjugator-1.0.0/src/japyconjugator/verbs/conjugate.py
--rw-rw-rw-   0        0        0     2677 2023-04-15 11:29:51.000000 japyconjugator-1.0.0/src/japyconjugator/verbs/conjugation_helpers.py
--rw-rw-rw-   0        0        0     1607 2023-04-16 21:09:18.000000 japyconjugator-1.0.0/src/japyconjugator/verbs/conjugators.py
--rw-rw-rw-   0        0        0      227 2023-04-16 20:38:14.000000 japyconjugator-1.0.0/src/japyconjugator/verbs/defs.py
-drwxrwxrwx   0        0        0        0 2023-04-17 12:18:33.732914 japyconjugator-1.0.0/src/japyconjugator.egg-info/
--rw-rw-rw-   0        0        0     1166 2023-04-17 12:18:33.000000 japyconjugator-1.0.0/src/japyconjugator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      675 2023-04-17 12:18:33.000000 japyconjugator-1.0.0/src/japyconjugator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 12:18:33.000000 japyconjugator-1.0.0/src/japyconjugator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-17 12:18:33.000000 japyconjugator-1.0.0/src/japyconjugator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:48.853253 japyconjugator-1.0.2/
+-rw-rw-rw-   0        0        0     1090 2023-04-17 13:14:24.000000 japyconjugator-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1166 2023-04-17 13:16:48.853253 japyconjugator-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      607 2023-04-17 13:14:24.000000 japyconjugator-1.0.2/README.md
+-rw-rw-rw-   0        0        0      547 2023-04-17 13:16:33.000000 japyconjugator-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-17 13:16:48.853253 japyconjugator-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:48.822004 japyconjugator-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:48.837629 japyconjugator-1.0.2/src/japyconjugator/
+-rw-rw-rw-   0        0        0        0 2023-04-17 13:14:24.000000 japyconjugator-1.0.2/src/japyconjugator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:48.837629 japyconjugator-1.0.2/src/japyconjugator/adjectives/
+-rw-rw-rw-   0        0        0       24 2023-04-17 13:14:24.000000 japyconjugator-1.0.2/src/japyconjugator/adjectives/__init__.py
+-rw-rw-rw-   0        0        0      625 2023-04-17 13:14:24.000000 japyconjugator-1.0.2/src/japyconjugator/adjectives/conjugate.py
+-rw-rw-rw-   0        0        0      911 2023-04-17 13:14:24.000000 japyconjugator-1.0.2/src/japyconjugator/adjectives/conjugation_helpers.py
+-rw-rw-rw-   0        0        0     1239 2023-04-17 13:14:24.000000 japyconjugator-1.0.2/src/japyconjugator/adjectives/conjugators.py
+-rw-rw-rw-   0        0        0      241 2023-04-17 13:14:24.000000 japyconjugator-1.0.2/src/japyconjugator/adjectives/defs.py
+-rw-rw-rw-   0        0        0      103 2023-04-17 13:14:24.000000 japyconjugator-1.0.2/src/japyconjugator/defs.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:48.853253 japyconjugator-1.0.2/src/japyconjugator/verbs/
+-rw-rw-rw-   0        0        0       24 2023-04-17 13:14:24.000000 japyconjugator-1.0.2/src/japyconjugator/verbs/__init__.py
+-rw-rw-rw-   0        0        0      635 2023-04-17 13:14:24.000000 japyconjugator-1.0.2/src/japyconjugator/verbs/conjugate.py
+-rw-rw-rw-   0        0        0     2677 2023-04-17 13:14:24.000000 japyconjugator-1.0.2/src/japyconjugator/verbs/conjugation_helpers.py
+-rw-rw-rw-   0        0        0     1607 2023-04-17 13:14:24.000000 japyconjugator-1.0.2/src/japyconjugator/verbs/conjugators.py
+-rw-rw-rw-   0        0        0      233 2023-04-17 13:14:24.000000 japyconjugator-1.0.2/src/japyconjugator/verbs/defs.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:48.837629 japyconjugator-1.0.2/src/japyconjugator.egg-info/
+-rw-rw-rw-   0        0        0     1166 2023-04-17 13:16:48.000000 japyconjugator-1.0.2/src/japyconjugator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      675 2023-04-17 13:16:48.000000 japyconjugator-1.0.2/src/japyconjugator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 13:16:48.000000 japyconjugator-1.0.2/src/japyconjugator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-17 13:16:48.000000 japyconjugator-1.0.2/src/japyconjugator.egg-info/top_level.txt
```

### Comparing `japyconjugator-1.0.0/LICENSE` & `japyconjugator-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `japyconjugator-1.0.0/PKG-INFO` & `japyconjugator-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: japyconjugator
-Version: 1.0.0
+Version: 1.0.2
 Summary: A python package for conjugating verbs in the Japanese language.
 Author: Simone Bondi
 Project-URL: Repository, https://github.com/Shibodd/japyconjugator
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `japyconjugator-1.0.0/README.md` & `japyconjugator-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `japyconjugator-1.0.0/pyproject.toml` & `japyconjugator-1.0.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "japyconjugator"
-version = "1.0.0"
+version = "1.0.2"
 authors = [
     { name = "Simone Bondi" },
 ]
 description = "A python package for conjugating verbs in the Japanese language."
 readme = "README.md"
 requires-python = ">=3"
 classifiers = [
```

### Comparing `japyconjugator-1.0.0/src/japyconjugator/adjectives/conjugate.py` & `japyconjugator-1.0.2/src/japyconjugator/adjectives/conjugate.py`

 * *Files identical despite different names*

### Comparing `japyconjugator-1.0.0/src/japyconjugator/adjectives/conjugation_helpers.py` & `japyconjugator-1.0.2/src/japyconjugator/adjectives/conjugation_helpers.py`

 * *Files identical despite different names*

### Comparing `japyconjugator-1.0.0/src/japyconjugator/adjectives/conjugators.py` & `japyconjugator-1.0.2/src/japyconjugator/adjectives/conjugators.py`

 * *Files identical despite different names*

### Comparing `japyconjugator-1.0.0/src/japyconjugator/verbs/conjugate.py` & `japyconjugator-1.0.2/src/japyconjugator/verbs/conjugate.py`

 * *Files identical despite different names*

### Comparing `japyconjugator-1.0.0/src/japyconjugator/verbs/conjugation_helpers.py` & `japyconjugator-1.0.2/src/japyconjugator/verbs/conjugation_helpers.py`

 * *Files identical despite different names*

### Comparing `japyconjugator-1.0.0/src/japyconjugator/verbs/conjugators.py` & `japyconjugator-1.0.2/src/japyconjugator/verbs/conjugators.py`

 * *Files identical despite different names*

### Comparing `japyconjugator-1.0.0/src/japyconjugator.egg-info/PKG-INFO` & `japyconjugator-1.0.2/src/japyconjugator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: japyconjugator
-Version: 1.0.0
+Version: 1.0.2
 Summary: A python package for conjugating verbs in the Japanese language.
 Author: Simone Bondi
 Project-URL: Repository, https://github.com/Shibodd/japyconjugator
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `japyconjugator-1.0.0/src/japyconjugator.egg-info/SOURCES.txt` & `japyconjugator-1.0.2/src/japyconjugator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

