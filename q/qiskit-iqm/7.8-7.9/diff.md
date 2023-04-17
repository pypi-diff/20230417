# Comparing `tmp/qiskit-iqm-7.8.tar.gz` & `tmp/qiskit-iqm-7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit-iqm-7.8.tar", last modified: Thu Mar 23 07:16:26 2023, max compression
+gzip compressed data, was "qiskit-iqm-7.9.tar", last modified: Tue Apr  4 13:24:37 2023, max compression
```

## Comparing `qiskit-iqm-7.8.tar` & `qiskit-iqm-7.9.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 07:16:26.286036 qiskit-iqm-7.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 07:16:26.278036 qiskit-iqm-7.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 07:16:26.282036 qiskit-iqm-7.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-03-23 07:15:29.000000 qiskit-iqm-7.8/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-03-23 07:15:29.000000 qiskit-iqm-7.8/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-03-23 07:15:29.000000 qiskit-iqm-7.8/.github/workflows/tag_and_release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-03-23 07:15:29.000000 qiskit-iqm-7.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-03-23 07:15:29.000000 qiskit-iqm-7.8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-03-23 07:15:29.000000 qiskit-iqm-7.8/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-03-23 07:15:29.000000 qiskit-iqm-7.8/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-23 07:15:29.000000 qiskit-iqm-7.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15203 2023-03-23 07:16:26.286036 qiskit-iqm-7.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-03-23 07:15:29.000000 qiskit-iqm-7.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 07:16:26.282036 qiskit-iqm-7.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-23 07:15:29.000000 qiskit-iqm-7.8/docs/API.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-03-23 07:15:29.000000 qiskit-iqm-7.8/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 07:16:26.282036 qiskit-iqm-7.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-23 07:15:29.000000 qiskit-iqm-7.8/docs/_static/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 07:16:26.282036 qiskit-iqm-7.8/docs/_static/images/
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-03-23 07:15:29.000000 qiskit-iqm-7.8/docs/_static/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)   194362 2023-03-23 07:15:29.000000 qiskit-iqm-7.8/docs/_static/images/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 07:16:26.282036 qiskit-iqm-7.8/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-03-23 07:15:29.000000 qiskit-iqm-7.8/docs/_templates/autosummary-class-template.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-03-23 07:15:29.000000 qiskit-iqm-7.8/docs/_templates/autosummary-module-template.rst
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-03-23 07:15:29.000000 qiskit-iqm-7.8/docs/_templates/page.html
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-03-23 07:15:29.000000 qiskit-iqm-7.8/docs/_templates/versioning.html
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-23 07:15:29.000000 qiskit-iqm-7.8/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-23 07:15:29.000000 qiskit-iqm-7.8/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-03-23 07:15:29.000000 qiskit-iqm-7.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-03-23 07:15:29.000000 qiskit-iqm-7.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-23 07:15:29.000000 qiskit-iqm-7.8/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13294 2023-03-23 07:15:29.000000 qiskit-iqm-7.8/docs/user_guide.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 07:16:26.282036 qiskit-iqm-7.8/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-03-23 07:15:29.000000 qiskit-iqm-7.8/examples/bell_measure.py
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-03-23 07:15:29.000000 qiskit-iqm-7.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 07:16:26.286036 qiskit-iqm-7.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 07:16:26.278036 qiskit-iqm-7.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 07:16:26.282036 qiskit-iqm-7.8/src/qiskit_iqm/
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-03-23 07:15:29.000000 qiskit-iqm-7.8/src/qiskit_iqm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 07:16:26.286036 qiskit-iqm-7.8/src/qiskit_iqm/fake_backends/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-23 07:15:29.000000 qiskit-iqm-7.8/src/qiskit_iqm/fake_backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-03-23 07:15:29.000000 qiskit-iqm-7.8/src/qiskit_iqm/fake_backends/fake_adonis.py
--rw-r--r--   0 runner    (1001) docker     (123)    12986 2023-03-23 07:15:29.000000 qiskit-iqm-7.8/src/qiskit_iqm/fake_backends/iqm_fake_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-03-23 07:15:29.000000 qiskit-iqm-7.8/src/qiskit_iqm/iqm_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-03-23 07:15:29.000000 qiskit-iqm-7.8/src/qiskit_iqm/iqm_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-03-23 07:15:29.000000 qiskit-iqm-7.8/src/qiskit_iqm/iqm_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 07:15:29.000000 qiskit-iqm-7.8/src/qiskit_iqm/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-03-23 07:15:29.000000 qiskit-iqm-7.8/src/qiskit_iqm/qiskit_to_iqm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 07:16:26.286036 qiskit-iqm-7.8/src/qiskit_iqm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15203 2023-03-23 07:16:26.000000 qiskit-iqm-7.8/src/qiskit_iqm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-03-23 07:16:26.000000 qiskit-iqm-7.8/src/qiskit_iqm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 07:16:26.000000 qiskit-iqm-7.8/src/qiskit_iqm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-03-23 07:16:26.000000 qiskit-iqm-7.8/src/qiskit_iqm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-23 07:16:26.000000 qiskit-iqm-7.8/src/qiskit_iqm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-03-23 07:15:29.000000 qiskit-iqm-7.8/tag-from-pipeline.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 07:16:26.286036 qiskit-iqm-7.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-03-23 07:15:29.000000 qiskit-iqm-7.8/tests/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 07:15:29.000000 qiskit-iqm-7.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-03-23 07:15:29.000000 qiskit-iqm-7.8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 07:16:26.286036 qiskit-iqm-7.8/tests/fake_backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 07:15:29.000000 qiskit-iqm-7.8/tests/fake_backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-03-23 07:15:29.000000 qiskit-iqm-7.8/tests/fake_backends/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-03-23 07:15:29.000000 qiskit-iqm-7.8/tests/fake_backends/test_fake_adonis.py
--rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-03-23 07:15:29.000000 qiskit-iqm-7.8/tests/fake_backends/test_iqm_fake_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-03-23 07:15:29.000000 qiskit-iqm-7.8/tests/test_iqm_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-03-23 07:15:29.000000 qiskit-iqm-7.8/tests/test_iqm_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    11726 2023-03-23 07:15:29.000000 qiskit-iqm-7.8/tests/test_iqm_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-03-23 07:15:29.000000 qiskit-iqm-7.8/tests/test_qiskit_to_iqm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-03-23 07:15:29.000000 qiskit-iqm-7.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:24:37.231975 qiskit-iqm-7.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:24:37.223974 qiskit-iqm-7.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:24:37.227975 qiskit-iqm-7.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/.github/workflows/tag_and_release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5766 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15203 2023-04-04 13:24:37.231975 qiskit-iqm-7.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:24:37.227975 qiskit-iqm-7.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/docs/API.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:24:37.227975 qiskit-iqm-7.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/docs/_static/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:24:37.227975 qiskit-iqm-7.9/docs/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/docs/_static/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)   194362 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/docs/_static/images/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:24:37.227975 qiskit-iqm-7.9/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/docs/_templates/autosummary-class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/docs/_templates/autosummary-module-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/docs/_templates/page.html
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/docs/_templates/versioning.html
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13782 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/docs/user_guide.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:24:37.227975 qiskit-iqm-7.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/examples/bell_measure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 13:24:37.231975 qiskit-iqm-7.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:24:37.223974 qiskit-iqm-7.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:24:37.231975 qiskit-iqm-7.9/src/qiskit_iqm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/src/qiskit_iqm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:24:37.231975 qiskit-iqm-7.9/src/qiskit_iqm/fake_backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/src/qiskit_iqm/fake_backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/src/qiskit_iqm/fake_backends/fake_adonis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12986 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/src/qiskit_iqm/fake_backends/iqm_fake_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/src/qiskit_iqm/iqm_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/src/qiskit_iqm/iqm_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7199 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/src/qiskit_iqm/iqm_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/src/qiskit_iqm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/src/qiskit_iqm/qiskit_to_iqm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:24:37.231975 qiskit-iqm-7.9/src/qiskit_iqm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15203 2023-04-04 13:24:37.000000 qiskit-iqm-7.9/src/qiskit_iqm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-04 13:24:37.000000 qiskit-iqm-7.9/src/qiskit_iqm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 13:24:37.000000 qiskit-iqm-7.9/src/qiskit_iqm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-04 13:24:37.000000 qiskit-iqm-7.9/src/qiskit_iqm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-04 13:24:37.000000 qiskit-iqm-7.9/src/qiskit_iqm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/tag-from-pipeline.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:24:37.231975 qiskit-iqm-7.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/tests/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:24:37.231975 qiskit-iqm-7.9/tests/fake_backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/tests/fake_backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/tests/fake_backends/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/tests/fake_backends/test_fake_adonis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/tests/fake_backends/test_iqm_fake_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/tests/test_iqm_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/tests/test_iqm_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/tests/test_iqm_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/tests/test_qiskit_to_iqm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/tox.ini
```

### Comparing `qiskit-iqm-7.8/.github/workflows/ci.yml` & `qiskit-iqm-7.9/.github/workflows/ci.yml`

 * *Files 11% similar despite different names*

```diff
@@ -11,36 +11,36 @@
 
     strategy:
       matrix:
         platform: [ ubuntu-latest, macos-latest, windows-latest ]
         python-version: [ '3.9', '3.10' ]
 
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
         with:
           fetch-depth: 0
       - name: Setup Python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           python -m pip install -e ".[dev]"
           python -m pip install tox-gh-actions==2.12.0
       - name: Run tests
         run: tox
   test_docs:
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
         with:
           fetch-depth: 0
       - name: Setup Python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: '3.9'
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           python -m pip install -e ".[dev, docs]"
           sudo apt-get install graphviz
```

### Comparing `qiskit-iqm-7.8/.github/workflows/publish.yml` & `qiskit-iqm-7.9/.github/workflows/publish.yml`

 * *Files 6% similar despite different names*

```diff
@@ -12,19 +12,19 @@
         required: true
 
 jobs:
   push_to_pypi:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
       - name: Fetch all history for all tags and branches
         run: git fetch --prune --unshallow
       - name: Setup Python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: '3.9'
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install -e ".[dev,cicd]"
       - name: Build and publish
@@ -36,19 +36,19 @@
           TWINE_USERNAME: ${{ secrets.PYPI_USER }}
           TWINE_PASSWORD: ${{ secrets.PYPI_PASSWORD }}
 
   publish_docs:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
         with:
           fetch-depth: 0
       - name: Setup Python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: '3.9'
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install -e ".[dev, docs]"
           sudo apt-get install graphviz
```

### Comparing `qiskit-iqm-7.8/.github/workflows/tag_and_release.yml` & `qiskit-iqm-7.9/.github/workflows/tag_and_release.yml`

 * *Files 2% similar despite different names*

```diff
@@ -11,27 +11,27 @@
       - 'CHANGELOG.rst'
 
 jobs:
   check_version:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
         with:
           fetch-depth: 0
       - name: Check version in changelog
         run: bash ./tag-from-pipeline.sh verify_changelog_version
 
   create_tag_and_release:
     needs: check_version
     runs-on: ubuntu-latest
     if: ${{ github.ref == 'refs/heads/main' }}
 
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
         with:
           fetch-depth: 0
       - name: Create new tag and release
         run: bash ./tag-from-pipeline.sh create_new_tag
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `qiskit-iqm-7.8/CHANGELOG.rst` & `qiskit-iqm-7.9/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =========
 Changelog
 =========
 
+Version 7.9
+===========
+
+* Add request into result metadata `#51 <https://github.com/iqm-finland/qiskit-on-iqm/pull/51>`_
+
 Version 7.8
 ===========
 
 * Drop circuit metadata if it is not JSON serializable `#49 <https://github.com/iqm-finland/qiskit-on-iqm/pull/49>`_
 * Produce ``UserWarning`` if metadata is dropped `#49 <https://github.com/iqm-finland/qiskit-on-iqm/pull/49>`_
 
 Version 7.7
```

### Comparing `qiskit-iqm-7.8/CONTRIBUTING.rst` & `qiskit-iqm-7.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-7.8/LICENSE` & `qiskit-iqm-7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-7.8/PKG-INFO` & `qiskit-iqm-7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-iqm
-Version: 7.8
+Version: 7.9
 Summary: Qiskit adapter for IQM's quantum architectures
 Author-email: IQM Finland Oy <developers@meetiqm.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `qiskit-iqm-7.8/README.rst` & `qiskit-iqm-7.9/README.rst`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-7.8/docs/Makefile` & `qiskit-iqm-7.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-7.8/docs/_static/images/favicon.ico` & `qiskit-iqm-7.9/docs/_static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-7.8/docs/_static/images/logo.png` & `qiskit-iqm-7.9/docs/_static/images/logo.png`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-7.8/docs/_templates/autosummary-class-template.rst` & `qiskit-iqm-7.9/docs/_templates/autosummary-class-template.rst`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-7.8/docs/_templates/autosummary-module-template.rst` & `qiskit-iqm-7.9/docs/_templates/autosummary-module-template.rst`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-7.8/docs/_templates/page.html` & `qiskit-iqm-7.9/docs/_templates/page.html`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-7.8/docs/_templates/versioning.html` & `qiskit-iqm-7.9/docs/_templates/versioning.html`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-7.8/docs/conf.py` & `qiskit-iqm-7.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-7.8/docs/index.rst` & `qiskit-iqm-7.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-7.8/docs/user_guide.rst` & `qiskit-iqm-7.9/docs/user_guide.rst`

 * *Files 1% similar despite different names*

```diff
@@ -101,14 +101,30 @@
 `Cortex CLI <https://github.com/iqm-finland/cortex-cli>`_ to retrieve and automatically refresh access tokens,
 then set the ``IQM_TOKENS_FILE`` environment variable to use those tokens.
 See Cortex CLI's `documentation <https://iqm-finland.github.io/cortex-cli/readme.html>`__ for details.
 Alternatively, authorize with the IQM_AUTH_SERVER, IQM_AUTH_USERNAME and IQM_AUTH_PASSWORD environment variables
 or pass them as arguments to the constructor of :class:`.IQMProvider`, however this approach is less secure
 and considered as deprecated.
 
+The results of a job, that was executed with IQM quantum computer, contain the original request with the
+qubit mapping that was used in execution. You can check this mapping once execution has finished.
+
+.. code-block:: python
+
+    print(job.result().request.qubit_mapping)
+
+::
+
+    [
+      SingleQubitMapping(logical_name='0', physical_name='QB1'),
+      SingleQubitMapping(logical_name='1', physical_name='QB2'),
+      SingleQubitMapping(logical_name='2', physical_name='QB3')
+    ]
+
+
 The ``backend`` instance we created above provides all the standard backend functionality that one expects from a
 backend in Qiskit. For this example, I am connected to an IQM backend that features a 5-qubit chip with star-like
 connectivity:
 
 ::
 
           QB1
@@ -132,14 +148,15 @@
 At IQM we identify qubits by their names, e.g. 'QB1', 'QB2', etc. as demonstrated above. In Qiskit, qubits are
 identified by their indices in the quantum register, as you can see from the printed coupling map above. Most of the
 time you do not need to deal with IQM-style qubit names when using Qiskit, however when you need, the methods
 :meth:`.IQMBackend.qubit_name_to_index` and :meth:`.IQMBackend.index_to_qubit_name` can become handy.
 
 Now we can study how the circuit gets transpiled:
 
+
 .. code-block:: python
 
     from qiskit.compiler import transpile
 
     qc_transpiled = transpile(qc, backend=backend, layout_method='sabre', optimization_level=3)
 
     print(qc_transpiled.draw(output='text'))
```

### Comparing `qiskit-iqm-7.8/examples/bell_measure.py` & `qiskit-iqm-7.9/examples/bell_measure.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-7.8/pyproject.toml` & `qiskit-iqm-7.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-7.8/src/qiskit_iqm/__init__.py` & `qiskit-iqm-7.9/src/qiskit_iqm/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-7.8/src/qiskit_iqm/fake_backends/__init__.py` & `qiskit-iqm-7.9/src/qiskit_iqm/fake_backends/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-7.8/src/qiskit_iqm/fake_backends/fake_adonis.py` & `qiskit-iqm-7.9/src/qiskit_iqm/fake_backends/fake_adonis.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-7.8/src/qiskit_iqm/fake_backends/iqm_fake_backend.py` & `qiskit-iqm-7.9/src/qiskit_iqm/fake_backends/iqm_fake_backend.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-7.8/src/qiskit_iqm/iqm_backend.py` & `qiskit-iqm-7.9/src/qiskit_iqm/iqm_backend.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-7.8/src/qiskit_iqm/iqm_job.py` & `qiskit-iqm-7.9/src/qiskit_iqm/iqm_job.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 
 from collections import Counter
 from datetime import date
 from typing import Optional, Union
 import uuid
 
-from iqm_client import CircuitMeasurementResults, IQMClient, RunResult, Status
+from iqm_client import CircuitMeasurementResults, IQMClient, RunRequest, RunResult, Status
 import numpy as np
 from qiskit.providers import JobStatus, JobV1
 from qiskit.result import Counts, Result
 
 from qiskit_iqm.qiskit_to_iqm import MeasurementKey
 
 
@@ -37,14 +37,15 @@
         **kwargs: arguments to be passed to the initializer of the parent class
     """
 
     def __init__(self, backend: 'qiskit_iqm.IQMBackend', job_id: str, **kwargs):  # type: ignore
         super().__init__(backend, job_id=job_id, **kwargs)
         self._result: Union[None, list[tuple[str, list[str]]]] = None
         self._calibration_set_id: Optional[uuid.UUID] = None
+        self._request: Optional[RunRequest] = None
         self._client: IQMClient = backend.client
         self.circuit_metadata: Optional[list] = None  # Metadata that was originally associated with circuits by user
 
     def _format_iqm_results(self, iqm_result: RunResult) -> list[tuple[str, list[str]]]:
         """Convert the measurement results from a circuit(s) run into the Qiskit format."""
         if iqm_result.measurements is None:
             raise ValueError(f'Cannot format IQM result without measurements. Job status is ${iqm_result.status}')
@@ -92,14 +93,15 @@
     def cancel(self):
         raise NotImplementedError('Canceling jobs is currently not supported.')
 
     def result(self) -> Result:
         if not self._result:
             results = self._client.wait_for_results(uuid.UUID(self._job_id))
             self._calibration_set_id = results.metadata.calibration_set_id
+            self._request = results.metadata.request
             self._result = self._format_iqm_results(results)
             # RemoteIQMBackend.run() populates circuit_metadata, so it may be None if method wasn't called in current
             # session. In that case retrieve circuit metadata from RunResult.metadata.request.circuits[n].metadata
             if self.circuit_metadata is None:
                 self.circuit_metadata = []
                 self.circuit_metadata = [c.metadata for c in results.metadata.request.circuits]
 
@@ -120,14 +122,15 @@
                     },
                     'header': {'name': name},
                     'calibration_set_id': self._calibration_set_id,
                 }
                 for i, (name, measurement_results) in enumerate(self._result)
             ],
             'date': date.today(),
+            'request': self._request,
         }
         return Result.from_dict(result_dict)
 
     def status(self) -> JobStatus:
         if self._result:
             return JobStatus.DONE
```

### Comparing `qiskit-iqm-7.8/src/qiskit_iqm/iqm_provider.py` & `qiskit-iqm-7.9/src/qiskit_iqm/iqm_provider.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Qiskit Backend Provider for IQM backends.
 """
 from importlib.metadata import version
+from functools import reduce
 from typing import Optional, Union
 import warnings
 
 from iqm_client import Circuit, Instruction, IQMClient
 from iqm_client.util import to_json_dict
 import numpy as np
 from qiskit import QuantumCircuit
@@ -57,15 +58,18 @@
         if len(circuits) == 0:
             raise ValueError('Empty list of circuits submitted for execution.')
 
         shots = options.get('shots', self.options.shots)
         calibration_set_id = options.get('calibration_set_id', self.options.calibration_set_id)
 
         circuits_serialized: list[Circuit] = [self.serialize_circuit(circuit) for circuit in circuits]
-        qubit_mapping = {str(idx): qb for idx, qb in self._idx_to_qb.items()}
+        used_indices: set[int] = reduce(
+            lambda qubits, circuit: qubits.union(set(int(q) for q in circuit.all_qubits())), circuits_serialized, set()
+        )
+        qubit_mapping = {str(idx): qb for idx, qb in self._idx_to_qb.items() if idx in used_indices}
         uuid = self.client.submit_circuits(
             circuits_serialized, qubit_mapping=qubit_mapping, calibration_set_id=calibration_set_id, shots=shots
         )
         job = IQMJob(self, str(uuid), shots=shots)
         job.circuit_metadata = [c.metadata for c in circuits]
         return job
```

### Comparing `qiskit-iqm-7.8/src/qiskit_iqm/qiskit_to_iqm.py` & `qiskit-iqm-7.9/src/qiskit_iqm/qiskit_to_iqm.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-7.8/src/qiskit_iqm.egg-info/PKG-INFO` & `qiskit-iqm-7.9/src/qiskit_iqm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-iqm
-Version: 7.8
+Version: 7.9
 Summary: Qiskit adapter for IQM's quantum architectures
 Author-email: IQM Finland Oy <developers@meetiqm.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `qiskit-iqm-7.8/src/qiskit_iqm.egg-info/SOURCES.txt` & `qiskit-iqm-7.9/src/qiskit_iqm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-7.8/tag-from-pipeline.sh` & `qiskit-iqm-7.9/tag-from-pipeline.sh`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-7.8/tests/conftest.py` & `qiskit-iqm-7.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-7.8/tests/fake_backends/conftest.py` & `qiskit-iqm-7.9/tests/fake_backends/conftest.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-7.8/tests/fake_backends/test_fake_adonis.py` & `qiskit-iqm-7.9/tests/fake_backends/test_fake_adonis.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-7.8/tests/fake_backends/test_iqm_fake_backend.py` & `qiskit-iqm-7.9/tests/fake_backends/test_iqm_fake_backend.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-7.8/tests/test_iqm_backend.py` & `qiskit-iqm-7.9/tests/test_iqm_backend.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-7.8/tests/test_iqm_job.py` & `qiskit-iqm-7.9/tests/test_iqm_job.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Testing IQMJob.
 """
 import uuid
 
-from iqm_client import IQMClient, RunResult, RunStatus, Status
+from iqm_client import IQMClient, RunResult, RunStatus, SingleQubitMapping, Status
 import mockito
 from mockito import mock, when
 import pytest
 from qiskit import QuantumCircuit
 from qiskit.providers import JobStatus
 from qiskit.result import Counts
 from qiskit.result import Result as QiskitResult
@@ -50,14 +50,18 @@
 def iqm_metadata():
     return {
         'calibration_set_id': 'df124054-f6d8-41f9-b880-8487f90018f9',
         'request': {
             'shots': 4,
             'circuits': [{'name': 'circuit_1', 'instructions': [], 'metadata': {'a': 'b'}}],
             'calibration_set_id': 'df124054-f6d8-41f9-b880-8487f90018f9',
+            'qubit_mapping': [
+                SingleQubitMapping(logical_name='0', physical_name='QB1'),
+                SingleQubitMapping(logical_name='1', physical_name='QB2'),
+            ],
         },
     }
 
 
 def test_submit_raises(job):
     with pytest.raises(NotImplementedError, match='You should never have to submit jobs by calling this method.'):
         job.submit()
@@ -105,14 +109,15 @@
 
     assert isinstance(result, QiskitResult)
     assert result.get_memory() == ['0100 11', '0100 10', '0100 01', '0100 10']
     assert result.get_counts() == Counts({'0100 11': 1, '0100 10': 2, '0100 01': 1})
     for r in result.results:
         assert r.calibration_set_id == uuid.UUID('df124054-f6d8-41f9-b880-8487f90018f9')
         assert r.data.metadata == {'a': 'b'}
+    assert result.request.qubit_mapping == iqm_metadata['request']['qubit_mapping']
 
     # Assert that repeated call does not query the client (i.e. works without calling the mocked wait_for_results)
     # and call to status() does not call any functions from client.
     result = job.result()
     assert isinstance(result, QiskitResult)
     assert job.status() == JobStatus.DONE
     mockito.verify(job._client, times=1).wait_for_results(uuid.UUID(job.job_id()))
@@ -124,14 +129,19 @@
         'request': {
             'shots': 4,
             'circuits': [
                 {'name': 'circuit_1', 'instructions': [], 'metadata': {'a': 0}},
                 {'name': 'circuit_2', 'instructions': [], 'metadata': {'a': 1}},
             ],
             'calibration_set_id': '9d75904b-0c93-461f-b1dc-bd200cfad1f1',
+            'qubit_mapping': [
+                SingleQubitMapping(logical_name='0', physical_name='QB1'),
+                SingleQubitMapping(logical_name='1', physical_name='QB2'),
+                SingleQubitMapping(logical_name='2', physical_name='QB3'),
+            ],
         },
     }
     client_result = RunResult(
         status=Status.READY,
         measurements=[iqm_result_two_registers, iqm_result_two_registers],
         metadata=iqm_metadata_multiple_circuits,
     )
@@ -144,7 +154,8 @@
         assert result.get_memory(circuit_idx) == ['0100 11', '0100 10', '0100 01', '0100 10']
         assert result.get_counts(circuit_idx) == Counts({'0100 11': 1, '0100 10': 2, '0100 01': 1})
     assert result.get_counts(QuantumCircuit(name='circuit_1')) == Counts({'0100 11': 1, '0100 10': 2, '0100 01': 1})
     assert result.get_counts(QuantumCircuit(name='circuit_2')) == Counts({'0100 11': 1, '0100 10': 2, '0100 01': 1})
     for i, r in enumerate(result.results):
         assert r.calibration_set_id == uuid.UUID('9d75904b-0c93-461f-b1dc-bd200cfad1f1')
         assert r.data.metadata == {'a': i}
+    assert result.request.qubit_mapping == iqm_metadata_multiple_circuits['request']['qubit_mapping']
```

### Comparing `qiskit-iqm-7.8/tests/test_iqm_provider.py` & `qiskit-iqm-7.9/tests/test_iqm_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,19 +34,14 @@
 def backend(linear_architecture_3q):
     client = mock(IQMClient)
     when(client).get_quantum_architecture().thenReturn(linear_architecture_3q)
     return IQMBackend(client)
 
 
 @pytest.fixture
-def qubit_mapping():
-    return {'0': 'QB1', '1': 'QB2', '2': 'QB3'}
-
-
-@pytest.fixture
 def circuit():
     return QuantumCircuit(3, 3)
 
 
 def test_default_options(backend):
     assert backend.options.shots == 1024
     assert backend.options.calibration_set_id is None
@@ -218,21 +213,21 @@
 
     patch(backend.run, run_mock)
     execute(
         circuit, backend, shots=10, calibration_set_id='92d8dd9a-2678-467e-a20b-ef9c1a594d1f', something_else=[1, 2, 3]
     )
 
 
-def test_run_single_circuit(backend, qubit_mapping, circuit):
+def test_run_single_circuit(backend, circuit):
     circuit.measure(0, 0)
     circuit_ser = backend.serialize_circuit(circuit)
     some_id = uuid.uuid4()
     shots = 10
     when(backend.client).submit_circuits(
-        [circuit_ser], qubit_mapping=qubit_mapping, calibration_set_id=None, shots=shots
+        [circuit_ser], qubit_mapping={'0': 'QB1'}, calibration_set_id=None, shots=shots
     ).thenReturn(some_id)
     job = backend.run(circuit, shots=shots)
     assert isinstance(job, IQMJob)
     assert job.job_id() == str(some_id)
 
     # Should also work if the circuit is passed inside a list
     job = backend.run([circuit], shots=shots)
@@ -249,39 +244,39 @@
     backend.client.submit_circuits = lambda *args, **kwargs: some_id
     job = backend.run([circuit_1, circuit_2], shots=10)
     assert isinstance(job, IQMJob)
     assert job.job_id() == str(some_id)
     assert job.circuit_metadata == [circuit_1.metadata, circuit_2.metadata]
 
 
-def test_run_with_custom_calibration_set_id(backend, qubit_mapping, circuit):
+def test_run_with_custom_calibration_set_id(backend, circuit):
     circuit.measure(0, 0)
     circuit_ser = backend.serialize_circuit(circuit)
     some_id = uuid.uuid4()
     shots = 10
     calibration_set_id = '67e77465-d90e-4839-986e-9270f952b743'
     when(backend.client).submit_circuits(
-        [circuit_ser], qubit_mapping=qubit_mapping, calibration_set_id=calibration_set_id, shots=shots
+        [circuit_ser], qubit_mapping={'0': 'QB1'}, calibration_set_id=calibration_set_id, shots=shots
     ).thenReturn(some_id)
 
     backend.run([circuit], calibration_set_id=calibration_set_id, shots=shots)
 
 
-def test_run_batch_of_circuits(backend, qubit_mapping, circuit):
+def test_run_batch_of_circuits(backend, circuit):
     theta = Parameter('theta')
     theta_range = np.linspace(0, 2 * np.pi, 3)
     shots = 10
     some_id = uuid.uuid4()
     circuit.cz(0, 1)
     circuit.r(theta, 0, 0)
     circuit.cz(0, 1)
     circuits = [circuit.bind_parameters({theta: t}) for t in theta_range]
     circuits_serialized = [backend.serialize_circuit(circuit) for circuit in circuits]
     when(backend.client).submit_circuits(
-        circuits_serialized, qubit_mapping=qubit_mapping, calibration_set_id=None, shots=shots
+        circuits_serialized, qubit_mapping={'0': 'QB1', '1': 'QB2'}, calibration_set_id=None, shots=shots
     ).thenReturn(some_id)
 
     job = backend.run(circuits, shots=shots)
     assert isinstance(job, IQMJob)
     assert job.job_id() == str(some_id)
```

### Comparing `qiskit-iqm-7.8/tests/test_qiskit_to_iqm.py` & `qiskit-iqm-7.9/tests/test_qiskit_to_iqm.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-7.8/tox.ini` & `qiskit-iqm-7.9/tox.ini`

 * *Files identical despite different names*

