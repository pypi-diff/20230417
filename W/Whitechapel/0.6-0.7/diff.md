# Comparing `tmp/whitechapel-0.6.tar.gz` & `tmp/whitechapel-0.7.tar.gz`

## Comparing `whitechapel-0.6.tar` & `whitechapel-0.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 whitechapel-0.6/.gitlab-ci.yml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 whitechapel-0.6/pyproject.tmpl
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 whitechapel-0.6/src/whitechapel/VERSION
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 whitechapel-0.6/src/whitechapel/__init__.py
--rwxr-xr-x   0        0        0     5394 2020-02-02 00:00:00.000000 whitechapel-0.6/src/whitechapel/__main__.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 whitechapel-0.6/.gitignore
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 whitechapel-0.6/README.md
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 whitechapel-0.6/pyproject.toml
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 whitechapel-0.6/PKG-INFO
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 whitechapel-0.7/.gitlab-ci.yml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 whitechapel-0.7/pyproject.tmpl
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 whitechapel-0.7/src/whitechapel/VERSION
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 whitechapel-0.7/src/whitechapel/__init__.py
+-rwxr-xr-x   0        0        0     5394 2020-02-02 00:00:00.000000 whitechapel-0.7/src/whitechapel/__main__.py
+-rw-r--r--   0        0        0     3221 2020-02-02 00:00:00.000000 whitechapel-0.7/.gitignore
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 whitechapel-0.7/README.md
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 whitechapel-0.7/pyproject.toml
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 whitechapel-0.7/PKG-INFO
```

### Comparing `whitechapel-0.6/.gitlab-ci.yml` & `whitechapel-0.7/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `whitechapel-0.6/pyproject.tmpl` & `whitechapel-0.7/pyproject.tmpl`

 * *Files identical despite different names*

### Comparing `whitechapel-0.6/src/whitechapel/__main__.py` & `whitechapel-0.7/src/whitechapel/__main__.py`

 * *Files identical despite different names*

### Comparing `whitechapel-0.6/pyproject.toml` & `whitechapel-0.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "Whitechapel"
-version = "0.6"
+version = "0.7"
 authors = [
   { name="Alexandre Croix", email="a.croix@cylab.be" },
 ]
 description = "MD5 hash cracker"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `whitechapel-0.6/PKG-INFO` & `whitechapel-0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Whitechapel
-Version: 0.6
+Version: 0.7
 Summary: MD5 hash cracker
 Project-URL: Homepage, https://gitlab.cylab.be/cylab/whitechapel
 Project-URL: Bug Tracker, https://gitlab.cylab.be/cylab/whitechapel/-/issues
 Author-email: Alexandre Croix <a.croix@cylab.be>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

