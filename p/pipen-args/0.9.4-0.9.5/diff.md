# Comparing `tmp/pipen_args-0.9.4.tar.gz` & `tmp/pipen_args-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipen_args-0.9.4.tar", max compression
+gzip compressed data, was "pipen_args-0.9.5.tar", max compression
```

## Comparing `pipen_args-0.9.4.tar` & `pipen_args-0.9.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2173 2023-04-16 23:41:11.568259 pipen_args-0.9.4/README.md
--rw-r--r--   0        0        0      969 2023-04-16 23:41:11.568259 pipen_args-0.9.4/pipen_args/__init__.py
--rw-r--r--   0        0        0     3872 2023-04-16 23:41:11.568259 pipen_args-0.9.4/pipen_args/defaults.py
--rw-r--r--   0        0        0     9934 2023-04-16 23:41:11.568259 pipen_args-0.9.4/pipen_args/parser_.py
--rw-r--r--   0        0        0     5505 2023-04-16 23:41:11.568259 pipen_args-0.9.4/pipen_args/plugin.py
--rw-r--r--   0        0        0     3277 2023-04-16 23:41:11.572259 pipen_args-0.9.4/pipen_args/procgroup.py
--rw-r--r--   0        0        0       22 2023-04-16 23:41:11.572259 pipen_args-0.9.4/pipen_args/version.py
--rw-r--r--   0        0        0     1185 2023-04-16 23:41:11.572259 pipen_args-0.9.4/pyproject.toml
--rw-r--r--   0        0        0     3016 1970-01-01 00:00:00.000000 pipen_args-0.9.4/setup.py
--rw-r--r--   0        0        0     2864 1970-01-01 00:00:00.000000 pipen_args-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0     2173 2023-04-17 06:58:36.561008 pipen_args-0.9.5/README.md
+-rw-r--r--   0        0        0      969 2023-04-17 06:58:36.561008 pipen_args-0.9.5/pipen_args/__init__.py
+-rw-r--r--   0        0        0     3872 2023-04-17 06:58:36.561008 pipen_args-0.9.5/pipen_args/defaults.py
+-rw-r--r--   0        0        0     9934 2023-04-17 06:58:36.561008 pipen_args-0.9.5/pipen_args/parser_.py
+-rw-r--r--   0        0        0     7971 2023-04-17 06:58:36.561008 pipen_args-0.9.5/pipen_args/plugin.py
+-rw-r--r--   0        0        0     3277 2023-04-17 06:58:36.561008 pipen_args-0.9.5/pipen_args/procgroup.py
+-rw-r--r--   0        0        0       22 2023-04-17 06:58:36.561008 pipen_args-0.9.5/pipen_args/version.py
+-rw-r--r--   0        0        0     1185 2023-04-17 06:58:36.561008 pipen_args-0.9.5/pyproject.toml
+-rw-r--r--   0        0        0     3016 1970-01-01 00:00:00.000000 pipen_args-0.9.5/setup.py
+-rw-r--r--   0        0        0     2864 1970-01-01 00:00:00.000000 pipen_args-0.9.5/PKG-INFO
```

### Comparing `pipen_args-0.9.4/README.md` & `pipen_args-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `pipen_args-0.9.4/pipen_args/__init__.py` & `pipen_args-0.9.5/pipen_args/__init__.py`

 * *Files identical despite different names*

### Comparing `pipen_args-0.9.4/pipen_args/defaults.py` & `pipen_args-0.9.5/pipen_args/defaults.py`

 * *Files identical despite different names*

### Comparing `pipen_args-0.9.4/pipen_args/parser_.py` & `pipen_args-0.9.5/pipen_args/parser_.py`

 * *Files identical despite different names*

### Comparing `pipen_args-0.9.4/pipen_args/procgroup.py` & `pipen_args-0.9.5/pipen_args/procgroup.py`

 * *Files identical despite different names*

### Comparing `pipen_args-0.9.4/pyproject.toml` & `pipen_args-0.9.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pipen-args"
-version = "0.9.4"
+version = "0.9.5"
 description = "Command-line argument parser for pipen."
 authors = ["pwwang <pwwang@pwwang.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/pwwang/pipen-args"
 repository = "https://github.com/pwwang/pipen-args"
```

### Comparing `pipen_args-0.9.4/setup.py` & `pipen_args-0.9.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['pipen-annotate>=0.7.1,<0.8.0']
 
 entry_points = \
 {'pipen': ['args = pipen_args.plugin:ArgsPlugin']}
 
 setup_kwargs = {
     'name': 'pipen-args',
-    'version': '0.9.4',
+    'version': '0.9.5',
     'description': 'Command-line argument parser for pipen.',
     'long_description': '# pipen-args\n\nCommand line argument parser for [pipen][1]\n\n## Usage\n\n```python\nfrom pipen import Proc, Pipen\n\n\nclass Process(Proc):\n    """My process\n\n    Input:\n        a: Input data\n    """\n    input = \'a\'\n    input_data = range(10)\n    script = \'echo {{in.a}}\'\n\nPipen().set_start(Process).run()\n```\n\n```shell\n$ python example.py --help\nUsage: test.py [-h | -h+] [options]\n\nUndescribed process.\nUse `@configfile` to load default values for the options.\n\nPipeline Options:\n  --name NAME           The name for the pipeline, will affect the default workdir and\n                        outdir. [default: pipen-0]\n  --profile PROFILE     The default profile from the configuration to run the pipeline.\n                        This profile will be used unless a profile is specified in the\n                        process or in the .run method of pipen. You can check the\n                        available profiles by running `pipen profile`\n  --outdir OUTDIR       The output directory of the pipeline [default: ./<name>_results]\n  --forks FORKS         How many jobs to run simultaneously by the scheduler\n  --scheduler SCHEDULER\n                        The scheduler to run the jobs\n\nNamespace <in>:\n  --in.a A [A ...]      Input data\n\nOptional Arguments:\n  -h, --help, -h+, --help+\n                        show help message (with + to show more options) and exit\n```\n\nSee more examples in `tests/pipelines/` folder.\n\n## Metadata for Proc envs items\n\nThe metadata in the docstring of env items determines how the arguments are defined.\n\n```python\nclass Process(Proc):\n    """My process\n\n    # other docstring sections\n\n    Envs:\n        a (<metadata>): ...\n    """\n```\n\nThe metadata could be key-value pairs separated by `;`. The separator `:` or `=` is used to\nseparate the key and value. The value is optional. If the value is not specified, it\nwill be set to `True`. The keys are valid arguments of `argx.ArgumentParser.add_argument`, except that `hidden` will be interpreted as `show=False` in `argx.ArgumentParser.add_argument`. If the value of `choices` is not specified, the subkeys of the env item will be used as the choices.\n\n[1]: https://github.com/pwwang/pipen\n',
     'author': 'pwwang',
     'author_email': 'pwwang@pwwang.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/pwwang/pipen-args',
```

### Comparing `pipen_args-0.9.4/PKG-INFO` & `pipen_args-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipen-args
-Version: 0.9.4
+Version: 0.9.5
 Summary: Command-line argument parser for pipen.
 Home-page: https://github.com/pwwang/pipen-args
 License: MIT
 Author: pwwang
 Author-email: pwwang@pwwang.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

