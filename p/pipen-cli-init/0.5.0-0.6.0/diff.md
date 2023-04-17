# Comparing `tmp/pipen_cli_init-0.5.0.tar.gz` & `tmp/pipen_cli_init-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipen_cli_init-0.5.0.tar", max compression
+gzip compressed data, was "pipen_cli_init-0.6.0.tar", max compression
```

## Comparing `pipen_cli_init-0.5.0.tar` & `pipen_cli_init-0.6.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1187 2023-03-30 05:35:13.086747 pipen_cli_init-0.5.0/pipen_cli_init/__init__.py
--rw-r--r--   0        0        0       99 2023-03-30 05:35:13.086747 pipen_cli_init-0.5.0/pipen_cli_init/template/.copier-answers.yml.jinja
--rw-r--r--   0        0        0      215 2023-03-30 05:35:13.086747 pipen_cli_init-0.5.0/pipen_cli_init/template/README.md.jinja
--rw-r--r--   0        0        0      810 2023-03-30 05:35:13.086747 pipen_cli_init-0.5.0/pipen_cli_init/template/copier.yml
--rw-r--r--   0        0        0      688 2023-03-30 05:35:13.086747 pipen_cli_init-0.5.0/pipen_cli_init/template/pyproject.toml.jinja
--rw-r--r--   0        0        0        0 2023-03-30 05:35:13.086747 pipen_cli_init-0.5.0/pipen_cli_init/template/{{pipeline_name}}/__init__.py
--rw-r--r--   0        0        0       62 2023-03-30 05:35:13.086747 pipen_cli_init-0.5.0/pipen_cli_init/template/{{pipeline_name}}/__main__.py
--rw-r--r--   0        0        0      258 2023-03-30 05:35:13.086747 pipen_cli_init-0.5.0/pipen_cli_init/template/{{pipeline_name}}/main.py.jinja
--rw-r--r--   0        0        0      480 2023-03-30 05:35:13.086747 pipen_cli_init-0.5.0/pipen_cli_init/template/{{pipeline_name}}/processes.py.jinja
--rw-r--r--   0        0        0       84 2023-03-30 05:35:13.086747 pipen_cli_init-0.5.0/pipen_cli_init/template/{{pipeline_name}}/scripts/ExampleProcess.sh
--rw-r--r--   0        0        0      197 2023-03-30 05:35:13.086747 pipen_cli_init-0.5.0/pipen_cli_init/template/{{pipeline_name}}/{% if report %}reports{% endif %}/ExampleProcess.svelte
--rw-r--r--   0        0        0      642 2023-03-30 05:35:13.086747 pipen_cli_init-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1054 1970-01-01 00:00:00.000000 pipen_cli_init-0.5.0/setup.py
--rw-r--r--   0        0        0      581 1970-01-01 00:00:00.000000 pipen_cli_init-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1187 2023-04-17 07:13:33.658275 pipen_cli_init-0.6.0/pipen_cli_init/__init__.py
+-rw-r--r--   0        0        0       99 2023-04-17 07:13:33.658275 pipen_cli_init-0.6.0/pipen_cli_init/template/.copier-answers.yml.jinja
+-rw-r--r--   0        0        0      215 2023-04-17 07:13:33.658275 pipen_cli_init-0.6.0/pipen_cli_init/template/README.md.jinja
+-rw-r--r--   0        0        0      810 2023-04-17 07:13:33.658275 pipen_cli_init-0.6.0/pipen_cli_init/template/copier.yml
+-rw-r--r--   0        0        0      680 2023-04-17 07:13:33.658275 pipen_cli_init-0.6.0/pipen_cli_init/template/pyproject.toml.jinja
+-rw-r--r--   0        0        0        0 2023-04-17 07:13:33.658275 pipen_cli_init-0.6.0/pipen_cli_init/template/{{pipeline_name}}/__init__.py
+-rw-r--r--   0        0        0       62 2023-04-17 07:13:33.658275 pipen_cli_init-0.6.0/pipen_cli_init/template/{{pipeline_name}}/__main__.py
+-rw-r--r--   0        0        0      258 2023-04-17 07:13:33.658275 pipen_cli_init-0.6.0/pipen_cli_init/template/{{pipeline_name}}/main.py.jinja
+-rw-r--r--   0        0        0      480 2023-04-17 07:13:33.658275 pipen_cli_init-0.6.0/pipen_cli_init/template/{{pipeline_name}}/processes.py.jinja
+-rw-r--r--   0        0        0       84 2023-04-17 07:13:33.658275 pipen_cli_init-0.6.0/pipen_cli_init/template/{{pipeline_name}}/scripts/ExampleProcess.sh
+-rw-r--r--   0        0        0      197 2023-04-17 07:13:33.658275 pipen_cli_init-0.6.0/pipen_cli_init/template/{{pipeline_name}}/{% if report %}reports{% endif %}/ExampleProcess.svelte
+-rw-r--r--   0        0        0      641 2023-04-17 07:13:33.658275 pipen_cli_init-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1051 1970-01-01 00:00:00.000000 pipen_cli_init-0.6.0/setup.py
+-rw-r--r--   0        0        0      578 1970-01-01 00:00:00.000000 pipen_cli_init-0.6.0/PKG-INFO
```

### Comparing `pipen_cli_init-0.5.0/pipen_cli_init/__init__.py` & `pipen_cli_init-0.6.0/pipen_cli_init/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 from pathlib import Path
 from pipen.cli._hooks import CLIPlugin
 from copier import run_auto
 
-__version__ = "0.5.0"
+__version__ = "0.6.0"
 
 if TYPE_CHECKING:
     from argx import ArgumentParser, Namespace
 
 TEMPLATE_PATH = Path(__file__).parent.joinpath("template")
```

### Comparing `pipen_cli_init-0.5.0/pipen_cli_init/template/copier.yml` & `pipen_cli_init-0.6.0/pipen_cli_init/template/copier.yml`

 * *Files identical despite different names*

### Comparing `pipen_cli_init-0.5.0/pipen_cli_init/template/pyproject.toml.jinja` & `pipen_cli_init-0.6.0/pipen_cli_init/template/pyproject.toml.jinja`

 * *Files 4% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 version = "0.0.1"
 description = "{{pipeline_desc}}"
 authors = ["{{author}} <{{author_email}}>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
-python = "^3.7.1"
-pipen = "^0.7"
-pipen-filters = "^0.6"
-pipen-verbose = "^0.5"
-pipen-args = "^0.8"
+python = "^3.8"
+pipen = "^0.9"
+pipen-filters = "^0.7"
+pipen-verbose = "^0.6"
+pipen-args = "^0.9.5"
 {% if report -%}
-pipen-report = "^0.8"
+pipen-report = "^0.9"
 {%- endif %}
 
 [tool.poetry.dev-dependencies]
 
 {% if console_script %}
 [tool.poetry.scripts]
 {{pipeline_name}} = "{{pipeline_name}}.main:main"
@@ -25,9 +25,9 @@
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 80
-target-version = ['py37', 'py38', 'py39', 'py310']
+target-version = ['py38', 'py39', 'py310']
 include = '\.pyi?$'
```

### Comparing `pipen_cli_init-0.5.0/pyproject.toml` & `pipen_cli_init-0.6.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "pipen-cli-init"
-version = "0.5.0"
+version = "0.6.0"
 description = "A pipen cli plugin to create a pipen project (pipeline)"
 authors = ["pwwang <pwwang@pwwang.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
-python = "^3.7.1"
-pipen = "^0.7"
+python = "^3.8"
+pipen = "^0.9"
 copier = "^7"
 
 [tool.poetry.build]
 generate-setup-file = true
 
 [tool.poetry.dev-dependencies]
 
@@ -23,9 +23,9 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
 ignore_missing_imports = true
 
 [tool.black]
 line-length = 80
-target-version = ['py37', 'py38', 'py39']
+target-version = ['py38', 'py39', 'py310']
 include = '\.pyi?$'
```

### Comparing `pipen_cli_init-0.5.0/setup.py` & `pipen_cli_init-0.6.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,31 +8,31 @@
 {'': ['*'],
  'pipen_cli_init': ['template/*'],
  'pipen_cli_init.template.{{pipeline_name}}': ['scripts/*',
                                                '{% if report %}reports{% endif '
                                                '%}/*']}
 
 install_requires = \
-['copier>=7,<8', 'pipen>=0.7,<0.8']
+['copier>=7,<8', 'pipen>=0.9,<0.10']
 
 entry_points = \
 {'pipen_cli': ['cli-init = pipen_cli_init:PipenCliInit']}
 
 setup_kwargs = {
     'name': 'pipen-cli-init',
-    'version': '0.5.0',
+    'version': '0.6.0',
     'description': 'A pipen cli plugin to create a pipen project (pipeline)',
     'long_description': 'None',
     'author': 'pwwang',
     'author_email': 'pwwang@pwwang.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.7.1,<4.0.0',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `pipen_cli_init-0.5.0/PKG-INFO` & `pipen_cli_init-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pipen-cli-init
-Version: 0.5.0
+Version: 0.6.0
 Summary: A pipen cli plugin to create a pipen project (pipeline)
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
 Requires-Dist: copier (>=7,<8)
-Requires-Dist: pipen (>=0.7,<0.8)
+Requires-Dist: pipen (>=0.9,<0.10)
```

