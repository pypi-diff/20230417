# Comparing `tmp/alteryx_open_src_update_checker-3.0.1.tar.gz` & `tmp/alteryx_open_src_update_checker-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/github/workspace/dist/.tmp-zmvncqm6/alteryx_open_src_update_checker-3.0.1.tar", last modified: Thu Dec 22 21:05:47 2022, max compression
+gzip compressed data, was "/github/workspace/dist/.tmp-h51ivn6a/alteryx_open_src_update_checker-3.1.0.tar", last modified: Mon Apr 17 15:23:30 2023, max compression
```

## Comparing `alteryx_open_src_update_checker-3.0.1.tar` & `alteryx_open_src_update_checker-3.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-22 21:05:47.000000 alteryx_open_src_update_checker-3.0.1/
--rw-r--r--   0 root         (0) root         (0)     1513 2022-12-22 21:05:32.000000 alteryx_open_src_update_checker-3.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3102 2022-12-22 21:05:47.000000 alteryx_open_src_update_checker-3.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1659 2022-12-22 21:05:32.000000 alteryx_open_src_update_checker-3.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-22 21:05:47.000000 alteryx_open_src_update_checker-3.0.1/alteryx_open_src_update_checker/
--rw-r--r--   0 root         (0) root         (0)      147 2022-12-22 21:05:32.000000 alteryx_open_src_update_checker-3.0.1/alteryx_open_src_update_checker/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1066 2022-12-22 21:05:32.000000 alteryx_open_src_update_checker-3.0.1/alteryx_open_src_update_checker/functions.py
--rw-r--r--   0 root         (0) root         (0)       51 2022-12-22 21:05:32.000000 alteryx_open_src_update_checker-3.0.1/alteryx_open_src_update_checker/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-22 21:05:47.000000 alteryx_open_src_update_checker-3.0.1/alteryx_open_src_update_checker/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2022-12-22 21:05:32.000000 alteryx_open_src_update_checker-3.0.1/alteryx_open_src_update_checker/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9057 2022-12-22 21:05:32.000000 alteryx_open_src_update_checker-3.0.1/alteryx_open_src_update_checker/tests/test_ayx_open_source_update_checker.py
--rw-r--r--   0 root         (0) root         (0)      112 2022-12-22 21:05:32.000000 alteryx_open_src_update_checker-3.0.1/alteryx_open_src_update_checker/tests/test_version.py
--rw-r--r--   0 root         (0) root         (0)      558 2022-12-22 21:05:32.000000 alteryx_open_src_update_checker-3.0.1/alteryx_open_src_update_checker/utils.py
--rw-r--r--   0 root         (0) root         (0)       22 2022-12-22 21:05:32.000000 alteryx_open_src_update_checker-3.0.1/alteryx_open_src_update_checker/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-22 21:05:47.000000 alteryx_open_src_update_checker-3.0.1/alteryx_open_src_update_checker.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3102 2022-12-22 21:05:47.000000 alteryx_open_src_update_checker-3.0.1/alteryx_open_src_update_checker.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      704 2022-12-22 21:05:47.000000 alteryx_open_src_update_checker-3.0.1/alteryx_open_src_update_checker.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-22 21:05:47.000000 alteryx_open_src_update_checker-3.0.1/alteryx_open_src_update_checker.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      199 2022-12-22 21:05:47.000000 alteryx_open_src_update_checker-3.0.1/alteryx_open_src_update_checker.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       37 2022-12-22 21:05:47.000000 alteryx_open_src_update_checker-3.0.1/alteryx_open_src_update_checker.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2871 2022-12-22 21:05:32.000000 alteryx_open_src_update_checker-3.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-12-22 21:05:47.000000 alteryx_open_src_update_checker-3.0.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:23:30.000000 alteryx_open_src_update_checker-3.1.0/
+-rw-r--r--   0 root         (0) root         (0)     1513 2023-04-17 15:23:16.000000 alteryx_open_src_update_checker-3.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3153 2023-04-17 15:23:30.000000 alteryx_open_src_update_checker-3.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-17 15:23:16.000000 alteryx_open_src_update_checker-3.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:23:30.000000 alteryx_open_src_update_checker-3.1.0/alteryx_open_src_update_checker/
+-rw-r--r--   0 root         (0) root         (0)      147 2023-04-17 15:23:16.000000 alteryx_open_src_update_checker-3.1.0/alteryx_open_src_update_checker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1066 2023-04-17 15:23:16.000000 alteryx_open_src_update_checker-3.1.0/alteryx_open_src_update_checker/functions.py
+-rw-r--r--   0 root         (0) root         (0)       51 2023-04-17 15:23:16.000000 alteryx_open_src_update_checker-3.1.0/alteryx_open_src_update_checker/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:23:30.000000 alteryx_open_src_update_checker-3.1.0/alteryx_open_src_update_checker/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 15:23:16.000000 alteryx_open_src_update_checker-3.1.0/alteryx_open_src_update_checker/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9057 2023-04-17 15:23:16.000000 alteryx_open_src_update_checker-3.1.0/alteryx_open_src_update_checker/tests/test_ayx_open_source_update_checker.py
+-rw-r--r--   0 root         (0) root         (0)      112 2023-04-17 15:23:16.000000 alteryx_open_src_update_checker-3.1.0/alteryx_open_src_update_checker/tests/test_version.py
+-rw-r--r--   0 root         (0) root         (0)      558 2023-04-17 15:23:16.000000 alteryx_open_src_update_checker-3.1.0/alteryx_open_src_update_checker/utils.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-17 15:23:16.000000 alteryx_open_src_update_checker-3.1.0/alteryx_open_src_update_checker/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:23:30.000000 alteryx_open_src_update_checker-3.1.0/alteryx_open_src_update_checker.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3153 2023-04-17 15:23:30.000000 alteryx_open_src_update_checker-3.1.0/alteryx_open_src_update_checker.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      704 2023-04-17 15:23:30.000000 alteryx_open_src_update_checker-3.1.0/alteryx_open_src_update_checker.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 15:23:30.000000 alteryx_open_src_update_checker-3.1.0/alteryx_open_src_update_checker.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      203 2023-04-17 15:23:30.000000 alteryx_open_src_update_checker-3.1.0/alteryx_open_src_update_checker.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-04-17 15:23:30.000000 alteryx_open_src_update_checker-3.1.0/alteryx_open_src_update_checker.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     3009 2023-04-17 15:23:16.000000 alteryx_open_src_update_checker-3.1.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 15:23:30.000000 alteryx_open_src_update_checker-3.1.0/setup.cfg
```

### Comparing `alteryx_open_src_update_checker-3.0.1/LICENSE` & `alteryx_open_src_update_checker-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alteryx_open_src_update_checker-3.0.1/PKG-INFO` & `alteryx_open_src_update_checker-3.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alteryx_open_src_update_checker
-Version: 3.0.1
+Version: 3.1.0
 Summary: an update checker for alteryx open source libraries
 Author-email: "Alteryx, Inc." <open_source_support@alteryx.com>
 Maintainer-email: "Alteryx, Inc." <open_source_support@alteryx.com>
 License: BSD 3-clause
 Project-URL: Source Code, https://github.com/alteryx/alteryx-open-src-update-checker/
 Project-URL: Issue Tracker, https://github.com/alteryx/alteryx-open-src-update-checker/issues
 Project-URL: Twitter, https://twitter.com/alteryxoss
@@ -16,14 +16,15 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Requires-Python: <4,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

#### html2text {}

```diff
@@ -1,27 +1,28 @@
-Metadata-Version: 2.1 Name: alteryx_open_src_update_checker Version: 3.0.1
+Metadata-Version: 2.1 Name: alteryx_open_src_update_checker Version: 3.1.0
 Summary: an update checker for alteryx open source libraries Author-email:
 "Alteryx, Inc."
 alteryx.com> Maintainer-email: "Alteryx, Inc."
 alteryx.com> License: BSD 3-clause Project-URL: Source Code, https://
 github.com/alteryx/alteryx-open-src-update-checker/ Project-URL: Issue Tracker,
 https://github.com/alteryx/alteryx-open-src-update-checker/issues Project-URL:
 Twitter, https://twitter.com/alteryxoss Project-URL: Chat, https://
 join.slack.com/t/alteryx-oss/shared_invite/zt-182tyvuxv-NzIn6eiCEf8TBziuKp0bNA
 Keywords: data science,machine learning Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Science/Research Classifier:
 Intended Audience :: Developers Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Operating System
-:: Microsoft :: Windows Classifier: Operating System :: POSIX Classifier:
-Operating System :: Unix Classifier: Operating System :: MacOS Requires-Python:
-<4,>=3.8 Description-Content-Type: text/markdown Provides-Extra: dev Provides-
-Extra: test License-File: LICENSE # Alteryx Open Source Update Checker
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS Requires-Python: <4,>=3.8 Description-
+Content-Type: text/markdown Provides-Extra: dev Provides-Extra: test License-
+File: LICENSE # Alteryx Open Source Update Checker
                            [Tests] [PyPI_Downloads]
 ===============================================================================
 Alteryx open source update checker is a Python library to automatically check
 that you have the latest version of an Alteryx open source library. If your
 Alteryx open source library is out of date, a warning to upgrade will be shown.
 ## Installation - Install with pip (as an add-on to Alteryx open source
 libraries): ```bash python -m pip install "featuretools[updater]" python -m pip
```

### Comparing `alteryx_open_src_update_checker-3.0.1/README.md` & `alteryx_open_src_update_checker-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `alteryx_open_src_update_checker-3.0.1/alteryx_open_src_update_checker/functions.py` & `alteryx_open_src_update_checker-3.1.0/alteryx_open_src_update_checker/functions.py`

 * *Files identical despite different names*

### Comparing `alteryx_open_src_update_checker-3.0.1/alteryx_open_src_update_checker/tests/test_ayx_open_source_update_checker.py` & `alteryx_open_src_update_checker-3.1.0/alteryx_open_src_update_checker/tests/test_ayx_open_source_update_checker.py`

 * *Files identical despite different names*

### Comparing `alteryx_open_src_update_checker-3.0.1/alteryx_open_src_update_checker/utils.py` & `alteryx_open_src_update_checker-3.1.0/alteryx_open_src_update_checker/utils.py`

 * *Files identical despite different names*

### Comparing `alteryx_open_src_update_checker-3.0.1/alteryx_open_src_update_checker.egg-info/PKG-INFO` & `alteryx_open_src_update_checker-3.1.0/alteryx_open_src_update_checker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alteryx-open-src-update-checker
-Version: 3.0.1
+Version: 3.1.0
 Summary: an update checker for alteryx open source libraries
 Author-email: "Alteryx, Inc." <open_source_support@alteryx.com>
 Maintainer-email: "Alteryx, Inc." <open_source_support@alteryx.com>
 License: BSD 3-clause
 Project-URL: Source Code, https://github.com/alteryx/alteryx-open-src-update-checker/
 Project-URL: Issue Tracker, https://github.com/alteryx/alteryx-open-src-update-checker/issues
 Project-URL: Twitter, https://twitter.com/alteryxoss
@@ -16,14 +16,15 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Requires-Python: <4,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

#### html2text {}

```diff
@@ -1,27 +1,28 @@
-Metadata-Version: 2.1 Name: alteryx-open-src-update-checker Version: 3.0.1
+Metadata-Version: 2.1 Name: alteryx-open-src-update-checker Version: 3.1.0
 Summary: an update checker for alteryx open source libraries Author-email:
 "Alteryx, Inc."
 alteryx.com> Maintainer-email: "Alteryx, Inc."
 alteryx.com> License: BSD 3-clause Project-URL: Source Code, https://
 github.com/alteryx/alteryx-open-src-update-checker/ Project-URL: Issue Tracker,
 https://github.com/alteryx/alteryx-open-src-update-checker/issues Project-URL:
 Twitter, https://twitter.com/alteryxoss Project-URL: Chat, https://
 join.slack.com/t/alteryx-oss/shared_invite/zt-182tyvuxv-NzIn6eiCEf8TBziuKp0bNA
 Keywords: data science,machine learning Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Science/Research Classifier:
 Intended Audience :: Developers Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Operating System
-:: Microsoft :: Windows Classifier: Operating System :: POSIX Classifier:
-Operating System :: Unix Classifier: Operating System :: MacOS Requires-Python:
-<4,>=3.8 Description-Content-Type: text/markdown Provides-Extra: dev Provides-
-Extra: test License-File: LICENSE # Alteryx Open Source Update Checker
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS Requires-Python: <4,>=3.8 Description-
+Content-Type: text/markdown Provides-Extra: dev Provides-Extra: test License-
+File: LICENSE # Alteryx Open Source Update Checker
                            [Tests] [PyPI_Downloads]
 ===============================================================================
 Alteryx open source update checker is a Python library to automatically check
 that you have the latest version of an Alteryx open source library. If your
 Alteryx open source library is out of date, a warning to upgrade will be shown.
 ## Installation - Install with pip (as an add-on to Alteryx open source
 libraries): ```bash python -m pip install "featuretools[updater]" python -m pip
```

### Comparing `alteryx_open_src_update_checker-3.0.1/alteryx_open_src_update_checker.egg-info/SOURCES.txt` & `alteryx_open_src_update_checker-3.1.0/alteryx_open_src_update_checker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alteryx_open_src_update_checker-3.0.1/pyproject.toml` & `alteryx_open_src_update_checker-3.1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     "Topic :: Software Development",
     "Topic :: Scientific/Engineering",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: POSIX",
     "Operating System :: Unix",
     "Operating System :: MacOS",
 ]
 authors = [
     {name="Alteryx, Inc.", email="open_source_support@alteryx.com"}
@@ -36,18 +37,17 @@
 "Source Code"= "https://github.com/alteryx/alteryx-open-src-update-checker/"
 "Issue Tracker" = "https://github.com/alteryx/alteryx-open-src-update-checker/issues"
 "Twitter" = "https://twitter.com/alteryxoss"
 "Chat" = "https://join.slack.com/t/alteryx-oss/shared_invite/zt-182tyvuxv-NzIn6eiCEf8TBziuKp0bNA"
 
 [project.optional-dependencies]
 dev = [
-    "ruff",
-    "isort == 5.10.1",
-    "black == 22.6.0",
-    "pre-commit == 2.20.0",
+    "ruff >= 0.0.239",
+    "black[jupyter] >= 23.1.0",
+    "pre-commit >= 2.20.0",
 ]
 test = [
     "pip >= 21.3.1",
     "pytest >= 7.1.2",
     "pytest-cov >= 3.0.0",
     "pytest-xdist >= 2.5.0",
     "featuretools",
@@ -86,24 +86,28 @@
     "alteryx_open_src_update_checker/tests/*"
 ]
 filterwarnings = [
     "ignore::DeprecationWarning",
     "ignore::PendingDeprecationWarning"
 ]
 
-[tool.isort]
-profile = "black"
-forced_separate = "alteryx_open_src_update_checker"
-known_first_party = "alteryx_open_src_update_checker"
-skip = "__init__.py"
-filter_files = true
-multi_line_output = 3
+[tool.ruff]
+select = [
+    # Pyflakes
+    "F",
+    # Pycodestyle
+    "E",
+    "W",
+    # isort
+    "I001"
+]
+src = ["alteryx_open_src_update_checker"]
 
-[tool.black]
-target-version = ['py311']
+[tool.ruff.isort]
+known-first-party = ["alteryx_open_src_update_checker"]
 
 [tool.coverage.run]
 source = ["alteryx_open_src_update_checker"]
 
 [tool.coverage.report]
 exclude_lines =[
     "pragma: no cover",
@@ -112,7 +116,14 @@
     "raise NotImplementedError",
     "if __name__ == .__main__.:",
     "if self._verbose:",
     "if verbose:",
     "if profile:",
     "pytest.skip"
 ]
+
+[build-system]
+requires = [
+    "setuptools >= 61.0.0",
+    "wheel"
+]
+build-backend = "setuptools.build_meta"
```

