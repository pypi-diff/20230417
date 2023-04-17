# Comparing `tmp/pygithubactions-0.1.4.tar.gz` & `tmp/pygithubactions-0.1.5.tar.gz`

## Comparing `pygithubactions-0.1.4.tar` & `pygithubactions-0.1.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 pygithubactions-0.1.4/.editorconfig
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 pygithubactions-0.1.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 pygithubactions-0.1.4/Makefile
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 pygithubactions-0.1.4/.github/dependabot.yml
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 pygithubactions-0.1.4/.github/workflows/lint.yml
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 pygithubactions-0.1.4/.github/workflows/main.yml
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 pygithubactions-0.1.4/.github/workflows/publish.yml
--rw-r--r--   0        0        0    46675 2020-02-02 00:00:00.000000 pygithubactions-0.1.4/docs/annotations.png
--rw-r--r--   0        0        0     6773 2020-02-02 00:00:00.000000 pygithubactions-0.1.4/docs/core.md
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 pygithubactions-0.1.4/pygithubactions/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygithubactions-0.1.4/pygithubactions/context/__init__.py
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 pygithubactions-0.1.4/pygithubactions/context/context.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygithubactions-0.1.4/pygithubactions/core/__init__.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 pygithubactions-0.1.4/pygithubactions/core/command.py
--rw-r--r--   0        0        0     8594 2020-02-02 00:00:00.000000 pygithubactions-0.1.4/pygithubactions/core/core.py
--rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 pygithubactions-0.1.4/pygithubactions/core/file_command.py
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 pygithubactions-0.1.4/pygithubactions/core/path_utils.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 pygithubactions-0.1.4/pygithubactions/core/utils.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 pygithubactions-0.1.4/tests/__init__.py
--rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 pygithubactions-0.1.4/tests/conftest.py
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 pygithubactions-0.1.4/tests/test_annotations.py
--rw-r--r--   0        0        0     3395 2020-02-02 00:00:00.000000 pygithubactions-0.1.4/tests/test_command.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 pygithubactions-0.1.4/tests/test_context.py
--rw-r--r--   0        0        0     3609 2020-02-02 00:00:00.000000 pygithubactions-0.1.4/tests/test_core.py
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 pygithubactions-0.1.4/tests/test_core_add_path.py
--rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 pygithubactions-0.1.4/tests/test_core_export_variable.py
--rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 pygithubactions-0.1.4/tests/test_core_get_input.py
--rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 pygithubactions-0.1.4/tests/test_core_save_state.py
--rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 pygithubactions-0.1.4/tests/test_core_set_output.py
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 pygithubactions-0.1.4/tests/test_path_utils.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 pygithubactions-0.1.4/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 pygithubactions-0.1.4/LICENSE
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 pygithubactions-0.1.4/README.md
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 pygithubactions-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 pygithubactions-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 pygithubactions-0.1.5/.editorconfig
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 pygithubactions-0.1.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 pygithubactions-0.1.5/Makefile
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 pygithubactions-0.1.5/.github/dependabot.yml
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 pygithubactions-0.1.5/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 pygithubactions-0.1.5/.github/workflows/main.yml
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 pygithubactions-0.1.5/.github/workflows/publish.yml
+-rw-r--r--   0        0        0    46675 2020-02-02 00:00:00.000000 pygithubactions-0.1.5/docs/annotations.png
+-rw-r--r--   0        0        0     6773 2020-02-02 00:00:00.000000 pygithubactions-0.1.5/docs/core.md
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 pygithubactions-0.1.5/pygithubactions/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygithubactions-0.1.5/pygithubactions/context/__init__.py
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 pygithubactions-0.1.5/pygithubactions/context/context.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygithubactions-0.1.5/pygithubactions/core/__init__.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 pygithubactions-0.1.5/pygithubactions/core/command.py
+-rw-r--r--   0        0        0     8594 2020-02-02 00:00:00.000000 pygithubactions-0.1.5/pygithubactions/core/core.py
+-rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 pygithubactions-0.1.5/pygithubactions/core/file_command.py
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 pygithubactions-0.1.5/pygithubactions/core/path_utils.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 pygithubactions-0.1.5/pygithubactions/core/utils.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 pygithubactions-0.1.5/tests/__init__.py
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 pygithubactions-0.1.5/tests/conftest.py
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 pygithubactions-0.1.5/tests/test_annotations.py
+-rw-r--r--   0        0        0     3395 2020-02-02 00:00:00.000000 pygithubactions-0.1.5/tests/test_command.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 pygithubactions-0.1.5/tests/test_context.py
+-rw-r--r--   0        0        0     3609 2020-02-02 00:00:00.000000 pygithubactions-0.1.5/tests/test_core.py
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 pygithubactions-0.1.5/tests/test_core_add_path.py
+-rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 pygithubactions-0.1.5/tests/test_core_export_variable.py
+-rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 pygithubactions-0.1.5/tests/test_core_get_input.py
+-rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 pygithubactions-0.1.5/tests/test_core_save_state.py
+-rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 pygithubactions-0.1.5/tests/test_core_set_output.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 pygithubactions-0.1.5/tests/test_path_utils.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 pygithubactions-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 pygithubactions-0.1.5/LICENSE
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 pygithubactions-0.1.5/README.md
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 pygithubactions-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 pygithubactions-0.1.5/PKG-INFO
```

### Comparing `pygithubactions-0.1.4/.pre-commit-config.yaml` & `pygithubactions-0.1.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pygithubactions-0.1.4/Makefile` & `pygithubactions-0.1.5/Makefile`

 * *Files identical despite different names*

### Comparing `pygithubactions-0.1.4/.github/workflows/lint.yml` & `pygithubactions-0.1.5/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `pygithubactions-0.1.4/.github/workflows/main.yml` & `pygithubactions-0.1.5/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `pygithubactions-0.1.4/docs/annotations.png` & `pygithubactions-0.1.5/docs/annotations.png`

 * *Files identical despite different names*

### Comparing `pygithubactions-0.1.4/docs/core.md` & `pygithubactions-0.1.5/docs/core.md`

 * *Files identical despite different names*

### Comparing `pygithubactions-0.1.4/pygithubactions/context/context.py` & `pygithubactions-0.1.5/pygithubactions/context/context.py`

 * *Files identical despite different names*

### Comparing `pygithubactions-0.1.4/pygithubactions/core/command.py` & `pygithubactions-0.1.5/pygithubactions/core/command.py`

 * *Files identical despite different names*

### Comparing `pygithubactions-0.1.4/pygithubactions/core/core.py` & `pygithubactions-0.1.5/pygithubactions/core/core.py`

 * *Files identical despite different names*

### Comparing `pygithubactions-0.1.4/pygithubactions/core/file_command.py` & `pygithubactions-0.1.5/pygithubactions/core/file_command.py`

 * *Files identical despite different names*

### Comparing `pygithubactions-0.1.4/pygithubactions/core/path_utils.py` & `pygithubactions-0.1.5/pygithubactions/core/path_utils.py`

 * *Files identical despite different names*

### Comparing `pygithubactions-0.1.4/pygithubactions/core/utils.py` & `pygithubactions-0.1.5/pygithubactions/core/utils.py`

 * *Files identical despite different names*

### Comparing `pygithubactions-0.1.4/tests/conftest.py` & `pygithubactions-0.1.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pygithubactions-0.1.4/tests/test_annotations.py` & `pygithubactions-0.1.5/tests/test_annotations.py`

 * *Files identical despite different names*

### Comparing `pygithubactions-0.1.4/tests/test_command.py` & `pygithubactions-0.1.5/tests/test_command.py`

 * *Files identical despite different names*

### Comparing `pygithubactions-0.1.4/tests/test_core.py` & `pygithubactions-0.1.5/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `pygithubactions-0.1.4/tests/test_core_add_path.py` & `pygithubactions-0.1.5/tests/test_core_add_path.py`

 * *Files identical despite different names*

### Comparing `pygithubactions-0.1.4/tests/test_core_export_variable.py` & `pygithubactions-0.1.5/tests/test_core_export_variable.py`

 * *Files identical despite different names*

### Comparing `pygithubactions-0.1.4/tests/test_core_get_input.py` & `pygithubactions-0.1.5/tests/test_core_get_input.py`

 * *Files identical despite different names*

### Comparing `pygithubactions-0.1.4/tests/test_core_save_state.py` & `pygithubactions-0.1.5/tests/test_core_save_state.py`

 * *Files identical despite different names*

### Comparing `pygithubactions-0.1.4/tests/test_core_set_output.py` & `pygithubactions-0.1.5/tests/test_core_set_output.py`

 * *Files identical despite different names*

### Comparing `pygithubactions-0.1.4/tests/test_path_utils.py` & `pygithubactions-0.1.5/tests/test_path_utils.py`

 * *Files identical despite different names*

### Comparing `pygithubactions-0.1.4/.gitignore` & `pygithubactions-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `pygithubactions-0.1.4/LICENSE` & `pygithubactions-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pygithubactions-0.1.4/pyproject.toml` & `pygithubactions-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pygithubactions-0.1.4/PKG-INFO` & `pygithubactions-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygithubactions
-Version: 0.1.4
+Version: 0.1.5
 Summary: Github actions core library implemented in python
 Project-URL: Homepage, https://github.com/lestex/pygithubactions.git
 Project-URL: Source, https://github.com/lestex/pygithubactions.git
 Author-email: Andrey Larin <lestex@gmail.com>
 License-File: LICENSE
 Keywords: pygithubactions
 Classifier: Intended Audience :: Developers
```

