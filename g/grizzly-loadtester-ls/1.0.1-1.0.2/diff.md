# Comparing `tmp/grizzly-loadtester-ls-1.0.1.tar.gz` & `tmp/grizzly-loadtester-ls-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grizzly-loadtester-ls-1.0.1.tar", last modified: Wed Apr  5 14:46:50 2023, max compression
+gzip compressed data, was "grizzly-loadtester-ls-1.0.2.tar", last modified: Mon Apr 17 05:44:37 2023, max compression
```

## Comparing `grizzly-loadtester-ls-1.0.1.tar` & `grizzly-loadtester-ls-1.0.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:46:50.758206 grizzly-loadtester-ls-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-05 14:46:29.000000 grizzly-loadtester-ls-1.0.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-05 14:46:50.754206 grizzly-loadtester-ls-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-05 14:46:29.000000 grizzly-loadtester-ls-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 14:46:29.000000 grizzly-loadtester-ls-1.0.1/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-04-05 14:46:29.000000 grizzly-loadtester-ls-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 14:46:50.758206 grizzly-loadtester-ls-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:46:50.750206 grizzly-loadtester-ls-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:46:50.754206 grizzly-loadtester-ls-1.0.1/src/grizzly_loadtester_ls.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-05 14:46:50.000000 grizzly-loadtester-ls-1.0.1/src/grizzly_loadtester_ls.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-05 14:46:50.000000 grizzly-loadtester-ls-1.0.1/src/grizzly_loadtester_ls.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 14:46:50.000000 grizzly-loadtester-ls-1.0.1/src/grizzly_loadtester_ls.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-05 14:46:50.000000 grizzly-loadtester-ls-1.0.1/src/grizzly_loadtester_ls.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-05 14:46:50.000000 grizzly-loadtester-ls-1.0.1/src/grizzly_loadtester_ls.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-05 14:46:50.000000 grizzly-loadtester-ls-1.0.1/src/grizzly_loadtester_ls.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:46:50.754206 grizzly-loadtester-ls-1.0.1/src/grizzly_ls/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-05 14:46:29.000000 grizzly-loadtester-ls-1.0.1/src/grizzly_ls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-04-05 14:46:29.000000 grizzly-loadtester-ls-1.0.1/src/grizzly_ls/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22794 2023-04-05 14:46:29.000000 grizzly-loadtester-ls-1.0.1/src/grizzly_ls/server.py
--rw-r--r--   0 runner    (1001) docker     (123)    13175 2023-04-05 14:46:29.000000 grizzly-loadtester-ls-1.0.1/src/grizzly_ls/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-04-05 14:46:29.000000 grizzly-loadtester-ls-1.0.1/src/grizzly_ls/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:46:50.754206 grizzly-loadtester-ls-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 14:46:29.000000 grizzly-loadtester-ls-1.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-05 14:46:29.000000 grizzly-loadtester-ls-1.0.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-04-05 14:46:29.000000 grizzly-loadtester-ls-1.0.1/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-05 14:46:29.000000 grizzly-loadtester-ls-1.0.1/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-04-05 14:46:29.000000 grizzly-loadtester-ls-1.0.1/tests/test___main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37800 2023-04-05 14:46:29.000000 grizzly-loadtester-ls-1.0.1/tests/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-04-05 14:46:29.000000 grizzly-loadtester-ls-1.0.1/tests/test_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-04-05 14:46:29.000000 grizzly-loadtester-ls-1.0.1/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:46:50.754206 grizzly-loadtester-ls-1.0.1/types/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:46:50.754206 grizzly-loadtester-ls-1.0.1/types/behave/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 14:46:29.000000 grizzly-loadtester-ls-1.0.1/types/behave/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-05 14:46:29.000000 grizzly-loadtester-ls-1.0.1/types/behave/i18n.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-05 14:46:29.000000 grizzly-loadtester-ls-1.0.1/types/behave/matchers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-05 14:46:29.000000 grizzly-loadtester-ls-1.0.1/types/behave/runner_util.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-05 14:46:29.000000 grizzly-loadtester-ls-1.0.1/types/behave/step_registry.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-05 14:46:29.000000 grizzly-loadtester-ls-1.0.1/types/parse.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-05 14:46:29.000000 grizzly-loadtester-ls-1.0.1/types/sre_parse.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:44:37.937979 grizzly-loadtester-ls-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-17 05:44:13.000000 grizzly-loadtester-ls-1.0.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-17 05:44:37.937979 grizzly-loadtester-ls-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-17 05:44:13.000000 grizzly-loadtester-ls-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:44:13.000000 grizzly-loadtester-ls-1.0.2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-04-17 05:44:13.000000 grizzly-loadtester-ls-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 05:44:37.937979 grizzly-loadtester-ls-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:44:37.933979 grizzly-loadtester-ls-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:44:37.933979 grizzly-loadtester-ls-1.0.2/src/grizzly_loadtester_ls.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-17 05:44:37.000000 grizzly-loadtester-ls-1.0.2/src/grizzly_loadtester_ls.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-17 05:44:37.000000 grizzly-loadtester-ls-1.0.2/src/grizzly_loadtester_ls.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 05:44:37.000000 grizzly-loadtester-ls-1.0.2/src/grizzly_loadtester_ls.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-17 05:44:37.000000 grizzly-loadtester-ls-1.0.2/src/grizzly_loadtester_ls.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-17 05:44:37.000000 grizzly-loadtester-ls-1.0.2/src/grizzly_loadtester_ls.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-17 05:44:37.000000 grizzly-loadtester-ls-1.0.2/src/grizzly_loadtester_ls.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:44:37.933979 grizzly-loadtester-ls-1.0.2/src/grizzly_ls/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-17 05:44:13.000000 grizzly-loadtester-ls-1.0.2/src/grizzly_ls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-04-17 05:44:13.000000 grizzly-loadtester-ls-1.0.2/src/grizzly_ls/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22794 2023-04-17 05:44:13.000000 grizzly-loadtester-ls-1.0.2/src/grizzly_ls/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13175 2023-04-17 05:44:13.000000 grizzly-loadtester-ls-1.0.2/src/grizzly_ls/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-04-17 05:44:13.000000 grizzly-loadtester-ls-1.0.2/src/grizzly_ls/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:44:37.933979 grizzly-loadtester-ls-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:44:13.000000 grizzly-loadtester-ls-1.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-17 05:44:13.000000 grizzly-loadtester-ls-1.0.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-04-17 05:44:13.000000 grizzly-loadtester-ls-1.0.2/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-17 05:44:13.000000 grizzly-loadtester-ls-1.0.2/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-04-17 05:44:13.000000 grizzly-loadtester-ls-1.0.2/tests/test___main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37800 2023-04-17 05:44:13.000000 grizzly-loadtester-ls-1.0.2/tests/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-04-17 05:44:13.000000 grizzly-loadtester-ls-1.0.2/tests/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-04-17 05:44:13.000000 grizzly-loadtester-ls-1.0.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:44:37.937979 grizzly-loadtester-ls-1.0.2/types/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:44:37.937979 grizzly-loadtester-ls-1.0.2/types/behave/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:44:13.000000 grizzly-loadtester-ls-1.0.2/types/behave/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-17 05:44:13.000000 grizzly-loadtester-ls-1.0.2/types/behave/i18n.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-17 05:44:13.000000 grizzly-loadtester-ls-1.0.2/types/behave/matchers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-17 05:44:13.000000 grizzly-loadtester-ls-1.0.2/types/behave/runner_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-17 05:44:13.000000 grizzly-loadtester-ls-1.0.2/types/behave/step_registry.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-17 05:44:13.000000 grizzly-loadtester-ls-1.0.2/types/parse.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-17 05:44:13.000000 grizzly-loadtester-ls-1.0.2/types/sre_parse.pyi
```

### Comparing `grizzly-loadtester-ls-1.0.1/LICENSE.md` & `grizzly-loadtester-ls-1.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-ls-1.0.1/PKG-INFO` & `grizzly-loadtester-ls-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grizzly-loadtester-ls
-Version: 1.0.1
+Version: 1.0.2
 Summary: LSP server implementation for grizzly-loadtester load scenario development
 Author-email: biometria <opensource@biometria.se>
 License: MIT
 Project-URL: Documentation, https://biometria-se.github.io/grizzly/
 Project-URL: Code, https://github.com/biometria-se/grizzly-lsp/
 Project-URL: Tracker, https://github.com/Biometria-se/grizzly/issues
 Keywords: locust,behave,grizzly,grizzly-loadtester,loadtest,load,performance,traffic generator
```

### Comparing `grizzly-loadtester-ls-1.0.1/pyproject.toml` & `grizzly-loadtester-ls-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     'pylint',
     'flake8-pyproject',
     'black',
     'mypy',
     'grizzly-loadtester',
     'requests',
     'types-requests',
-    'pip-licenses',
+    'pip-licenses <4.2.0',
     'pytablewriter'
 ]
 
 ci = [
     'build',
     'twine'
 ]
```

### Comparing `grizzly-loadtester-ls-1.0.1/src/grizzly_loadtester_ls.egg-info/PKG-INFO` & `grizzly-loadtester-ls-1.0.2/src/grizzly_loadtester_ls.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grizzly-loadtester-ls
-Version: 1.0.1
+Version: 1.0.2
 Summary: LSP server implementation for grizzly-loadtester load scenario development
 Author-email: biometria <opensource@biometria.se>
 License: MIT
 Project-URL: Documentation, https://biometria-se.github.io/grizzly/
 Project-URL: Code, https://github.com/biometria-se/grizzly-lsp/
 Project-URL: Tracker, https://github.com/Biometria-se/grizzly/issues
 Keywords: locust,behave,grizzly,grizzly-loadtester,loadtest,load,performance,traffic generator
```

### Comparing `grizzly-loadtester-ls-1.0.1/src/grizzly_loadtester_ls.egg-info/SOURCES.txt` & `grizzly-loadtester-ls-1.0.2/src/grizzly_loadtester_ls.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-ls-1.0.1/src/grizzly_ls/__main__.py` & `grizzly-loadtester-ls-1.0.2/src/grizzly_ls/__main__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-ls-1.0.1/src/grizzly_ls/server.py` & `grizzly-loadtester-ls-1.0.2/src/grizzly_ls/server.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-ls-1.0.1/src/grizzly_ls/text.py` & `grizzly-loadtester-ls-1.0.2/src/grizzly_ls/text.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-ls-1.0.1/src/grizzly_ls/utils.py` & `grizzly-loadtester-ls-1.0.2/src/grizzly_ls/utils.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-ls-1.0.1/tests/fixtures.py` & `grizzly-loadtester-ls-1.0.2/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-ls-1.0.1/tests/test___main__.py` & `grizzly-loadtester-ls-1.0.2/tests/test___main__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-ls-1.0.1/tests/test_server.py` & `grizzly-loadtester-ls-1.0.2/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-ls-1.0.1/tests/test_text.py` & `grizzly-loadtester-ls-1.0.2/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-ls-1.0.1/tests/test_utils.py` & `grizzly-loadtester-ls-1.0.2/tests/test_utils.py`

 * *Files identical despite different names*

