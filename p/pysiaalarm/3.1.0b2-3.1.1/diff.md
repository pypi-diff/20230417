# Comparing `tmp/pysiaalarm-3.1.0b2.tar.gz` & `tmp/pysiaalarm-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysiaalarm-3.1.0b2.tar", last modified: Tue Dec  6 13:15:43 2022, max compression
+gzip compressed data, was "pysiaalarm-3.1.1.tar", last modified: Mon Apr 17 14:42:17 2023, max compression
```

## Comparing `pysiaalarm-3.1.0b2.tar` & `pysiaalarm-3.1.1.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 13:15:43.396448 pysiaalarm-3.1.0b2/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 13:15:43.380447 pysiaalarm-3.1.0b2/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 13:15:43.372448 pysiaalarm-3.1.0b2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 13:15:43.380447 pysiaalarm-3.1.0b2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      857 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      703 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      564 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      184 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      461 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 13:15:43.380447 pysiaalarm-3.1.0b2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      641 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      128 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2022-12-06 13:15:43.396448 pysiaalarm-3.1.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      354 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 13:15:43.384448 pysiaalarm-3.1.0b2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    67606 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/docs/SIA Codes, OS Malevich 2.8_2.9.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    58035 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/docs/SIA Codes.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   133582 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/docs/SIA_code.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 13:15:43.384448 pysiaalarm-3.1.0b2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       41 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5485 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/docs/codes.csv
--rw-r--r--   0 runner    (1001) docker     (123)    15906 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/docs/codes.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     9499 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)       39 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      233 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      311 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      712 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      712 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/pytest.old
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2022-12-06 13:15:43.400448 pysiaalarm-3.1.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      705 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 13:15:43.372448 pysiaalarm-3.1.0b2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 13:15:43.388448 pysiaalarm-3.1.0b2/src/pysiaalarm/
--rw-r--r--   0 runner    (1001) docker     (123)      958 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/src/pysiaalarm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/src/pysiaalarm/account.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 13:15:43.392448 pysiaalarm-3.1.0b2/src/pysiaalarm/aio/
--rw-r--r--   0 runner    (1001) docker     (123)      312 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/src/pysiaalarm/aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5809 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/src/pysiaalarm/aio/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/src/pysiaalarm/aio/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/src/pysiaalarm/base_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6062 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/src/pysiaalarm/base_server.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/src/pysiaalarm/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 13:15:43.392448 pysiaalarm-3.1.0b2/src/pysiaalarm/data/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/src/pysiaalarm/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4682 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/src/pysiaalarm/data/adm_mapping.json
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/src/pysiaalarm/data/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    58799 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/src/pysiaalarm/data/sia_codes.json
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/src/pysiaalarm/data/xdata.json
--rw-r--r--   0 runner    (1001) docker     (123)      733 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/src/pysiaalarm/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    20270 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/src/pysiaalarm/event.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/src/pysiaalarm/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 13:15:43.392448 pysiaalarm-3.1.0b2/src/pysiaalarm/sync/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/src/pysiaalarm/sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/src/pysiaalarm/sync/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/src/pysiaalarm/sync/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/src/pysiaalarm/sync/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 13:15:43.392448 pysiaalarm-3.1.0b2/src/pysiaalarm/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/src/pysiaalarm/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/src/pysiaalarm/utils/counter.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/src/pysiaalarm/utils/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/src/pysiaalarm/utils/regexes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 13:15:43.388448 pysiaalarm-3.1.0b2/src/pysiaalarm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2022-12-06 13:15:43.000000 pysiaalarm-3.1.0b2/src/pysiaalarm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2022-12-06 13:15:43.000000 pysiaalarm-3.1.0b2/src/pysiaalarm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-06 13:15:43.000000 pysiaalarm-3.1.0b2/src/pysiaalarm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-06 13:15:26.000000 pysiaalarm-3.1.0b2/src/pysiaalarm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      186 2022-12-06 13:15:43.000000 pysiaalarm-3.1.0b2/src/pysiaalarm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2022-12-06 13:15:43.000000 pysiaalarm-3.1.0b2/src/pysiaalarm.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 13:15:43.396448 pysiaalarm-3.1.0b2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/tests/encrypted_config.json
--rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/tests/ha.json
--rw-r--r--   0 runner    (1001) docker     (123)      739 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/tests/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/tests/run_aio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5329 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/tests/run_re.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/tests/test_alarm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/tests/test_alarm_aio.py
--rw-r--r--   0 runner    (1001) docker     (123)    14135 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/tests/test_sia_package.py
--rw-r--r--   0 runner    (1001) docker     (123)    14546 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/tests/test_sia_package_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     4519 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/tests/unencrypted_config.json
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2022-12-06 13:15:13.000000 pysiaalarm-3.1.0b2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:42:17.688524 pysiaalarm-3.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:42:17.664523 pysiaalarm-3.1.1/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:42:17.648523 pysiaalarm-3.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:42:17.664523 pysiaalarm-3.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:42:17.664523 pysiaalarm-3.1.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-17 14:42:17.688524 pysiaalarm-3.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:42:17.672524 pysiaalarm-3.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    67606 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/docs/SIA Codes, OS Malevich 2.8_2.9.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    58035 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/docs/SIA Codes.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   133582 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/docs/SIA_code.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:42:17.672524 pysiaalarm-3.1.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/docs/codes.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    15906 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/docs/codes.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     9499 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/pytest.old
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-04-17 14:42:17.692524 pysiaalarm-3.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:42:17.652523 pysiaalarm-3.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:42:17.676524 pysiaalarm-3.1.1/src/pysiaalarm/
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/src/pysiaalarm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/src/pysiaalarm/account.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:42:17.680524 pysiaalarm-3.1.1/src/pysiaalarm/aio/
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/src/pysiaalarm/aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/src/pysiaalarm/aio/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/src/pysiaalarm/aio/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/src/pysiaalarm/base_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/src/pysiaalarm/base_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/src/pysiaalarm/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:42:17.680524 pysiaalarm-3.1.1/src/pysiaalarm/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/src/pysiaalarm/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/src/pysiaalarm/data/adm_mapping.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/src/pysiaalarm/data/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58799 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/src/pysiaalarm/data/sia_codes.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/src/pysiaalarm/data/xdata.json
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/src/pysiaalarm/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19289 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/src/pysiaalarm/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/src/pysiaalarm/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:42:17.684524 pysiaalarm-3.1.1/src/pysiaalarm/sync/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/src/pysiaalarm/sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/src/pysiaalarm/sync/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/src/pysiaalarm/sync/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/src/pysiaalarm/sync/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:42:17.684524 pysiaalarm-3.1.1/src/pysiaalarm/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/src/pysiaalarm/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/src/pysiaalarm/utils/counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/src/pysiaalarm/utils/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/src/pysiaalarm/utils/regexes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:42:17.676524 pysiaalarm-3.1.1/src/pysiaalarm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-17 14:42:17.000000 pysiaalarm-3.1.1/src/pysiaalarm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-04-17 14:42:17.000000 pysiaalarm-3.1.1/src/pysiaalarm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 14:42:17.000000 pysiaalarm-3.1.1/src/pysiaalarm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 14:42:05.000000 pysiaalarm-3.1.1/src/pysiaalarm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-17 14:42:17.000000 pysiaalarm-3.1.1/src/pysiaalarm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-17 14:42:17.000000 pysiaalarm-3.1.1/src/pysiaalarm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:42:17.688524 pysiaalarm-3.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/tests/encrypted_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/tests/ha.json
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/tests/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/tests/run_aio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5329 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/tests/run_re.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/tests/test_alarm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/tests/test_alarm_aio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14135 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/tests/test_sia_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14797 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/tests/test_sia_package_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/tests/unencrypted_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-04-17 14:41:50.000000 pysiaalarm-3.1.1/tox.ini
```

### Comparing `pysiaalarm-3.1.0b2/.coveragerc` & `pysiaalarm-3.1.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b2/.devcontainer/Dockerfile` & `pysiaalarm-3.1.1/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b2/.devcontainer/devcontainer.json` & `pysiaalarm-3.1.1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b2/.github/workflows/main.yml` & `pysiaalarm-3.1.1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b2/.github/workflows/release.yaml` & `pysiaalarm-3.1.1/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b2/.gitignore` & `pysiaalarm-3.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b2/.vscode/launch.json` & `pysiaalarm-3.1.1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b2/.vscode/settings.json` & `pysiaalarm-3.1.1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b2/LICENSE.txt` & `pysiaalarm-3.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b2/PKG-INFO` & `pysiaalarm-3.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysiaalarm
-Version: 3.1.0b2
+Version: 3.1.1
 Summary: Python package for creating a client that talks with SIA-based alarm systems.
 Author: E.A. van Valkenburg
 Author-email: github@vanvalkenburg.eu
 License: MIT
 Project-URL: Documentation, https://github.com/eavanvalkenburg/pysiaalarm
 Project-URL: Source, https://github.com/eavanvalkenburg/pysiaalarm
 Platform: any
```

### Comparing `pysiaalarm-3.1.0b2/README.md` & `pysiaalarm-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b2/docs/Makefile` & `pysiaalarm-3.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b2/docs/SIA Codes, OS Malevich 2.8_2.9.xlsx` & `pysiaalarm-3.1.1/docs/SIA Codes, OS Malevich 2.8_2.9.xlsx`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b2/docs/SIA Codes.xlsx` & `pysiaalarm-3.1.1/docs/SIA Codes.xlsx`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b2/docs/SIA_code.pdf` & `pysiaalarm-3.1.1/docs/SIA_code.pdf`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b2/docs/codes.csv` & `pysiaalarm-3.1.1/docs/codes.csv`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b2/docs/codes.pdf` & `pysiaalarm-3.1.1/docs/codes.pdf`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b2/docs/conf.py` & `pysiaalarm-3.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b2/docs/index.rst` & `pysiaalarm-3.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b2/pytest.ini` & `pysiaalarm-3.1.1/pytest.ini`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b2/pytest.old` & `pysiaalarm-3.1.1/pytest.old`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b2/setup.cfg` & `pysiaalarm-3.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b2/setup.py` & `pysiaalarm-3.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b2/src/pysiaalarm/__init__.py` & `pysiaalarm-3.1.1/src/pysiaalarm/__init__.py`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b2/src/pysiaalarm/account.py` & `pysiaalarm-3.1.1/src/pysiaalarm/account.py`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b2/src/pysiaalarm/aio/client.py` & `pysiaalarm-3.1.1/src/pysiaalarm/aio/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import asyncio
 from abc import abstractmethod
 import logging
 from collections.abc import Awaitable, Callable
 from types import TracebackType
 from typing import Any, Type
 
-from .. import __author__, __copyright__, __license__, __version__
 from ..account import SIAAccount
 from ..base_client import BaseSIAClient
 from ..event import SIAEvent
 from ..utils import CommunicationsProtocol
 from .server import SIAServerTCP, SIAServerUDP
 
 _LOGGER = logging.getLogger(__name__)
@@ -39,14 +38,15 @@
 
     def __init__(
         self,
         host: str,
         port: int,
         accounts: list[SIAAccount],
         function: Callable[[SIAEvent], Awaitable[None]],
+        **kwargs: Any,
     ):
         """Create the asynchronous SIA Client object.
 
         Arguments:
             host {str} -- Host to run the server on, usually would be ""
             port {int} -- The port the server listens to.
             accounts {List[SIAAccount]} -- List of SIA Accounts to add.
```

### Comparing `pysiaalarm-3.1.0b2/src/pysiaalarm/aio/server.py` & `pysiaalarm-3.1.1/src/pysiaalarm/aio/server.py`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b2/src/pysiaalarm/base_client.py` & `pysiaalarm-3.1.1/src/pysiaalarm/base_client.py`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b2/src/pysiaalarm/base_server.py` & `pysiaalarm-3.1.1/src/pysiaalarm/base_server.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,38 +41,37 @@
         """
         self.accounts = accounts
         self.func = func
         self.async_func = async_func
         self.counts = counts
         self.shutdown_flag = False
 
-    def parse_and_check_event(self, line: bytes) -> EventsType | None:
+    def parse_and_check_event(self, data: bytes) -> EventsType | None:
         """Parse and check the line and create the event, check the account and define the response.
 
         Args:
-            line (bytes): Line to parse
+            line (str): Line to parse
 
         Returns:
             SIAEvent: The SIAEvent type of the parsed line.
             ResponseType: The response to send to the alarm.
 
         """
-        if not line.strip():
+        line = str.strip(data.decode("ascii", errors="ignore"))
+        if not line:
             return None
         self.log_and_count(COUNTER_EVENTS, line=line)
         try:
             event = SIAEvent.from_line(line, self.accounts)
         except NoAccountError as exc:
             self.log_and_count(COUNTER_ACCOUNT, line, exception=exc)
-            binary_crc = NAKEvent.check_crc_type(line)
-            return NAKEvent(binary_crc=binary_crc)
+            return NAKEvent()
         except EventFormatError as exc:
             self.log_and_count(COUNTER_FORMAT, line, exception=exc)
-            binary_crc = NAKEvent.check_crc_type(line)
-            return NAKEvent(binary_crc=binary_crc)
+            return NAKEvent()
 
         if isinstance(event, OHEvent):
             return event  # pragma: no cover
         if not event.valid_message:
             self.log_and_count(COUNTER_CRC, event=event)
         elif not event.sia_account:
             self.log_and_count(COUNTER_ACCOUNT, event=event)
@@ -111,15 +110,15 @@
             self.func(event)
         except Exception as exp:  # pylint: disable=broad-except
             self.log_and_count(COUNTER_USER_CODE, event=event, exception=exp)
 
     def log_and_count(
         self,
         counter: str,
-        line: str | bytes | None = None,
+        line: str | None = None,
         event: SIAEvent | None = None,
         exception: Exception | None = None,
     ) -> None:
         """Log the appropriate line and increment the right counter."""
         if counter == COUNTER_ACCOUNT and exception is not None:
             _LOGGER.warning(
                 "There is no account for a encrypted line, line was: %s",
```

### Comparing `pysiaalarm-3.1.0b2/src/pysiaalarm/data/adm_mapping.json` & `pysiaalarm-3.1.1/src/pysiaalarm/data/adm_mapping.json`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b2/src/pysiaalarm/data/data.py` & `pysiaalarm-3.1.1/src/pysiaalarm/data/data.py`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b2/src/pysiaalarm/data/sia_codes.json` & `pysiaalarm-3.1.1/src/pysiaalarm/data/sia_codes.json`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b2/src/pysiaalarm/data/xdata.json` & `pysiaalarm-3.1.1/src/pysiaalarm/data/xdata.json`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b2/src/pysiaalarm/errors.py` & `pysiaalarm-3.1.1/src/pysiaalarm/errors.py`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b2/src/pysiaalarm/event.py` & `pysiaalarm-3.1.1/src/pysiaalarm/event.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 @dataclass  # type: ignore
 class BaseEvent(ABC):
     """Base class for Events."""
 
     # From Main Matcher
     full_message: str | None = None
     msg_crc: str | None = None
-    binary_crc: bool = False
     length: str | None = None
     encrypted: bool | None = None
     message_type: str | MessageTypes | None = None
     receiver: str = "R0"
     line: str = "L0"
     account: str | None = None
     sequence: str | None = None
@@ -114,46 +113,36 @@
         if not self.sia_account.key_b:
             return None  # pragma: no cover
         cypher = AES.new(self.sia_account.key_b, AES.MODE_CBC, IV)
         if isinstance(cypher, CbcMode):
             return cypher
         return None  # pragma: no cover
 
-    @staticmethod
-    def check_crc_type(incoming: bytes) -> bool:
-        """Check if the CRC is binary or not."""
-        return len(incoming.split(b'"')[0]) == 7
-
     @classmethod
     def from_line(
-        cls,
-        data: bytes,
-        accounts: dict[str, SIAAccount] | None = None,
+        cls, incoming: str, accounts: dict[str, SIAAccount] | None = None
     ) -> SIAEvent:
         """Create a Event from a line.
 
         Arguments:
             incoming {str} -- The line to be parsed.
             accounts {List[SIAAccount]} -- accounts to check against, optional
 
         Raises:
             EventFormatError: If the event is not formatted according to SIA DC09 or ADM-CID.
 
         """
-        binary_crc = BaseEvent.check_crc_type(data)
-        incoming = str.strip(data.decode("ascii", errors="ignore"))
         line_match = MAIN_MATCHER.match(incoming)
         if not line_match:
             oh_event = OH_MATCHER.match(incoming)
             if oh_event:
                 fields = oh_event.groupdict()
                 return OHEvent(
                     full_message=incoming,
                     msg_crc="",
-                    binary_crc=binary_crc,
                     message_type=MessageTypes.OH,
                     length=str(len(incoming)),
                     encrypted=False,
                     receiver=fields["receiver"],
                     line=fields["line"],
                     account=fields["account"],
                     id=fields["id"],
@@ -168,15 +157,14 @@
         sia_account = None
         if accounts and acc:
             sia_account = accounts.get(acc, None)
 
         return SIAEvent(
             full_message=incoming[8:],
             msg_crc=main_content["crc"],
-            binary_crc=binary_crc,
             length=main_content["length"],
             encrypted=encrypted,
             message_type=main_content["message_type"],
             sequence=main_content["sequence"],
             receiver=main_content["receiver"],
             line=main_content["line"],
             account=acc,
@@ -199,21 +187,22 @@
     @staticmethod
     def _crc_calc(msg: str | None) -> str | None:
         """Calculate the CRC of the msg."""
         if msg is None:  # pragma: no cover
             return None
         crc = 0
         for letter in str.encode(msg):
+            temp = letter
             for _ in range(0, 8):
-                letter ^= crc & 1
+                temp ^= crc & 1
                 crc >>= 1
-                if (letter & 1) != 0:
+                if (temp & 1) != 0:
                     crc ^= 0xA001
-                letter >>= 1
-        return "%04X" % crc
+                temp >>= 1
+        return ("%x" % crc).upper().zfill(4)
 
     def to_dict(self, **kwargs: Any) -> dict[str, Any]:
         """Create a dict from the dataclass.
 
         Kwargs are only there for legacy (after no longer using dataclasses_json),
         so remove any other arguments from this function.
         """
@@ -237,31 +226,28 @@
         if "_xdata_parsed" in event:
             event.pop("_xdata_parsed")
         if "timestamp" in event and event["timestamp"] is not None:
             event["timestamp"] = datetime.fromisoformat(event["timestamp"])
         return cls(**event)
 
 
+
 @dataclass
 class SIAEvent(BaseEvent):
     """Class for SIAEvents."""
 
     def __post_init__(self) -> None:
         """Run post init logic."""
         # Convert the message type to the enum
         if isinstance(self.message_type, str):  # pragma: no cover
             self.message_type = MessageTypes(self.message_type)
 
         # Calculate the CRC of the message.
         if not self.calc_crc:
             self.calc_crc = self._crc_calc(self.full_message)
-            if self.calc_crc is not None:
-                if self.binary_crc:
-                    calc_crc = int(self.calc_crc, 16)
-                    self.calc_crc = str(bytes([calc_crc >> 16, calc_crc & 0xFF]))
         # If there is encrypted content and a key, decrypt
         if self.encrypted_content:
             if not self.sia_account or not self.sia_account.encrypted:
                 raise NoAccountError("No account present with encrypted message.")
             if not self._encrypted_content_decrypted:
                 self.decrypt_content()
         # If there is content (either after decrypting or directly) parse
@@ -367,17 +353,14 @@
         else:
             encrypted_content = self.encrypt_content(
                 f']{x_data if x_data else ""}{self._get_timestamp(self.sia_account.device_timezone)}'
             )
             res = f'"*{response_type.value}"{self.sequence}{self.receiver}{self.line}#{self.account}[{encrypted_content}'
         header = ("%04x" % len(res)).upper()
         new_crc = self._crc_calc(res)
-        if self.binary_crc and new_crc is not None:
-            new_crc_int = int(new_crc, 16)
-            new_crc = str(bytes([new_crc_int >> 16, new_crc_int & 0xFF]))
         return f"\n{new_crc}{header}{res}\r".encode("ascii")
 
     def decrypt_content(self) -> None:
         """Decrypt the content, if encrypted account, otherwise pass back the event."""
         if not self.encrypted_content:  # pragma: no cover
             return None
         decr = self._get_crypter()
@@ -489,15 +472,14 @@
 Receiver: {self.receiver}, \
 Line: {self.line}, \
 Timestamp: {self.timestamp}, \
 Length: {self.length}, \
 Sequence: {self.sequence}, \
 CRC: {self.msg_crc}, \
 Calc CRC: {self.calc_crc}, \
-Binary CRC: {self.binary_crc}, \
 Encrypted Content: {self.encrypted_content}, \
 Full Message: {self.full_message}."
 
 
 @dataclass
 class OHEvent(SIAEvent):
     """Class for OH events."""
@@ -546,15 +528,11 @@
 
         Returns:
             str -- Response to send back to sender.
 
         """
         res = f'"NAK"0000L0R0A0[]{self._get_timestamp()}'
         header = ("%04x" % len(res)).upper()
-        new_crc = self._crc_calc(res)
-        if self.binary_crc and new_crc is not None:
-            new_crc_int = int(new_crc, 16)
-            new_crc = str(bytes([new_crc_int >> 16, new_crc_int & 0xFF]))
-        return f"\n{new_crc}{header}{res}\r".encode("ascii")
+        return f"\n{self._crc_calc(res)}{header}{res}\r".encode("ascii")
 
 
 EventsType = Union[SIAEvent, OHEvent, NAKEvent]
```

### Comparing `pysiaalarm-3.1.0b2/src/pysiaalarm/sync/client.py` & `pysiaalarm-3.1.1/src/pysiaalarm/sync/client.py`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b2/src/pysiaalarm/sync/handler.py` & `pysiaalarm-3.1.1/src/pysiaalarm/sync/handler.py`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b2/src/pysiaalarm/sync/server.py` & `pysiaalarm-3.1.1/src/pysiaalarm/sync/server.py`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b2/src/pysiaalarm/utils/counter.py` & `pysiaalarm-3.1.1/src/pysiaalarm/utils/counter.py`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b2/src/pysiaalarm/utils/enums.py` & `pysiaalarm-3.1.1/src/pysiaalarm/utils/enums.py`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b2/src/pysiaalarm/utils/regexes.py` & `pysiaalarm-3.1.1/src/pysiaalarm/utils/regexes.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,57 +27,51 @@
 (?P<line>L[A-Fa-f0-9]{1,6})
 [#]?(?P<account>[A-Fa-f0-9]{3,16})?
 [\[]
 (?P<rest>.*)
 """
 MAIN_MATCHER = re.compile(main_regex, re.X)
 
-# Content matcher, with shared pre and post expressions.
-xdata_ts_regex = r"""
-[\]]
-(?:\[(?:(?<=\[)(?P<xdata>.*)(?=\]))\])?
-(?:_(?<=_)(?P<timestamp>[0-9:,-]*)?)?$
-"""
-
-sia_content_regex = (
-    r"""
+sia_content_regex = r"""
 [#]?(?P<account>[A-Fa-f0-9]{3,16})?
 [|]?
 [N]?
 (?:ti)?(?:(?<=ti)(?P<ti>\d{2}:\d{2}))?\/?
 (?:id)?(?:(?<=id)(?P<id>\d*))?\/?
 (?:ri)?(?:(?<=ri)(?P<ri>\d*))?\/?
 (?P<code>[a-zA-Z]{2})?
 (?P<message>.[^\[\]]*)?
+[\]]
+(?:\[(?:(?<=\[)(?P<xdata>.*)(?=\]))\])?
+[_]?
+(?P<timestamp>[0-9:,-]*)?$
 """
-    + xdata_ts_regex
-)
+SIA_CONTENT_MATCHER = re.compile(sia_content_regex, re.X)
 
-adm_content_regex = (
-    r"""
+encr_sia_content_regex = r"""(?:[^\|\[\]]*)[|]?"""
+ENCR_SIA_CONTENT_MATCHER = re.compile(encr_sia_content_regex + sia_content_regex, re.X)
+
+adm_content_regex = r"""
 [#]?(?P<account>[A-F0-9]{3,16})?
 [|]?
 (?P<event_qualifier>\d{1})
 (?P<event_type>\d{3})
 \s
 (?P<partition>\d{2})
 \s
 (?P<ri>\d{3})
+[\]]
+(?:\[(?:(?<=\[)(?P<xdata>.[^\[\]]*)(?=\]))\])?
+[_]?
+(?P<timestamp>[0-9:,-]*)?$
 """
-    + xdata_ts_regex
-)
-
-encr_content_regex = r"""
-(?:[^\|\[\]]*)[|]?
-"""
-
-SIA_CONTENT_MATCHER = re.compile(sia_content_regex, re.X)
 ADM_CONTENT_MATCHER = re.compile(adm_content_regex, re.X)
-ENCR_SIA_CONTENT_MATCHER = re.compile(encr_content_regex + sia_content_regex, re.X)
-ENCR_ADM_CONTENT_MATCHER = re.compile(encr_content_regex + adm_content_regex, re.X)
+
+encr_adm_content_regex = r"""(?:[^\|\[\]]*)[|]?"""
+ENCR_ADM_CONTENT_MATCHER = re.compile(encr_adm_content_regex + adm_content_regex, re.X)
 
 
 def _get_matcher(
     message_type: MessageTypes | str, encrypted: bool = False
 ) -> re.Pattern:
     """Extract the content using the different regexes."""
     if message_type == MessageTypes.ADMCID:
```

### Comparing `pysiaalarm-3.1.0b2/src/pysiaalarm.egg-info/PKG-INFO` & `pysiaalarm-3.1.1/src/pysiaalarm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysiaalarm
-Version: 3.1.0b2
+Version: 3.1.1
 Summary: Python package for creating a client that talks with SIA-based alarm systems.
 Author: E.A. van Valkenburg
 Author-email: github@vanvalkenburg.eu
 License: MIT
 Project-URL: Documentation, https://github.com/eavanvalkenburg/pysiaalarm
 Project-URL: Source, https://github.com/eavanvalkenburg/pysiaalarm
 Platform: any
```

### Comparing `pysiaalarm-3.1.0b2/src/pysiaalarm.egg-info/SOURCES.txt` & `pysiaalarm-3.1.1/src/pysiaalarm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b2/tests/run.py` & `pysiaalarm-3.1.1/tests/run.py`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b2/tests/run_aio.py` & `pysiaalarm-3.1.1/tests/run_aio.py`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b2/tests/run_re.py` & `pysiaalarm-3.1.1/tests/run_re.py`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b2/tests/test_alarm.py` & `pysiaalarm-3.1.1/tests/test_alarm.py`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b2/tests/test_alarm_aio.py` & `pysiaalarm-3.1.1/tests/test_alarm_aio.py`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b2/tests/test_sia_package.py` & `pysiaalarm-3.1.1/tests/test_sia_package.py`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b2/tests/test_sia_package_cases.py` & `pysiaalarm-3.1.1/tests/test_sia_package_cases.py`

 * *Files 8% similar despite different names*

```diff
@@ -113,211 +113,219 @@
     Emits these fields: "line, account_id, code_type, code, error, extended_data_flag, encrypted_flag"
 
     """
 
     def case_bug(self):
         """Test case from #11."""
         return (
-            rb'9618004D"SIA-DCS"7960L0#123456[#123456|Nri1CL0^VX FRONTE ^]_22:40:48,04-11-2021',
+            r'9618004D"SIA-DCS"7960L0#123456[#123456|Nri1CL0^VX FRONTE ^]_22:40:48,04-11-2021',
             "123456",
             "Closing Report",
             "CL",
             None,
             False,
             False,
         )
 
     def case_bug2(self):
         """Test case from SIA #42."""
         return (
-            rb'5670004D"SIA-DCS"8070L0#123456[#123456|Nri0KR1^TAST. 001 ^]_13:49:12,04-13-2021',
+            r'5670004D"SIA-DCS"8070L0#123456[#123456|Nri0KR1^TAST. 001 ^]_13:49:12,04-13-2021',
             "123456",
             "Heat Restoral",
             "KR",
             None,
             False,
             False,
         )
 
     def case_dc04(self):
         """Test case DC04 format - NOT SUPPORTED so throws an error."""
         return (
-            rb'<x0A>CE110032"SIA-DCS"9876R579BDFL789ABC#12345A[#12345A|NFA129]_14:12:04,09-25-201',
+            r'<x0A>CE110032"SIA-DCS"9876R579BDFL789ABC#12345A[#12345A|NFA129]_14:12:04,09-25-201',
             "12345A",
             None,
             None,
             EventFormatError,
             False,
             False,
         )
 
     def case_adm_cid(self):
         """Test case ADM-CID format."""
         return (
-            rb'87CD0037"ADM-CID"9876R579BDFL789ABC#12345A[#12345A|1110 00 129]_14:12:04,09-25-2011',
+            r'87CD0037"ADM-CID"9876R579BDFL789ABC#12345A[#12345A|1110 00 129]_14:12:04,09-25-2011',
             "12345A",
             "Fire Alarm",
             "FA",
             None,
             False,
             False,
         )
 
     def case_adm_cid2(self):
         """Test case ADM-CID format."""
         return (
-            rb'57150047"ADM-CID"0247R4F39L4F39#4F39[#4F39|3401 01 057]',
+            r'57150047"ADM-CID"0247R4F39L4F39#4F39[#4F39|3401 01 057]',
             "4F39",
             "Closing Report",
             "CL",
             None,
             False,
             False,
         )
 
     def case_code_jc(self):
         """Input a closing report event in SIA DC-09 with JC code."""
         return (
-            rb'97F90078"SIA-DCS"6002L0#AAA[|Nri2/JC12]_12:58:23,09-15-2021',
+            r'97F90078"SIA-DCS"6002L0#AAA[|Nri2/JC12]_12:58:23,09-15-2021',
             "AAA",
             "User code tamper canceled",
             "JC",
             None,
             False,
             False,
         )
 
     def case_xdata_M(self):
         """Input a closing report event in SIA DC-09 with M xdata."""
         return (
-            rb'87570078"SIA-DCS"6002L0#AAA[|Nri1/CL501][M0026B9E4268B]_14:12:04,09-25-2019',
+            r'87570078"SIA-DCS"6002L0#AAA[|Nri1/CL501][M0026B9E4268B]_14:12:04,09-25-2019',
             "AAA",
             "Closing Report",
             "CL",
             None,
             True,
             False,
         )
 
     def case_xdata_K(self):
         """Input a closing report event in SIA DC-09 with K xdata."""
         return (
-            (
-                rf'02310052"SIA-DCS"6002L0#{ACCOUNT}[|Nri1/RP000][KAAAAAAAAAAAAAAAA]_14:12:04,09-25-2019'
-            ).encode(),
+            rf'02310052"SIA-DCS"6002L0#{ACCOUNT}[|Nri1/RP000][KAAAAAAAAAAAAAAAA]_14:12:04,09-25-2019',
             ACCOUNT,
             "Automatic Test",
             "RP",
             None,
             True,
             False,
         )
 
     def case_xdata_X_and_Y(self):
         """Input a closing report event in SIA DC-09 with K xdata."""
         return (
-            (
-                rf'5B090059"SIA-DCS"0004L0#{ACCOUNT}[#{ACCOUNT}|Nri1/PA501][X006E07.7777777][Y49N06.6666666]_20:45:46,04-22-2021'
-            ).encode(),
+            rf'5B090059"SIA-DCS"0004L0#{ACCOUNT}[#{ACCOUNT}|Nri1/PA501][X006E07.7777777][Y49N06.6666666]_20:45:46,04-22-2021',
             ACCOUNT,
             "Panic Alarm",
             "PA",
             None,
             True,
             False,
         )
 
     def case_encrypted(self):
         """Input a encrypted line."""
         return (
-            rb'60AB0078"*SIA-DCS"5994L0#AAA[5AB718E008C616BF16F6468033A11326B0F7546CAB230910BCA10E4DEBA42283C436E4F8EFF50931070DDE36D5BB5F0C',
+            r'60AB0078"*SIA-DCS"5994L0#AAA[5AB718E008C616BF16F6468033A11326B0F7546CAB230910BCA10E4DEBA42283C436E4F8EFF50931070DDE36D5BB5F0C',
             "AAA",
             None,
             None,
             None,
             False,
             True,
         )
 
     def case_encrypted_adm(self):
         """Input a encrypted ADM line."""
         return (
-            rb'D0850078"*ADM-CID"6879R0L0#123F[64F7ADD9BA9377DBF2C014BC709329BEEE345B5F20C60B7EB9D2C6B8C222666B13D0B4A114B448B0AC555FCC658DB6EE',
+            r'D0850078"*ADM-CID"6879R0L0#123F[64F7ADD9BA9377DBF2C014BC709329BEEE345B5F20C60B7EB9D2C6B8C222666B13D0B4A114B448B0AC555FCC658DB6EE',
             "123F",
             None,
             None,
             None,
             False,
             True,
         )
 
     def case_oh(self):
         """Input a OH event."""
         return (
-            rb"SR0001L0001    006969XX    [ID00000000]",
+            r"SR0001L0001    006969XX    [ID00000000]",
             "006969XX",
             "Automatic Test",
             "RP",
             None,
             False,
             False,
         )
 
     def case_cl(self):
         """Input a closing report event in SIA DC-09."""
         return (
-            rb'E5D50078"SIA-DCS"6002L0#AAA[|Nri1/CL501]_14:12:04,09-25-2019',
+            r'E5D50078"SIA-DCS"6002L0#AAA[|Nri1/CL501]_14:12:04,09-25-2019',
             "AAA",
             "Closing Report",
             "CL",
             None,
             False,
             False,
         )
 
     def case_op(self):
         """Input a opening report event."""
         return (
-            rb'90820051"SIA-DCS"4738R0001L0001[#006969|Nri04/OP001NM]',
+            r'90820051"SIA-DCS"4738R0001L0001[#006969|Nri04/OP001NM]',
             "006969",
             "Opening Report",
             "OP",
             None,
             False,
             False,
         )
 
     def case_null(self):
         """Input a encrypted null event."""
         return (
-            rb'76D80055"*NULL"0000R0L0#AAAB[B4BC8B40D0E6D959D6BEA78E88CC0B2155741A3C44FBB96D476A3E557CAD64D9',
+            r'76D80055"*NULL"0000R0L0#AAAB[B4BC8B40D0E6D959D6BEA78E88CC0B2155741A3C44FBB96D476A3E557CAD64D9',
             "AAAB",
             None,
             None,
             None,
             False,
             True,
         )
 
+    # def case_null2(self):
+    #     """Input a unencrypted null event, based on issue #42."""
+    #     return (
+    #         rb'CA2F0038"NULL"0000L0#7890[#0000|0000 00 000]_22:13:29,12-29-2022',
+    #         "7890",
+    #         "Automatic Test",
+    #         "RP",
+    #         None,
+    #         False,
+    #         False,
+    #     )
+
     def case_wa(self):
         """Input a water alarm event."""
         return (
-            rb'C4160279"SIA-DCS"5268L0#AAA[Nri1/WA000]_08:40:47,07-08-2020',
+            r'C4160279"SIA-DCS"5268L0#AAA[Nri1/WA000]_08:40:47,07-08-2020',
             "AAA",
             "Water Alarm",
             "WA",
             None,
             False,
             False,
         )
 
     def case_eventformaterror(self):
         """Input a event format error event."""
         return (
-            rb"this is not a parsable event",
+            r"this is not a parsable event",
             None,
             None,
             None,
             EventFormatError,
             False,
             False,
         )
```

### Comparing `pysiaalarm-3.1.0b2/tests/test_utils.py` & `pysiaalarm-3.1.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pysiaalarm-3.1.0b2/tox.ini` & `pysiaalarm-3.1.1/tox.ini`

 * *Files identical despite different names*

