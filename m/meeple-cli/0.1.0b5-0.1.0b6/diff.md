# Comparing `tmp/meeple-cli-0.1.0b5.tar.gz` & `tmp/meeple-cli-0.1.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meeple-cli-0.1.0b5.tar", last modified: Mon Apr 10 18:07:10 2023, max compression
+gzip compressed data, was "meeple-cli-0.1.0b6.tar", last modified: Mon Apr 17 03:57:16 2023, max compression
```

## Comparing `meeple-cli-0.1.0b5.tar` & `meeple-cli-0.1.0b6.tar`

### file list

```diff
@@ -1,47 +1,54 @@
--rw-r--r--   0        0        0       66 2023-04-10 18:07:01.108505 meeple-cli-0.1.0b5/.flake8
--rw-r--r--   0        0        0     1146 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     1035 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/.github/workflows/python-test.yml
--rw-r--r--   0        0        0      289 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/.gitignore
--rw-r--r--   0        0        0      168 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/.markdownlint.yaml
--rw-r--r--   0        0        0     1174 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1073 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/LICENSE
--rw-r--r--   0        0        0     4293 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/README.md
--rw-r--r--   0        0        0     4834 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/docs/changelog.md
--rw-r--r--   0        0        0      876 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/justfile
--rw-r--r--   0        0        0     1014 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/pyproject.toml
--rw-r--r--   0        0        0      112 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/__init__.py
--rw-r--r--   0        0        0      639 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/command/__init__.py
--rw-r--r--   0        0        0     1498 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/command/add.py
--rw-r--r--   0        0        0     1983 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/command/collections.py
--rw-r--r--   0        0        0      941 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/command/completions.py
--rw-r--r--   0        0        0     1385 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/command/delete.py
--rw-r--r--   0        0        0     1489 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/command/drop.py
--rw-r--r--   0        0        0     4990 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/command/find.py
--rw-r--r--   0        0        0      566 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/command/hot.py
--rw-r--r--   0        0        0     1490 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/command/info.py
--rw-r--r--   0        0        0     3027 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/command/list.py
--rw-r--r--   0        0        0     2394 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/command/move.py
--rw-r--r--   0        0        0      658 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/command/new.py
--rw-r--r--   0        0        0     1182 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/command/open.py
--rw-r--r--   0        0        0     1179 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/command/rename.py
--rw-r--r--   0        0        0      848 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/command/search.py
--rw-r--r--   0        0        0     3403 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/command/stats.py
--rw-r--r--   0        0        0     2634 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/command/update.py
--rw-r--r--   0        0        0     1153 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/root.py
--rw-r--r--   0        0        0        0 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/type/__init__.py
--rw-r--r--   0        0        0      278 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/type/collection.py
--rw-r--r--   0        0        0     4385 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/type/item.py
--rw-r--r--   0        0        0        0 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/util/__init__.py
--rw-r--r--   0        0        0     1450 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/util/api_util.py
--rw-r--r--   0        0        0      697 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/util/cmd_util.py
--rw-r--r--   0        0        0     2024 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/util/collection_util.py
--rw-r--r--   0        0        0      235 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/util/completion_util.py
--rw-r--r--   0        0        0     2596 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/util/data_util.py
--rw-r--r--   0        0        0      935 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/util/filter_util.py
--rw-r--r--   0        0        0      652 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/util/fs_util.py
--rw-r--r--   0        0        0      352 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/util/input_util.py
--rw-r--r--   0        0        0     2489 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/util/output_util.py
--rw-r--r--   0        0        0     1940 2023-04-10 18:07:01.116505 meeple-cli-0.1.0b5/src/meeple/util/sort_util.py
--rw-r--r--   0        0        0        0 2023-04-10 18:07:01.116505 meeple-cli-0.1.0b5/tests/__init__.py
--rw-r--r--   0        0        0      313 2023-04-10 18:07:01.116505 meeple-cli-0.1.0b5/tests/test_root.py
--rw-r--r--   0        0        0     5293 1970-01-01 00:00:00.000000 meeple-cli-0.1.0b5/PKG-INFO
+-rw-r--r--   0        0        0       66 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/.flake8
+-rw-r--r--   0        0        0     1090 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1290 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/.github/workflows/python-test.yml
+-rw-r--r--   0        0        0      289 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/.gitignore
+-rw-r--r--   0        0        0      168 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/.markdownlint.yaml
+-rw-r--r--   0        0        0     1347 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1073 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/LICENSE
+-rw-r--r--   0        0        0     4284 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/README.md
+-rw-r--r--   0        0        0      249 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/codecov.yml
+-rw-r--r--   0        0        0     5188 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/docs/changelog.md
+-rw-r--r--   0        0        0      830 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/justfile
+-rw-r--r--   0        0        0     1014 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/pyproject.toml
+-rw-r--r--   0        0        0      112 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/__init__.py
+-rw-r--r--   0        0        0      639 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/command/__init__.py
+-rw-r--r--   0        0        0     1498 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/command/add.py
+-rw-r--r--   0        0        0     2251 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/command/collections.py
+-rw-r--r--   0        0        0      941 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/command/completions.py
+-rw-r--r--   0        0        0     1385 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/command/delete.py
+-rw-r--r--   0        0        0     1489 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/command/drop.py
+-rw-r--r--   0        0        0     5333 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/command/find.py
+-rw-r--r--   0        0        0      670 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/command/hot.py
+-rw-r--r--   0        0        0     1490 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/command/info.py
+-rw-r--r--   0        0        0     3644 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/command/list.py
+-rw-r--r--   0        0        0     2394 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/command/move.py
+-rw-r--r--   0        0        0      658 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/command/new.py
+-rw-r--r--   0        0        0     1182 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/command/open.py
+-rw-r--r--   0        0        0     1179 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/command/rename.py
+-rw-r--r--   0        0        0      948 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/command/search.py
+-rw-r--r--   0        0        0     3403 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/command/stats.py
+-rw-r--r--   0        0        0     2640 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/command/update.py
+-rw-r--r--   0        0        0     1153 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/root.py
+-rw-r--r--   0        0        0        0 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/type/__init__.py
+-rw-r--r--   0        0        0      278 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/type/collection.py
+-rw-r--r--   0        0        0     4385 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/type/item.py
+-rw-r--r--   0        0        0        0 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/util/__init__.py
+-rw-r--r--   0        0        0     1450 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/util/api_util.py
+-rw-r--r--   0        0        0      697 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/util/cmd_util.py
+-rw-r--r--   0        0        0     2024 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/util/collection_util.py
+-rw-r--r--   0        0        0      235 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/util/completion_util.py
+-rw-r--r--   0        0        0     2596 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/util/data_util.py
+-rw-r--r--   0        0        0      927 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/util/filter_util.py
+-rw-r--r--   0        0        0      617 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/util/fs_util.py
+-rw-r--r--   0        0        0      352 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/util/input_util.py
+-rw-r--r--   0        0        0     3543 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/util/output_util.py
+-rw-r--r--   0        0        0     2616 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/src/meeple/util/sort_util.py
+-rw-r--r--   0        0        0        0 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/tests/__init__.py
+-rw-r--r--   0        0        0      313 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/tests/test_root.py
+-rw-r--r--   0        0        0        0 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/tests/util/__init__.py
+-rw-r--r--   0        0        0     1879 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/tests/util/test_filter_util.py
+-rw-r--r--   0        0        0     2188 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/tests/util/test_fs_util.py
+-rw-r--r--   0        0        0      565 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/tests/util/test_input_util.py
+-rw-r--r--   0        0        0     2274 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/tests/util/test_output_util.py
+-rw-r--r--   0        0        0     2525 2023-04-17 03:57:10.671394 meeple-cli-0.1.0b6/tests/util/test_sort_util.py
+-rw-r--r--   0        0        0     5283 1970-01-01 00:00:00.000000 meeple-cli-0.1.0b6/PKG-INFO
```

### Comparing `meeple-cli-0.1.0b5/.github/workflows/python-publish.yml` & `meeple-cli-0.1.0b6/.github/workflows/python-publish.yml`

 * *Files 18% similar despite different names*

```diff
@@ -28,11 +28,10 @@
       - name: Install dependencies via pip
         run: |
           python -m pip install --upgrade pip
           python -m pip install flit
       - name: Build package via flit
         run: flit build
       - name: Publish package to pypi
-        uses: pypa/gh-action-pypi-publish@27b31702a0e7fc50959f5ad993c78deac1bdfc29
+        uses: pypa/gh-action-pypi-publish@release/v1
         with:
-          user: __token__
           password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `meeple-cli-0.1.0b5/.github/workflows/python-test.yml` & `meeple-cli-0.1.0b6/.github/workflows/python-test.yml`

 * *Files 16% similar despite different names*

```diff
@@ -18,20 +18,26 @@
 
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
+      - name: Run linters via pre-commit
+        uses: pre-commit/action@v3.0.0
       - name: Install dependencies via pip
         run: |
           python -m pip install --upgrade pip
           python -m pip install flit
       - name: Install package via flit
         run: |
           flit install
-      - name: Run linters via pre-commit
-        run: |
-          pre-commit run --all-files
       - name: Run tests via pytest
         run: |
-          pytest
+          pytest -v --cov-report xml --cov meeple
+      - name: Upload test coverage to Codecov
+        uses: codecov/codecov-action@v3
+        with:
+          token: ${{ secrets.CODECOV_TOKEN }}
+          files: ./coverage.xml
+          fail_ci_if_error: true
+          verbose: true
```

### Comparing `meeple-cli-0.1.0b5/.pre-commit-config.yaml` & `meeple-cli-0.1.0b6/.pre-commit-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -34,11 +34,16 @@
     rev: v8.16.2
     hooks:
       - id: gitleaks
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: v3.0.0-alpha.6
     hooks:
       - id: prettier
+  - repo: https://github.com/returntocorp/semgrep
+    rev: v1.17.1
+    hooks:
+      - id: semgrep
+        args: ["--config", "auto", "--error", "--skip-unknown-extensions"]
   - repo: https://github.com/dosisod/refurb
     rev: v1.15.0
     hooks:
       - id: refurb
```

### Comparing `meeple-cli-0.1.0b5/LICENSE` & `meeple-cli-0.1.0b6/LICENSE`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b5/README.md` & `meeple-cli-0.1.0b6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # meeple-cli
 
 [![build status](https://img.shields.io/github/actions/workflow/status/boldandbrad/meeple-cli/python-test.yml?branch=main&logo=github)](https://github.com/boldandbrad/meeple-cli/actions/workflows/python-test.yml?query=branch%3Amain)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
+[![codecov](https://codecov.io/gh/boldandbrad/meeple-cli/branch/main/graph/badge.svg)](https://codecov.io/gh/boldandbrad/meeple-cli)
 [![pypi](https://img.shields.io/pypi/v/meeple-cli)](https://pypi.org/project/meeple-cli/)
 [![downloads](https://img.shields.io/pypi/dm/meeple-cli)](https://pypistats.org/packages/meeple-cli)
 
-<!-- [![codecov](https://codecov.io/gh/boldandbrad/meeple-cli/branch/main/graph/badge.svg)](https://codecov.io/gh/boldandbrad/meeple-cli) -->
 <!-- [![Docs](https://img.shields.io/website?down_message=down&label=docs&up_message=online&url=https%3A%2F%2Fboldandbrad.github.io%2Fmeeple-cli%2F)](https://boldandbrad.github.io/meeple-cli/) -->
 
 **Local board game collection manager. Powered by
 [BoardGameGeek](https://boardgamegeek.com).**
 
 > Disclaimer: Neither `meeple-cli` nor its maintainers are affiliated with
 > [BoardGameGeek](https://boardgamegeek.com).
```

### Comparing `meeple-cli-0.1.0b5/docs/changelog.md` & `meeple-cli-0.1.0b6/docs/changelog.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,24 @@
 The format is based on
 [Keep a Changelog](https://keepachangelog.com/en/1.1.0/ "Keep a Changelog"),
 and this project adheres to
 [Semantic Versioning](https://semver.org/spec/v2.0.0.html "Semantic Versioning").
 
 ## [Unreleased]
 
+## [v0.1.0b6] - 2023-04-16
+
+### Added
+
+- `GENERAL` - Sortedby column indicator in sorted output.
+- `meeple list` - _Type_ column included if output contains both boardgames and expansions.
+- `TESTS` - Increase test coverage.
+- `CI` - Report test coverage to [Codecov](https://codecov.io).
+- `CI` - Speed up test github action with `pre-commit` caching.
+
 ## [v0.1.0b5] - 2023-04-10
 
 ### Added
 
 - `meeple info`: `-v/--verbose` - Output additional details.
 - `meeple open`: `-y/--yes` - Bypass confirmation.
 - `meeple find`/`meeple list`: `--sort` - Sort output by _time_.
```

### Comparing `meeple-cli-0.1.0b5/justfile` & `meeple-cli-0.1.0b6/justfile`

 * *Files 27% similar despite different names*

```diff
@@ -1,46 +1,45 @@
 
 # activate venv
 venv:
     . .venv/bin/activate
 
-# install meeple-cli
+# install meeple-cli from local
 install:
+    pip install -q .
+
+# install meeple-cli via flit
+flit-install:
     pip install flit
     flit install
 
 # install editable
 dev-install:
-    pip install -e .
+    pip install -q -e .
 
 # lint and format
 lint:
-    pre-commit run --all-files
+    pre-commit run --show-diff-on-failure --all-files
 
 # run all tests
 test: install
     pytest
 
 # run all tests with coverage
 test-cov: install
-    pytest --cov-report=xml --cov=./src/meeple/
+    pytest -v --cov-report xml --cov meeple
 
 # build dist
 build:
     flit build
 
 # generate homebrew formula
 brew: install
     poet -f meeple-cli >> formula.rb
 
-# check code and deps for vulns
-# snyk doesn't currently support flit project with pyproject.toml
-# deps:
-#     snyk test --file=pyproject.toml
-
 # remove artifacts
 # TODO: remove __pycache__ dirs from src/ and tests/
 cleanup:
     rm -f .coverage
     rm -f coverage.xml
     rm -f formula.rb
     rm -rf .pytest_cache
```

### Comparing `meeple-cli-0.1.0b5/pyproject.toml` & `meeple-cli-0.1.0b6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -25,23 +25,23 @@
 Home = "https://github.com/boldandbrad/meeple-cli"
 
 [project.optional-dependencies]
 test = [
   "pytest >=6",
   "pytest-cov",
   "pytest-mock",
-  "codecov",
 ]
 dev = [
   "black",
   "flake8",
   "flit",
   "isort",
   "pre-commit",
   "homebrew-pypi-poet",
+  "semgrep",
   "refurb",
 ]
 
 [tool.flit.module]
 name = "meeple"
 
 [tool.isort]
```

### Comparing `meeple-cli-0.1.0b5/src/meeple/command/__init__.py` & `meeple-cli-0.1.0b6/src/meeple/command/__init__.py`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b5/src/meeple/command/add.py` & `meeple-cli-0.1.0b6/src/meeple/command/add.py`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b5/src/meeple/command/collections.py` & `meeple-cli-0.1.0b6/src/meeple/command/collections.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 import sys
 
 import click
 
 from meeple.type.collection import Collection
 from meeple.util.collection_util import get_collections
 from meeple.util.data_util import get_collection_data, last_updated
-from meeple.util.output_util import print_table, print_warning
-from meeple.util.sort_util import sort_collections
+from meeple.util.output_util import (
+    CollectionHeader,
+    fmt_headers,
+    print_table,
+    print_warning,
+)
+from meeple.util.sort_util import COLLECTION_SORT_KEYS, sort_collections
 
 
 @click.command()
 @click.option(
     "--sort",
-    type=click.Choice(
-        ["name", "boardgames", "expansions", "updated"], case_sensitive=False
-    ),
+    type=click.Choice(COLLECTION_SORT_KEYS, case_sensitive=False),
     default="updated",
     show_default=True,
     help="Sort output by the provided column.",
 )
 @click.option("-v", "--verbose", is_flag=True, help="Output additional details.")
 @click.help_option("-h", "--help")
 def collections(sort: str, verbose: bool) -> None:
@@ -38,20 +41,29 @@
     for collection in collections:
         boardgames, expansions = get_collection_data(collection)
         collection_list.append(
             Collection(collection, boardgames, expansions, last_updated(collection))
         )
 
     # sort output
-    collection_list = sort_collections(collection_list, sort)
+    collection_list, sort_direction = sort_collections(collection_list, sort)
 
     # prepare table data
-    headers = ["Name"]
+    headers = [CollectionHeader.NAME]
     if verbose:
-        headers.extend(["Boardgames", "Expansions", "Last Updated"])
+        headers.extend(
+            [
+                CollectionHeader.BOARDGAMES,
+                CollectionHeader.EXPANSIONS,
+                CollectionHeader.UPDATED,
+            ]
+        )
+
+    # format headers
+    headers = fmt_headers(headers, sort, sort_direction)
 
     rows = []
     for collection in collection_list:
         cols = [collection.name]
         # include additional data if the user chose verbose output
         if verbose:
             cols.extend(
```

### Comparing `meeple-cli-0.1.0b5/src/meeple/command/completions.py` & `meeple-cli-0.1.0b6/src/meeple/command/completions.py`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b5/src/meeple/command/delete.py` & `meeple-cli-0.1.0b6/src/meeple/command/delete.py`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b5/src/meeple/command/drop.py` & `meeple-cli-0.1.0b6/src/meeple/command/drop.py`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b5/src/meeple/command/find.py` & `meeple-cli-0.1.0b6/src/meeple/command/find.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 from meeple.type.collection import Collection
 from meeple.util.collection_util import are_collections, get_collections
 from meeple.util.completion_util import complete_collections
 from meeple.util.data_util import get_collection_data
 from meeple.util.filter_util import filterby_players, filterby_playtime, filterby_weight
 from meeple.util.output_util import (
+    ItemHeader,
+    fmt_headers,
     fmt_players,
     fmt_playtime,
     fmt_rank,
     fmt_rating,
     fmt_type,
     fmt_weight,
     fmt_year,
@@ -107,27 +109,39 @@
         result_items = filterby_players(result_items, players)
     if max_time:
         result_items = filterby_playtime(result_items, max_time)
     if weight:
         result_items = filterby_weight(result_items, weight)
 
     # sort output
-    result_items = sort_items(result_items, sort)
+    result_items, sort_direction = sort_items(result_items, sort)
 
     # prepare table headers
-    headers = ["ID", "Name"]
+    headers = [ItemHeader.ID, ItemHeader.NAME]
     # include type column if neither type is ommitted
     if item_type not in ("bg", "ex"):
-        headers.append("Type")
+        headers.append(ItemHeader.TYPE)
     # include collections column if more than one collection was included
     if len(collections) > 1:
-        headers.append("Collection(s)")
+        headers.append(ItemHeader.COLLECTION)
     # include additional columns if verbose flag present
     if verbose:
-        headers.extend(["Year", "Rank", "Rating", "Weight", "Players", "Play Time"])
+        headers.extend(
+            [
+                ItemHeader.YEAR,
+                ItemHeader.RANK,
+                ItemHeader.RATING,
+                ItemHeader.WEIGHT,
+                ItemHeader.PLAYERS,
+                ItemHeader.TIME,
+            ]
+        )
+
+    # format headers
+    headers = fmt_headers(headers, sort, sort_direction)
 
     # prepare table data
     rows = []
     for item in result_items:
         cols = [str(item.id), item.name]
         # include type data if neither type is ommitted
         if item_type not in ("bg", "ex"):
```

### Comparing `meeple-cli-0.1.0b5/src/meeple/command/hot.py` & `meeple-cli-0.1.0b6/src/meeple/command/hot.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import click
 
 from meeple.util.api_util import get_bgg_hot
-from meeple.util.output_util import print_table
+from meeple.util.output_util import ItemHeader, fmt_headers, print_table
 
 
 @click.command()
 @click.help_option("-h", "--help")
 def hot() -> None:
     """List current BoardGameGeek trending items."""
     # retrieve hotness data from BoardGameGeek
     api_result = get_bgg_hot()
 
     # prepare table data
-    headers = ["#", "ID", "Name"]
+    headers = [ItemHeader.COUNT, ItemHeader.ID, ItemHeader.NAME]
+    headers = fmt_headers(headers, None, None)
+
     rows = []
     for idx, item in enumerate(api_result):
         cols = []
         cols.extend([str(idx + 1), str(item.id), item.name])
         rows.append(cols)
 
     print_table(rows, headers)
```

### Comparing `meeple-cli-0.1.0b5/src/meeple/command/info.py` & `meeple-cli-0.1.0b6/src/meeple/command/info.py`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b5/src/meeple/command/list.py` & `meeple-cli-0.1.0b6/src/meeple/command/list.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,18 +2,21 @@
 
 import click
 
 from meeple.util.collection_util import is_collection
 from meeple.util.completion_util import complete_collections
 from meeple.util.data_util import get_collection_data
 from meeple.util.output_util import (
+    ItemHeader,
+    fmt_headers,
     fmt_players,
     fmt_playtime,
     fmt_rank,
     fmt_rating,
+    fmt_type,
     fmt_weight,
     fmt_year,
     print_error,
     print_table,
     print_warning,
 )
 from meeple.util.sort_util import ITEM_SORT_KEYS, sort_items
@@ -71,24 +74,42 @@
         out_list = boardgames
     elif item_type == "ex":
         out_list = expansions
     else:
         out_list = boardgames + expansions
 
     # sort output
-    out_list = sort_items(out_list, sort)
+    out_list, sort_direction = sort_items(out_list, sort)
 
     # prepare table data
-    headers = ["ID", "Name"]
+    headers = [ItemHeader.ID, ItemHeader.NAME]
+    # include type column if neither type is ommitted
+    if item_type not in ("bg", "ex"):
+        headers.append(ItemHeader.TYPE)
     if verbose:
-        headers.extend(["Year", "Rank", "Rating", "Weight", "Players", "Play Time"])
+        headers.extend(
+            [
+                ItemHeader.YEAR,
+                ItemHeader.RANK,
+                ItemHeader.RATING,
+                ItemHeader.WEIGHT,
+                ItemHeader.PLAYERS,
+                ItemHeader.TIME,
+            ]
+        )
+
+    # format headers
+    headers = fmt_headers(headers, sort, sort_direction)
 
     rows = []
     for item in out_list:
         cols = [str(item.id), item.name]
+        # include type data if neither type is ommitted
+        if item_type not in ("bg", "ex"):
+            cols.append(fmt_type(item.type))
         # include additional data if the user chose verbose output
         if verbose:
             cols.extend(
                 [
                     fmt_year(item.year),
                     fmt_rank(str(item.rank)),
                     fmt_rating(item.rating),
```

### Comparing `meeple-cli-0.1.0b5/src/meeple/command/move.py` & `meeple-cli-0.1.0b6/src/meeple/command/move.py`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b5/src/meeple/command/new.py` & `meeple-cli-0.1.0b6/src/meeple/command/new.py`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b5/src/meeple/command/open.py` & `meeple-cli-0.1.0b6/src/meeple/command/open.py`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b5/src/meeple/command/rename.py` & `meeple-cli-0.1.0b6/src/meeple/command/rename.py`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b5/src/meeple/command/stats.py` & `meeple-cli-0.1.0b6/src/meeple/command/stats.py`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b5/src/meeple/command/update.py` & `meeple-cli-0.1.0b6/src/meeple/command/update.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,17 +55,17 @@
             if item_type == BOARDGAME_TYPE:
                 boardgames.append(item)
             if item_type == EXPANSION_TYPE:
                 expansions.append(item)
 
         # sort board games by rank and expansions by rating
         if boardgames:
-            boardgames = sort_items(boardgames, "rank")
+            boardgames, _ = sort_items(boardgames, "rank")
         if expansions:
-            expansions = sort_items(expansions, "rating")
+            expansions, _ = sort_items(expansions, "rating")
 
         # save results
         update_result = {
             "boardgames": [boardgame.__dict__ for boardgame in boardgames],
             "expansions": [expansion.__dict__ for expansion in expansions],
         }
         write_collection_data(collection, update_result)
```

### Comparing `meeple-cli-0.1.0b5/src/meeple/root.py` & `meeple-cli-0.1.0b6/src/meeple/root.py`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b5/src/meeple/type/item.py` & `meeple-cli-0.1.0b6/src/meeple/type/item.py`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b5/src/meeple/util/api_util.py` & `meeple-cli-0.1.0b6/src/meeple/util/api_util.py`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b5/src/meeple/util/cmd_util.py` & `meeple-cli-0.1.0b6/src/meeple/util/cmd_util.py`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b5/src/meeple/util/collection_util.py` & `meeple-cli-0.1.0b6/src/meeple/util/collection_util.py`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b5/src/meeple/util/data_util.py` & `meeple-cli-0.1.0b6/src/meeple/util/data_util.py`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b5/src/meeple/util/sort_util.py` & `meeple-cli-0.1.0b6/src/meeple/util/sort_util.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,54 @@
 from meeple.type.collection import Collection
 from meeple.type.item import Item
+from meeple.util.output_util import SORT_ASC_SYMBOL, SORT_DESC_SYMBOL
 
+COLLECTION_SORT_KEYS = ["name", "boardgames", "expansions", "updated"]
 ITEM_SORT_KEYS = ["rank", "rating", "weight", "year", "name", "id", "time"]
 
 
 def _handle_str_rank(item: Item):
     try:
         return int(item.rank)
     except ValueError:
         return float("inf")
 
 
 def sort_collections(collection_list: [Collection], sort_key: str) -> [Collection]:
     match sort_key:
         case "name":
-            return sorted(collection_list, key=lambda collection: collection.name)
+            return (
+                sorted(collection_list, key=lambda collection: collection.name),
+                SORT_ASC_SYMBOL,
+            )
         case "boardgames":
-            return sorted(
-                collection_list,
-                key=lambda collection: len(collection.boardgames),
-                reverse=True,
+            return (
+                sorted(
+                    collection_list,
+                    key=lambda collection: len(collection.boardgames),
+                    reverse=True,
+                ),
+                SORT_DESC_SYMBOL,
             )
         case "expansions":
-            return sorted(
-                collection_list,
-                key=lambda collection: len(collection.expansions),
-                reverse=True,
+            return (
+                sorted(
+                    collection_list,
+                    key=lambda collection: len(collection.expansions),
+                    reverse=True,
+                ),
+                SORT_DESC_SYMBOL,
             )
-    return sorted(
-        collection_list,
-        key=lambda collection: collection.last_updated,
-        reverse=True,
+    return (
+        sorted(
+            collection_list,
+            key=lambda collection: collection.last_updated,
+            reverse=True,
+        ),
+        SORT_DESC_SYMBOL,
     )
 
 
 def sort_items(item_list: [Item], sort_key: str) -> [Item]:
     """Sort the given item list by the given key. Defaults to sort by rating.
 
     Args:
@@ -42,19 +56,28 @@
         sort_key (str): key to sort by.
 
     Returns:
         [Item]: sorted list of Item.
     """
     match sort_key:
         case "rank":
-            return sorted(item_list, key=_handle_str_rank)
+            return sorted(item_list, key=_handle_str_rank), SORT_ASC_SYMBOL
         case "weight":
-            return sorted(item_list, key=lambda item: item.weight, reverse=True)
+            return (
+                sorted(item_list, key=lambda item: item.weight, reverse=True),
+                SORT_DESC_SYMBOL,
+            )
         case "year":
-            return sorted(item_list, key=lambda item: item.year)
+            return sorted(item_list, key=lambda item: item.year), SORT_ASC_SYMBOL
         case "name":
-            return sorted(item_list, key=lambda item: item.name)
+            return sorted(item_list, key=lambda item: item.name), SORT_ASC_SYMBOL
         case "id":
-            return sorted(item_list, key=lambda item: int(item.id))
+            return sorted(item_list, key=lambda item: int(item.id)), SORT_ASC_SYMBOL
         case "time":
-            return sorted(item_list, key=lambda item: int(item.playtime))
-    return sorted(item_list, key=lambda item: item.rating, reverse=True)
+            return (
+                sorted(item_list, key=lambda item: int(item.playtime)),
+                SORT_ASC_SYMBOL,
+            )
+    return (
+        sorted(item_list, key=lambda item: item.rating, reverse=True),
+        SORT_DESC_SYMBOL,
+    )
```

### Comparing `meeple-cli-0.1.0b5/PKG-INFO` & `meeple-cli-0.1.0b6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meeple-cli
-Version: 0.1.0b5
+Version: 0.1.0b6
 Summary: Local board game collection manager. Powered by BoardGameGeek.
 Author-email: Bradley Wojcik <bradleycwojcik@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: click >=8
 Requires-Dist: rich >=13
@@ -13,31 +13,31 @@
 Requires-Dist: pyyaml >=6
 Requires-Dist: black ; extra == "dev"
 Requires-Dist: flake8 ; extra == "dev"
 Requires-Dist: flit ; extra == "dev"
 Requires-Dist: isort ; extra == "dev"
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: homebrew-pypi-poet ; extra == "dev"
+Requires-Dist: semgrep ; extra == "dev"
 Requires-Dist: refurb ; extra == "dev"
 Requires-Dist: pytest >=6 ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: pytest-mock ; extra == "test"
-Requires-Dist: codecov ; extra == "test"
 Project-URL: Home, https://github.com/boldandbrad/meeple-cli
 Provides-Extra: dev
 Provides-Extra: test
 
 # meeple-cli
 
 [![build status](https://img.shields.io/github/actions/workflow/status/boldandbrad/meeple-cli/python-test.yml?branch=main&logo=github)](https://github.com/boldandbrad/meeple-cli/actions/workflows/python-test.yml?query=branch%3Amain)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
+[![codecov](https://codecov.io/gh/boldandbrad/meeple-cli/branch/main/graph/badge.svg)](https://codecov.io/gh/boldandbrad/meeple-cli)
 [![pypi](https://img.shields.io/pypi/v/meeple-cli)](https://pypi.org/project/meeple-cli/)
 [![downloads](https://img.shields.io/pypi/dm/meeple-cli)](https://pypistats.org/packages/meeple-cli)
 
-<!-- [![codecov](https://codecov.io/gh/boldandbrad/meeple-cli/branch/main/graph/badge.svg)](https://codecov.io/gh/boldandbrad/meeple-cli) -->
 <!-- [![Docs](https://img.shields.io/website?down_message=down&label=docs&up_message=online&url=https%3A%2F%2Fboldandbrad.github.io%2Fmeeple-cli%2F)](https://boldandbrad.github.io/meeple-cli/) -->
 
 **Local board game collection manager. Powered by
 [BoardGameGeek](https://boardgamegeek.com).**
 
 > Disclaimer: Neither `meeple-cli` nor its maintainers are affiliated with
 > [BoardGameGeek](https://boardgamegeek.com).
```

