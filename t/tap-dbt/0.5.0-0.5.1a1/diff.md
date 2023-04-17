# Comparing `tmp/tap_dbt-0.5.0.tar.gz` & `tmp/tap_dbt-0.5.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_dbt-0.5.0.tar", max compression
+gzip compressed data, was "tap_dbt-0.5.1a1.tar", max compression
```

## Comparing `tap_dbt-0.5.0.tar` & `tap_dbt-0.5.1a1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11357 2023-04-15 00:25:27.799289 tap_dbt-0.5.0/LICENSE
--rw-r--r--   0        0        0     5269 2023-04-15 00:25:27.799289 tap_dbt-0.5.0/README.md
--rw-r--r--   0        0        0     1148 2023-04-15 00:25:27.799289 tap_dbt-0.5.0/pyproject.toml
--rw-r--r--   0        0        0       40 2023-04-15 00:25:27.799289 tap_dbt-0.5.0/tap_dbt/__init__.py
--rw-r--r--   0        0        0     2360 2023-04-15 00:25:27.799289 tap_dbt-0.5.0/tap_dbt/client.py
--rw-r--r--   0        0        0     1780 2023-04-15 00:25:27.799289 tap_dbt-0.5.0/tap_dbt/schemas/accounts.json
--rw-r--r--   0        0        0     2264 2023-04-15 00:25:27.803289 tap_dbt-0.5.0/tap_dbt/schemas/jobs.json
--rw-r--r--   0        0        0     1821 2023-04-15 00:25:27.803289 tap_dbt-0.5.0/tap_dbt/schemas/projects.json
--rw-r--r--   0        0        0     3368 2023-04-15 00:25:27.803289 tap_dbt-0.5.0/tap_dbt/schemas/runs.json
--rw-r--r--   0        0        0     3538 2023-04-15 00:25:27.803289 tap_dbt-0.5.0/tap_dbt/streams.py
--rw-r--r--   0        0        0     2033 2023-04-15 00:25:27.803289 tap_dbt-0.5.0/tap_dbt/tap.py
--rw-r--r--   0        0        0     6163 1970-01-01 00:00:00.000000 tap_dbt-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-17 19:55:15.889690 tap_dbt-0.5.1a1/LICENSE
+-rw-r--r--   0        0        0     4899 2023-04-17 19:55:15.889690 tap_dbt-0.5.1a1/README.md
+-rw-r--r--   0        0        0     1615 2023-04-17 19:55:31.785910 tap_dbt-0.5.1a1/pyproject.toml
+-rw-r--r--   0        0        0       40 2023-04-17 19:55:15.889690 tap_dbt-0.5.1a1/tap_dbt/__init__.py
+-rw-r--r--   0        0        0     2360 2023-04-17 19:55:15.889690 tap_dbt-0.5.1a1/tap_dbt/client.py
+-rw-r--r--   0        0        0     1780 2023-04-17 19:55:15.889690 tap_dbt-0.5.1a1/tap_dbt/schemas/accounts.json
+-rw-r--r--   0        0        0     2264 2023-04-17 19:55:15.889690 tap_dbt-0.5.1a1/tap_dbt/schemas/jobs.json
+-rw-r--r--   0        0        0     1821 2023-04-17 19:55:15.889690 tap_dbt-0.5.1a1/tap_dbt/schemas/projects.json
+-rw-r--r--   0        0        0     3368 2023-04-17 19:55:15.889690 tap_dbt-0.5.1a1/tap_dbt/schemas/runs.json
+-rw-r--r--   0        0        0     3538 2023-04-17 19:55:15.889690 tap_dbt-0.5.1a1/tap_dbt/streams.py
+-rw-r--r--   0        0        0     2033 2023-04-17 19:55:15.889690 tap_dbt-0.5.1a1/tap_dbt/tap.py
+-rw-r--r--   0        0        0     5795 1970-01-01 00:00:00.000000 tap_dbt-0.5.1a1/PKG-INFO
```

### Comparing `tap_dbt-0.5.0/LICENSE` & `tap_dbt-0.5.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `tap_dbt-0.5.0/README.md` & `tap_dbt-0.5.1a1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 # tap-dbt
 
 [![PyPI](https://img.shields.io/pypi/v/tap-dbt.svg?color=blue)](https://pypi.org/project/tap-dbt/)
 [![Python versions](https://img.shields.io/pypi/pyversions/tap-dbt.svg)](https://pypi.org/project/tap-dbt/)
 [![Singer](https://img.shields.io/badge/Singer-Tap-purple.svg)](https://hub.meltano.com/taps/dbt)
-[![Super-Linter](https://github.com/edgarrmondragon/tap-dbt/actions/workflows/superlinter.yml/badge.svg)](https://github.com/edgarrmondragon/tap-dbt/actions/workflows/superlinter.yml)
 [![TestPyPI](https://github.com/edgarrmondragon/tap-dbt/actions/workflows/test-pypi.yml/badge.svg)](https://github.com/edgarrmondragon/tap-dbt/actions/workflows/test-pypi.yml)
 [![Test Tap](https://github.com/edgarrmondragon/tap-dbt/actions/workflows/test-tap.yml/badge.svg)](https://github.com/edgarrmondragon/tap-dbt/actions/workflows/test-tap.yml)
-[![CodeQL](https://github.com/edgarrmondragon/tap-dbt/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/edgarrmondragon/tap-dbt/actions/workflows/codeql-analysis.yml)
 
 `tap-dbt` is a Singer tap for the [dbt Cloud API v2][dbtcloud].
 
 Built with the [Singer SDK][sdk].
 
 - [Installation](#Installation)
 - [Features](#Features)
```

### Comparing `tap_dbt-0.5.0/pyproject.toml` & `tap_dbt-0.5.1a1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 [tool.isort]
 profile = "black"
 multi_line_output = 3 # Vertical Hanging Indent
 src_paths = "tap_dbt"
 
 [tool.poetry]
 name = "tap-dbt"
-version = "0.5.0"
+version = "0.5.1a1"
 description = "Singer tap for dbt, built with the Singer SDK."
 license = "Apache-2.0"
 authors = ["Edgar Ramírez Mondragón <edgarrm358@sample.com>"]
 maintainers = ["Edgar Ramírez Mondragón <edgarrm358@sample.com>"]
 readme = "README.md"
 repository = "https://github.com/edgarrmondragon/tap-dbt"
 keywords = ["singer.io", "elt", "dbt", "singer-sdk"]
@@ -32,14 +32,29 @@
 faker = ">=17.6,<19.0"
 pytest = "^7.2.2"
 responses = "^0.23.1"
 
 [tool.poetry.scripts]
 tap-dbt = 'tap_dbt.tap:cli'
 
+[tool.poetry-dynamic-versioning]
+enable = false
+format-jinja = """
+    {%- if distance == 0 -%}
+        {{ serialize_pep440(base, stage, revision) }}
+    {%- elif revision is not none -%}
+        {{ serialize_pep440(base, stage, revision + 1, dev=distance, metadata=[commit]) }}
+    {%- else -%}
+        {{ serialize_pep440(bump_version(base), stage, revision, dev=distance, metadata=[commit]) }}
+    {%- endif -%}
+"""
+metadata = true
+style = "pep440"
+vcs = "git"
+
 [tool.ruff]
 ignore = ["ANN101"]
 line-length = 88
 select = ["ALL"]
 src = ["tap_dbt", "tests"]
 target-version = "py37"
```

### Comparing `tap_dbt-0.5.0/tap_dbt/client.py` & `tap_dbt-0.5.1a1/tap_dbt/client.py`

 * *Files identical despite different names*

### Comparing `tap_dbt-0.5.0/tap_dbt/schemas/accounts.json` & `tap_dbt-0.5.1a1/tap_dbt/schemas/accounts.json`

 * *Files identical despite different names*

### Comparing `tap_dbt-0.5.0/tap_dbt/schemas/jobs.json` & `tap_dbt-0.5.1a1/tap_dbt/schemas/jobs.json`

 * *Files identical despite different names*

### Comparing `tap_dbt-0.5.0/tap_dbt/schemas/projects.json` & `tap_dbt-0.5.1a1/tap_dbt/schemas/projects.json`

 * *Files identical despite different names*

### Comparing `tap_dbt-0.5.0/tap_dbt/schemas/runs.json` & `tap_dbt-0.5.1a1/tap_dbt/schemas/runs.json`

 * *Files identical despite different names*

### Comparing `tap_dbt-0.5.0/tap_dbt/streams.py` & `tap_dbt-0.5.1a1/tap_dbt/streams.py`

 * *Files identical despite different names*

### Comparing `tap_dbt-0.5.0/tap_dbt/tap.py` & `tap_dbt-0.5.1a1/tap_dbt/tap.py`

 * *Files identical despite different names*

### Comparing `tap_dbt-0.5.0/PKG-INFO` & `tap_dbt-0.5.1a1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tap-dbt
-Version: 0.5.0
+Version: 0.5.1a1
 Summary: Singer tap for dbt, built with the Singer SDK.
 Home-page: https://github.com/edgarrmondragon/tap-dbt
 License: Apache-2.0
 Keywords: singer.io,elt,dbt,singer-sdk
 Author: Edgar Ramírez Mondragón
 Author-email: edgarrm358@sample.com
 Maintainer: Edgar Ramírez Mondragón
@@ -22,18 +22,16 @@
 Description-Content-Type: text/markdown
 
 # tap-dbt
 
 [![PyPI](https://img.shields.io/pypi/v/tap-dbt.svg?color=blue)](https://pypi.org/project/tap-dbt/)
 [![Python versions](https://img.shields.io/pypi/pyversions/tap-dbt.svg)](https://pypi.org/project/tap-dbt/)
 [![Singer](https://img.shields.io/badge/Singer-Tap-purple.svg)](https://hub.meltano.com/taps/dbt)
-[![Super-Linter](https://github.com/edgarrmondragon/tap-dbt/actions/workflows/superlinter.yml/badge.svg)](https://github.com/edgarrmondragon/tap-dbt/actions/workflows/superlinter.yml)
 [![TestPyPI](https://github.com/edgarrmondragon/tap-dbt/actions/workflows/test-pypi.yml/badge.svg)](https://github.com/edgarrmondragon/tap-dbt/actions/workflows/test-pypi.yml)
 [![Test Tap](https://github.com/edgarrmondragon/tap-dbt/actions/workflows/test-tap.yml/badge.svg)](https://github.com/edgarrmondragon/tap-dbt/actions/workflows/test-tap.yml)
-[![CodeQL](https://github.com/edgarrmondragon/tap-dbt/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/edgarrmondragon/tap-dbt/actions/workflows/codeql-analysis.yml)
 
 `tap-dbt` is a Singer tap for the [dbt Cloud API v2][dbtcloud].
 
 Built with the [Singer SDK][sdk].
 
 - [Installation](#Installation)
 - [Features](#Features)
```

