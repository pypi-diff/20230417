# Comparing `tmp/meltanolabs_target_snowflake-0.0.2.tar.gz` & `tmp/meltanolabs_target_snowflake-0.1.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meltanolabs_target_snowflake-0.0.2.tar", max compression
+gzip compressed data, was "meltanolabs_target_snowflake-0.1.1a1.tar", max compression
```

## Comparing `meltanolabs_target_snowflake-0.0.2.tar` & `meltanolabs_target_snowflake-0.1.1a1.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     3135 2022-12-08 14:44:53.449198 meltanolabs_target_snowflake-0.0.2/README.md
--rw-r--r--   0        0        0     1087 2022-12-08 14:45:34.613598 meltanolabs_target_snowflake-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       89 2022-12-08 14:45:34.613598 meltanolabs_target_snowflake-0.0.2/target_snowflake/__init__.py
--rw-r--r--   0        0        0    15082 2022-12-08 14:44:53.449198 meltanolabs_target_snowflake-0.0.2/target_snowflake/sinks.py
--rw-r--r--   0        0        0     2163 2022-12-08 14:44:53.449198 meltanolabs_target_snowflake-0.0.2/target_snowflake/target.py
--rw-r--r--   0        0        0       39 2022-12-08 14:44:53.449198 meltanolabs_target_snowflake-0.0.2/target_snowflake/tests/__init__.py
--rw-r--r--   0        0        0      656 2022-12-08 14:44:53.449198 meltanolabs_target_snowflake-0.0.2/target_snowflake/tests/test_core.py
--rw-r--r--   0        0        0     4208 1970-01-01 00:00:00.000000 meltanolabs_target_snowflake-0.0.2/setup.py
--rw-r--r--   0        0        0     3839 1970-01-01 00:00:00.000000 meltanolabs_target_snowflake-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     3135 2023-04-17 21:16:34.330190 meltanolabs_target_snowflake-0.1.1a1/README.md
+-rw-r--r--   0        0        0     1091 2023-04-17 21:17:03.655981 meltanolabs_target_snowflake-0.1.1a1/pyproject.toml
+-rw-r--r--   0        0        0       93 2023-04-17 21:17:03.655981 meltanolabs_target_snowflake-0.1.1a1/target_snowflake/__init__.py
+-rw-r--r--   0        0        0    15115 2023-04-17 21:16:34.334190 meltanolabs_target_snowflake-0.1.1a1/target_snowflake/sinks.py
+-rw-r--r--   0        0        0     2163 2023-04-17 21:16:34.334190 meltanolabs_target_snowflake-0.1.1a1/target_snowflake/target.py
+-rw-r--r--   0        0        0       39 2023-04-17 21:16:34.334190 meltanolabs_target_snowflake-0.1.1a1/target_snowflake/tests/__init__.py
+-rw-r--r--   0        0        0      656 2023-04-17 21:16:34.334190 meltanolabs_target_snowflake-0.1.1a1/target_snowflake/tests/test_core.py
+-rw-r--r--   0        0        0     3833 1970-01-01 00:00:00.000000 meltanolabs_target_snowflake-0.1.1a1/PKG-INFO
```

### Comparing `meltanolabs_target_snowflake-0.0.2/README.md` & `meltanolabs_target_snowflake-0.1.1a1/README.md`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_snowflake-0.0.2/pyproject.toml` & `meltanolabs_target_snowflake-0.1.1a1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "meltanolabs-target-snowflake"
-version = "0.0.2"
+version = "0.1.1-a.1"
 description = "`target-snowflake` is a Singer target for Snowflake, built with the Meltano SDK for Singer Targets."
 readme = "README.md"
 authors = ["Ken Payne"]
 keywords = [
     "ELT",
     "Snowflake",
 ]
@@ -12,15 +12,15 @@
 packages = [
     { include = "target_snowflake" }
 ]
 
 [tool.poetry.dependencies]
 python = "<3.11,>=3.7.1"
 requests = "^2.25.1"
-singer-sdk = "^0.13.0"
+singer-sdk = "0.17.0"
 snowflake-sqlalchemy = "^1.4.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.5"
 tox = "^3.24.4"
 flake8 = "^3.9.2"
 black = "^21.9b0"
@@ -41,8 +41,8 @@
 [tool.poetry.scripts]
 # CLI declaration
 target-snowflake = 'target_snowflake.target:TargetSnowflake.cli'
 
 [tool.poetry-dynamic-versioning]
 enable = true
 vcs = "git"
-style = "semver"
+style = "semver"
```

### Comparing `meltanolabs_target_snowflake-0.0.2/target_snowflake/sinks.py` & `meltanolabs_target_snowflake-0.1.1a1/target_snowflake/sinks.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,18 @@
 from typing import Any, Dict, Iterable, Mapping, Optional, Sequence, Tuple, cast
 from urllib.parse import urlparse
 from uuid import uuid4
 
 import snowflake.sqlalchemy.custom_types as sct
 import sqlalchemy
 from singer_sdk import typing as th
+from singer_sdk.connectors import SQLConnector
 from singer_sdk.helpers._batch import BaseBatchFileEncoding, BatchConfig
 from singer_sdk.helpers._typing import conform_record_data_types
-from singer_sdk.sinks import SQLConnector, SQLSink
+from singer_sdk.sinks import SQLSink
 from singer_sdk.streams.core import lazy_chunked_generator
 from snowflake.sqlalchemy import URL
 from sqlalchemy.sql import text
 
 
 class TypeMap:
     def __init__(self, operator, map_value, match_value=None):
```

### Comparing `meltanolabs_target_snowflake-0.0.2/target_snowflake/target.py` & `meltanolabs_target_snowflake-0.1.1a1/target_snowflake/target.py`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_snowflake-0.0.2/target_snowflake/tests/test_core.py` & `meltanolabs_target_snowflake-0.1.1a1/target_snowflake/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_snowflake-0.0.2/setup.py` & `meltanolabs_target_snowflake-0.1.1a1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,126 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: meltanolabs-target-snowflake
+Version: 0.1.1a1
+Summary: `target-snowflake` is a Singer target for Snowflake, built with the Meltano SDK for Singer Targets.
+License: Apache 2.0
+Keywords: ELT,Snowflake
+Author: Ken Payne
+Requires-Python: >=3.7.1,<3.11
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Dist: requests (>=2.25.1,<3.0.0)
+Requires-Dist: singer-sdk (==0.17.0)
+Requires-Dist: snowflake-sqlalchemy (>=1.4.1,<2.0.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['target_snowflake', 'target_snowflake.tests']
+# target-snowflake
 
-package_data = \
-{'': ['*']}
+`target-snowflake` is a Singer target for Snowflake.
 
-install_requires = \
-['requests>=2.25.1,<3.0.0',
- 'singer-sdk>=0.13.0,<0.14.0',
- 'snowflake-sqlalchemy>=1.4.1,<2.0.0']
-
-entry_points = \
-{'console_scripts': ['target-snowflake = '
-                     'target_snowflake.target:TargetSnowflake.cli']}
-
-setup_kwargs = {
-    'name': 'meltanolabs-target-snowflake',
-    'version': '0.0.2',
-    'description': '`target-snowflake` is a Singer target for Snowflake, built with the Meltano SDK for Singer Targets.',
-    'long_description': '# target-snowflake\n\n`target-snowflake` is a Singer target for Snowflake.\n\nBuild with the [Meltano Target SDK](https://sdk.meltano.com).\n\n## Installation\n\n- [ ] `Developer TODO:` Update the below as needed to correctly describe the install procedure. For instance, if you do not have a PyPi repo, or if you want users to directly install from your git repo, you can modify this step as appropriate.\n\n```bash\npipx install target-snowflake\n```\n\n## Configuration\n\n### Accepted Config Options\n\n- [ ] `Developer TODO:` Provide a list of config options accepted by the target.\n\nA full list of supported settings and capabilities for this\ntarget is available by running:\n\n```bash\ntarget-snowflake --about\n```\n\n### Configure using environment variables\n\nThis Singer target will automatically import any environment variables within the working directory\'s\n`.env` if the `--config=ENV` is provided, such that config values will be considered if a matching\nenvironment variable is set either in the terminal context or in the `.env` file.\n\n### Source Authentication and Authorization\n\n- [ ] `Developer TODO:` If your target requires special access on the source system, or any special authentication requirements, provide those here.\n\n## Usage\n\nYou can easily run `target-snowflake` by itself or in a pipeline using [Meltano](https://meltano.com/).\n\n### Executing the Target Directly\n\n```bash\ntarget-snowflake --version\ntarget-snowflake --help\n# Test using the "Carbon Intensity" sample:\ntap-carbon-intensity | target-snowflake --config /path/to/target-snowflake-config.json\n```\n\n## Developer Resources\n\n- [ ] `Developer TODO:` As a first step, scan the entire project for the text "`TODO:`" and complete any recommended steps, deleting the "TODO" references once completed.\n\n### Initialize your Development Environment\n\n```bash\npipx install poetry\npoetry install\n```\n\n### Create and Run Tests\n\nCreate tests within the `target_snowflake/tests` subfolder and\n  then run:\n\n```bash\npoetry run pytest\n```\n\nYou can also test the `target-snowflake` CLI interface directly using `poetry run`:\n\n```bash\npoetry run target-snowflake --help\n```\n\n### Testing with [Meltano](https://meltano.com/)\n\n_**Note:** This target will work in any Singer environment and does not require Meltano.\nExamples here are for convenience and to streamline end-to-end orchestration scenarios._\n\nYour project comes with a custom `meltano.yml` project file already created. Open the `meltano.yml` and follow any _"TODO"_ items listed in\nthe file.\n\nNext, install Meltano (if you haven\'t already) and any needed plugins:\n\n```bash\n# Install meltano\npipx install meltano\n# Initialize meltano within this directory\ncd target-snowflake\nmeltano install\n```\n\nNow you can test and orchestrate using Meltano:\n\n```bash\n# Test invocation:\nmeltano invoke target-snowflake --version\n# OR run a test `elt` pipeline with the Carbon Intensity sample tap:\nmeltano elt tap-carbon-intensity target-snowflake\n```\n\n### SDK Dev Guide\n\nSee the [dev guide](https://sdk.meltano.com/en/latest/dev_guide.html) for more instructions on how to use the Meltano SDK to\ndevelop your own Singer taps and targets.\n',
-    'author': 'Ken Payne',
-    'author_email': 'None',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7.1,<3.11',
-}
+Build with the [Meltano Target SDK](https://sdk.meltano.com).
 
+## Installation
+
+- [ ] `Developer TODO:` Update the below as needed to correctly describe the install procedure. For instance, if you do not have a PyPi repo, or if you want users to directly install from your git repo, you can modify this step as appropriate.
+
+```bash
+pipx install target-snowflake
+```
+
+## Configuration
+
+### Accepted Config Options
+
+- [ ] `Developer TODO:` Provide a list of config options accepted by the target.
+
+A full list of supported settings and capabilities for this
+target is available by running:
+
+```bash
+target-snowflake --about
+```
+
+### Configure using environment variables
+
+This Singer target will automatically import any environment variables within the working directory's
+`.env` if the `--config=ENV` is provided, such that config values will be considered if a matching
+environment variable is set either in the terminal context or in the `.env` file.
+
+### Source Authentication and Authorization
+
+- [ ] `Developer TODO:` If your target requires special access on the source system, or any special authentication requirements, provide those here.
+
+## Usage
+
+You can easily run `target-snowflake` by itself or in a pipeline using [Meltano](https://meltano.com/).
+
+### Executing the Target Directly
+
+```bash
+target-snowflake --version
+target-snowflake --help
+# Test using the "Carbon Intensity" sample:
+tap-carbon-intensity | target-snowflake --config /path/to/target-snowflake-config.json
+```
+
+## Developer Resources
+
+- [ ] `Developer TODO:` As a first step, scan the entire project for the text "`TODO:`" and complete any recommended steps, deleting the "TODO" references once completed.
+
+### Initialize your Development Environment
+
+```bash
+pipx install poetry
+poetry install
+```
+
+### Create and Run Tests
+
+Create tests within the `target_snowflake/tests` subfolder and
+  then run:
+
+```bash
+poetry run pytest
+```
+
+You can also test the `target-snowflake` CLI interface directly using `poetry run`:
+
+```bash
+poetry run target-snowflake --help
+```
+
+### Testing with [Meltano](https://meltano.com/)
+
+_**Note:** This target will work in any Singer environment and does not require Meltano.
+Examples here are for convenience and to streamline end-to-end orchestration scenarios._
+
+Your project comes with a custom `meltano.yml` project file already created. Open the `meltano.yml` and follow any _"TODO"_ items listed in
+the file.
+
+Next, install Meltano (if you haven't already) and any needed plugins:
+
+```bash
+# Install meltano
+pipx install meltano
+# Initialize meltano within this directory
+cd target-snowflake
+meltano install
+```
+
+Now you can test and orchestrate using Meltano:
+
+```bash
+# Test invocation:
+meltano invoke target-snowflake --version
+# OR run a test `elt` pipeline with the Carbon Intensity sample tap:
+meltano elt tap-carbon-intensity target-snowflake
+```
+
+### SDK Dev Guide
+
+See the [dev guide](https://sdk.meltano.com/en/latest/dev_guide.html) for more instructions on how to use the Meltano SDK to
+develop your own Singer taps and targets.
 
-setup(**setup_kwargs)
```

