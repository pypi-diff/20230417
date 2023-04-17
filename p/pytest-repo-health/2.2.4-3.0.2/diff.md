# Comparing `tmp/pytest-repo-health-2.2.4.tar.gz` & `tmp/pytest-repo-health-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytest-repo-health-2.2.4.tar", last modified: Thu Dec 16 18:53:09 2021, max compression
+gzip compressed data, was "pytest-repo-health-3.0.2.tar", last modified: Mon Apr 17 20:19:29 2023, max compression
```

## Comparing `pytest-repo-health-2.2.4.tar` & `pytest-repo-health-3.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-16 18:53:09.000000 pytest-repo-health-2.2.4/
--rw-r--r--   0 runner    (1001) docker     (121)     2541 2021-12-16 18:53:06.000000 pytest-repo-health-2.2.4/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)    35135 2021-12-16 18:53:06.000000 pytest-repo-health-2.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      218 2021-12-16 18:53:06.000000 pytest-repo-health-2.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7257 2021-12-16 18:53:09.000000 pytest-repo-health-2.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6433 2021-12-16 18:53:06.000000 pytest-repo-health-2.2.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-16 18:53:09.000000 pytest-repo-health-2.2.4/pytest_repo_health/
--rw-r--r--   0 runner    (1001) docker     (121)     2433 2021-12-16 18:53:06.000000 pytest-repo-health-2.2.4/pytest_repo_health/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-16 18:53:09.000000 pytest-repo-health-2.2.4/pytest_repo_health/fixtures/
--rw-r--r--   0 runner    (1001) docker     (121)       80 2021-12-16 18:53:06.000000 pytest-repo-health-2.2.4/pytest_repo_health/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      990 2021-12-16 18:53:06.000000 pytest-repo-health-2.2.4/pytest_repo_health/fixtures/git.py
--rw-r--r--   0 runner    (1001) docker     (121)     2704 2021-12-16 18:53:06.000000 pytest-repo-health-2.2.4/pytest_repo_health/fixtures/github.py
--rw-r--r--   0 runner    (1001) docker     (121)     6695 2021-12-16 18:53:06.000000 pytest-repo-health-2.2.4/pytest_repo_health/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)     1304 2021-12-16 18:53:06.000000 pytest-repo-health-2.2.4/pytest_repo_health/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-16 18:53:09.000000 pytest-repo-health-2.2.4/pytest_repo_health.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7257 2021-12-16 18:53:09.000000 pytest-repo-health-2.2.4/pytest_repo_health.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      599 2021-12-16 18:53:09.000000 pytest-repo-health-2.2.4/pytest_repo_health.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-16 18:53:09.000000 pytest-repo-health-2.2.4/pytest_repo_health.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       47 2021-12-16 18:53:09.000000 pytest-repo-health-2.2.4/pytest_repo_health.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-16 18:53:09.000000 pytest-repo-health-2.2.4/pytest_repo_health.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       39 2021-12-16 18:53:09.000000 pytest-repo-health-2.2.4/pytest_repo_health.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2021-12-16 18:53:09.000000 pytest-repo-health-2.2.4/pytest_repo_health.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-16 18:53:09.000000 pytest-repo-health-2.2.4/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)      443 2021-12-16 18:53:06.000000 pytest-repo-health-2.2.4/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (121)     1101 2021-12-16 18:53:06.000000 pytest-repo-health-2.2.4/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-16 18:53:09.000000 pytest-repo-health-2.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     5648 2021-12-16 18:53:06.000000 pytest-repo-health-2.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 20:19:29.905156 pytest-repo-health-3.0.2/
+-rw-r--r--   0 runner    (1001) docker     (122)     2803 2023-04-17 20:19:22.000000 pytest-repo-health-3.0.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35135 2023-04-17 20:19:22.000000 pytest-repo-health-3.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      218 2023-04-17 20:19:22.000000 pytest-repo-health-3.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     7276 2023-04-17 20:19:29.905156 pytest-repo-health-3.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6525 2023-04-17 20:19:22.000000 pytest-repo-health-3.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 20:19:29.905156 pytest-repo-health-3.0.2/pytest_repo_health/
+-rw-r--r--   0 runner    (1001) docker     (122)     2433 2023-04-17 20:19:22.000000 pytest-repo-health-3.0.2/pytest_repo_health/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 20:19:29.905156 pytest-repo-health-3.0.2/pytest_repo_health/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-04-17 20:19:22.000000 pytest-repo-health-3.0.2/pytest_repo_health/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      990 2023-04-17 20:19:22.000000 pytest-repo-health-3.0.2/pytest_repo_health/fixtures/git.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2704 2023-04-17 20:19:22.000000 pytest-repo-health-3.0.2/pytest_repo_health/fixtures/github.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6893 2023-04-17 20:19:22.000000 pytest-repo-health-3.0.2/pytest_repo_health/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1308 2023-04-17 20:19:22.000000 pytest-repo-health-3.0.2/pytest_repo_health/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 20:19:29.905156 pytest-repo-health-3.0.2/pytest_repo_health.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     7276 2023-04-17 20:19:29.000000 pytest-repo-health-3.0.2/pytest_repo_health.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      599 2023-04-17 20:19:29.000000 pytest-repo-health-3.0.2/pytest_repo_health.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-17 20:19:29.000000 pytest-repo-health-3.0.2/pytest_repo_health.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-04-17 20:19:29.000000 pytest-repo-health-3.0.2/pytest_repo_health.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-17 20:19:29.000000 pytest-repo-health-3.0.2/pytest_repo_health.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       39 2023-04-17 20:19:29.000000 pytest-repo-health-3.0.2/pytest_repo_health.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-04-17 20:19:29.000000 pytest-repo-health-3.0.2/pytest_repo_health.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 20:19:29.905156 pytest-repo-health-3.0.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      443 2023-04-17 20:19:22.000000 pytest-repo-health-3.0.2/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1215 2023-04-17 20:19:22.000000 pytest-repo-health-3.0.2/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-17 20:19:29.905156 pytest-repo-health-3.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     5596 2023-04-17 20:19:22.000000 pytest-repo-health-3.0.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pytest-repo-health-2.2.4/CHANGELOG.rst` & `pytest-repo-health-3.0.2/CHANGELOG.rst`

 * *Files 17% similar despite different names*

```diff
@@ -10,94 +10,114 @@
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
-[2.2.4] - 2021-12-16
-~~~~~~~~~~~~~~~~~~~~
+
+3.0.2 - 2023-04-17
+~~~~~~~~~~~~~~~~~~
+
+* If a check is an ``async def``, but is not marked with
+  ``@pytest.mark.asyncio``, raise a true error, not just a warning that can be
+  lost in the logs.
+
+* Correct packaging errors.
+
+
+3.0.0 - 2022-10-13
+~~~~~~~~~~~~~~~~~~
+
+BREAKING CHANGE
+_______________
+
+* Dropped Python 3.7 support
+
+
+2.2.4 - 2021-12-16
+~~~~~~~~~~~~~~~~~~
 
 Fixed
 _____
 
 * Allow matching remote URL for .github repo
 
 
-[2.2.3] - 2021-11-23
-~~~~~~~~~~~~~~~~~~~~
+2.2.3 - 2021-11-23
+~~~~~~~~~~~~~~~~~~
 
 No change.
 
-[2.2.2] - 2021-11-23
-~~~~~~~~~~~~~~~~~~~~
+2.2.2 - 2021-11-23
+~~~~~~~~~~~~~~~~~~
 
 Removed
 _______
 
 * Removed Python 3.6 support as it is reaching end of life in December 2021
 
-[2.1.0] - 2020-11-03
-~~~~~~~~~~~~~~~~~~~~
+2.1.0 - 2020-11-03
+~~~~~~~~~~~~~~~~~~
 
 Added
 _____
 
 * Added ability to set filename for checks metadata file. You can now give a file path after --repo-health-metadata flag
 
-[2.0.1] - 2020-08-12
-~~~~~~~~~~~~~~~~~~~~
+2.0.1 - 2020-08-12
+~~~~~~~~~~~~~~~~~~
 
 Fixed
 _____
 
 * Fixed uploads to PyPI from Travis CI
 
-[2.0.0] - 2020-08-12
-~~~~~~~~~~~~~~~~~~~~
+2.0.0 - 2020-08-12
+~~~~~~~~~~~~~~~~~~
 
 Removed
 _______
 
 * Removed support for Python 3.5.  Versions 3.5.3 and above will likely still work for now, but they are no longer being tested; this lets us upgrade some dependencies and avoid confusion when aiohttp fails to install under 3.5.2 and below.  Python 3.5 reaches EOL in 1 month anyway.
 
 Fixed
 _____
 
 * Recent versions of github.py installed from source control are now supported (and recommended if you want to inspect a repository's code of conduct, as 0.5.0 has a bug that throws an exception when attempting this).
 * Checks can now be run on a ``.github`` repository (the regular expression used to parse out the organization and repository names didn't work with this before)
 
-[1.1.1] - 2020-07-21
-~~~~~~~~~~~~~~~~~~~~
+1.1.1 - 2020-07-21
+~~~~~~~~~~~~~~~~~~
 
 Fixed
 _____
 
 * Gracefully handle errors in fetching data from GitHub
 
-[1.1.0] - 2020-07-16
-~~~~~~~~~~~~~~~~~~~~
+1.1.0 - 2020-07-16
+~~~~~~~~~~~~~~~~~~
 
 Added
 _____
 
 * New fixtures that allow checks to easily fetch information about a git
   repository: ``git_repo`` and ``git_origin_url``
 
 * New fixtures that allow checks to easily fetch information from the GitHub API
   about the repository: ``github_client`` and ``github_repo``
 
-[1.0.0] - 2020-05-13
-~~~~~~~~~~~~~~~~~~~~
+1.0.0 - 2020-05-13
+~~~~~~~~~~~~~~~~~~
 
 Added
 _____
 
 * ``--repo-health-metadata`` option to collect metadata for each check and save it in a YAML file.
 
 * Added the current timestamp to the output (under ``TIMESTAMP``)
 
 
-[0.1.0] - 2020-04-13
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+0.1.0 - 2020-04-13
+~~~~~~~~~~~~~~~~~~
 
 Initial release.
```

### Comparing `pytest-repo-health-2.2.4/LICENSE` & `pytest-repo-health-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-repo-health-2.2.4/PKG-INFO` & `pytest-repo-health-3.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
 Name: pytest-repo-health
-Version: 2.2.4
+Version: 3.0.2
 Summary: A pytest plugin to report on repository standards conformance
 Home-page: https://github.com/edX/pytest-repo-health
 Author: edX
 Author-email: oscm@edx.org
 License: Apache Software License 2.0
 Keywords: pytest edx
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Topic :: Software Development :: Testing
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ==================
 pytest-repo-health
 ==================
 
 
@@ -30,16 +28,16 @@
     :target: https://pypi.org/project/pytest-repo-health
     :alt: PyPI version
 
 .. image:: https://img.shields.io/pypi/pyversions/pytest-repo-health.svg
     :target: https://pypi.org/project/pytest-repo-health
     :alt: Python versions
 
-.. image:: https://github.com/edx/pytest-repo-health/workflows/Python%20CI/badge.svg?branch=master
-    :target: https://github.com/edx/pytest-repo-health/actions?query=workflow%3A%22Python+CI%22
+.. image:: https://github.com/openedx/pytest-repo-health/workflows/Python%20CI/badge.svg?branch=master
+    :target: https://github.com/openedx/pytest-repo-health/actions?query=workflow%3A%22Python+CI%22
     :alt: CI
 
 .. image:: https://ci.appveyor.com/api/projects/status/github/edx/pytest-repo-health?branch=master
     :target: https://ci.appveyor.com/project/edx/pytest-repo-health/branch/master
     :alt: See Build Status on AppVeyor
 
 ----
@@ -68,17 +66,18 @@
 Usage
 -----
 
 Once installed, use this command to run checks::
 
     $ pytest -c <() --noconftest --repo-health --repo-health-path <path to dir with checks> --repo-path <path to repo to check>
 
-The -c and --noconftest options are needed to stop pytest from incorrectly reading configuration files in the repo you are checking.
+The -c and --noconftest options are needed to stop pytest from incorrectly reading configuration files in the repo you are checking::
 
     -c file: load configuration from `file` instead of trying to locate one of the implicit configuration files. Helpful if invocation dir defines "add-opts" in one of its files.
+
     --noconftest: Don't load any conftest.py files. Helpful in case invocation dir/repository has conftest files that change configurations or cause pytest to run unnecessary code.
 
 Other pytest options can be used.  For example, `-k` is helpful for running a subset of checks.
 
 The "all_results" dictionary will be written as YAML to repo_health.yaml.
 
 
@@ -93,22 +92,24 @@
 Checks naming convention:
 
 - python_functions = "check_*"
 - python_files = "check_*.py"
 
 Checks Discovery
 ----------------
+
 Pytest will look for checks in these directories, though it will only successfully run checks in the first place it finds them:
 - Dir of pytest invocation(so current dir)
 - Dir where pytest-repo-health is installed
 - Dir specified by --repo-health-path flag in pytest invocation
 
 
 Args
 ----
+
 Arguments added by plugin::
 
   --repo-health: this arg needs to be present for plugin to do anything
 
   --repo-path <dir path> : the path to dir on which to perform checks. If not preset, checks will be performed on current dir
 
   --repo-health-path <dir path>: path to where checks are located. If not preset, plugin will look for checks in current repo
@@ -139,27 +140,27 @@
 Please see ``LICENSE.txt`` for details.
 
 How To Contribute
 -----------------
 
 Contributions are very welcome.
 
-Please read `How To Contribute <https://github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details.
+Please read `How To Contribute <https://github.com/openedx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details.
 
 Even though they were written with ``edx-platform`` in mind, the guidelines
 should be followed for Open edX code in general.
 
 The pull request description template should be automatically applied if you are creating a pull request from GitHub.  Otherwise you
-can find it it at `PULL_REQUEST_TEMPLATE.md <https://github.com/edx/pytest-repo-health/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_
+can find it it at `PULL_REQUEST_TEMPLATE.md <https://github.com/openedx/pytest-repo-health/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_
 
 Issues
 ------
 
 The issue report template should be automatically applied if you are creating an issue on GitHub as well.  Otherwise you
-can find it at `ISSUE_TEMPLATE.md <https://github.com/edx/pytest-repo-health/blob/master/.github/ISSUE_TEMPLATE.md>`_
+can find it at `ISSUE_TEMPLATE.md <https://github.com/openedx/pytest-repo-health/blob/master/.github/ISSUE_TEMPLATE.md>`_
 
 
 If you encounter any problems, please `file an issue`_ along with a detailed description.
 
 Reporting Security Issues
 -------------------------
 
@@ -169,20 +170,19 @@
 Getting Help
 ------------
 
 Have a question about this repository, or about Open edX in general?  Please
 refer to this `list of resources`_ if you need any assistance.
 
 .. _list of resources: https://open.edx.org/getting-help
+.. _edx-repo-health: https://github.com/openedx/edx-repo-health
 .. _`Cookiecutter`: https://github.com/audreyr/cookiecutter
 .. _`@hackebrot`: https://github.com/hackebrot
 .. _`BSD-3`: http://opensource.org/licenses/BSD-3-Clause
 .. _`GNU GPL v3.0`: http://www.gnu.org/licenses/gpl-3.0.txt
 .. _`Apache Software License 2.0`: http://www.apache.org/licenses/LICENSE-2.0
 .. _`cookiecutter-pytest-plugin`: https://github.com/pytest-dev/cookiecutter-pytest-plugin
-.. _`file an issue`: https://github.com/edx/pytest-repo-health/issues
+.. _`file an issue`: https://github.com/openedx/pytest-repo-health/issues
 .. _`pytest`: https://github.com/pytest-dev/pytest
 .. _`tox`: https://tox.readthedocs.io/en/latest/
 .. _`pip`: https://pypi.org/project/pip/
 .. _`PyPI`: https://pypi.org/project
-
-
```

### Comparing `pytest-repo-health-2.2.4/README.rst` & `pytest-repo-health-3.0.2/pytest_repo_health.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,43 @@
+Metadata-Version: 2.1
+Name: pytest-repo-health
+Version: 3.0.2
+Summary: A pytest plugin to report on repository standards conformance
+Home-page: https://github.com/edX/pytest-repo-health
+Author: edX
+Author-email: oscm@edx.org
+License: Apache Software License 2.0
+Keywords: pytest edx
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Natural Language :: English
+Classifier: Topic :: Software Development :: Testing
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
 ==================
 pytest-repo-health
 ==================
 
 
 .. image:: https://img.shields.io/pypi/v/pytest-repo-health.svg
     :target: https://pypi.org/project/pytest-repo-health
     :alt: PyPI version
 
 .. image:: https://img.shields.io/pypi/pyversions/pytest-repo-health.svg
     :target: https://pypi.org/project/pytest-repo-health
     :alt: Python versions
 
-.. image:: https://github.com/edx/pytest-repo-health/workflows/Python%20CI/badge.svg?branch=master
-    :target: https://github.com/edx/pytest-repo-health/actions?query=workflow%3A%22Python+CI%22
+.. image:: https://github.com/openedx/pytest-repo-health/workflows/Python%20CI/badge.svg?branch=master
+    :target: https://github.com/openedx/pytest-repo-health/actions?query=workflow%3A%22Python+CI%22
     :alt: CI
 
 .. image:: https://ci.appveyor.com/api/projects/status/github/edx/pytest-repo-health?branch=master
     :target: https://ci.appveyor.com/project/edx/pytest-repo-health/branch/master
     :alt: See Build Status on AppVeyor
 
 ----
@@ -45,17 +66,18 @@
 Usage
 -----
 
 Once installed, use this command to run checks::
 
     $ pytest -c <() --noconftest --repo-health --repo-health-path <path to dir with checks> --repo-path <path to repo to check>
 
-The -c and --noconftest options are needed to stop pytest from incorrectly reading configuration files in the repo you are checking.
+The -c and --noconftest options are needed to stop pytest from incorrectly reading configuration files in the repo you are checking::
 
     -c file: load configuration from `file` instead of trying to locate one of the implicit configuration files. Helpful if invocation dir defines "add-opts" in one of its files.
+
     --noconftest: Don't load any conftest.py files. Helpful in case invocation dir/repository has conftest files that change configurations or cause pytest to run unnecessary code.
 
 Other pytest options can be used.  For example, `-k` is helpful for running a subset of checks.
 
 The "all_results" dictionary will be written as YAML to repo_health.yaml.
 
 
@@ -70,22 +92,24 @@
 Checks naming convention:
 
 - python_functions = "check_*"
 - python_files = "check_*.py"
 
 Checks Discovery
 ----------------
+
 Pytest will look for checks in these directories, though it will only successfully run checks in the first place it finds them:
 - Dir of pytest invocation(so current dir)
 - Dir where pytest-repo-health is installed
 - Dir specified by --repo-health-path flag in pytest invocation
 
 
 Args
 ----
+
 Arguments added by plugin::
 
   --repo-health: this arg needs to be present for plugin to do anything
 
   --repo-path <dir path> : the path to dir on which to perform checks. If not preset, checks will be performed on current dir
 
   --repo-health-path <dir path>: path to where checks are located. If not preset, plugin will look for checks in current repo
@@ -116,27 +140,27 @@
 Please see ``LICENSE.txt`` for details.
 
 How To Contribute
 -----------------
 
 Contributions are very welcome.
 
-Please read `How To Contribute <https://github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details.
+Please read `How To Contribute <https://github.com/openedx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details.
 
 Even though they were written with ``edx-platform`` in mind, the guidelines
 should be followed for Open edX code in general.
 
 The pull request description template should be automatically applied if you are creating a pull request from GitHub.  Otherwise you
-can find it it at `PULL_REQUEST_TEMPLATE.md <https://github.com/edx/pytest-repo-health/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_
+can find it it at `PULL_REQUEST_TEMPLATE.md <https://github.com/openedx/pytest-repo-health/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_
 
 Issues
 ------
 
 The issue report template should be automatically applied if you are creating an issue on GitHub as well.  Otherwise you
-can find it at `ISSUE_TEMPLATE.md <https://github.com/edx/pytest-repo-health/blob/master/.github/ISSUE_TEMPLATE.md>`_
+can find it at `ISSUE_TEMPLATE.md <https://github.com/openedx/pytest-repo-health/blob/master/.github/ISSUE_TEMPLATE.md>`_
 
 
 If you encounter any problems, please `file an issue`_ along with a detailed description.
 
 Reporting Security Issues
 -------------------------
 
@@ -146,18 +170,19 @@
 Getting Help
 ------------
 
 Have a question about this repository, or about Open edX in general?  Please
 refer to this `list of resources`_ if you need any assistance.
 
 .. _list of resources: https://open.edx.org/getting-help
+.. _edx-repo-health: https://github.com/openedx/edx-repo-health
 .. _`Cookiecutter`: https://github.com/audreyr/cookiecutter
 .. _`@hackebrot`: https://github.com/hackebrot
 .. _`BSD-3`: http://opensource.org/licenses/BSD-3-Clause
 .. _`GNU GPL v3.0`: http://www.gnu.org/licenses/gpl-3.0.txt
 .. _`Apache Software License 2.0`: http://www.apache.org/licenses/LICENSE-2.0
 .. _`cookiecutter-pytest-plugin`: https://github.com/pytest-dev/cookiecutter-pytest-plugin
-.. _`file an issue`: https://github.com/edx/pytest-repo-health/issues
+.. _`file an issue`: https://github.com/openedx/pytest-repo-health/issues
 .. _`pytest`: https://github.com/pytest-dev/pytest
 .. _`tox`: https://tox.readthedocs.io/en/latest/
 .. _`pip`: https://pypi.org/project/pip/
 .. _`PyPI`: https://pypi.org/project
```

### Comparing `pytest-repo-health-2.2.4/pytest_repo_health/__init__.py` & `pytest-repo-health-3.0.2/pytest_repo_health/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Plugin configures pytest to run repo health checks on a code repository.
 Plugin takes care of gathering checks, running checks,
 and outputting report based on data gathered during checks.
 """
 from typing import Union
 
-__version__ = "2.2.4"
+__version__ = "3.0.2"
 
 
 def health_metadata(parent_path: list, output_keys: dict):
     """
     Make a decorator that attaches metadata to the target function.
 
     ``output_keys`` is a dictionary that documents the output keys of the checker.
```

### Comparing `pytest-repo-health-2.2.4/pytest_repo_health/fixtures/git.py` & `pytest-repo-health-3.0.2/pytest_repo_health/fixtures/git.py`

 * *Files identical despite different names*

### Comparing `pytest-repo-health-2.2.4/pytest_repo_health/fixtures/github.py` & `pytest-repo-health-3.0.2/pytest_repo_health/fixtures/github.py`

 * *Files identical despite different names*

### Comparing `pytest-repo-health-2.2.4/pytest_repo_health/plugin.py` & `pytest-repo-health-3.0.2/pytest_repo_health/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 """
 pytest plugin to test if specific repo follows standards
 """
+
+import datetime
 import os
+import warnings
 from collections import defaultdict
-import datetime
 
 import pytest
 import yaml
 
 from .fixtures.git import git_origin_url, git_repo  # pylint: disable=unused-import
 from .fixtures.github import github_client, github_repo  # pylint: disable=unused-import
 from .utils import get_repo_remote_name
 
 session_data_holder_dict = defaultdict(dict)
 session_data_holder_dict["TIMESTAMP"] = datetime.datetime.now().date()
 
 
+@pytest.fixture(autouse=True)
+def set_warnings() -> None:
+    """Force asyncio mistakes to be errors"""
+    warnings.simplefilter("error", pytest.PytestUnhandledCoroutineWarning)
+
+
 @pytest.fixture(scope="session")
 def all_results():
     return session_data_holder_dict
 
 
 def pytest_configure(config):
     """
```

### Comparing `pytest-repo-health-2.2.4/pytest_repo_health/utils.py` & `pytest-repo-health-3.0.2/pytest_repo_health/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Assumes the last slash-separated component of the remote URL is the
 # name of the repo, providing for a possible extra `.git` or an extra
 # forward slash at the end. This works for Github's path structure
 # (which is what we need) but should also work for various other
 # remotes.
 #
 # Examples:
-# - https://github.com/edx/edx-platform.git
+# - https://github.com/openedx/edx-platform.git
 # - git@github.com:edx/edx-platform.git
 URL_PATTERN = r"^(git@|https://).*/(?P<repo_name>[a-zA-Z0-9_\-.]+?)(\.git)?/?$"
 
 
 def get_repo_remote_name(repo_path):
     """
     Returns the repo name from the remote url for the repo_path provided.
```

### Comparing `pytest-repo-health-2.2.4/pytest_repo_health.egg-info/PKG-INFO` & `pytest-repo-health-3.0.2/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,22 @@
-Metadata-Version: 2.1
-Name: pytest-repo-health
-Version: 2.2.4
-Summary: A pytest plugin to report on repository standards conformance
-Home-page: https://github.com/edX/pytest-repo-health
-Author: edX
-Author-email: oscm@edx.org
-License: Apache Software License 2.0
-Keywords: pytest edx
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Natural Language :: English
-Classifier: Topic :: Software Development :: Testing
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ==================
 pytest-repo-health
 ==================
 
 
 .. image:: https://img.shields.io/pypi/v/pytest-repo-health.svg
     :target: https://pypi.org/project/pytest-repo-health
     :alt: PyPI version
 
 .. image:: https://img.shields.io/pypi/pyversions/pytest-repo-health.svg
     :target: https://pypi.org/project/pytest-repo-health
     :alt: Python versions
 
-.. image:: https://github.com/edx/pytest-repo-health/workflows/Python%20CI/badge.svg?branch=master
-    :target: https://github.com/edx/pytest-repo-health/actions?query=workflow%3A%22Python+CI%22
+.. image:: https://github.com/openedx/pytest-repo-health/workflows/Python%20CI/badge.svg?branch=master
+    :target: https://github.com/openedx/pytest-repo-health/actions?query=workflow%3A%22Python+CI%22
     :alt: CI
 
 .. image:: https://ci.appveyor.com/api/projects/status/github/edx/pytest-repo-health?branch=master
     :target: https://ci.appveyor.com/project/edx/pytest-repo-health/branch/master
     :alt: See Build Status on AppVeyor
 
 ----
@@ -68,17 +45,18 @@
 Usage
 -----
 
 Once installed, use this command to run checks::
 
     $ pytest -c <() --noconftest --repo-health --repo-health-path <path to dir with checks> --repo-path <path to repo to check>
 
-The -c and --noconftest options are needed to stop pytest from incorrectly reading configuration files in the repo you are checking.
+The -c and --noconftest options are needed to stop pytest from incorrectly reading configuration files in the repo you are checking::
 
     -c file: load configuration from `file` instead of trying to locate one of the implicit configuration files. Helpful if invocation dir defines "add-opts" in one of its files.
+
     --noconftest: Don't load any conftest.py files. Helpful in case invocation dir/repository has conftest files that change configurations or cause pytest to run unnecessary code.
 
 Other pytest options can be used.  For example, `-k` is helpful for running a subset of checks.
 
 The "all_results" dictionary will be written as YAML to repo_health.yaml.
 
 
@@ -93,22 +71,24 @@
 Checks naming convention:
 
 - python_functions = "check_*"
 - python_files = "check_*.py"
 
 Checks Discovery
 ----------------
+
 Pytest will look for checks in these directories, though it will only successfully run checks in the first place it finds them:
 - Dir of pytest invocation(so current dir)
 - Dir where pytest-repo-health is installed
 - Dir specified by --repo-health-path flag in pytest invocation
 
 
 Args
 ----
+
 Arguments added by plugin::
 
   --repo-health: this arg needs to be present for plugin to do anything
 
   --repo-path <dir path> : the path to dir on which to perform checks. If not preset, checks will be performed on current dir
 
   --repo-health-path <dir path>: path to where checks are located. If not preset, plugin will look for checks in current repo
@@ -139,27 +119,27 @@
 Please see ``LICENSE.txt`` for details.
 
 How To Contribute
 -----------------
 
 Contributions are very welcome.
 
-Please read `How To Contribute <https://github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details.
+Please read `How To Contribute <https://github.com/openedx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details.
 
 Even though they were written with ``edx-platform`` in mind, the guidelines
 should be followed for Open edX code in general.
 
 The pull request description template should be automatically applied if you are creating a pull request from GitHub.  Otherwise you
-can find it it at `PULL_REQUEST_TEMPLATE.md <https://github.com/edx/pytest-repo-health/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_
+can find it it at `PULL_REQUEST_TEMPLATE.md <https://github.com/openedx/pytest-repo-health/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_
 
 Issues
 ------
 
 The issue report template should be automatically applied if you are creating an issue on GitHub as well.  Otherwise you
-can find it at `ISSUE_TEMPLATE.md <https://github.com/edx/pytest-repo-health/blob/master/.github/ISSUE_TEMPLATE.md>`_
+can find it at `ISSUE_TEMPLATE.md <https://github.com/openedx/pytest-repo-health/blob/master/.github/ISSUE_TEMPLATE.md>`_
 
 
 If you encounter any problems, please `file an issue`_ along with a detailed description.
 
 Reporting Security Issues
 -------------------------
 
@@ -169,20 +149,19 @@
 Getting Help
 ------------
 
 Have a question about this repository, or about Open edX in general?  Please
 refer to this `list of resources`_ if you need any assistance.
 
 .. _list of resources: https://open.edx.org/getting-help
+.. _edx-repo-health: https://github.com/openedx/edx-repo-health
 .. _`Cookiecutter`: https://github.com/audreyr/cookiecutter
 .. _`@hackebrot`: https://github.com/hackebrot
 .. _`BSD-3`: http://opensource.org/licenses/BSD-3-Clause
 .. _`GNU GPL v3.0`: http://www.gnu.org/licenses/gpl-3.0.txt
 .. _`Apache Software License 2.0`: http://www.apache.org/licenses/LICENSE-2.0
 .. _`cookiecutter-pytest-plugin`: https://github.com/pytest-dev/cookiecutter-pytest-plugin
-.. _`file an issue`: https://github.com/edx/pytest-repo-health/issues
+.. _`file an issue`: https://github.com/openedx/pytest-repo-health/issues
 .. _`pytest`: https://github.com/pytest-dev/pytest
 .. _`tox`: https://tox.readthedocs.io/en/latest/
 .. _`pip`: https://pypi.org/project/pip/
 .. _`PyPI`: https://pypi.org/project
-
-
```

### Comparing `pytest-repo-health-2.2.4/pytest_repo_health.egg-info/SOURCES.txt` & `pytest-repo-health-3.0.2/pytest_repo_health.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-repo-health-2.2.4/requirements/constraints.txt` & `pytest-repo-health-3.0.2/requirements/constraints.txt`

 * *Files 13% similar despite different names*

```diff
@@ -7,20 +7,22 @@
 # link to other information that will help people in the future to remove the
 # pin when possible.  Writing an issue against the offending project and
 # linking to it here is good.
 
 # Common constraints for edx repos
 -c https://raw.githubusercontent.com/edx/edx-lint/master/edx_lint/files/common_constraints.txt
  
-# Tox and virtualenv require importlib-metadata<3.0 to support python3.5
-# so pinning until both packages drop support for python3.5 &
-# update their required importlib-metadata version constraint
-importlib-metadata<3.0
-
 # aiohttp latest version 3.7.3 requires chardet<4.0, can be removed once aiohttp==4.0.0 is released.
 chardet<4.0
 
 # diff-cover==4.2.0 requires chardet==4.0.0 which is pinned due to aiohttp issue
 diff-cover<4.2.0
 
 # requests has a constraint idna<3 in it, so pinning it unless requests updates the constraint
 idna<3.0
+
+# requests has a constraint charset-normalizer~=2.0.0 which so the version can't be bumped for now.
+charset-normalizer~=2.0.0
+
+# importlib_metadata is constrained in pycodestyle. This can be removed once the upstream constraint is resolved.
+# https://github.com/PyCQA/pydocstyle/blob/master/pyproject.toml#L25
+importlib-metadata<5.0.0
```

### Comparing `pytest-repo-health-2.2.4/setup.py` & `pytest-repo-health-3.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -114,30 +114,29 @@
     name='pytest-repo-health',
     version=VERSION,
     author='edX',
     author_email='oscm@edx.org',
     url='https://github.com/edX/pytest-repo-health',
     description='A pytest plugin to report on repository standards conformance',
     long_description=read('README.rst'),
-    long_description_content_type="text/markdown",
+    long_description_content_type="text/x-rst",
     packages=find_packages(exclude=["tests"]),
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     install_requires=load_requirements('requirements/base.in'),
     zip_safe=False,
     keywords='pytest edx',
     license="Apache Software License 2.0",
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Natural Language :: English',
         'Topic :: Software Development :: Testing',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
     ],
     entry_points={
         'pytest11': [
             'plugin = pytest_repo_health.plugin',
         ],
     },
```

