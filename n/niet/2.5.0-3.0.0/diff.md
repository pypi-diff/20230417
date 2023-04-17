# Comparing `tmp/niet-2.5.0.tar.gz` & `tmp/niet-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "niet-2.5.0.tar", last modified: Fri Feb 10 14:50:29 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `niet-2.5.0.tar` & `niet-3.0.0.tar`

### file list

```diff
@@ -1,37 +1,23 @@
-drwxr-xr-x   0 hberaud   (1000) hberaud   (1000)        0 2023-02-10 14:50:29.666339 niet-2.5.0/
--rw-r--r--   0 hberaud   (1000) hberaud   (1000)     2836 2022-09-06 09:32:46.000000 niet-2.5.0/.travis.yml
--rw-r--r--   0 hberaud   (1000) hberaud   (1000)      263 2023-02-10 14:50:29.000000 niet-2.5.0/AUTHORS
--rw-r--r--   0 hberaud   (1000) hberaud   (1000)     3268 2022-09-06 09:32:46.000000 niet-2.5.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 hberaud   (1000) hberaud   (1000)     8642 2022-09-06 09:32:46.000000 niet-2.5.0/CONTRIBUTING.md
--rw-r--r--   0 hberaud   (1000) hberaud   (1000)     3540 2023-02-10 14:50:29.000000 niet-2.5.0/ChangeLog
--rw-r--r--   0 hberaud   (1000) hberaud   (1000)     3031 2022-09-06 09:32:46.000000 niet-2.5.0/ChangeLog.md
--rw-r--r--   0 hberaud   (1000) hberaud   (1000)     1137 2022-09-06 09:32:46.000000 niet-2.5.0/LICENSE
--rw-r--r--   0 hberaud   (1000) hberaud   (1000)    24279 2023-02-10 14:50:29.666339 niet-2.5.0/PKG-INFO
--rw-r--r--   0 hberaud   (1000) hberaud   (1000)      128 2022-09-06 09:32:46.000000 niet-2.5.0/Pipfile
--rw-r--r--   0 hberaud   (1000) hberaud   (1000)    23268 2022-09-06 09:32:46.000000 niet-2.5.0/README.md
-drwxr-xr-x   0 hberaud   (1000) hberaud   (1000)        0 2023-02-10 14:50:29.665338 niet-2.5.0/niet/
--rw-r--r--   0 hberaud   (1000) hberaud   (1000)     7449 2022-09-07 07:50:14.000000 niet-2.5.0/niet/__init__.py
--rw-r--r--   0 hberaud   (1000) hberaud   (1000)       79 2022-09-06 09:32:46.000000 niet-2.5.0/niet/__main__.py
--rw-r--r--   0 hberaud   (1000) hberaud   (1000)     2337 2022-09-06 09:32:46.000000 niet-2.5.0/niet/output.py
--rw-r--r--   0 hberaud   (1000) hberaud   (1000)      363 2022-09-06 09:32:46.000000 niet-2.5.0/niet/url.py
-drwxr-xr-x   0 hberaud   (1000) hberaud   (1000)        0 2023-02-10 14:50:29.666339 niet-2.5.0/niet.egg-info/
--rw-r--r--   0 hberaud   (1000) hberaud   (1000)    24279 2023-02-10 14:50:29.000000 niet-2.5.0/niet.egg-info/PKG-INFO
--rw-r--r--   0 hberaud   (1000) hberaud   (1000)      580 2023-02-10 14:50:29.000000 niet-2.5.0/niet.egg-info/SOURCES.txt
--rw-r--r--   0 hberaud   (1000) hberaud   (1000)        1 2023-02-10 14:50:29.000000 niet-2.5.0/niet.egg-info/dependency_links.txt
--rw-r--r--   0 hberaud   (1000) hberaud   (1000)       45 2023-02-10 14:50:29.000000 niet-2.5.0/niet.egg-info/entry_points.txt
--rw-r--r--   0 hberaud   (1000) hberaud   (1000)        1 2023-02-10 14:50:23.000000 niet-2.5.0/niet.egg-info/not-zip-safe
--rw-r--r--   0 hberaud   (1000) hberaud   (1000)       47 2023-02-10 14:50:29.000000 niet-2.5.0/niet.egg-info/pbr.json
--rw-r--r--   0 hberaud   (1000) hberaud   (1000)       30 2023-02-10 14:50:29.000000 niet-2.5.0/niet.egg-info/requires.txt
--rw-r--r--   0 hberaud   (1000) hberaud   (1000)        5 2023-02-10 14:50:29.000000 niet-2.5.0/niet.egg-info/top_level.txt
--rw-r--r--   0 hberaud   (1000) hberaud   (1000)       30 2022-09-06 09:32:46.000000 niet-2.5.0/requirements.txt
--rw-r--r--   0 hberaud   (1000) hberaud   (1000)      725 2023-02-10 14:50:29.667338 niet-2.5.0/setup.cfg
--rw-r--r--   0 hberaud   (1000) hberaud   (1000)      126 2022-09-06 09:32:46.000000 niet-2.5.0/setup.py
--rw-r--r--   0 hberaud   (1000) hberaud   (1000)       29 2022-09-06 09:32:46.000000 niet-2.5.0/test-requirements.txt
-drwxr-xr-x   0 hberaud   (1000) hberaud   (1000)        0 2023-02-10 14:50:29.666339 niet-2.5.0/tests/
-drwxr-xr-x   0 hberaud   (1000) hberaud   (1000)        0 2023-02-10 14:50:29.666339 niet-2.5.0/tests/samples/
--rw-r--r--   0 hberaud   (1000) hberaud   (1000)      231 2022-09-06 09:32:46.000000 niet-2.5.0/tests/samples/sample.json
--rw-r--r--   0 hberaud   (1000) hberaud   (1000)      136 2022-09-06 09:32:46.000000 niet-2.5.0/tests/samples/sample.yaml
--rw-r--r--   0 hberaud   (1000) hberaud   (1000)      127 2022-09-06 09:32:46.000000 niet-2.5.0/tests/samples/sample_not_indented.json
--rw-r--r--   0 hberaud   (1000) hberaud   (1000)      852 2022-09-06 09:32:46.000000 niet-2.5.0/tests/test_output.py
--rw-r--r--   0 hberaud   (1000) hberaud   (1000)     1082 2022-09-06 09:32:46.000000 niet-2.5.0/tests/test_url.py
--rw-r--r--   0 hberaud   (1000) hberaud   (1000)      697 2022-09-06 09:32:46.000000 niet-2.5.0/tox.ini
+-rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 niet-3.0.0/.travis.yml
+-rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 niet-3.0.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     8112 2020-02-02 00:00:00.000000 niet-3.0.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 niet-3.0.0/ChangeLog.md
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 niet-3.0.0/Pipfile
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 niet-3.0.0/setup.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 niet-3.0.0/test-requirements.txt
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 niet-3.0.0/tox.ini
+-rw-r--r--   0        0        0     7449 2020-02-02 00:00:00.000000 niet-3.0.0/niet/__init__.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 niet-3.0.0/niet/__main__.py
+-rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 niet-3.0.0/niet/output.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 niet-3.0.0/niet/url.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 niet-3.0.0/tests/test_output.py
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 niet-3.0.0/tests/test_url.py
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 niet-3.0.0/tests/samples/sample.json
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 niet-3.0.0/tests/samples/sample.yaml
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 niet-3.0.0/tests/samples/sample_not_indented.json
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 niet-3.0.0/.gitignore
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 niet-3.0.0/AUTHORS
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 niet-3.0.0/LICENSE
+-rw-r--r--   0        0        0    23268 2020-02-02 00:00:00.000000 niet-3.0.0/README.md
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 niet-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0    24207 2020-02-02 00:00:00.000000 niet-3.0.0/PKG-INFO
```

### Comparing `niet-2.5.0/.travis.yml` & `niet-3.0.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `niet-2.5.0/CODE_OF_CONDUCT.md` & `niet-3.0.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `niet-2.5.0/CONTRIBUTING.md` & `niet-3.0.0/CONTRIBUTING.md`

 * *Files 6% similar despite different names*

```diff
@@ -157,49 +157,40 @@
 Code formating and PEP8 validation:
 ```shell
 $ tox -e pep8
 ```
 
 Unit tests:
 ```shell
-$ tox # by default run tests en python 2.7, 3.4, 3.5, 3.6
+$ tox # by default run tests with all the python versions specified in tox.ini
 ```
 
 > Note: If you have just a specific version of python installed on your system, you can test like this:
 ```shell
-$ tox -e py35 # test with python 3.5
+$ tox -e py311 # test with python 3.11
 ```
 
 Security analyze:
 ```shell
 bandit -r niet
 ```
 
-
 ### Pull Requests
 
 If everything work fine you can create your pull request.
 
 Before ensure you have [squash your commits](http://gitready.com/advanced/2009/02/10/squashing-commits-with-rebase.html).
 
 > Be sure to submit your pull request on the upstream `master` branch!
 
-By using [git-pull-request](https://github.com/jd/git-pull-request):
-```shell
-$ pip install -U git-pull-request # if not installed
-$ git pull-request 
-Forked repository: https://github.com/openuado/niet
-Force-pushing branch `somefeature' to remote `github'
-Counting objects: 5, done.
-Delta compression using up to 4 threads.
-Compressing objects: 100% (4/4), done.
-Writing objects: 100% (5/5), 562 bytes | 0 bytes/s, done.
-Total 5 (delta 3), reused 0 (delta 0)
-remote: Resolving deltas: 100% (3/3), completed with 3 local objects.
-To https://github.com/openuado/niet.git
- + 73a733f7...1be2bf29 somefeature -> somefeature (forced update)
- Pull-request created: https://github.com/openuado/niet/pull/33
-```
-
-Or manually directly from github:
+You can create your pull request manually directly from github:
 * Include examples, outputs, etc... whenever possible.
 * Include screenshots and animated GIFs in your pull request whenever possible.
+
+### Deploy niet on PyPi
+
+```
+python -m pip install build twine
+python -m build
+twine check dist/*
+twine upload dist/*
+```
```

### Comparing `niet-2.5.0/ChangeLog` & `niet-3.0.0/ChangeLog.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,59 +1,32 @@
 CHANGES
 =======
 
-2.5.0
------
-
-* [fix #72] return key equal to False and 0 rather than raising an element not found
-* use underscore in setup.cfg
-* add a research example
-* add defensive design error messages
-* add separator
-* Speak about niet is story
-* [#68] update PyYAML to 5.4.1 (from 5.1)
-
-2.4.0
------
-
-* update badges
-* update badges
-* ignore pbr's generated changelog
-* update changelog
-
 2.3.0
 -----
 
 * Adding a debug mode to niet
-* [doc] add more examples for the \`comma\` format
+* [doc] add more examples for the `comma` format
 
 2.2.0
 -----
 
-* update changelog
-* [feat] add the comma output format
-* [doc] improve examples
+* [feature] adding the comma output format
+* [fix] improve alignement on the help's format
+* [fix] rename unit test module
 
 2.1.0
 -----
 
-* update changelog
-* [doc] reorder sections
-* [doc] reorder sections
-* [doc] fix comment order
-* [feat] retrieve input data from a raw web resource
+* [feature] allow niet to work on web resources (distant JSON/YAML file)
 
 2.0
 ---
 
-* Drop support of py27
-* drop py34 from travis
-* Manage virtual env through tox
-* Drop python 3.4 support
-* Update Changelog
+* drop support of python 2.7
 
 1.8.2
 -----
 
 * fix use newline format on single value
 * add download badge
 * update changelog
```

### Comparing `niet-2.5.0/LICENSE` & `niet-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `niet-2.5.0/PKG-INFO` & `niet-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 Metadata-Version: 2.1
 Name: niet
-Version: 2.5.0
-Summary: Shell config file parser (json, yaml)
-Home-page: https://github.com/openuado/niet/
-Author: openuado
-Author-email: herveberaud.pro@gmail.com
+Version: 3.0.0
+Summary: A command-line tool to work with YAML and JSON files.
+Author-email: Hervé Beraud <herveberaud.pro@gmail.com>
 License: MIT
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Information Technology
+License-File: AUTHORS
+License-File: LICENSE
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Requires: pbr
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development
+Classifier: Topic :: Utilities
+Requires-Python: >=3.9
+Requires-Dist: jmespath>=0.9.4
+Requires-Dist: pyyaml>=5.1
+Provides-Extra: build
+Requires-Dist: build; extra == 'build'
+Requires-Dist: twine; extra == 'build'
 Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: AUTHORS
 
 # niet
 
 [![Build Status](https://travis-ci.org/openuado/niet.svg?branch=master)](https://travis-ci.org/openuado/niet)
 ![PyPI](https://img.shields.io/pypi/v/niet.svg)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/niet.svg)
 ![PyPI - Status](https://img.shields.io/pypi/status/niet.svg)
@@ -800,18 +804,7 @@
 If you want to contribute to niet [please first read the contribution guidelines](CONTRIBUTING.md)
 
 ## Licence
 
 This project is under the MIT License.
 
 [See the license file for more details](LICENSE)
-
-Henry Tang <henryykt@gmail.com>
-Hervé Beraud <hberaud@redhat.com>
-Hervé Beraud <herveberaud.pro@gmail.com>
-Sebastien Boyron <sebastien@boyron.eu>
-Sébastien Boyron <sboyron@localhost.localdomain>
-dj4ngo <sebastien@boyron.eu>
-rechthemoon <rechthemoon@gmail.com>
-
-
-
```

### Comparing `niet-2.5.0/README.md` & `niet-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `niet-2.5.0/niet/__init__.py` & `niet-3.0.0/niet/__init__.py`

 * *Files identical despite different names*

### Comparing `niet-2.5.0/niet/output.py` & `niet-3.0.0/niet/output.py`

 * *Files identical despite different names*

### Comparing `niet-2.5.0/tests/test_output.py` & `niet-3.0.0/tests/test_output.py`

 * *Files identical despite different names*

### Comparing `niet-2.5.0/tests/test_url.py` & `niet-3.0.0/tests/test_url.py`

 * *Files identical despite different names*

