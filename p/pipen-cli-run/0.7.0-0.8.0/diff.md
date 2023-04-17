# Comparing `tmp/pipen_cli_run-0.7.0.tar.gz` & `tmp/pipen_cli_run-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipen_cli_run-0.7.0.tar", max compression
+gzip compressed data, was "pipen_cli_run-0.8.0.tar", max compression
```

## Comparing `pipen_cli_run-0.7.0.tar` & `pipen_cli_run-0.8.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      312 2023-03-30 06:22:46.972778 pipen_cli_run-0.7.0/README.md
--rw-r--r--   0        0        0       83 2023-03-30 06:22:46.972778 pipen_cli_run-0.7.0/pipen_cli_run/__init__.py
--rw-r--r--   0        0        0     5737 2023-03-30 06:22:46.972778 pipen_cli_run-0.7.0/pipen_cli_run/entry.py
--rw-r--r--   0        0        0       46 2023-03-30 06:22:46.972778 pipen_cli_run-0.7.0/pipen_cli_run/version.py
--rw-r--r--   0        0        0     1334 2023-03-30 06:22:46.976778 pipen_cli_run-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     1125 1970-01-01 00:00:00.000000 pipen_cli_run-0.7.0/setup.py
--rw-r--r--   0        0        0     1018 1970-01-01 00:00:00.000000 pipen_cli_run-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      312 2023-04-17 00:01:54.857841 pipen_cli_run-0.8.0/README.md
+-rw-r--r--   0        0        0       83 2023-04-17 00:01:54.857841 pipen_cli_run-0.8.0/pipen_cli_run/__init__.py
+-rw-r--r--   0        0        0     5714 2023-04-17 00:01:54.857841 pipen_cli_run-0.8.0/pipen_cli_run/entry.py
+-rw-r--r--   0        0        0       46 2023-04-17 00:01:54.857841 pipen_cli_run-0.8.0/pipen_cli_run/version.py
+-rw-r--r--   0        0        0     1335 2023-04-17 00:01:54.857841 pipen_cli_run-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     1126 1970-01-01 00:00:00.000000 pipen_cli_run-0.8.0/setup.py
+-rw-r--r--   0        0        0     1019 1970-01-01 00:00:00.000000 pipen_cli_run-0.8.0/PKG-INFO
```

### Comparing `pipen_cli_run-0.7.0/pipen_cli_run/entry.py` & `pipen_cli_run-0.8.0/pipen_cli_run/entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,15 @@
                     help=(
                         "Arguments for the process or pipeline (Use -h/--help "
                         "to see the arguments for the process or pipeline)"
                     )
                 )
 
     def exec_command(self, args: Namespace) -> None:
-        from pipen_args import parser, install  # noqa: F401
+        from pipen_args import parser
 
         nsmod_name = args.PROC_NAMESPACE
         pname = args.PROCESS_OR_PIPELINE
         if (
             type(self.entry_points[nsmod_name]).__name__ == "EntryPoint"
         ):  # pragma: no cover
             self.entry_points[nsmod_name] = self.entry_points[nsmod_name].load()
```

### Comparing `pipen_cli_run-0.7.0/pyproject.toml` & `pipen_cli_run-0.8.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "pipen-cli-run"
-version = "0.7.0"
+version = "0.8.0"
 description = "A pipen cli plugin to run a process or a pipeline"
 authors = ["pwwang <pwwang@pwwang.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/pwwang/pipen-cli-run"
 repository = "https://github.com/pwwang/pipen-cli-run"
 
 [tool.poetry.dependencies]
-python = "^3.7.1"
-pipen-args = "^0.8"
+python = "^3.8"
+pipen-args = "^0.9.4"
 
 [tool.poetry.build]
 generate-setup-file = true
 
 [tool.poetry.dev-dependencies]
 pytest = "^7"
 pytest-cov = "^4"
@@ -26,15 +26,15 @@
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 79
-target-version = ['py37', 'py38', 'py39']
+target-version = ['py38', 'py39', 'py310']
 include = '\.pyi?$'
 
 [tool.mypy]
 ignore_missing_imports = true
 allow_redefinition = true
 disable_error_code = ["attr-defined", "no-redef"]
 show_error_codes = true
```

### Comparing `pipen_cli_run-0.7.0/setup.py` & `pipen_cli_run-0.8.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,31 +4,31 @@
 packages = \
 ['pipen_cli_run']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['pipen-args>=0.8,<0.9']
+['pipen-args>=0.9.4,<0.10.0']
 
 entry_points = \
 {'pipen_cli': ['cli-run = pipen_cli_run:PipenCliRunPlugin']}
 
 setup_kwargs = {
     'name': 'pipen-cli-run',
-    'version': '0.7.0',
+    'version': '0.8.0',
     'description': 'A pipen cli plugin to run a process or a pipeline',
     'long_description': '# pipen-cli-run\n\nA pipen cli plugin to run a process or a pipeline\n\n## Install\n\n```shell\npip install -U pipen-cli-run\n```\n\n## Usage\n\n### Register a namespace\n\n`pyproject.toml`\n```toml\n[tool.poetry.plugins.pipen_cli_run]\nns = "yourpackage.ns"\n```\n\n`ns` should be a module where you define you processes/pipelines\n',
     'author': 'pwwang',
     'author_email': 'pwwang@pwwang.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/pwwang/pipen-cli-run',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.7.1,<4.0.0',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `pipen_cli_run-0.7.0/PKG-INFO` & `pipen_cli_run-0.8.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pipen-cli-run
-Version: 0.7.0
+Version: 0.8.0
 Summary: A pipen cli plugin to run a process or a pipeline
 Home-page: https://github.com/pwwang/pipen-cli-run
 License: MIT
 Author: pwwang
 Author-email: pwwang@pwwang.com
-Requires-Python: >=3.7.1,<4.0.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pipen-args (>=0.8,<0.9)
+Requires-Dist: pipen-args (>=0.9.4,<0.10.0)
 Project-URL: Repository, https://github.com/pwwang/pipen-cli-run
 Description-Content-Type: text/markdown
 
 # pipen-cli-run
 
 A pipen cli plugin to run a process or a pipeline
```

