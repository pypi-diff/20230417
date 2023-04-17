# Comparing `tmp/pyproject_pre_commit-0.0.6.tar.gz` & `tmp/pyproject_pre_commit-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproject_pre_commit-0.0.6.tar", max compression
+gzip compressed data, was "pyproject_pre_commit-0.0.7.tar", max compression
```

## Comparing `pyproject_pre_commit-0.0.6.tar` & `pyproject_pre_commit-0.0.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11337 2023-04-10 01:49:55.792857 pyproject_pre_commit-0.0.6/LICENSE
--rw-r--r--   0        0        0     5374 2023-04-10 01:49:55.792857 pyproject_pre_commit-0.0.6/README.md
--rw-r--r--   0        0        0     2944 2023-04-10 01:49:56.316854 pyproject_pre_commit-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      118 2023-04-10 01:49:56.320855 pyproject_pre_commit-0.0.6/src/pyproject_pre_commit/__init__.py
--rw-r--r--   0        0        0     1751 2023-04-10 01:49:55.792857 pyproject_pre_commit-0.0.6/src/pyproject_pre_commit/pyproject_pre_commit.py
--rw-r--r--   0        0        0     7485 1970-01-01 00:00:00.000000 pyproject_pre_commit-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0    11337 2023-04-17 01:02:26.086021 pyproject_pre_commit-0.0.7/LICENSE
+-rw-r--r--   0        0        0     5374 2023-04-17 01:02:26.086021 pyproject_pre_commit-0.0.7/README.md
+-rw-r--r--   0        0        0     2944 2023-04-17 01:02:26.770022 pyproject_pre_commit-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      118 2023-04-17 01:02:26.770022 pyproject_pre_commit-0.0.7/src/pyproject_pre_commit/__init__.py
+-rw-r--r--   0        0        0     1751 2023-04-17 01:02:26.086021 pyproject_pre_commit-0.0.7/src/pyproject_pre_commit/pyproject_pre_commit.py
+-rw-r--r--   0        0        0     7485 1970-01-01 00:00:00.000000 pyproject_pre_commit-0.0.7/PKG-INFO
```

### Comparing `pyproject_pre_commit-0.0.6/LICENSE` & `pyproject_pre_commit-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyproject_pre_commit-0.0.6/README.md` & `pyproject_pre_commit-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pyproject_pre_commit-0.0.6/pyproject.toml` & `pyproject_pre_commit-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyproject-pre-commit"
-version = "0.0.6"
+version = "0.0.7"
 description = "pre-commit hooks for python projects using pyproject.toml."
 authors = ["rcmdnk <rcmdnk@gmail.com>"]
 repository = "https://github.com/rcmdnk/pyproject-pre-commit"
 homepage = "https://github.com/rcmdnk/pyproject-pre-commit"
 readme = "README.md"
 license = "Apache-2.0"
 keywords = ["pre-commit", "pyproject.toml", "poetry"]
@@ -23,15 +23,15 @@
 pre-commit = "3.2.2"
 black = "23.3.0"
 blacken-docs = "1.13.0"
 flake8-pyproject = "1.2.3"
 flake8-annotations-complexity = "0.0.7"
 flake8-bugbear = "23.3.23"
 flake8-builtins = "2.1.0"
-flake8-comprehensions = "3.11.1"
+flake8-comprehensions = "3.12.0"
 flake8-debugger = "4.1.2"
 flake8-docstrings = "1.7.0"
 flake8-executable = "2.1.3"
 flake8-pep3101 = "^2.0.0"
 flake8-print = "5.0.0"
 flake8-rst-docstrings = "0.3.0"
 flake8-string-format = "0.3.0"
@@ -45,15 +45,15 @@
 shellcheck-py = "0.9.0.2"
 mdformat = "0.7.16"
 mdformat-gfm = "0.3.5"
 mdformat-frontmatter = "2.0.1"
 mdformat-footnote = "0.1.1"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "7.3.0"
+pytest = "7.3.1"
 pytest-cov = "4.0.0"
 pytest-xdist = "3.2.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pyproject_pre_commit-0.0.6/src/pyproject_pre_commit/pyproject_pre_commit.py` & `pyproject_pre_commit-0.0.7/src/pyproject_pre_commit/pyproject_pre_commit.py`

 * *Files identical despite different names*

### Comparing `pyproject_pre_commit-0.0.6/PKG-INFO` & `pyproject_pre_commit-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject-pre-commit
-Version: 0.0.6
+Version: 0.0.7
 Summary: pre-commit hooks for python projects using pyproject.toml.
 Home-page: https://github.com/rcmdnk/pyproject-pre-commit
 License: Apache-2.0
 Keywords: pre-commit,pyproject.toml,poetry
 Author: rcmdnk
 Author-email: rcmdnk@gmail.com
 Requires-Python: >=3.8.1,<3.12
@@ -24,15 +24,15 @@
 Requires-Dist: autopep8 (==2.0.2)
 Requires-Dist: bandit[toml] (==1.7.5)
 Requires-Dist: black (==23.3.0)
 Requires-Dist: blacken-docs (==1.13.0)
 Requires-Dist: flake8-annotations-complexity (==0.0.7)
 Requires-Dist: flake8-bugbear (==23.3.23)
 Requires-Dist: flake8-builtins (==2.1.0)
-Requires-Dist: flake8-comprehensions (==3.11.1)
+Requires-Dist: flake8-comprehensions (==3.12.0)
 Requires-Dist: flake8-debugger (==4.1.2)
 Requires-Dist: flake8-docstrings (==1.7.0)
 Requires-Dist: flake8-executable (==2.1.3)
 Requires-Dist: flake8-pep3101 (>=2.0.0,<3.0.0)
 Requires-Dist: flake8-print (==5.0.0)
 Requires-Dist: flake8-pyproject (==1.2.3)
 Requires-Dist: flake8-rst-docstrings (==0.3.0)
```

