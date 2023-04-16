# Comparing `tmp/experiment-config-0.1.tar.gz` & `tmp/experiment-config-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "experiment-config-0.1.tar", last modified: Fri Feb 17 01:02:55 2023, max compression
+gzip compressed data, was "dist/experiment-config-0.2.tar", last modified: Sun Apr 16 22:31:55 2023, max compression
```

## Comparing `experiment-config-0.1.tar` & `experiment-config-0.2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-02-17 01:02:55.404455 experiment-config-0.1/
--rw-r--r--   0 ahalev     (502) staff       (20)     1073 2023-01-29 22:38:50.000000 experiment-config-0.1/LICENSE.txt
--rw-r--r--   0 ahalev     (502) staff       (20)      508 2023-02-17 01:02:55.404286 experiment-config-0.1/PKG-INFO
--rw-r--r--   0 ahalev     (502) staff       (20)      178 2023-02-17 01:02:25.000000 experiment-config-0.1/README.md
--rw-r--r--   0 ahalev     (502) staff       (20)       38 2023-02-17 01:02:55.404503 experiment-config-0.1/setup.cfg
--rw-r--r--   0 ahalev     (502) staff       (20)      863 2023-02-17 00:30:05.000000 experiment-config-0.1/setup.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-02-17 01:02:55.401430 experiment-config-0.1/src/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-02-17 01:02:55.402784 experiment-config-0.1/src/experiment_config.egg-info/
--rw-r--r--   0 ahalev     (502) staff       (20)      508 2023-02-17 01:02:55.000000 experiment-config-0.1/src/experiment_config.egg-info/PKG-INFO
--rw-r--r--   0 ahalev     (502) staff       (20)      380 2023-02-17 01:02:55.000000 experiment-config-0.1/src/experiment_config.egg-info/SOURCES.txt
--rw-r--r--   0 ahalev     (502) staff       (20)        1 2023-02-17 01:02:55.000000 experiment-config-0.1/src/experiment_config.egg-info/dependency_links.txt
--rw-r--r--   0 ahalev     (502) staff       (20)       28 2023-02-17 01:02:55.000000 experiment-config-0.1/src/experiment_config.egg-info/requires.txt
--rw-r--r--   0 ahalev     (502) staff       (20)        7 2023-02-17 01:02:55.000000 experiment-config-0.1/src/experiment_config.egg-info/top_level.txt
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-02-17 01:02:55.403478 experiment-config-0.1/src/expfig/
--rw-r--r--   0 ahalev     (502) staff       (20)      125 2023-02-15 22:42:50.000000 experiment-config-0.1/src/expfig/__init__.py
--rw-r--r--   0 ahalev     (502) staff       (20)     6795 2023-02-17 00:30:05.000000 experiment-config-0.1/src/expfig/fig.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-02-17 01:02:55.403959 experiment-config-0.1/src/expfig/logger/
--rw-r--r--   0 ahalev     (502) staff       (20)       45 2023-02-15 22:42:50.000000 experiment-config-0.1/src/expfig/logger/__init__.py
--rw-r--r--   0 ahalev     (502) staff       (20)     1281 2023-02-15 22:42:50.000000 experiment-config-0.1/src/expfig/logger/log_dir.py
--rw-r--r--   0 ahalev     (502) staff       (20)     4093 2023-02-17 00:30:05.000000 experiment-config-0.1/src/expfig/namespacify.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-16 22:31:55.000000 experiment-config-0.2/
+-rw-r--r--   0 ahalev     (502) staff       (20)     1073 2023-01-29 22:38:50.000000 experiment-config-0.2/LICENSE.txt
+-rw-r--r--   0 ahalev     (502) staff       (20)     8624 2023-04-16 22:31:55.000000 experiment-config-0.2/PKG-INFO
+-rw-r--r--   0 ahalev     (502) staff       (20)     8185 2023-03-08 21:19:36.000000 experiment-config-0.2/README.md
+-rw-r--r--   0 ahalev     (502) staff       (20)       38 2023-04-16 22:31:55.000000 experiment-config-0.2/setup.cfg
+-rw-r--r--   0 ahalev     (502) staff       (20)      929 2023-04-16 22:31:35.000000 experiment-config-0.2/setup.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-16 22:31:55.000000 experiment-config-0.2/src/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-16 22:31:55.000000 experiment-config-0.2/src/experiment_config.egg-info/
+-rw-r--r--   0 ahalev     (502) staff       (20)     8624 2023-04-16 22:31:55.000000 experiment-config-0.2/src/experiment_config.egg-info/PKG-INFO
+-rw-r--r--   0 ahalev     (502) staff       (20)      411 2023-04-16 22:31:55.000000 experiment-config-0.2/src/experiment_config.egg-info/SOURCES.txt
+-rw-r--r--   0 ahalev     (502) staff       (20)        1 2023-04-16 22:31:55.000000 experiment-config-0.2/src/experiment_config.egg-info/dependency_links.txt
+-rw-r--r--   0 ahalev     (502) staff       (20)       28 2023-04-16 22:31:55.000000 experiment-config-0.2/src/experiment_config.egg-info/requires.txt
+-rw-r--r--   0 ahalev     (502) staff       (20)        7 2023-04-16 22:31:55.000000 experiment-config-0.2/src/experiment_config.egg-info/top_level.txt
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-16 22:31:55.000000 experiment-config-0.2/src/expfig/
+-rw-r--r--   0 ahalev     (502) staff       (20)      126 2023-03-08 21:19:36.000000 experiment-config-0.2/src/expfig/__init__.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     8087 2023-04-16 22:26:51.000000 experiment-config-0.2/src/expfig/fig.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-16 22:31:55.000000 experiment-config-0.2/src/expfig/logging/
+-rw-r--r--   0 ahalev     (502) staff       (20)       76 2023-03-08 21:19:36.000000 experiment-config-0.2/src/expfig/logging/__init__.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     1281 2023-03-08 21:19:36.000000 experiment-config-0.2/src/expfig/logging/log_dir.py
+-rw-r--r--   0 ahalev     (502) staff       (20)      381 2023-03-08 21:19:36.000000 experiment-config-0.2/src/expfig/logging/logger.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     6505 2023-04-08 23:03:36.000000 experiment-config-0.2/src/expfig/namespacify.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `experiment-config-0.1/LICENSE.txt` & `experiment-config-0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `experiment-config-0.1/setup.py` & `experiment-config-0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 from pathlib import Path
 from setuptools import setup, find_packages
 
 DESCRIPTION = 'A yaml-based configuration for reproducible python experiments.'
-VERSION = '0.1'
-MAINTAINER = "Avishai Halev"
-MAINTAINER_EMAIL = "avishaihalev@gmail.com"
-LICENSE = "MIT License"
-PROJECT_URLS = {}
+VERSION = '0.2'
+MAINTAINER = 'Avishai Halev'
+MAINTAINER_EMAIL = 'avishaihalev@gmail.com'
+LICENSE = 'MIT License'
+PROJECT_URLS = {
+    'Source Code': 'https://github.com/ahalev/experiment-config'
+}
 EXTRAS = {
-    "dev": ["pytest"]
+    'dev': ['pytest']
 }
 
 setup(
-    name="experiment-config",
-    package_dir={"": "src"},
-    packages=find_packages("src"),
-    python_requires=">=3.6",
+    name='experiment-config',
+    package_dir={'': 'src'},
+    packages=find_packages('src'),
+    python_requires='>=3.6',
     version=VERSION,
     maintainer=MAINTAINER,
     maintainer_email=MAINTAINER_EMAIL,
     project_urls=PROJECT_URLS,
     description=DESCRIPTION,
     license=LICENSE,
-    long_description=(Path(__file__).parent / "README.md").read_text(),
-    long_description_content_type="text/markdown",
+    long_description=(Path(__file__).parent / 'README.md').read_text(),
+    long_description_content_type='text/markdown',
     include_package_data=True,
     install_requires=[
-        "pandas",
-        "pyyaml"
+        'pandas',
+        'pyyaml'
     ],
     extras_require=EXTRAS
 
 )
```

### Comparing `experiment-config-0.1/src/expfig/fig.py` & `experiment-config-0.2/src/expfig/fig.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,189 +1,226 @@
 import argparse
+import sys
 import os
 import pandas as pd
 import yaml
 
+from copy import deepcopy
 
 from collections import UserDict
-from logging import getLogger
 from pathlib import Path
 from warnings import warn
 
 from . import Namespacify, nested_dict_update
+from .logging import get_logger
 
-logger = getLogger(__name__)
 
 DEFAULT_CONFIG_PATH = os.path.join(os.getcwd(), 'default_config.yaml')
 
 
 class Config(Namespacify):
     def __init__(self, config=None, keys_for_name=(), name_prefix='', default=DEFAULT_CONFIG_PATH):
         self.default_config = DefaultConfig(self._parse_default(config, default)).with_name_from_keys(*keys_for_name, prefix=name_prefix)
 
+        self.logger = get_logger()
+        self.verbosity = 0
+
         super().__init__(self._parse_config())
 
-        if config is not None:
-            self._update_with_config(config)
+        self.update_with_configs(config)
+        # if config is not None:
+        #     self._update_with_config(config)
 
         self.with_name_from_keys(*keys_for_name, prefix=name_prefix)
-        self._verbose()
+        self.verbose(self.verbosity)
 
-    def serialize_to_dir(self, log_dir, fname='config.yaml', use_existing_dir=False, with_default=False):
-        log_dir = super().serialize_to_dir(log_dir, fname=fname, use_existing_dir=use_existing_dir)
+    def _parse_default(self, config, default):
+        candidates = [Path(default), (Path(sys.argv[0]).parent / default)]
 
-        if with_default:
-            path = Path(fname)
+        if config is not None and isinstance(config, (str, Path)):
+            candidates.extend([Path(config), (Path(sys.argv[0]).parent / config)])
 
-            def fname_func(kind): return (path.parent / f'{path.stem}_{kind}').with_suffix(path.suffix)
+        for candidate in candidates:
+            if candidate.exists():
+                return candidate
+
+        candidates_str = '\n\t'.join(str(x.absolute()) for x in candidates)
+        err_msg = f'Attempted to resolve default config in the following order:\n\t{candidates_str}.\n' \
+                  f'Unable to find a file amongst these candidates.'
+        raise ValueError(err_msg)
 
-            self.default_config.serialize_to_dir(log_dir,
-                                                 fname=fname_func('default'),
-                                                 use_existing_dir=True)
+    def _parse_config(self):
+        # First we parse any --config arguments and load those
+        # Then we can override them with any other passed values.
+        base_config = deepcopy(self.default_config)
+        config_files, other_args = self._create_config_file_parser().parse_known_args()
+
+        self.update_with_configs(config_files.config, base_config)
+        # for config_file in config_files.config:
+        #     self._update_with_config(config_file, updatee=base_config)
 
-            (self ^ self.default_config).serialize_to_dir(log_dir,
-                                                          fname=fname_func('difference'),
-                                                          use_existing_dir=True)
-        return log_dir
+        parsed_args = self._create_parser(default=base_config).parse_known_args(other_args)
 
-    def _parse_default(self, config, default):
-        if os.path.exists(default):
-            return default
-        elif config is not None and os.path.exists(config):
-            return config
-        else:
-            raise ValueError(f'Default config path {os.path.abspath(default)} does not point to a file. '
-                             f'Passed config {config} does not either.')
+        if len(parsed_args[1]):
+            bad_args = [x.replace("--", "") for x in parsed_args[1] if x.startswith("--")]
+            valid_args = "\n\t\t".join(sorted(parsed_args[0].__dict__.keys()))
+            warn(f'Unrecognized arguments {bad_args}.\n\tValid arguments:\n\t\t{valid_args}')
 
-    def _verbose(self, level='from_config'):
-        if level == 'from_config':
-            try:
-                level = self.context.verbose
-            except AttributeError:
-                level = 0
+        args_dict = parsed_args[0].__dict__
 
-        if level >= 2:
-            logger.info('Trainer config:')
-            self.pprint(indent=1)
-        if level >= 1:
-            xor = self ^ self.default_config
-            print(f'\n{"-"*10}\n')
-            if xor:
-                logger.info('Custom trainer config (difference from default):')
-                xor.pprint(indent=1)
-            else:
-                logger.info('No difference from default.')
+        args_dict = self._extract_verbosity(args_dict)
+        restructured = restructure_arguments(args_dict)
+
+        self._check_restructured(restructured, self.default_config)
+        return restructured
+
+    def _create_parser(self, default=None):
+        parser = argparse.ArgumentParser(prog='GridRL')
+        for arg_name, arg_info in self._get_arguments(d=default).items():
+            parser.add_argument(f'--{arg_name}', **arg_info)
+
+        if parser.get_default('verbose') is None:
+            parser.add_argument('--verbose', default=0, type=int)
+
+        return parser
+
+    def _create_config_file_parser(self):
+        parser = argparse.ArgumentParser(prog='GridRLConfig')
+        parser.add_argument('--config', default=[], nargs='+')
+        return parser
+
+    def update_with_configs(self, configs, updatee=None):
+        if configs is None:
+            return self
+        elif not pd.api.types.is_list_like(configs) or pd.api.types.is_dict_like(configs):
+            configs = [configs]
+
+        for config in configs:
+            updatee = self._update_with_config(config, updatee=updatee)
+
+        return updatee
 
     def _update_with_config(self, config, updatee=None):
-        if isinstance(config, str):
+        if isinstance(config, (str, Path)):
             config = _config_from_yaml(config)
 
         config = self._restructure_as_necessary(config)
 
         if updatee:
-            nested_dict_update(updatee, config)
+            return nested_dict_update(updatee, config)
         else:
-            nested_dict_update(self, config)
+            return nested_dict_update(self, config)
 
     def _restructure_as_necessary(self, config):
         if any('.' in k for k in config.keys()):
             if any(isinstance(v, dict) for v in config.values()):
                 raise ValueError('Cannot combine nested dict config arguments with "." deliminated arguments.')
 
-            config = self._restructure_arguments(config)
+            config = restructure_arguments(config)
+
+        return config
+
+    def _extract_verbosity(self, config):
+        self.verbosity = config['verbose']
+
+        try:
+            _ = self.default_config.verbose
+        except AttributeError:
+            config.pop('verbose')
 
         return config
 
+    def _check_restructured(self, restructured, default_config, *stack):
+        for key, value in default_config.items():
+            if key not in restructured:
+                raise RuntimeError(f'Missing key {"->".join([*stack, key])} in restructured config.')
+            elif isinstance(value, dict):
+                self._check_restructured(restructured[key], value, *stack, key)
+
     def _get_arguments(self, key='', d=None):
         if d is None:
             d = self.default_config
 
         args = {}
 
         for k, v in d.items():
             new_key = f'{key}.{k}' if key else k
-            if isinstance(v, (dict, UserDict)):
+            if isinstance(v, (dict, UserDict)) and len(v):
                 args.update(self._get_arguments(key=new_key, d=v))
             else:
                 args[new_key] = self._collect_argument(v)
 
         return args
 
     def _collect_argument(self, default_val):
+        if not default_val and not isinstance(default_val, (float, int, bool)):
+            _type = str
+        else:
+            _type = type(default_val)
+
         arg = {
             'default': default_val,
-            'type': type(default_val),
+            'type': _type,
         }
         if hasattr(default_val, '__len__') and not isinstance(default_val, str):
             arg["nargs"] = '+'
 
         return arg
 
-    def _parse_config(self):
-        parsed_args = self._create_parser().parse_known_args()
-
-        if len(parsed_args[1]):
-            bad_args = [x.replace("--", "") for x in parsed_args[1] if x.startswith("--")]
-            valid_args = "\n\t\t".join(sorted(parsed_args[0].__dict__.keys()))
-            warn(f'Unrecognized arguments {bad_args}.\n\tValid arguments:\n\t\t{valid_args}')
-
-        config_files = parsed_args[0].__dict__.pop('config')
-        restructured = self._restructure_arguments(parsed_args[0].__dict__)
-
-        if config_files is not None:
-            for config_file in config_files:
-                self._update_with_config(config_file, updatee=restructured)
-
-        self._check_restructured(restructured, self.default_config)
-        return restructured
-
-    def _create_parser(self):
-        parser = argparse.ArgumentParser(prog='GridRL')
-        for arg_name, arg_info in self._get_arguments().items():
-            parser.add_argument(f'--{arg_name}', **arg_info)
+    def serialize_to_dir(self, log_dir, fname='config.yaml', use_existing_dir=False, with_default=False):
+        log_dir = super().serialize_to_dir(log_dir, fname=fname, use_existing_dir=use_existing_dir)
 
-        parser.add_argument('--config', default=None, nargs='+')
+        if with_default:
+            path = Path(fname)
 
-        return parser
+            def fname_func(kind): return (path.parent / f'{path.stem}_{kind}').with_suffix(path.suffix)
 
-    def _restructure_arguments(self, config):
-        if isinstance(config, dict):
-            keys = [key.split('.') for key in config.keys()]
-            keys_series = pd.Series(index=pd.MultiIndex.from_frame(pd.DataFrame(keys)), data=config.values())
-        else:
-            keys_series = config
+            self.default_config.serialize_to_dir(log_dir,
+                                                 fname=fname_func('default'),
+                                                 use_existing_dir=True)
 
-        restructured = {}
+            (self ^ self.default_config).serialize_to_dir(log_dir,
+                                                          fname=fname_func('difference'),
+                                                          use_existing_dir=True)
+        return log_dir
 
-        for key in keys_series.index.get_level_values(0).unique():
-            subset = keys_series[key]
-            if subset.index.dropna('all').empty:
-                restructured.update({key: subset.item()})
-            elif subset.index.dropna().nlevels == 1:
-                restructured.update({key: subset.to_dict()})
+    def verbose(self, level):
+        if level >= 2:
+            self.logger.info('Trainer config:')
+            self.pprint(indent=1, log_func=self.logger.info)
+        if level >= 1:
+            xor = self ^ self.default_config
+            print(f'\n{"-"*10}\n')
+            if xor:
+                self.logger.info('Custom trainer config (difference from default):')
+                xor.pprint(indent=1, log_func=self.logger.info)
             else:
-                restructured.update({key: self._restructure_arguments(subset)})
-
-        return restructured
-
-    def _check_restructured(self, restructured, default_config, *stack):
-        for key, value in default_config.items():
-            if key not in restructured:
-                raise RuntimeError(f'Missing key {"->".join([*stack, key])} in restructured config.')
-            elif isinstance(value, dict):
-                self._check_restructured(restructured[key], value, *stack, key)
+                self.logger.info('No difference from default.')
 
 
 class DefaultConfig(Namespacify):
     def __init__(self, file_path):
         super().__init__(_config_from_yaml(file_path))
 
 
 def _config_from_yaml(file_path):
-    contents = Path(file_path).open('r')
+    contents = Path(file_path).expanduser().open('r')
     loaded_contents = yaml.safe_load(contents)
 
     if not isinstance(loaded_contents, dict):
         raise ValueError(f'Contents of file "{file_path}" deserialize into object of type '
                          f'{type(loaded_contents).__name__}, should be dict.')
 
     return loaded_contents
+
+
+def restructure_arguments(arguments):
+    if set(arguments.keys()) == {''}:
+        return arguments['']
+
+    restructured = {}
+    for key, value in arguments.items():
+        top_key, _, bottom_keys = key.partition('.')
+        update_with = {top_key: restructure_arguments({bottom_keys: value})}
+        nested_dict_update(restructured, update_with)
+
+    return restructured
```

### Comparing `experiment-config-0.1/src/expfig/logger/log_dir.py` & `experiment-config-0.2/src/expfig/logging/log_dir.py`

 * *Files identical despite different names*

