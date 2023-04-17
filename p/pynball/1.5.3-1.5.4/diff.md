# Comparing `tmp/pynball-1.5.3.tar.gz` & `tmp/pynball-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynball-1.5.3.tar", last modified: Sun Apr  9 07:36:17 2023, max compression
+gzip compressed data, was "pynball-1.5.4.tar", last modified: Mon Apr 17 18:23:42 2023, max compression
```

## Comparing `pynball-1.5.3.tar` & `pynball-1.5.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 07:36:17.140355 pynball-1.5.3/
--rw-rw-rw-   0        0        0      155 2022-07-17 14:14:50.000000 pynball-1.5.3/AUTHORS.md
--rw-rw-rw-   0        0        0     6404 2023-04-09 07:36:04.000000 pynball-1.5.3/CHANGELOG.md
--rw-rw-rw-   0        0        0     1074 2022-05-31 13:06:01.000000 pynball-1.5.3/LICENSE
--rw-rw-rw-   0        0        0      203 2022-07-17 14:14:50.000000 pynball-1.5.3/MANIFEST.in
--rw-rw-rw-   0        0        0    12054 2023-04-09 07:36:17.140355 pynball-1.5.3/PKG-INFO
--rw-rw-rw-   0        0        0    10737 2023-04-09 07:31:38.000000 pynball-1.5.3/README.md
--rw-rw-rw-   0        0        0     2212 2022-10-08 17:05:50.000000 pynball-1.5.3/pyproject.toml
--rw-rw-rw-   0        0        0     1550 2023-04-09 07:36:17.155982 pynball-1.5.3/setup.cfg
--rw-rw-rw-   0        0        0      108 2022-05-31 13:06:01.000000 pynball-1.5.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-09 07:36:16.959407 pynball-1.5.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-09 07:36:16.993249 pynball-1.5.3/src/pynball/
--rw-rw-rw-   0        0        0      269 2023-04-09 07:36:04.000000 pynball-1.5.3/src/pynball/__init__.py
--rw-rw-rw-   0        0        0    30835 2023-04-06 18:58:07.000000 pynball-1.5.3/src/pynball/pynball.py
-drwxrwxrwx   0        0        0        0 2023-04-09 07:36:17.008911 pynball-1.5.3/src/pynball.egg-info/
--rw-rw-rw-   0        0        0    12054 2023-04-09 07:36:16.000000 pynball-1.5.3/src/pynball.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      693 2023-04-09 07:36:16.000000 pynball-1.5.3/src/pynball.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 07:36:16.000000 pynball-1.5.3/src/pynball.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-04-09 07:36:16.000000 pynball-1.5.3/src/pynball.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       45 2023-04-09 07:36:16.000000 pynball-1.5.3/src/pynball.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-09 07:36:16.000000 pynball-1.5.3/src/pynball.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-09 07:36:17.140355 pynball-1.5.3/tests/
--rw-rw-rw-   0        0        0      574 2022-03-26 17:49:23.000000 pynball-1.5.3/tests/test__check_pyenv.py
--rw-rw-rw-   0        0        0     1159 2022-03-26 17:49:24.000000 pynball-1.5.3/tests/test__check_virtual_env.py
--rw-rw-rw-   0        0        0      374 2022-03-26 17:46:41.000000 pynball-1.5.3/tests/test__execute.py
--rw-rw-rw-   0        0        0     3502 2023-04-05 14:01:44.000000 pynball-1.5.3/tests/test__get_pynball.py
--rw-rw-rw-   0        0        0      759 2022-03-26 13:16:29.000000 pynball-1.5.3/tests/test__message.py
--rw-rw-rw-   0        0        0     1802 2022-04-04 12:59:03.000000 pynball-1.5.3/tests/test__set_get_del_env.py
--rw-rw-rw-   0        0        0      437 2022-04-03 21:08:13.000000 pynball-1.5.3/tests/test__set_pynball.py
--rw-rw-rw-   0        0        0     1183 2022-03-26 22:14:26.000000 pynball-1.5.3/tests/test_add.py
--rw-rw-rw-   0        0        0      630 2022-04-03 21:08:13.000000 pynball-1.5.3/tests/test_delete.py
--rw-rw-rw-   0        0        0      869 2022-04-06 20:25:30.000000 pynball-1.5.3/tests/test_lsproject.py
--rw-rw-rw-   0        0        0     1714 2022-03-27 15:36:00.000000 pynball-1.5.3/tests/test_mkproject.py
--rw-rw-rw-   0        0        0     1442 2022-03-27 15:34:50.000000 pynball-1.5.3/tests/test_rmproject.py
--rw-rw-rw-   0        0        0      418 2023-04-05 14:49:56.000000 pynball-1.5.3/tests/test_version.py
--rw-rw-rw-   0        0        0     1014 2023-04-05 14:01:44.000000 pynball-1.5.3/tests/test_versions.py
+drwxrwxrwx   0        0        0        0 2023-04-17 18:23:42.413279 pynball-1.5.4/
+-rw-rw-rw-   0        0        0      155 2022-07-17 14:14:50.000000 pynball-1.5.4/AUTHORS.md
+-rw-rw-rw-   0        0        0     7122 2023-04-17 18:23:29.000000 pynball-1.5.4/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1075 2023-04-09 16:05:23.000000 pynball-1.5.4/LICENSE
+-rw-rw-rw-   0        0        0      203 2022-07-17 14:14:50.000000 pynball-1.5.4/MANIFEST.in
+-rw-rw-rw-   0        0        0    12584 2023-04-17 18:23:42.413279 pynball-1.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0    11247 2023-04-17 14:12:33.000000 pynball-1.5.4/README.md
+-rw-rw-rw-   0        0        0     2212 2022-10-08 17:05:50.000000 pynball-1.5.4/pyproject.toml
+-rw-rw-rw-   0        0        0     1550 2023-04-17 18:23:42.415290 pynball-1.5.4/setup.cfg
+-rw-rw-rw-   0        0        0      108 2022-05-31 13:06:01.000000 pynball-1.5.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 18:23:42.298413 pynball-1.5.4/src/
+drwxrwxrwx   0        0        0        0 2023-04-17 18:23:42.339531 pynball-1.5.4/src/pynball/
+-rw-rw-rw-   0        0        0      269 2023-04-17 18:23:29.000000 pynball-1.5.4/src/pynball/__init__.py
+-rw-rw-rw-   0        0        0    31282 2023-04-17 18:18:09.000000 pynball-1.5.4/src/pynball/pynball.py
+drwxrwxrwx   0        0        0        0 2023-04-17 18:23:42.347532 pynball-1.5.4/src/pynball.egg-info/
+-rw-rw-rw-   0        0        0    12584 2023-04-17 18:23:42.000000 pynball-1.5.4/src/pynball.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      693 2023-04-17 18:23:42.000000 pynball-1.5.4/src/pynball.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 18:23:42.000000 pynball-1.5.4/src/pynball.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-04-17 18:23:42.000000 pynball-1.5.4/src/pynball.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       45 2023-04-17 18:23:42.000000 pynball-1.5.4/src/pynball.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-17 18:23:42.000000 pynball-1.5.4/src/pynball.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 18:23:42.411280 pynball-1.5.4/tests/
+-rw-rw-rw-   0        0        0      574 2022-03-26 17:49:23.000000 pynball-1.5.4/tests/test__check_pyenv.py
+-rw-rw-rw-   0        0        0     1159 2022-03-26 17:49:24.000000 pynball-1.5.4/tests/test__check_virtual_env.py
+-rw-rw-rw-   0        0        0      374 2022-03-26 17:46:41.000000 pynball-1.5.4/tests/test__execute.py
+-rw-rw-rw-   0        0        0     3502 2023-04-05 14:01:44.000000 pynball-1.5.4/tests/test__get_pynball.py
+-rw-rw-rw-   0        0        0      759 2022-03-26 13:16:29.000000 pynball-1.5.4/tests/test__message.py
+-rw-rw-rw-   0        0        0     1802 2022-04-04 12:59:03.000000 pynball-1.5.4/tests/test__set_get_del_env.py
+-rw-rw-rw-   0        0        0      437 2022-04-03 21:08:13.000000 pynball-1.5.4/tests/test__set_pynball.py
+-rw-rw-rw-   0        0        0     1183 2022-03-26 22:14:26.000000 pynball-1.5.4/tests/test_add.py
+-rw-rw-rw-   0        0        0      630 2022-04-03 21:08:13.000000 pynball-1.5.4/tests/test_delete.py
+-rw-rw-rw-   0        0        0      869 2022-04-06 20:25:30.000000 pynball-1.5.4/tests/test_lsproject.py
+-rw-rw-rw-   0        0        0     1714 2022-03-27 15:36:00.000000 pynball-1.5.4/tests/test_mkproject.py
+-rw-rw-rw-   0        0        0     1442 2022-03-27 15:34:50.000000 pynball-1.5.4/tests/test_rmproject.py
+-rw-rw-rw-   0        0        0      418 2023-04-05 14:49:56.000000 pynball-1.5.4/tests/test_version.py
+-rw-rw-rw-   0        0        0     1014 2023-04-05 14:01:44.000000 pynball-1.5.4/tests/test_versions.py
```

### Comparing `pynball-1.5.3/CHANGELOG.md` & `pynball-1.5.4/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.5.4 (2023-04-17)
+### Fix
+* File open encoding error ([`4304034`](https://github.com/Stephen-RA-King/pynball/commit/4304034b56d81cb34ffce552294a20a07fd55ea7))
+
+### Documentation
+* Rename base cookiecutter ([`9db5538`](https://github.com/Stephen-RA-King/pynball/commit/9db5538bfecb24210b138997f4efaeb7f3ffef34))
+* Update meta ([`5275172`](https://github.com/Stephen-RA-King/pynball/commit/52751725028692807284dc65ac8101781bd30e50))
+* Add pre-coomit.ci badge and docs sections ([`71ef0a6`](https://github.com/Stephen-RA-King/pynball/commit/71ef0a654672246a7db13b9e038dbf87c8d74c36))
+* Correct type ([`5e350d2`](https://github.com/Stephen-RA-King/pynball/commit/5e350d27199ba2d80f86eb23a02edbf34249125a))
+
 ## v1.5.3 (2023-04-09)
 ### Fix
 * Missing url links ([`c7209ee`](https://github.com/Stephen-RA-King/pynball/commit/c7209eeeb1e09ea8cc35049d5d7deabd94104cc1))
 
 ## v1.5.2 (2023-04-08)
 ### Documentation
 * Add mnissing docstrings to functions ([`d19176f`](https://github.com/Stephen-RA-King/pynball/commit/d19176f36d3abe491f006757600bc87a885bbb20))
```

### Comparing `pynball-1.5.3/LICENSE` & `pynball-1.5.4/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -10,12 +10,12 @@
 furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all
 copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+FITNESS FOR A PARTICULAR PURPOSE AND NON INFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `pynball-1.5.3/PKG-INFO` & `pynball-1.5.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynball
-Version: 1.5.3
+Version: 1.5.4
 Summary: Utility command line tool to manage python versions
 Home-page: https://github.com/stephen-ra-king/pynball
 Download-URL: 
 Author: Stephen R A King
 Author-email: stephen.ra.king@gmail.com
 Maintainer: Stephen R A King
 Maintainer-email: stephen.ra.king@gmail.com
@@ -34,14 +34,15 @@
 [![PyPI][pypi-image]][pypi-url]
 [![Downloads][downloads-image]][downloads-url]
 [![Status][status-image]][pypi-url]
 [![Python Version][python-version-image]][pypi-url]
 [![Format][format-image]][pypi-url]
 [![tests][tests-image]][tests-url]
 [![Codecov][codecov-image]][codecov-url]
+[![pre-commit.ci][pre-commit.ci-image]][pre-commit.ci-url]
 [![CodeFactor][codefactor-image]][codefactor-url]
 [![Codeclimate][codeclimate-image]][codeclimate-url]
 [![CodeQl][codeql-image]][codeql-url]
 [![readthedocs][readthedocs-image]][readthedocs-url]
 [![pre-commit][pre-commit-image]][pre-commit-url]
 [![Imports: isort][isort-image]][isort-url]
 [![Code style: black][black-image]][black-url]
@@ -56,46 +57,54 @@
 
 You may have a requirement for development on various versions of Python.
 Or you may have a mixture of installations including pyenv, custom installations,
 system installations etc. Pynball can make leveraging such environments a lot easier.
 
 ## Features
 
+---
+
 - Consolidates all Python installations including [**pyenv**][pyenv-url] into one management system
 - Easily create Virtual Environments using any Python version.
 - Track which virtual environments have which Python versions and tox versions.
 - Quickly change the System interpreter
 
 ## Pre Installation Requirements
 
+---
+
 #### Minimum Requirements
 
 1. Python 3.8+
 2. [**pipx**][pipx-url]
 3. [**Virtualenv**][virtualenv-url] (which has benefits over venv)
 4. [**Virtualenvwrapper**][virtualenvwrapper-url]
 
 #### For Maximum Benefits additionally install the following:
 
 1. [**pyenv**][pyenv-url]
 
 ## Installation
 
+---
+
 **OS X & Linux:**
 
 Will be supported in version 2
 
 **Windows:**
 
 ```sh
 pipx install pynball
 ```
 
 ## Usage example
 
+---
+
 ### View Available commands
 
 ```sh
 pynball
 Usage: pynball [OPTIONS] COMMAND [ARGS]...
 
   Utility script to help manage development with various versions of Python in
@@ -229,39 +238,50 @@
 3.6.8     D:\PYTHON\3.6.8 : --> System Interpreter
 3.5.4     D:\PYTHON\3.5.4
 3.5.2     C:\Users\conta\.pyenv\pyenv-win\versions\3.5.2
 ```
 
 _For more information, please refer to the wiki_
 
-## [Wiki][wiki]
-
 ## Documentation
 
+---
+
 [**Read the Docs**](https://pynball.readthedocs.io/en/latest/?)
 
+- [**Example Usage**](https://pynball.readthedocs.io/en/latest/example.html)
+- [**Credits**](https://pynball.readthedocs.io/en/latest/example.html)
+- [**Changelog**](https://pynball.readthedocs.io/en/latest/changelog.html)
+- [**API Reference**](https://pynball.readthedocs.io/en/latest/autoapi/index.html)
+
+- [**Wiki**][wiki]
+
 ## Meta
 
+---
+
 [![](assets/linkedin.png)](https://www.linkedin.com/in/sr-king)
 [![](assets/github.png)](https://github.com/Stephen-RA-King)
 [![](assets/pypi.png)](https://pypi.org/project/pynball)
 [![](assets/www.png)](https://www.justpython.tech)
 [![](assets/email.png)](mailto:sking.github@gmail.com)
 
-Author: Stephen R A King
+Stephen R A King : sking.github@gmail.com
+
+Distributed under the MIT license. See [![][license-image]][license-url] for more information.
 
-Distributed under the MIT License. See `LICENSE` for more information.
+Created with Cookiecutter template: [**pydough**][pydough-url] version 1.2.1
 
 <!-- Markdown link & img dfn's -->
 
 [bandit-image]: https://img.shields.io/badge/security-bandit-yellow.svg
 [bandit-url]: https://github.com/PyCQA/bandit
 [black-image]: https://img.shields.io/badge/code%20style-black-000000.svg
 [black-url]: https://github.com/psf/black
-[cc_template-url]: https://github.com/Stephen-RA-King/cc_template
+[pydough-url]: https://github.com/Stephen-RA-King/pydough
 [codeclimate-image]: https://api.codeclimate.com/v1/badges/9543c409696e9976a987/maintainability
 [codeclimate-url]: https://codeclimate.com/github/Stephen-RA-King/pynball/maintainability
 [codecov-image]: https://codecov.io/gh/Stephen-RA-King/pynball/branch/main/graph/badge.svg
 [codecov-url]: https://app.codecov.io/gh/Stephen-RA-King/pynball
 [codefactor-image]: https://www.codefactor.io/repository/github/Stephen-RA-King/pynball/badge
 [codefactor-url]: https://www.codefactor.io/repository/github/Stephen-RA-King/pynball
 [codeql-image]: https://github.com/Stephen-RA-King/pynball/actions/workflows/github-code-scanning/codeql/badge.svg
```

### Comparing `pynball-1.5.3/README.md` & `pynball-1.5.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 [![PyPI][pypi-image]][pypi-url]
 [![Downloads][downloads-image]][downloads-url]
 [![Status][status-image]][pypi-url]
 [![Python Version][python-version-image]][pypi-url]
 [![Format][format-image]][pypi-url]
 [![tests][tests-image]][tests-url]
 [![Codecov][codecov-image]][codecov-url]
+[![pre-commit.ci][pre-commit.ci-image]][pre-commit.ci-url]
 [![CodeFactor][codefactor-image]][codefactor-url]
 [![Codeclimate][codeclimate-image]][codeclimate-url]
 [![CodeQl][codeql-image]][codeql-url]
 [![readthedocs][readthedocs-image]][readthedocs-url]
 [![pre-commit][pre-commit-image]][pre-commit-url]
 [![Imports: isort][isort-image]][isort-url]
 [![Code style: black][black-image]][black-url]
@@ -27,46 +28,54 @@
 
 You may have a requirement for development on various versions of Python.
 Or you may have a mixture of installations including pyenv, custom installations,
 system installations etc. Pynball can make leveraging such environments a lot easier.
 
 ## Features
 
+---
+
 - Consolidates all Python installations including [**pyenv**][pyenv-url] into one management system
 - Easily create Virtual Environments using any Python version.
 - Track which virtual environments have which Python versions and tox versions.
 - Quickly change the System interpreter
 
 ## Pre Installation Requirements
 
+---
+
 #### Minimum Requirements
 
 1. Python 3.8+
 2. [**pipx**][pipx-url]
 3. [**Virtualenv**][virtualenv-url] (which has benefits over venv)
 4. [**Virtualenvwrapper**][virtualenvwrapper-url]
 
 #### For Maximum Benefits additionally install the following:
 
 1. [**pyenv**][pyenv-url]
 
 ## Installation
 
+---
+
 **OS X & Linux:**
 
 Will be supported in version 2
 
 **Windows:**
 
 ```sh
 pipx install pynball
 ```
 
 ## Usage example
 
+---
+
 ### View Available commands
 
 ```sh
 pynball
 Usage: pynball [OPTIONS] COMMAND [ARGS]...
 
   Utility script to help manage development with various versions of Python in
@@ -200,39 +209,50 @@
 3.6.8     D:\PYTHON\3.6.8 : --> System Interpreter
 3.5.4     D:\PYTHON\3.5.4
 3.5.2     C:\Users\conta\.pyenv\pyenv-win\versions\3.5.2
 ```
 
 _For more information, please refer to the wiki_
 
-## [Wiki][wiki]
-
 ## Documentation
 
+---
+
 [**Read the Docs**](https://pynball.readthedocs.io/en/latest/?)
 
+- [**Example Usage**](https://pynball.readthedocs.io/en/latest/example.html)
+- [**Credits**](https://pynball.readthedocs.io/en/latest/example.html)
+- [**Changelog**](https://pynball.readthedocs.io/en/latest/changelog.html)
+- [**API Reference**](https://pynball.readthedocs.io/en/latest/autoapi/index.html)
+
+- [**Wiki**][wiki]
+
 ## Meta
 
+---
+
 [![](assets/linkedin.png)](https://www.linkedin.com/in/sr-king)
 [![](assets/github.png)](https://github.com/Stephen-RA-King)
 [![](assets/pypi.png)](https://pypi.org/project/pynball)
 [![](assets/www.png)](https://www.justpython.tech)
 [![](assets/email.png)](mailto:sking.github@gmail.com)
 
-Author: Stephen R A King
+Stephen R A King : sking.github@gmail.com
+
+Distributed under the MIT license. See [![][license-image]][license-url] for more information.
 
-Distributed under the MIT License. See `LICENSE` for more information.
+Created with Cookiecutter template: [**pydough**][pydough-url] version 1.2.1
 
 <!-- Markdown link & img dfn's -->
 
 [bandit-image]: https://img.shields.io/badge/security-bandit-yellow.svg
 [bandit-url]: https://github.com/PyCQA/bandit
 [black-image]: https://img.shields.io/badge/code%20style-black-000000.svg
 [black-url]: https://github.com/psf/black
-[cc_template-url]: https://github.com/Stephen-RA-King/cc_template
+[pydough-url]: https://github.com/Stephen-RA-King/pydough
 [codeclimate-image]: https://api.codeclimate.com/v1/badges/9543c409696e9976a987/maintainability
 [codeclimate-url]: https://codeclimate.com/github/Stephen-RA-King/pynball/maintainability
 [codecov-image]: https://codecov.io/gh/Stephen-RA-King/pynball/branch/main/graph/badge.svg
 [codecov-url]: https://app.codecov.io/gh/Stephen-RA-King/pynball
 [codefactor-image]: https://www.codefactor.io/repository/github/Stephen-RA-King/pynball/badge
 [codefactor-url]: https://www.codefactor.io/repository/github/Stephen-RA-King/pynball
 [codeql-image]: https://github.com/Stephen-RA-King/pynball/actions/workflows/github-code-scanning/codeql/badge.svg
```

### Comparing `pynball-1.5.3/pyproject.toml` & `pynball-1.5.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pynball-1.5.3/setup.cfg` & `pynball-1.5.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `pynball-1.5.3/src/pynball/pynball.py` & `pynball-1.5.4/src/pynball/pynball.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,22 +8,27 @@
 import fnmatch
 import os
 import re
 import shutil
 import stat
 import subprocess
 import sys
+
+# TODO: implement conditional imports based on OS
 import winreg
 from pathlib import Path
 from typing import Any
 
 # Third party modules
 import click
+
+# TODO: replace 3rd party libmagic library with standard mimetypes library
 import magic
 
+#: Specifies the operating system to which the module is installed
 _PLATFORM = sys.platform
 if _PLATFORM != "win32":
     print(
         "Your Operating system is not supported yet."
         "Linux will be supported in version 2."
     )
     sys.exit(1)
@@ -167,14 +172,15 @@
             key = winreg.OpenKey(_USER_KEY, _USER_SUBKEY, 0, winreg.KEY_ALL_ACCESS)
         elif scope == "system":
             key = winreg.OpenKey(_SYSTEM_KEY, _SYSTEM_SUBKEY, 0, winreg.KEY_ALL_ACCESS)
         winreg.SetValueEx(key, name, 0, winreg.REG_SZ, value)  # noqa
         winreg.CloseKey(key)
     else:
         pass
+        # TODO: generate linux version of _setenv
 
 
 def _getenv(scope: str, name: str) -> Any:
     """Gets an environment variable given a scope and key name.
 
     Note:
         No need to open the key as they are one of the predefined HKEY_* constants.
@@ -203,14 +209,15 @@
         try:
             value, _ = winreg.QueryValueEx(key, name)  # noqa
         except FileNotFoundError:
             value = None
         return value
     else:
         pass
+        # TODO: generate linux version of _getenv
 
 
 def _delenv(scope: str, name: str) -> None:
     """A utility method to delete an environment variable key from the named scope.
 
     Note:
         No need to open the key as they are one of the predefined HKEY_* constants.
@@ -237,14 +244,15 @@
         try:
             winreg.DeleteValue(key, name)  # noqa
         except OSError as e:
             message = f"Deletion of key: '{name}' failed -\n {e}"
             _feedback(message, "warning")
     else:
         pass
+        # TODO: generate linux version of _delenv
 
 
 def _set_pynball(dict_object: dict[str, Path], varname: str) -> None:
     """Accepts and converts a dictionary object, then writes to the registry.
 
     Args:
         dict_object:  The dictionary. Format: {"name: str": "path to version": Path,}
@@ -774,17 +782,18 @@
             ):
                 file_search.append(file)
             if old_name in str(file):
                 file_name_change.append(file)
         elif old_name in str(file) and file.stem not in ignore_dirs:
             dir_name_change.append(file)
 
+    # TODO: find a solution to possible encoding issues here
     # replace text inside files
     for file in file_search:
-        text = file.read_text()
+        text = file.read_text(encoding="utf-8", errors="ignore")
         text = text.replace(old_name, new_name)
         file.write_text(text)
 
     # replace text in filenames
     for file in file_name_change:
         old_file_name = file.name
         new_file_name = old_file_name.replace(old_name, new_name)
```

### Comparing `pynball-1.5.3/src/pynball.egg-info/PKG-INFO` & `pynball-1.5.4/src/pynball.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynball
-Version: 1.5.3
+Version: 1.5.4
 Summary: Utility command line tool to manage python versions
 Home-page: https://github.com/stephen-ra-king/pynball
 Download-URL: 
 Author: Stephen R A King
 Author-email: stephen.ra.king@gmail.com
 Maintainer: Stephen R A King
 Maintainer-email: stephen.ra.king@gmail.com
@@ -34,14 +34,15 @@
 [![PyPI][pypi-image]][pypi-url]
 [![Downloads][downloads-image]][downloads-url]
 [![Status][status-image]][pypi-url]
 [![Python Version][python-version-image]][pypi-url]
 [![Format][format-image]][pypi-url]
 [![tests][tests-image]][tests-url]
 [![Codecov][codecov-image]][codecov-url]
+[![pre-commit.ci][pre-commit.ci-image]][pre-commit.ci-url]
 [![CodeFactor][codefactor-image]][codefactor-url]
 [![Codeclimate][codeclimate-image]][codeclimate-url]
 [![CodeQl][codeql-image]][codeql-url]
 [![readthedocs][readthedocs-image]][readthedocs-url]
 [![pre-commit][pre-commit-image]][pre-commit-url]
 [![Imports: isort][isort-image]][isort-url]
 [![Code style: black][black-image]][black-url]
@@ -56,46 +57,54 @@
 
 You may have a requirement for development on various versions of Python.
 Or you may have a mixture of installations including pyenv, custom installations,
 system installations etc. Pynball can make leveraging such environments a lot easier.
 
 ## Features
 
+---
+
 - Consolidates all Python installations including [**pyenv**][pyenv-url] into one management system
 - Easily create Virtual Environments using any Python version.
 - Track which virtual environments have which Python versions and tox versions.
 - Quickly change the System interpreter
 
 ## Pre Installation Requirements
 
+---
+
 #### Minimum Requirements
 
 1. Python 3.8+
 2. [**pipx**][pipx-url]
 3. [**Virtualenv**][virtualenv-url] (which has benefits over venv)
 4. [**Virtualenvwrapper**][virtualenvwrapper-url]
 
 #### For Maximum Benefits additionally install the following:
 
 1. [**pyenv**][pyenv-url]
 
 ## Installation
 
+---
+
 **OS X & Linux:**
 
 Will be supported in version 2
 
 **Windows:**
 
 ```sh
 pipx install pynball
 ```
 
 ## Usage example
 
+---
+
 ### View Available commands
 
 ```sh
 pynball
 Usage: pynball [OPTIONS] COMMAND [ARGS]...
 
   Utility script to help manage development with various versions of Python in
@@ -229,39 +238,50 @@
 3.6.8     D:\PYTHON\3.6.8 : --> System Interpreter
 3.5.4     D:\PYTHON\3.5.4
 3.5.2     C:\Users\conta\.pyenv\pyenv-win\versions\3.5.2
 ```
 
 _For more information, please refer to the wiki_
 
-## [Wiki][wiki]
-
 ## Documentation
 
+---
+
 [**Read the Docs**](https://pynball.readthedocs.io/en/latest/?)
 
+- [**Example Usage**](https://pynball.readthedocs.io/en/latest/example.html)
+- [**Credits**](https://pynball.readthedocs.io/en/latest/example.html)
+- [**Changelog**](https://pynball.readthedocs.io/en/latest/changelog.html)
+- [**API Reference**](https://pynball.readthedocs.io/en/latest/autoapi/index.html)
+
+- [**Wiki**][wiki]
+
 ## Meta
 
+---
+
 [![](assets/linkedin.png)](https://www.linkedin.com/in/sr-king)
 [![](assets/github.png)](https://github.com/Stephen-RA-King)
 [![](assets/pypi.png)](https://pypi.org/project/pynball)
 [![](assets/www.png)](https://www.justpython.tech)
 [![](assets/email.png)](mailto:sking.github@gmail.com)
 
-Author: Stephen R A King
+Stephen R A King : sking.github@gmail.com
+
+Distributed under the MIT license. See [![][license-image]][license-url] for more information.
 
-Distributed under the MIT License. See `LICENSE` for more information.
+Created with Cookiecutter template: [**pydough**][pydough-url] version 1.2.1
 
 <!-- Markdown link & img dfn's -->
 
 [bandit-image]: https://img.shields.io/badge/security-bandit-yellow.svg
 [bandit-url]: https://github.com/PyCQA/bandit
 [black-image]: https://img.shields.io/badge/code%20style-black-000000.svg
 [black-url]: https://github.com/psf/black
-[cc_template-url]: https://github.com/Stephen-RA-King/cc_template
+[pydough-url]: https://github.com/Stephen-RA-King/pydough
 [codeclimate-image]: https://api.codeclimate.com/v1/badges/9543c409696e9976a987/maintainability
 [codeclimate-url]: https://codeclimate.com/github/Stephen-RA-King/pynball/maintainability
 [codecov-image]: https://codecov.io/gh/Stephen-RA-King/pynball/branch/main/graph/badge.svg
 [codecov-url]: https://app.codecov.io/gh/Stephen-RA-King/pynball
 [codefactor-image]: https://www.codefactor.io/repository/github/Stephen-RA-King/pynball/badge
 [codefactor-url]: https://www.codefactor.io/repository/github/Stephen-RA-King/pynball
 [codeql-image]: https://github.com/Stephen-RA-King/pynball/actions/workflows/github-code-scanning/codeql/badge.svg
```

### Comparing `pynball-1.5.3/src/pynball.egg-info/SOURCES.txt` & `pynball-1.5.4/src/pynball.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pynball-1.5.3/tests/test__check_pyenv.py` & `pynball-1.5.4/tests/test__check_pyenv.py`

 * *Files identical despite different names*

### Comparing `pynball-1.5.3/tests/test__check_virtual_env.py` & `pynball-1.5.4/tests/test__check_virtual_env.py`

 * *Files identical despite different names*

### Comparing `pynball-1.5.3/tests/test__get_pynball.py` & `pynball-1.5.4/tests/test__get_pynball.py`

 * *Files identical despite different names*

### Comparing `pynball-1.5.3/tests/test__message.py` & `pynball-1.5.4/tests/test__message.py`

 * *Files identical despite different names*

### Comparing `pynball-1.5.3/tests/test__set_get_del_env.py` & `pynball-1.5.4/tests/test__set_get_del_env.py`

 * *Files identical despite different names*

### Comparing `pynball-1.5.3/tests/test_add.py` & `pynball-1.5.4/tests/test_add.py`

 * *Files identical despite different names*

### Comparing `pynball-1.5.3/tests/test_delete.py` & `pynball-1.5.4/tests/test_delete.py`

 * *Files identical despite different names*

### Comparing `pynball-1.5.3/tests/test_lsproject.py` & `pynball-1.5.4/tests/test_lsproject.py`

 * *Files identical despite different names*

### Comparing `pynball-1.5.3/tests/test_mkproject.py` & `pynball-1.5.4/tests/test_mkproject.py`

 * *Files identical despite different names*

### Comparing `pynball-1.5.3/tests/test_rmproject.py` & `pynball-1.5.4/tests/test_rmproject.py`

 * *Files identical despite different names*

### Comparing `pynball-1.5.3/tests/test_versions.py` & `pynball-1.5.4/tests/test_versions.py`

 * *Files identical despite different names*

