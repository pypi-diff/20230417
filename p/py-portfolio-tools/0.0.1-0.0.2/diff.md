# Comparing `tmp/py-portfolio-tools-0.0.1.tar.gz` & `tmp/py-portfolio-tools-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-portfolio-tools-0.0.1.tar", last modified: Mon Apr 17 12:35:20 2023, max compression
+gzip compressed data, was "py-portfolio-tools-0.0.2.tar", last modified: Mon Apr 17 12:41:52 2023, max compression
```

## Comparing `py-portfolio-tools-0.0.1.tar` & `py-portfolio-tools-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 12:35:20.337882 py-portfolio-tools-0.0.1/
--rw-rw-rw-   0        0        0     1075 2023-04-17 11:45:54.000000 py-portfolio-tools-0.0.1/LICENSE.md
--rw-rw-rw-   0        0        0     1229 2023-04-17 12:35:20.336908 py-portfolio-tools-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       44 2023-04-17 11:54:14.000000 py-portfolio-tools-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 12:35:20.323886 py-portfolio-tools-0.0.1/py-portfolio-tools/
--rw-rw-rw-   0        0        0        0 2023-04-17 11:57:01.000000 py-portfolio-tools-0.0.1/py-portfolio-tools/__init__.py
--rw-rw-rw-   0        0        0       84 2023-04-17 12:05:05.000000 py-portfolio-tools-0.0.1/py-portfolio-tools/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 12:35:20.336908 py-portfolio-tools-0.0.1/py_portfolio_tools.egg-info/
--rw-rw-rw-   0        0        0     1229 2023-04-17 12:35:20.000000 py-portfolio-tools-0.0.1/py_portfolio_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      300 2023-04-17 12:35:20.000000 py-portfolio-tools-0.0.1/py_portfolio_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 12:35:20.000000 py-portfolio-tools-0.0.1/py_portfolio_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-04-17 12:35:20.000000 py-portfolio-tools-0.0.1/py_portfolio_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-17 12:35:20.000000 py-portfolio-tools-0.0.1/py_portfolio_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 12:35:20.337882 py-portfolio-tools-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1657 2023-04-17 12:34:57.000000 py-portfolio-tools-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 12:41:52.187679 py-portfolio-tools-0.0.2/
+-rw-rw-rw-   0        0        0     1075 2023-04-17 11:45:54.000000 py-portfolio-tools-0.0.2/LICENSE.md
+-rw-rw-rw-   0        0        0     1198 2023-04-17 12:41:52.187679 py-portfolio-tools-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       44 2023-04-17 11:54:14.000000 py-portfolio-tools-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 12:41:52.170352 py-portfolio-tools-0.0.2/py-portfolio-tools/
+-rw-rw-rw-   0        0        0        0 2023-04-17 11:57:01.000000 py-portfolio-tools-0.0.2/py-portfolio-tools/__init__.py
+-rw-rw-rw-   0        0        0       84 2023-04-17 12:05:05.000000 py-portfolio-tools-0.0.2/py-portfolio-tools/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 12:41:52.186676 py-portfolio-tools-0.0.2/py_portfolio_tools.egg-info/
+-rw-rw-rw-   0        0        0     1198 2023-04-17 12:41:52.000000 py-portfolio-tools-0.0.2/py_portfolio_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      300 2023-04-17 12:41:52.000000 py-portfolio-tools-0.0.2/py_portfolio_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 12:41:52.000000 py-portfolio-tools-0.0.2/py_portfolio_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-04-17 12:41:52.000000 py-portfolio-tools-0.0.2/py_portfolio_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-17 12:41:52.000000 py-portfolio-tools-0.0.2/py_portfolio_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 12:41:52.187679 py-portfolio-tools-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1576 2023-04-17 12:40:58.000000 py-portfolio-tools-0.0.2/setup.py
```

### Comparing `py-portfolio-tools-0.0.1/LICENSE.md` & `py-portfolio-tools-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `py-portfolio-tools-0.0.1/PKG-INFO` & `py-portfolio-tools-0.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-portfolio-tools
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python Library and set of GUI tools for Portfolio Management
 Home-page: https://gitlab.com/Jaysmito101/py-portfolio-tools
 Author: Jaysmito Mukherjee
 Author-email: jaysmito101@gmail.com
 License: MIT
 Project-URL: Documentation, https://gitlab.com/Jaysmito101/py-portfolio-tools/-/wikis/Home
 Project-URL: Issue tracker, https://gitlab.com/Jaysmito101/py-portfolio-tools/-/issues
@@ -21,10 +21,8 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
-# py-portfolio-tools
-
-README comming soon...
+Coming Soon ...
```

### Comparing `py-portfolio-tools-0.0.1/py_portfolio_tools.egg-info/PKG-INFO` & `py-portfolio-tools-0.0.2/py_portfolio_tools.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-portfolio-tools
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python Library and set of GUI tools for Portfolio Management
 Home-page: https://gitlab.com/Jaysmito101/py-portfolio-tools
 Author: Jaysmito Mukherjee
 Author-email: jaysmito101@gmail.com
 License: MIT
 Project-URL: Documentation, https://gitlab.com/Jaysmito101/py-portfolio-tools/-/wikis/Home
 Project-URL: Issue tracker, https://gitlab.com/Jaysmito101/py-portfolio-tools/-/issues
@@ -21,10 +21,8 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
-# py-portfolio-tools
-
-README comming soon...
+Coming Soon ...
```

### Comparing `py-portfolio-tools-0.0.1/setup.py` & `py-portfolio-tools-0.0.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 from setuptools import setup, find_packages
 import re
 
-requirements = []
-with open('requirements.txt') as f:
-    requirements = f.read().splitlines()
+requirements = ['numpy', 'pandas', 'matplotlib'] 
 
-version = '0.0.1'
+version = '0.0.2'
 
 if not version:
     raise RuntimeError('version is not set')
 
-readme = ''
-with open('README.md') as f:
-    readme = f.read()
+readme = 'Coming Soon ...'
 
 setup(
     name = 'py-portfolio-tools',
     author = 'Jaysmito Mukherjee',
     author_email = 'jaysmito101@gmail.com',
     url = 'https://gitlab.com/Jaysmito101/py-portfolio-tools',
     project_urls = {
```

