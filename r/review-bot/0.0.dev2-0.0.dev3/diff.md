# Comparing `tmp/review-bot-0.0.dev2.tar.gz` & `tmp/review-bot-0.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "review-bot-0.0.dev2.tar", last modified: Mon Apr  3 10:36:16 2023, max compression
+gzip compressed data, was "review-bot-0.0.dev3.tar", last modified: Mon Apr 17 09:58:52 2023, max compression
```

## Comparing `review-bot-0.0.dev2.tar` & `review-bot-0.0.dev3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1089 2023-04-03 10:36:03.391214 review-bot-0.0.dev2/LICENSE
--rw-r--r--   0        0        0     2929 2023-04-03 10:36:03.391214 review-bot-0.0.dev2/README.rst
--rw-r--r--   0        0        0     1710 2023-04-03 10:36:03.391214 review-bot-0.0.dev2/pyproject.toml
--rw-r--r--   0        0        0      298 2023-04-03 10:36:03.391214 review-bot-0.0.dev2/src/review_bot/__init__.py
--rw-r--r--   0        0        0     3717 2023-04-03 10:36:03.391214 review-bot-0.0.dev2/src/review_bot/gh_interface.py
--rw-r--r--   0        0        0     4864 2023-04-03 10:36:03.391214 review-bot-0.0.dev2/src/review_bot/misc.py
--rw-r--r--   0        0        0     7834 2023-04-03 10:36:03.391214 review-bot-0.0.dev2/src/review_bot/open_ai_interface.py
--rw-r--r--   0        0        0     4321 1970-01-01 00:00:00.000000 review-bot-0.0.dev2/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-04-17 09:58:38.234545 review-bot-0.0.dev3/LICENSE
+-rw-r--r--   0        0        0     2929 2023-04-17 09:58:38.234545 review-bot-0.0.dev3/README.rst
+-rw-r--r--   0        0        0     1710 2023-04-17 09:58:38.234545 review-bot-0.0.dev3/pyproject.toml
+-rw-r--r--   0        0        0      298 2023-04-17 09:58:38.234545 review-bot-0.0.dev3/src/review_bot/__init__.py
+-rw-r--r--   0        0        0     3717 2023-04-17 09:58:38.234545 review-bot-0.0.dev3/src/review_bot/gh_interface.py
+-rw-r--r--   0        0        0     4864 2023-04-17 09:58:38.234545 review-bot-0.0.dev3/src/review_bot/misc.py
+-rw-r--r--   0        0        0     8120 2023-04-17 09:58:38.234545 review-bot-0.0.dev3/src/review_bot/open_ai_interface.py
+-rw-r--r--   0        0        0     4321 1970-01-01 00:00:00.000000 review-bot-0.0.dev3/PKG-INFO
```

### Comparing `review-bot-0.0.dev2/LICENSE` & `review-bot-0.0.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `review-bot-0.0.dev2/README.rst` & `review-bot-0.0.dev3/README.rst`

 * *Files identical despite different names*

### Comparing `review-bot-0.0.dev2/pyproject.toml` & `review-bot-0.0.dev3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 # Check https://flit.readthedocs.io/en/latest/pyproject_toml.html for all available sections
 name = "review-bot"
-version = "0.0.dev2"
+version = "0.0.dev3"
 description = "A python library to automatically generate suggestions and improvements for patches in GitHub PRs by leveraging the power of OpenAI."
 readme = "README.rst"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 authors = [
     {name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"},
 ]
```

### Comparing `review-bot-0.0.dev2/src/review_bot/gh_interface.py` & `review-bot-0.0.dev3/src/review_bot/gh_interface.py`

 * *Files identical despite different names*

### Comparing `review-bot-0.0.dev2/src/review_bot/misc.py` & `review-bot-0.0.dev3/src/review_bot/misc.py`

 * *Files identical despite different names*

### Comparing `review-bot-0.0.dev2/src/review_bot/open_ai_interface.py` & `review-bot-0.0.dev3/src/review_bot/open_ai_interface.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,17 @@
 LOG.setLevel("DEBUG")
 
 # Developer note:
 # There is a significant improvement in the completion using gpt-4 vs gpt-3.5-turbo
 OPEN_AI_MODEL = "gpt-4"
 
 
-def review_patch(owner, repo, pr, use_src=False, filter_filename=None):
+def review_patch(
+    owner, repo, pr, use_src=False, filter_filename=None, gh_access_token=None
+):
     """Review a patch in a pull request and generate suggestions for improvement.
 
     Parameters
     ----------
     owner : str
         The GitHub owner/organization of the repository.
     repo : str
@@ -27,22 +29,27 @@
     pr : str
         The pull request number.
     use_src : bool, default: False
         Use the source file as context for the patch. Works for small files and
         not for large ones.
     filter_filename : str, optional
         If set, filters out all but the file matching this string.
+    gh_access_token : str, optional
+        GitHub token needed to communicate with the repository. By default, ``None``,
+        which means it will try to read an existing env variable named ``GITHUB_TOKEN``.
 
     Returns
     -------
     list[dict]
         A dictionary containing suggestions for the reviewed patch.
     """
     # Fetch changed files and contents
-    changed_files = get_changed_files_and_contents(owner, repo, pr)
+    changed_files = get_changed_files_and_contents(
+        owner, repo, pr, gh_access_token=gh_access_token
+    )
 
     # assemble suggestions
     suggestions = []
     n_hits = 0
     for file_data in changed_files:
         filename = file_data["filename"]
         if filter_filename is not None and filename != filter_filename:
```

### Comparing `review-bot-0.0.dev2/PKG-INFO` & `review-bot-0.0.dev3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: review-bot
-Version: 0.0.dev2
+Version: 0.0.dev3
 Summary: A python library to automatically generate suggestions and improvements for patches in GitHub PRs by leveraging the power of OpenAI.
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: PyAnsys developers <pyansys.core@ansys.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

