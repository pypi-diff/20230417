# Comparing `tmp/remin-0.0.1.tar.gz` & `tmp/remin-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remin-0.0.1.tar", last modified: Fri Apr 14 23:02:23 2023, max compression
+gzip compressed data, was "remin-0.0.2.tar", last modified: Mon Apr 17 01:48:48 2023, max compression
```

## Comparing `remin-0.0.1.tar` & `remin-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-04-14 23:02:23.942868 remin-0.0.1/
--rw-rw-r--   0 salih     (1000) salih     (1000)     1799 2023-04-14 21:12:20.000000 remin-0.0.1/.gitignore
--rw-rw-r--   0 salih     (1000) salih     (1000)     1072 2023-04-14 21:12:20.000000 remin-0.0.1/LICENSE
--rw-rw-r--   0 salih     (1000) salih     (1000)      205 2023-04-14 22:52:11.000000 remin-0.0.1/Makefile
--rw-rw-r--   0 salih     (1000) salih     (1000)      581 2023-04-14 23:02:23.942868 remin-0.0.1/PKG-INFO
--rw-rw-r--   0 salih     (1000) salih     (1000)       43 2023-04-14 21:12:20.000000 remin-0.0.1/README.md
--rw-rw-r--   0 salih     (1000) salih     (1000)     1242 2023-04-14 22:44:59.000000 remin-0.0.1/pyproject.toml
--rw-rw-r--   0 salih     (1000) salih     (1000)       28 2023-04-14 23:01:53.000000 remin-0.0.1/requirements.txt
--rw-rw-r--   0 salih     (1000) salih     (1000)       38 2023-04-14 23:02:23.942868 remin-0.0.1/setup.cfg
-drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-04-14 23:02:23.942868 remin-0.0.1/src/
-drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-04-14 23:02:23.942868 remin-0.0.1/src/remin/
--rw-rw-r--   0 salih     (1000) salih     (1000)       28 2023-04-14 22:17:25.000000 remin-0.0.1/src/remin/__init__.py
--rw-rw-r--   0 salih     (1000) salih     (1000)       29 2023-04-14 22:18:57.000000 remin-0.0.1/src/remin/domain.py
--rw-rw-r--   0 salih     (1000) salih     (1000)       29 2023-04-14 22:18:13.000000 remin-0.0.1/src/remin/solver.py
-drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-04-14 23:02:23.942868 remin-0.0.1/src/remin.egg-info/
--rw-rw-r--   0 salih     (1000) salih     (1000)      581 2023-04-14 23:02:23.000000 remin-0.0.1/src/remin.egg-info/PKG-INFO
--rw-rw-r--   0 salih     (1000) salih     (1000)      295 2023-04-14 23:02:23.000000 remin-0.0.1/src/remin.egg-info/SOURCES.txt
--rw-rw-r--   0 salih     (1000) salih     (1000)        1 2023-04-14 23:02:23.000000 remin-0.0.1/src/remin.egg-info/dependency_links.txt
--rw-rw-r--   0 salih     (1000) salih     (1000)       74 2023-04-14 23:02:23.000000 remin-0.0.1/src/remin.egg-info/requires.txt
--rw-rw-r--   0 salih     (1000) salih     (1000)        6 2023-04-14 23:02:23.000000 remin-0.0.1/src/remin.egg-info/top_level.txt
+drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-04-17 01:48:48.423377 remin-0.0.2/
+-rw-rw-r--   0 salih     (1000) salih     (1000)     1828 2023-04-15 00:41:42.000000 remin-0.0.2/.gitignore
+-rw-rw-r--   0 salih     (1000) salih     (1000)     1072 2023-04-14 21:12:20.000000 remin-0.0.2/LICENSE
+-rw-rw-r--   0 salih     (1000) salih     (1000)      311 2023-04-17 01:44:50.000000 remin-0.0.2/Makefile
+-rw-rw-r--   0 salih     (1000) salih     (1000)     3164 2023-04-17 01:48:48.423377 remin-0.0.2/PKG-INFO
+-rw-rw-r--   0 salih     (1000) salih     (1000)     2625 2023-04-17 01:40:58.000000 remin-0.0.2/README.md
+-rw-rw-r--   0 salih     (1000) salih     (1000)     1255 2023-04-17 01:41:56.000000 remin-0.0.2/pyproject.toml
+-rw-rw-r--   0 salih     (1000) salih     (1000)       28 2023-04-14 23:01:53.000000 remin-0.0.2/requirements.txt
+-rw-rw-r--   0 salih     (1000) salih     (1000)       38 2023-04-17 01:48:48.423377 remin-0.0.2/setup.cfg
+drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-04-17 01:48:48.419377 remin-0.0.2/src/
+drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-04-17 01:48:48.423377 remin-0.0.2/src/remin/
+-rw-rw-r--   0 salih     (1000) salih     (1000)      120 2023-04-17 01:36:46.000000 remin-0.0.2/src/remin/__init__.py
+-rw-rw-r--   0 salih     (1000) salih     (1000)       29 2023-04-14 23:42:16.000000 remin-0.0.2/src/remin/domain.py
+-rw-rw-r--   0 salih     (1000) salih     (1000)      809 2023-04-17 01:46:30.000000 remin-0.0.2/src/remin/func.py
+-rw-rw-r--   0 salih     (1000) salih     (1000)      488 2023-04-17 01:44:59.000000 remin-0.0.2/src/remin/residual.py
+-rw-rw-r--   0 salih     (1000) salih     (1000)     1720 2023-04-17 01:44:59.000000 remin-0.0.2/src/remin/solver.py
+drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-04-17 01:48:48.423377 remin-0.0.2/src/remin.egg-info/
+-rw-rw-r--   0 salih     (1000) salih     (1000)     3164 2023-04-17 01:48:48.000000 remin-0.0.2/src/remin.egg-info/PKG-INFO
+-rw-rw-r--   0 salih     (1000) salih     (1000)      335 2023-04-17 01:48:48.000000 remin-0.0.2/src/remin.egg-info/SOURCES.txt
+-rw-rw-r--   0 salih     (1000) salih     (1000)        1 2023-04-17 01:48:48.000000 remin-0.0.2/src/remin.egg-info/dependency_links.txt
+-rw-rw-r--   0 salih     (1000) salih     (1000)       80 2023-04-17 01:48:48.000000 remin-0.0.2/src/remin.egg-info/requires.txt
+-rw-rw-r--   0 salih     (1000) salih     (1000)        6 2023-04-17 01:48:48.000000 remin-0.0.2/src/remin.egg-info/top_level.txt
```

### Comparing `remin-0.0.1/.gitignore` & `remin-0.0.2/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
 *.so
 
+# development/test
+devtest/
+
 # Distribution / packaging
 .Python
 build/
 develop-eggs/
 dist/
 downloads/
 eggs/
```

### Comparing `remin-0.0.1/LICENSE` & `remin-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `remin-0.0.1/pyproject.toml` & `remin-0.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -3,29 +3,30 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [project]
 name = "remin"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     { name="Salih Taşdelen", email="salih.tasdelen@hotmail.com"},
 ]
 description = "PINN solver implemented in Pytorch"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "torch >= 2.0.0",
     "pyDOE >= 0.3.8",
+    "numpy",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/SalihTasdelen/remin"
 "Bug Tracker" = "https://github.com/SalihTasdelen/remin/issues"
 
 [project.optional-dependencies]
```

