# Comparing `tmp/grizzly-loadtester-cli-3.1.5.tar.gz` & `tmp/grizzly-loadtester-cli-3.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grizzly-loadtester-cli-3.1.5.tar", last modified: Mon Jan  9 13:41:35 2023, max compression
+gzip compressed data, was "grizzly-loadtester-cli-3.1.6.tar", last modified: Mon Apr 17 05:45:01 2023, max compression
```

## Comparing `grizzly-loadtester-cli-3.1.5.tar` & `grizzly-loadtester-cli-3.1.6.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 13:41:35.413392 grizzly-loadtester-cli-3.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-01-09 13:41:10.000000 grizzly-loadtester-cli-3.1.5/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-01-09 13:41:10.000000 grizzly-loadtester-cli-3.1.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-01-09 13:41:10.000000 grizzly-loadtester-cli-3.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-01-09 13:41:35.413392 grizzly-loadtester-cli-3.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-01-09 13:41:10.000000 grizzly-loadtester-cli-3.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 13:41:35.409392 grizzly-loadtester-cli-3.1.5/grizzly_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-01-09 13:41:10.000000 grizzly-loadtester-cli-3.1.5/grizzly_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-01-09 13:41:10.000000 grizzly-loadtester-cli-3.1.5/grizzly_cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-09 13:41:35.000000 grizzly-loadtester-cli-3.1.5/grizzly_cli/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 13:41:35.409392 grizzly-loadtester-cli-3.1.5/grizzly_cli/argparse/
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-01-09 13:41:10.000000 grizzly-loadtester-cli-3.1.5/grizzly_cli/argparse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 13:41:35.413392 grizzly-loadtester-cli-3.1.5/grizzly_cli/argparse/bashcompletion/
--rw-r--r--   0 runner    (1001) docker     (123)    13240 2023-01-09 13:41:10.000000 grizzly-loadtester-cli-3.1.5/grizzly_cli/argparse/bashcompletion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-01-09 13:41:10.000000 grizzly-loadtester-cli-3.1.5/grizzly_cli/argparse/bashcompletion/bashcompletion.bash
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-01-09 13:41:10.000000 grizzly-loadtester-cli-3.1.5/grizzly_cli/argparse/bashcompletion/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8089 2023-01-09 13:41:10.000000 grizzly-loadtester-cli-3.1.5/grizzly_cli/argparse/markdown.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 13:41:35.413392 grizzly-loadtester-cli-3.1.5/grizzly_cli/distributed/
--rw-r--r--   0 runner    (1001) docker     (123)    11863 2023-01-09 13:41:10.000000 grizzly-loadtester-cli-3.1.5/grizzly_cli/distributed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-01-09 13:41:10.000000 grizzly-loadtester-cli-3.1.5/grizzly_cli/distributed/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-01-09 13:41:10.000000 grizzly-loadtester-cli-3.1.5/grizzly_cli/distributed/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-01-09 13:41:10.000000 grizzly-loadtester-cli-3.1.5/grizzly_cli/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-01-09 13:41:10.000000 grizzly-loadtester-cli-3.1.5/grizzly_cli/local.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-01-09 13:41:10.000000 grizzly-loadtester-cli-3.1.5/grizzly_cli/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-01-09 13:41:10.000000 grizzly-loadtester-cli-3.1.5/grizzly_cli/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 13:41:35.413392 grizzly-loadtester-cli-3.1.5/grizzly_cli/static/
--rw-r--r--   0 runner    (1001) docker     (123)     5293 2023-01-09 13:41:10.000000 grizzly-loadtester-cli-3.1.5/grizzly_cli/static/Containerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-01-09 13:41:10.000000 grizzly-loadtester-cli-3.1.5/grizzly_cli/static/compose.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    28490 2023-01-09 13:41:10.000000 grizzly-loadtester-cli-3.1.5/grizzly_cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 13:41:35.413392 grizzly-loadtester-cli-3.1.5/grizzly_loadtester_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-01-09 13:41:35.000000 grizzly-loadtester-cli-3.1.5/grizzly_loadtester_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-01-09 13:41:35.000000 grizzly-loadtester-cli-3.1.5/grizzly_loadtester_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-09 13:41:35.000000 grizzly-loadtester-cli-3.1.5/grizzly_loadtester_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-01-09 13:41:35.000000 grizzly-loadtester-cli-3.1.5/grizzly_loadtester_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-01-09 13:41:35.000000 grizzly-loadtester-cli-3.1.5/grizzly_loadtester_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-01-09 13:41:35.000000 grizzly-loadtester-cli-3.1.5/grizzly_loadtester_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-01-09 13:41:10.000000 grizzly-loadtester-cli-3.1.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 13:41:35.413392 grizzly-loadtester-cli-3.1.5/script/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3533 2023-01-09 13:41:10.000000 grizzly-loadtester-cli-3.1.5/script/docs-generate-licenses.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-09 13:41:35.413392 grizzly-loadtester-cli-3.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:45:01.378837 grizzly-loadtester-cli-3.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-17 05:44:36.000000 grizzly-loadtester-cli-3.1.6/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-17 05:44:36.000000 grizzly-loadtester-cli-3.1.6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-17 05:44:36.000000 grizzly-loadtester-cli-3.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-17 05:45:01.374837 grizzly-loadtester-cli-3.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-17 05:44:36.000000 grizzly-loadtester-cli-3.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:45:01.374837 grizzly-loadtester-cli-3.1.6/grizzly_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-17 05:44:36.000000 grizzly-loadtester-cli-3.1.6/grizzly_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-04-17 05:44:36.000000 grizzly-loadtester-cli-3.1.6/grizzly_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-17 05:45:01.000000 grizzly-loadtester-cli-3.1.6/grizzly_cli/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:45:01.374837 grizzly-loadtester-cli-3.1.6/grizzly_cli/argparse/
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-04-17 05:44:36.000000 grizzly-loadtester-cli-3.1.6/grizzly_cli/argparse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:45:01.374837 grizzly-loadtester-cli-3.1.6/grizzly_cli/argparse/bashcompletion/
+-rw-r--r--   0 runner    (1001) docker     (123)    13240 2023-04-17 05:44:36.000000 grizzly-loadtester-cli-3.1.6/grizzly_cli/argparse/bashcompletion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-17 05:44:36.000000 grizzly-loadtester-cli-3.1.6/grizzly_cli/argparse/bashcompletion/bashcompletion.bash
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-04-17 05:44:36.000000 grizzly-loadtester-cli-3.1.6/grizzly_cli/argparse/bashcompletion/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8089 2023-04-17 05:44:36.000000 grizzly-loadtester-cli-3.1.6/grizzly_cli/argparse/markdown.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:45:01.374837 grizzly-loadtester-cli-3.1.6/grizzly_cli/distributed/
+-rw-r--r--   0 runner    (1001) docker     (123)    11863 2023-04-17 05:44:36.000000 grizzly-loadtester-cli-3.1.6/grizzly_cli/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-04-17 05:44:36.000000 grizzly-loadtester-cli-3.1.6/grizzly_cli/distributed/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-04-17 05:44:36.000000 grizzly-loadtester-cli-3.1.6/grizzly_cli/distributed/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-04-17 05:44:36.000000 grizzly-loadtester-cli-3.1.6/grizzly_cli/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-17 05:44:36.000000 grizzly-loadtester-cli-3.1.6/grizzly_cli/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-17 05:44:36.000000 grizzly-loadtester-cli-3.1.6/grizzly_cli/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-04-17 05:44:36.000000 grizzly-loadtester-cli-3.1.6/grizzly_cli/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:45:01.374837 grizzly-loadtester-cli-3.1.6/grizzly_cli/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     5293 2023-04-17 05:44:36.000000 grizzly-loadtester-cli-3.1.6/grizzly_cli/static/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-04-17 05:44:36.000000 grizzly-loadtester-cli-3.1.6/grizzly_cli/static/compose.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    28038 2023-04-17 05:44:36.000000 grizzly-loadtester-cli-3.1.6/grizzly_cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:45:01.374837 grizzly-loadtester-cli-3.1.6/grizzly_loadtester_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-17 05:45:01.000000 grizzly-loadtester-cli-3.1.6/grizzly_loadtester_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-17 05:45:01.000000 grizzly-loadtester-cli-3.1.6/grizzly_loadtester_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 05:45:01.000000 grizzly-loadtester-cli-3.1.6/grizzly_loadtester_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-17 05:45:01.000000 grizzly-loadtester-cli-3.1.6/grizzly_loadtester_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-17 05:45:01.000000 grizzly-loadtester-cli-3.1.6/grizzly_loadtester_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-17 05:45:01.000000 grizzly-loadtester-cli-3.1.6/grizzly_loadtester_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-04-17 05:44:36.000000 grizzly-loadtester-cli-3.1.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:45:01.374837 grizzly-loadtester-cli-3.1.6/script/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3533 2023-04-17 05:44:36.000000 grizzly-loadtester-cli-3.1.6/script/docs-generate-licenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 05:45:01.378837 grizzly-loadtester-cli-3.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-17 05:44:36.000000 grizzly-loadtester-cli-3.1.6/test.py
```

### Comparing `grizzly-loadtester-cli-3.1.5/LICENSE.md` & `grizzly-loadtester-cli-3.1.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-cli-3.1.5/PKG-INFO` & `grizzly-loadtester-cli-3.1.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grizzly-loadtester-cli
-Version: 3.1.5
+Version: 3.1.6
 Summary: Command line interface for grizzly-loadtester
 Author-email: biometria <opensource@biometria.se>
 Project-URL: Documentation, https://biometria-se.github.io/grizzly/command-line-interface/usage/
 Project-URL: Code, https://github.com/biometria-se/grizzly/
 Project-URL: Tracker, https://github.com/Biometria-se/grizzly/issues
 Keywords: grizzly,grizzly-loadtester,cli,command line interface,locust,behave,load,loadtest,performance,traffic generator
 Classifier: Development Status :: 4 - Beta
```

### Comparing `grizzly-loadtester-cli-3.1.5/grizzly_cli/__init__.py` & `grizzly-loadtester-cli-3.1.6/grizzly_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-cli-3.1.5/grizzly_cli/__main__.py` & `grizzly-loadtester-cli-3.1.6/grizzly_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-cli-3.1.5/grizzly_cli/argparse/__init__.py` & `grizzly-loadtester-cli-3.1.6/grizzly_cli/argparse/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     def print_help(self, file: Optional[IO[str]] = None) -> None:
         '''Hook to make help more command line friendly, if there is markdown markers in the text.
         '''
         if not self.markdown_help:
             super().print_help(file)
             return
 
-        if self.formatter_class is not MarkdownFormatter:
+        if self.formatter_class is not MarkdownFormatter:  # type: ignore
             original_description = self.description
             original_actions = self._actions
 
             # code block "markers" are not really nice to have in cli help
             if self.description is not None:
                 self.description = '\n'.join([line for line in self.description.split('\n') if '```' not in line])
                 self.description = self.description.replace('\n\n', '\n')
@@ -49,15 +49,15 @@
             for action in self._actions:
                 if action.help is not None:
                     # remove any markdown link markers
                     action.help = re.sub(r'\[([^\]]*)\]\([^\)]*\)', r'\1', action.help)
 
         super().print_help(file)
 
-        if self.formatter_class is not MarkdownFormatter:
+        if self.formatter_class is not MarkdownFormatter:  # type: ignore
             self.description = original_description
             self._actions = original_actions
 
     def parse_args(self, args: Optional[Sequence[str]] = None, namespace: Optional[Namespace] = None) -> Namespace:  # type: ignore
         """
         Hook to add `--bash-complete` to all parsers, if enabled for parser.
         """
```

### Comparing `grizzly-loadtester-cli-3.1.5/grizzly_cli/argparse/bashcompletion/__init__.py` & `grizzly-loadtester-cli-3.1.6/grizzly_cli/argparse/bashcompletion/__init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-cli-3.1.5/grizzly_cli/argparse/bashcompletion/bashcompletion.bash` & `grizzly-loadtester-cli-3.1.6/grizzly_cli/argparse/bashcompletion/bashcompletion.bash`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-cli-3.1.5/grizzly_cli/argparse/bashcompletion/types.py` & `grizzly-loadtester-cli-3.1.6/grizzly_cli/argparse/bashcompletion/types.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-cli-3.1.5/grizzly_cli/argparse/markdown.py` & `grizzly-loadtester-cli-3.1.6/grizzly_cli/argparse/markdown.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-cli-3.1.5/grizzly_cli/distributed/__init__.py` & `grizzly-loadtester-cli-3.1.6/grizzly_cli/distributed/__init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-cli-3.1.5/grizzly_cli/distributed/build.py` & `grizzly-loadtester-cli-3.1.6/grizzly_cli/distributed/build.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-cli-3.1.5/grizzly_cli/distributed/clean.py` & `grizzly-loadtester-cli-3.1.6/grizzly_cli/distributed/clean.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-cli-3.1.5/grizzly_cli/init.py` & `grizzly-loadtester-cli-3.1.6/grizzly_cli/init.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Generator
 from argparse import Namespace as Arguments
 from os import path
 from pathlib import Path
+from packaging.version import Version
 
 from .utils import ask_yes_no
 from . import EXECUTION_CONTEXT, register_parser
 from .argparse import ArgumentSubParser
 
 # prefix components:
 space = '    '
@@ -139,15 +140,21 @@
     # create features/<project>.feature
     (structure_features / f'{args.project}.feature').write_text('''Feature: Template feature file
   Scenario: Template scenario
     Given a user of type "RestApi" with weight "1" load testing "$conf::template.host"
 ''')
 
     # create features/environment.py
-    (structure_features / 'environment.py').write_text('from grizzly.environment import *\n\n')
+    if args.grizzly_version is not None:
+        version = Version(args.grizzly_version)
+        if version < Version('2.6.0'):
+            grizzly_behave_module = 'environment'
+    else:
+        grizzly_behave_module = 'behave'
+    (structure_features / 'environment.py').write_text(f'from grizzly.{grizzly_behave_module} import *\n\n')
 
     # create features/requests directory
     (structure_features / 'requests').mkdir()
 
     # create features/steps directory
     structure_feature_steps = structure_features / 'steps'
     structure_feature_steps.mkdir()
```

### Comparing `grizzly-loadtester-cli-3.1.5/grizzly_cli/local.py` & `grizzly-loadtester-cli-3.1.6/grizzly_cli/local.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-cli-3.1.5/grizzly_cli/run.py` & `grizzly-loadtester-cli-3.1.6/grizzly_cli/run.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-cli-3.1.5/grizzly_cli/static/Containerfile` & `grizzly-loadtester-cli-3.1.6/grizzly_cli/static/Containerfile`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-cli-3.1.5/grizzly_cli/static/compose.yaml` & `grizzly-loadtester-cli-3.1.6/grizzly_cli/static/compose.yaml`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-cli-3.1.5/grizzly_cli/utils.py` & `grizzly-loadtester-cli-3.1.6/grizzly_cli/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -345,49 +345,44 @@
 
             grizzly_requirement_egg = grizzly_requirement
 
             # get grizzly version used in requirements.txt
             if re.match(r'^grizzly-loadtester(\[[^\]]*\])?$', grizzly_requirement):  # latest
                 grizzly_version = pypi.get('info', {}).get('version', None)
             else:
-                available_versions = [versioning.parse(available_version) for available_version in pypi.get('releases', {}).keys()]
                 conditions: List[Callable[[versioning.Version], bool]] = []
 
                 match = re.match(r'^(grizzly-loadtester(\[[^\]]*\])?)(.*?)$', grizzly_requirement)
 
                 if match:
                     grizzly_requirement_egg = match.group(1)
                     condition_expression = match.group(3)
 
                     for condition in condition_expression.split(',', 1):
                         version_string = re.sub(r'^[^0-9]{1,2}', '', condition)
                         condition_version = versioning.parse(version_string)
 
-                        if not isinstance(condition_version, versioning.Version):
-                            print(f'!! {condition} is a {condition_version.__class__.__name__}, expected Version', file=sys.stderr)
-                            break
-
                         if '>' in condition:
                             compare = condition_version.__le__ if '=' in condition else condition_version.__lt__
                         elif '<' in condition:
                             compare = condition_version.__ge__ if '=' in condition else condition_version.__gt__
                         else:
                             compare = condition_version.__eq__
 
                         conditions.append(compare)
 
                 matched_version = None
 
-                for available_version in available_versions:
-                    if not isinstance(available_version, versioning.Version):
-                        print(f'!! {str(available_version)} is a {available_version.__class__.__name__}, expected Version', file=sys.stderr)
-                        break
-
-                    if len(conditions) > 0 and all([compare(available_version) for compare in conditions]):
-                        matched_version = available_version
+                for available_version in pypi.get('releases', {}).keys():
+                    try:
+                        version = versioning.parse(available_version)
+                        if len(conditions) > 0 and all([compare(version) for compare in conditions]):
+                            matched_version = version
+                    except versioning.InvalidVersion:
+                        pass
 
                 if matched_version is None:
                     print(f'!! could not resolve {grizzly_requirement} to one specific version available at pypi', file=sys.stderr)
                 else:
                     grizzly_version = str(matched_version)
 
             if grizzly_version is not None:
```

### Comparing `grizzly-loadtester-cli-3.1.5/grizzly_loadtester_cli.egg-info/PKG-INFO` & `grizzly-loadtester-cli-3.1.6/grizzly_loadtester_cli.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grizzly-loadtester-cli
-Version: 3.1.5
+Version: 3.1.6
 Summary: Command line interface for grizzly-loadtester
 Author-email: biometria <opensource@biometria.se>
 Project-URL: Documentation, https://biometria-se.github.io/grizzly/command-line-interface/usage/
 Project-URL: Code, https://github.com/biometria-se/grizzly/
 Project-URL: Tracker, https://github.com/Biometria-se/grizzly/issues
 Keywords: grizzly,grizzly-loadtester,cli,command line interface,locust,behave,load,loadtest,performance,traffic generator
 Classifier: Development Status :: 4 - Beta
```

### Comparing `grizzly-loadtester-cli-3.1.5/grizzly_loadtester_cli.egg-info/SOURCES.txt` & `grizzly-loadtester-cli-3.1.6/grizzly_loadtester_cli.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 .editorconfig
 LICENSE.md
 MANIFEST.in
 README.md
 pyproject.toml
+test.py
 grizzly_cli/__init__.py
 grizzly_cli/__main__.py
 grizzly_cli/__version__.py
 grizzly_cli/init.py
 grizzly_cli/local.py
 grizzly_cli/py.typed
 grizzly_cli/run.py
```

### Comparing `grizzly-loadtester-cli-3.1.5/grizzly_loadtester_cli.egg-info/requires.txt` & `grizzly-loadtester-cli-3.1.6/grizzly_loadtester_cli.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 behave<2.0.0,>=1.2.6
 Jinja2<4.0.0,>=3.0.3
 requests<3.0.0,>=2.27.1
-packaging<22.0,>=21.3
+packaging>=21.3
 chardet<5.0.0,>=3.0.2
-tomli<2.0.0,>=1.2.3
+tomli<3.0.0,>=2.0.0
 
 [ci]
 build>=0.7.0
 twine>=3.8.0
 
 [dev]
 mypy<=1.0,>=0.931
@@ -16,15 +16,15 @@
 coverage[toml]<7.0.0,>=6.4.4
 pytest-cov<5.0.0,>=4.0.0
 pytest-mock<4.0.0,>=3.7.0
 pytest-timeout<3.0.0,>=2.1.0
 atomicwrites<2.0.0,>=1.4.0
 flake8-pyproject>=1.1.0
 requests-mock<2.0.0,>=1.9.3
-pip-licenses>=3.5.3
+pip-licenses<4.2.0,>=3.5.3
 pytablewriter>=0.64.1
 line-profiler>=3.5.1
 gevent<22.0.0,>=21.12.0
 flask==2.0.3
 pyyaml<7.0.0,>=6.0.0
 types-requests<3.0.0,>=2.27.13
 types-pyyaml
```

### Comparing `grizzly-loadtester-cli-3.1.5/pyproject.toml` & `grizzly-loadtester-cli-3.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ]
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
     "behave >=1.2.6,<2.0.0",
     "Jinja2 >=3.0.3,<4.0.0",
     "requests >=2.27.1,<3.0.0",
-    "packaging >=21.3,<22.0",
+    "packaging >=21.3",
     "chardet >=3.0.2,<5.0.0",
-    "tomli >=1.2.3,<2.0.0",
+    "tomli >=2.0.0,<3.0.0"
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
@@ -58,15 +58,15 @@
     "coverage[toml] >=6.4.4,<7.0.0",
     "pytest-cov >=4.0.0,<5.0.0",
     "pytest-mock >=3.7.0,<4.0.0",
     "pytest-timeout >=2.1.0,<3.0.0",
     "atomicwrites >=1.4.0,<2.0.0",
     "flake8-pyproject >=1.1.0",
     "requests-mock >=1.9.3,<2.0.0",
-    "pip-licenses >=3.5.3",
+    "pip-licenses >=3.5.3,<4.2.0",
     "pytablewriter >=0.64.1",
     "line-profiler >=3.5.1",
     "gevent >=21.12.0,<22.0.0",
     "flask ==2.0.3",
     "pyyaml >=6.0.0,<7.0.0",
     "types-requests >=2.27.13,<3.0.0",
     "types-pyyaml",
```

### Comparing `grizzly-loadtester-cli-3.1.5/script/docs-generate-licenses.py` & `grizzly-loadtester-cli-3.1.6/script/docs-generate-licenses.py`

 * *Files identical despite different names*

