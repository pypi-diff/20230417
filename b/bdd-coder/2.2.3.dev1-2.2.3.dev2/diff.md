# Comparing `tmp/bdd-coder-2.2.3.dev1.tar.gz` & `tmp/bdd-coder-2.2.3.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bdd-coder-2.2.3.dev1.tar", last modified: Sun Oct 16 22:01:51 2022, max compression
+gzip compressed data, was "dist/bdd-coder-2.2.3.dev2.tar", last modified: Mon Apr 17 12:15:57 2023, max compression
```

## Comparing `bdd-coder-2.2.3.dev1.tar` & `bdd-coder-2.2.3.dev2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 coleopter   (501) staff       (20)        0 2022-10-16 22:01:51.176556 bdd-coder-2.2.3.dev1/
--rw-r--r--   0 coleopter   (501) staff       (20)     1155 2022-08-31 13:08:29.000000 bdd-coder-2.2.3.dev1/LICENSE
--rw-r--r--   0 coleopter   (501) staff       (20)       73 2022-08-31 13:08:29.000000 bdd-coder-2.2.3.dev1/MANIFEST.in
--rw-r--r--   0 coleopter   (501) staff       (20)     9268 2022-10-16 22:01:51.176438 bdd-coder-2.2.3.dev1/PKG-INFO
--rw-r--r--   0 coleopter   (501) staff       (20)     8446 2022-08-31 13:08:29.000000 bdd-coder-2.2.3.dev1/README.md
-drwxr-xr-x   0 coleopter   (501) staff       (20)        0 2022-10-16 22:01:51.175619 bdd-coder-2.2.3.dev1/bdd_coder/
--rw-r--r--   0 coleopter   (501) staff       (20)        0 2022-10-11 23:43:09.000000 bdd-coder-2.2.3.dev1/bdd_coder/__init__.py
--rw-r--r--   0 coleopter   (501) staff       (20)    15682 2022-10-16 21:48:06.000000 bdd-coder-2.2.3.dev1/bdd_coder/coders.py
--rw-r--r--   0 coleopter   (501) staff       (20)     1789 2022-10-07 23:12:24.000000 bdd-coder-2.2.3.dev1/bdd_coder/commands.py
--rw-r--r--   0 coleopter   (501) staff       (20)    13926 2022-10-16 21:48:06.000000 bdd-coder-2.2.3.dev1/bdd_coder/decorators.py
--rw-r--r--   0 coleopter   (501) staff       (20)     1923 2022-10-16 21:48:06.000000 bdd-coder-2.2.3.dev1/bdd_coder/exceptions.py
--rw-r--r--   0 coleopter   (501) staff       (20)    12299 2022-10-16 21:48:06.000000 bdd-coder-2.2.3.dev1/bdd_coder/features.py
--rw-r--r--   0 coleopter   (501) staff       (20)     3460 2022-10-16 21:48:06.000000 bdd-coder-2.2.3.dev1/bdd_coder/stock.py
--rw-r--r--   0 coleopter   (501) staff       (20)     5988 2022-10-16 21:48:06.000000 bdd-coder-2.2.3.dev1/bdd_coder/tester.py
--rw-r--r--   0 coleopter   (501) staff       (20)     5296 2022-10-16 21:48:06.000000 bdd-coder-2.2.3.dev1/bdd_coder/text_utils.py
-drwxr-xr-x   0 coleopter   (501) staff       (20)        0 2022-10-16 22:01:51.176296 bdd-coder-2.2.3.dev1/bdd_coder.egg-info/
--rw-r--r--   0 coleopter   (501) staff       (20)     9268 2022-10-16 22:01:51.000000 bdd-coder-2.2.3.dev1/bdd_coder.egg-info/PKG-INFO
--rw-r--r--   0 coleopter   (501) staff       (20)      447 2022-10-16 22:01:51.000000 bdd-coder-2.2.3.dev1/bdd_coder.egg-info/SOURCES.txt
--rw-r--r--   0 coleopter   (501) staff       (20)        1 2022-10-16 22:01:51.000000 bdd-coder-2.2.3.dev1/bdd_coder.egg-info/dependency_links.txt
--rw-r--r--   0 coleopter   (501) staff       (20)      172 2022-10-16 22:01:51.000000 bdd-coder-2.2.3.dev1/bdd_coder.egg-info/entry_points.txt
--rw-r--r--   0 coleopter   (501) staff       (20)      165 2022-10-16 22:01:51.000000 bdd-coder-2.2.3.dev1/bdd_coder.egg-info/requires.txt
--rw-r--r--   0 coleopter   (501) staff       (20)       18 2022-10-16 22:01:51.000000 bdd-coder-2.2.3.dev1/bdd_coder.egg-info/top_level.txt
--rw-r--r--   0 coleopter   (501) staff       (20)       38 2022-10-16 22:01:51.176590 bdd-coder-2.2.3.dev1/setup.cfg
--rw-r--r--   0 coleopter   (501) staff       (20)     1693 2022-10-16 21:48:06.000000 bdd-coder-2.2.3.dev1/setup.py
--rw-r--r--   0 coleopter   (501) staff       (20)       47 2022-10-16 22:00:57.000000 bdd-coder-2.2.3.dev1/version.ini
+drwxr-xr-x   0 coleopter   (501) staff       (20)        0 2023-04-17 12:15:57.698143 bdd-coder-2.2.3.dev2/
+-rw-r--r--   0 coleopter   (501) staff       (20)     1155 2022-08-31 13:08:29.000000 bdd-coder-2.2.3.dev2/LICENSE
+-rw-r--r--   0 coleopter   (501) staff       (20)       73 2022-08-31 13:08:29.000000 bdd-coder-2.2.3.dev2/MANIFEST.in
+-rw-r--r--   0 coleopter   (501) staff       (20)     9268 2023-04-17 12:15:57.698027 bdd-coder-2.2.3.dev2/PKG-INFO
+-rw-r--r--   0 coleopter   (501) staff       (20)     8446 2022-08-31 13:08:29.000000 bdd-coder-2.2.3.dev2/README.md
+drwxr-xr-x   0 coleopter   (501) staff       (20)        0 2023-04-17 12:15:57.697179 bdd-coder-2.2.3.dev2/bdd_coder/
+-rw-r--r--   0 coleopter   (501) staff       (20)        0 2022-10-11 23:43:09.000000 bdd-coder-2.2.3.dev2/bdd_coder/__init__.py
+-rw-r--r--   0 coleopter   (501) staff       (20)    15682 2023-04-16 18:23:02.000000 bdd-coder-2.2.3.dev2/bdd_coder/coders.py
+-rw-r--r--   0 coleopter   (501) staff       (20)     1789 2023-04-17 11:59:19.000000 bdd-coder-2.2.3.dev2/bdd_coder/commands.py
+-rw-r--r--   0 coleopter   (501) staff       (20)    16321 2023-04-17 11:59:31.000000 bdd-coder-2.2.3.dev2/bdd_coder/decorators.py
+-rw-r--r--   0 coleopter   (501) staff       (20)     1923 2023-04-17 11:59:19.000000 bdd-coder-2.2.3.dev2/bdd_coder/exceptions.py
+-rw-r--r--   0 coleopter   (501) staff       (20)    12299 2023-04-16 18:23:02.000000 bdd-coder-2.2.3.dev2/bdd_coder/features.py
+-rw-r--r--   0 coleopter   (501) staff       (20)     3460 2023-04-16 18:23:02.000000 bdd-coder-2.2.3.dev2/bdd_coder/stock.py
+-rw-r--r--   0 coleopter   (501) staff       (20)     5988 2023-04-16 18:23:02.000000 bdd-coder-2.2.3.dev2/bdd_coder/tester.py
+-rw-r--r--   0 coleopter   (501) staff       (20)     5296 2023-04-16 18:23:02.000000 bdd-coder-2.2.3.dev2/bdd_coder/text_utils.py
+drwxr-xr-x   0 coleopter   (501) staff       (20)        0 2023-04-17 12:15:57.697886 bdd-coder-2.2.3.dev2/bdd_coder.egg-info/
+-rw-r--r--   0 coleopter   (501) staff       (20)     9268 2023-04-17 12:15:57.000000 bdd-coder-2.2.3.dev2/bdd_coder.egg-info/PKG-INFO
+-rw-r--r--   0 coleopter   (501) staff       (20)      447 2023-04-17 12:15:57.000000 bdd-coder-2.2.3.dev2/bdd_coder.egg-info/SOURCES.txt
+-rw-r--r--   0 coleopter   (501) staff       (20)        1 2023-04-17 12:15:57.000000 bdd-coder-2.2.3.dev2/bdd_coder.egg-info/dependency_links.txt
+-rw-r--r--   0 coleopter   (501) staff       (20)      172 2023-04-17 12:15:57.000000 bdd-coder-2.2.3.dev2/bdd_coder.egg-info/entry_points.txt
+-rw-r--r--   0 coleopter   (501) staff       (20)      180 2023-04-17 12:15:57.000000 bdd-coder-2.2.3.dev2/bdd_coder.egg-info/requires.txt
+-rw-r--r--   0 coleopter   (501) staff       (20)       18 2023-04-17 12:15:57.000000 bdd-coder-2.2.3.dev2/bdd_coder.egg-info/top_level.txt
+-rw-r--r--   0 coleopter   (501) staff       (20)       38 2023-04-17 12:15:57.698183 bdd-coder-2.2.3.dev2/setup.cfg
+-rw-r--r--   0 coleopter   (501) staff       (20)     1711 2023-04-17 11:59:31.000000 bdd-coder-2.2.3.dev2/setup.py
+-rw-r--r--   0 coleopter   (501) staff       (20)       47 2023-04-17 12:15:57.000000 bdd-coder-2.2.3.dev2/version.ini
```

### Comparing `bdd-coder-2.2.3.dev1/LICENSE` & `bdd-coder-2.2.3.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `bdd-coder-2.2.3.dev1/PKG-INFO` & `bdd-coder-2.2.3.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdd-coder
-Version: 2.2.3.dev1
+Version: 2.2.3.dev2
 Summary: Gherkin language in class-based tests - test suite blueprinting
 Home-page: https://bitbucket.org/coleopter/bdd-coder
 Author: Daniel Farré Manzorro
 Author-email: d.farre.m@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `bdd-coder-2.2.3.dev1/README.md` & `bdd-coder-2.2.3.dev2/README.md`

 * *Files identical despite different names*

### Comparing `bdd-coder-2.2.3.dev1/bdd_coder/coders.py` & `bdd-coder-2.2.3.dev2/bdd_coder/coders.py`

 * *Files identical despite different names*

### Comparing `bdd-coder-2.2.3.dev1/bdd_coder/commands.py` & `bdd-coder-2.2.3.dev2/bdd_coder/commands.py`

 * *Files identical despite different names*

### Comparing `bdd-coder-2.2.3.dev1/bdd_coder/decorators.py` & `bdd-coder-2.2.3.dev2/bdd_coder/decorators.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 """To be employed with `BddTester`"""
 from __future__ import annotations
 
+import inspect
+
 from collections import OrderedDict, defaultdict
 
 import datetime
 import itertools
 import functools
 import logging
 from logging.handlers import RotatingFileHandler
 
 from typing import Callable, Iterator, Optional, Union
 
 import pytest
+import pytest_asyncio
 
 from bdd_coder import exceptions
 from bdd_coder.features import StepSpec
 from bdd_coder import stock
 from bdd_coder.text_utils import (
     OK, FAIL, PENDING, TO, COMPLETION_MSG, BOLD, Style, indent, ExcInfo)
 
@@ -150,14 +153,15 @@
 
 class Step(StepSpec):
     def __init__(self, text: str, ordinal: int, scenario: Scenario):
         super().__init__(text, ordinal)
         self.scenario = scenario
         self.doc_scenario: Optional[Scenario] = None
         self.test_scenario: Optional[Scenario] = None
+        self.is_coroutine: bool
 
     @property
     def gherkin(self) -> Gherkin:
         return self.scenario.gherkin
 
     @property
     def fixture_param(self) -> Optional[list]:
@@ -170,48 +174,79 @@
         return f'{self.name}{id(self)}'
 
     def __str__(self) -> str:
         return (f'Doc scenario {self.name}' if self.doc_scenario is not None
                 else super().__str__())
 
     def __call__(self, step_method: Callable) -> Callable:
-        @functools.wraps(step_method)
+        self.is_coroutine = inspect.iscoroutinefunction(step_method)
+
+        return (self.make_async_step_method if self.is_coroutine else
+                self.make_sync_step_method)(step_method)
+
+    def make_sync_step_method(self, sync_method: Callable) -> Callable:
+        @pytest.fixture(name=self.fixture_name, params=self.fixture_param)
+        @functools.wraps(sync_method)
         def logger_step_method(tester, *args, **kwargs):
             if tester.current_run.symbol != PENDING:
                 return
 
             step_run = tester.current_run.get_pending_step_run(self)
             step_run.kwargs = {k: v for k, v in kwargs.items()
                                if k not in self.gherkin.fixtures_not_to_log}
             tester.param = self.fixture_param[0] if self.inputs else ()
 
             try:
-                step_run.result = step_method(tester, *args, **kwargs)
+                step_run.result = sync_method(tester, *args, **kwargs)
             except Exception:
                 step_run.result = ExcInfo()
                 step_run.symbol = FAIL
             else:
                 step_run.symbol = OK
 
                 if isinstance(step_run.result, tuple):
                     for name, value in zip(self.output_names, step_run.result):
                         self.gherkin.outputs[name].append(value)
+        return logger_step_method
+
+    def make_async_step_method(self, coroutine_method: Callable) -> Callable:
+        @pytest_asyncio.fixture(name=self.fixture_name, params=self.fixture_param)
+        @functools.wraps(coroutine_method)
+        async def logger_step_method(tester, *args, **kwargs):
+            if tester.current_run.symbol != PENDING:
+                return
+
+            step_run = tester.current_run.get_pending_step_run(self)
+            step_run.kwargs = {k: v for k, v in kwargs.items()
+                               if k not in self.gherkin.fixtures_not_to_log}
+            tester.param = self.fixture_param[0] if self.inputs else ()
 
-        return pytest.fixture(name=self.fixture_name, params=self.fixture_param)(
-            logger_step_method)
+            try:
+                step_run.result = await coroutine_method(tester, *args, **kwargs)
+            except Exception:
+                step_run.result = ExcInfo()
+                step_run.symbol = FAIL
+            else:
+                step_run.symbol = OK
+
+                if isinstance(step_run.result, tuple):
+                    for name, value in zip(self.output_names, step_run.result):
+                        self.gherkin.outputs[name].append(value)
+        return logger_step_method
 
 
 class Scenario(stock.Repr):
     def __init__(self, gherkin: Gherkin, *param_values):
         self.gherkin = gherkin
         self.param_values = param_values
         self.marked: bool = False
         self.ready: bool = False
         self.steps: list[Step]
         self.is_test: bool
+        self.is_coroutine: bool
 
     def __str__(self) -> str:
         return f'{self.steps[0]}...{self.steps[-1]} params={self.param_names}'
 
     @property
     def name(self) -> str:
         return self.method.__name__
@@ -270,28 +305,47 @@
         def scenario_doc_method(tester, *args, **kwargs):
             raise AssertionError('Doc scenario method called')
 
         return scenario_doc_method
 
     def make_test_method(self, marked_method: Callable) -> Callable:
         fine_steps, param_ids, param_values = self.refine()
+        self.is_coroutine = any(step.is_coroutine for step in fine_steps)
 
+        scenario_test_method = (self.make_async_test_method if self.is_coroutine else
+                                self.make_sync_test_method)(marked_method, fine_steps)
+
+        if len(param_ids) == 1:
+            param_values = tuple(v[0] for v in param_values)
+
+        if param_values:
+            return pytest.mark.parametrize(','.join(param_ids), param_values)(scenario_test_method)
+
+        return scenario_test_method
+
+    def make_sync_test_method(self, marked_method: Callable, fine_steps: list) -> Callable:
         @functools.wraps(marked_method)
         @pytest.mark.usefixtures(*(step.fixture_name for step in fine_steps))
         def scenario_test_method(tester, *args, **kwargs):
             __tracebackhide__ = True
 
             if tester.current_run.symbol == FAIL:
                 pytest.fail(reason=tester.current_run.result.next_traceback, pytrace=False)
 
-        if len(param_ids) == 1:
-            param_values = tuple(v[0] for v in param_values)
+        return scenario_test_method
 
-        if param_values:
-            return pytest.mark.parametrize(','.join(param_ids), param_values)(scenario_test_method)
+    def make_async_test_method(self, marked_method: Callable, fine_steps: list) -> Callable:
+        @functools.wraps(marked_method)
+        @pytest.mark.usefixtures(*(step.fixture_name for step in fine_steps))
+        @pytest.mark.asyncio
+        async def scenario_test_method(tester, *args, **kwargs):
+            __tracebackhide__ = True
+
+            if tester.current_run.symbol == FAIL:
+                pytest.fail(reason=tester.current_run.result.next_traceback, pytrace=False)
 
         return scenario_test_method
 
     def __call__(self, method) -> Callable:
         if self.marked is False:
             self.method = self.mark_method(method)
             self.marked = True
```

### Comparing `bdd-coder-2.2.3.dev1/bdd_coder/exceptions.py` & `bdd-coder-2.2.3.dev2/bdd_coder/exceptions.py`

 * *Files identical despite different names*

### Comparing `bdd-coder-2.2.3.dev1/bdd_coder/features.py` & `bdd-coder-2.2.3.dev2/bdd_coder/features.py`

 * *Files identical despite different names*

### Comparing `bdd-coder-2.2.3.dev1/bdd_coder/stock.py` & `bdd-coder-2.2.3.dev2/bdd_coder/stock.py`

 * *Files identical despite different names*

### Comparing `bdd-coder-2.2.3.dev1/bdd_coder/tester.py` & `bdd-coder-2.2.3.dev2/bdd_coder/tester.py`

 * *Files identical despite different names*

### Comparing `bdd-coder-2.2.3.dev1/bdd_coder/text_utils.py` & `bdd-coder-2.2.3.dev2/bdd_coder/text_utils.py`

 * *Files identical despite different names*

### Comparing `bdd-coder-2.2.3.dev1/bdd_coder.egg-info/PKG-INFO` & `bdd-coder-2.2.3.dev2/bdd_coder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdd-coder
-Version: 2.2.3.dev1
+Version: 2.2.3.dev2
 Summary: Gherkin language in class-based tests - test suite blueprinting
 Home-page: https://bitbucket.org/coleopter/bdd-coder
 Author: Daniel Farré Manzorro
 Author-email: d.farre.m@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `bdd-coder-2.2.3.dev1/setup.py` & `bdd-coder-2.2.3.dev2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 ini = configparser.ConfigParser()
 ini.read('version.ini')
 
 with open('README.md', encoding='utf-8') as readme:
     long_description = readme.read()
 
-tests_require = ['pytest-cov', 'freezegun']
+tests_require = ['pytest-cov', 'pytest-asyncio', 'freezegun']
 
 setuptools.setup(
     name=ini['version']['name'],
     version=ini['version']['value'],
     author='Daniel Farré Manzorro',
     author_email='d.farre.m@gmail.com',
     description='Gherkin language in class-based tests - test suite blueprinting',
```

