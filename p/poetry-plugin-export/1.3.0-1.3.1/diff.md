# Comparing `tmp/poetry_plugin_export-1.3.0.tar.gz` & `tmp/poetry_plugin_export-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_plugin_export-1.3.0.tar", max compression
+gzip compressed data, was "poetry_plugin_export-1.3.1.tar", max compression
```

## Comparing `poetry_plugin_export-1.3.0.tar` & `poetry_plugin_export-1.3.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1062 2023-01-30 16:37:00.479901 poetry_plugin_export-1.3.0/LICENSE
--rw-r--r--   0        0        0     1800 2023-01-30 16:37:00.479901 poetry_plugin_export-1.3.0/README.md
--rw-r--r--   0        0        0     2035 2023-01-30 16:37:00.483901 poetry_plugin_export-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      168 2023-01-30 16:37:00.483901 poetry_plugin_export-1.3.0/src/poetry_plugin_export/__init__.py
--rw-r--r--   0        0        0     3642 2023-01-30 16:37:00.483901 poetry_plugin_export-1.3.0/src/poetry_plugin_export/command.py
--rw-r--r--   0        0        0     7264 2023-01-30 16:37:00.483901 poetry_plugin_export-1.3.0/src/poetry_plugin_export/exporter.py
--rw-r--r--   0        0        0      957 2023-01-30 16:37:00.483901 poetry_plugin_export-1.3.0/src/poetry_plugin_export/plugins.py
--rw-r--r--   0        0        0     9175 2023-01-30 16:37:00.483901 poetry_plugin_export-1.3.0/src/poetry_plugin_export/walker.py
--rw-r--r--   0        0        0        0 2023-01-30 16:37:00.483901 poetry_plugin_export-1.3.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-01-30 16:37:00.483901 poetry_plugin_export-1.3.0/tests/command/__init__.py
--rw-r--r--   0        0        0     2590 2023-01-30 16:37:00.483901 poetry_plugin_export-1.3.0/tests/command/conftest.py
--rw-r--r--   0        0        0     7819 2023-01-30 16:37:00.483901 poetry_plugin_export-1.3.0/tests/command/test_command_export.py
--rw-r--r--   0        0        0     5325 2023-01-30 16:37:00.483901 poetry_plugin_export-1.3.0/tests/conftest.py
--rw-r--r--   0        0        0     1116 2023-01-30 16:37:00.483901 poetry_plugin_export-1.3.0/tests/fixtures/distributions/demo-0.1.0-py2.py3-none-any.whl
--rw-r--r--   0        0        0      961 2023-01-30 16:37:00.483901 poetry_plugin_export-1.3.0/tests/fixtures/distributions/demo-0.1.0.tar.gz
--rw-r--r--   0        0        0      264 2023-01-30 16:37:00.483901 poetry_plugin_export-1.3.0/tests/fixtures/project_with_nested_local/bar/pyproject.toml
--rw-r--r--   0        0        0      262 2023-01-30 16:37:00.483901 poetry_plugin_export-1.3.0/tests/fixtures/project_with_nested_local/foo/pyproject.toml
--rw-r--r--   0        0        0      324 2023-01-30 16:37:00.483901 poetry_plugin_export-1.3.0/tests/fixtures/project_with_nested_local/pyproject.toml
--rw-r--r--   0        0        0      221 2023-01-30 16:37:00.483901 poetry_plugin_export-1.3.0/tests/fixtures/project_with_nested_local/quix/pyproject.toml
--rw-r--r--   0        0        0        0 2023-01-30 16:37:00.483901 poetry_plugin_export-1.3.0/tests/fixtures/project_with_setup/my_package/__init__.py
--rw-r--r--   0        0        0      239 2023-01-30 16:37:00.483901 poetry_plugin_export-1.3.0/tests/fixtures/project_with_setup/project_with_setup.egg-info/PKG-INFO
--rw-r--r--   0        0        0      201 2023-01-30 16:37:00.483901 poetry_plugin_export-1.3.0/tests/fixtures/project_with_setup/project_with_setup.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        0 2023-01-30 16:37:00.483901 poetry_plugin_export-1.3.0/tests/fixtures/project_with_setup/project_with_setup.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       38 2023-01-30 16:37:00.483901 poetry_plugin_export-1.3.0/tests/fixtures/project_with_setup/project_with_setup.egg-info/requires.txt
--rw-r--r--   0        0        0       11 2023-01-30 16:37:00.483901 poetry_plugin_export-1.3.0/tests/fixtures/project_with_setup/project_with_setup.egg-info/top_level.txt
--rw-r--r--   0        0        0      416 2023-01-30 16:37:00.483901 poetry_plugin_export-1.3.0/tests/fixtures/project_with_setup/setup.py
--rw-r--r--   0        0        0       22 2023-01-30 16:37:00.483901 poetry_plugin_export-1.3.0/tests/fixtures/sample_project/README.rst
--rw-r--r--   0        0        0     1487 2023-01-30 16:37:00.483901 poetry_plugin_export-1.3.0/tests/fixtures/sample_project/pyproject.toml
--rw-r--r--   0        0        0       22 2023-01-30 16:37:00.483901 poetry_plugin_export-1.3.0/tests/fixtures/simple_project/README.rst
--rw-r--r--   0        0        0     1106 2023-01-30 16:37:00.483901 poetry_plugin_export-1.3.0/tests/fixtures/simple_project/dist/simple-project-1.2.3.tar.gz
--rw-r--r--   0        0        0     1320 2023-01-30 16:37:00.483901 poetry_plugin_export-1.3.0/tests/fixtures/simple_project/dist/simple_project-1.2.3-py2.py3-none-any.whl
--rw-r--r--   0        0        0      771 2023-01-30 16:37:00.483901 poetry_plugin_export-1.3.0/tests/fixtures/simple_project/pyproject.toml
--rw-r--r--   0        0        0        0 2023-01-30 16:37:00.483901 poetry_plugin_export-1.3.0/tests/fixtures/simple_project/simple_project/__init__.py
--rw-r--r--   0        0        0     3180 2023-01-30 16:37:00.483901 poetry_plugin_export-1.3.0/tests/helpers.py
--rw-r--r--   0        0        0     1262 2023-01-30 16:37:00.483901 poetry_plugin_export-1.3.0/tests/markers.py
--rw-r--r--   0        0        0    87815 2023-01-30 16:37:00.483901 poetry_plugin_export-1.3.0/tests/test_exporter.py
--rw-r--r--   0        0        0     1010 2023-01-30 16:37:00.483901 poetry_plugin_export-1.3.0/tests/types.py
--rw-r--r--   0        0        0     2826 1970-01-01 00:00:00.000000 poetry_plugin_export-1.3.0/setup.py
--rw-r--r--   0        0        0     2629 1970-01-01 00:00:00.000000 poetry_plugin_export-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-04-17 14:40:05.811764 poetry_plugin_export-1.3.1/LICENSE
+-rw-r--r--   0        0        0     1800 2023-04-17 14:40:05.811764 poetry_plugin_export-1.3.1/README.md
+-rw-r--r--   0        0        0     2035 2023-04-17 14:40:05.811764 poetry_plugin_export-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0      168 2023-04-17 14:40:05.811764 poetry_plugin_export-1.3.1/src/poetry_plugin_export/__init__.py
+-rw-r--r--   0        0        0     3678 2023-04-17 14:40:05.811764 poetry_plugin_export-1.3.1/src/poetry_plugin_export/command.py
+-rw-r--r--   0        0        0     7264 2023-04-17 14:40:05.811764 poetry_plugin_export-1.3.1/src/poetry_plugin_export/exporter.py
+-rw-r--r--   0        0        0      957 2023-04-17 14:40:05.811764 poetry_plugin_export-1.3.1/src/poetry_plugin_export/plugins.py
+-rw-r--r--   0        0        0     9933 2023-04-17 14:40:05.811764 poetry_plugin_export-1.3.1/src/poetry_plugin_export/walker.py
+-rw-r--r--   0        0        0        0 2023-04-17 14:40:05.811764 poetry_plugin_export-1.3.1/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-17 14:40:05.811764 poetry_plugin_export-1.3.1/tests/command/__init__.py
+-rw-r--r--   0        0        0     2549 2023-04-17 14:40:05.811764 poetry_plugin_export-1.3.1/tests/command/conftest.py
+-rw-r--r--   0        0        0     7819 2023-04-17 14:40:05.811764 poetry_plugin_export-1.3.1/tests/command/test_command_export.py
+-rw-r--r--   0        0        0     5325 2023-04-17 14:40:05.811764 poetry_plugin_export-1.3.1/tests/conftest.py
+-rw-r--r--   0        0        0     1116 2023-04-17 14:40:05.811764 poetry_plugin_export-1.3.1/tests/fixtures/distributions/demo-0.1.0-py2.py3-none-any.whl
+-rw-r--r--   0        0        0      961 2023-04-17 14:40:05.811764 poetry_plugin_export-1.3.1/tests/fixtures/distributions/demo-0.1.0.tar.gz
+-rw-r--r--   0        0        0      264 2023-04-17 14:40:05.811764 poetry_plugin_export-1.3.1/tests/fixtures/project_with_nested_local/bar/pyproject.toml
+-rw-r--r--   0        0        0      262 2023-04-17 14:40:05.811764 poetry_plugin_export-1.3.1/tests/fixtures/project_with_nested_local/foo/pyproject.toml
+-rw-r--r--   0        0        0      324 2023-04-17 14:40:05.811764 poetry_plugin_export-1.3.1/tests/fixtures/project_with_nested_local/pyproject.toml
+-rw-r--r--   0        0        0      221 2023-04-17 14:40:05.811764 poetry_plugin_export-1.3.1/tests/fixtures/project_with_nested_local/quix/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-17 14:40:05.811764 poetry_plugin_export-1.3.1/tests/fixtures/project_with_setup/my_package/__init__.py
+-rw-r--r--   0        0        0      239 2023-04-17 14:40:05.815764 poetry_plugin_export-1.3.1/tests/fixtures/project_with_setup/project_with_setup.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      201 2023-04-17 14:40:05.815764 poetry_plugin_export-1.3.1/tests/fixtures/project_with_setup/project_with_setup.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        0 2023-04-17 14:40:05.815764 poetry_plugin_export-1.3.1/tests/fixtures/project_with_setup/project_with_setup.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0       38 2023-04-17 14:40:05.815764 poetry_plugin_export-1.3.1/tests/fixtures/project_with_setup/project_with_setup.egg-info/requires.txt
+-rw-r--r--   0        0        0       11 2023-04-17 14:40:05.815764 poetry_plugin_export-1.3.1/tests/fixtures/project_with_setup/project_with_setup.egg-info/top_level.txt
+-rw-r--r--   0        0        0      416 2023-04-17 14:40:05.815764 poetry_plugin_export-1.3.1/tests/fixtures/project_with_setup/setup.py
+-rw-r--r--   0        0        0       22 2023-04-17 14:40:05.815764 poetry_plugin_export-1.3.1/tests/fixtures/sample_project/README.rst
+-rw-r--r--   0        0        0     1495 2023-04-17 14:40:05.815764 poetry_plugin_export-1.3.1/tests/fixtures/sample_project/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-04-17 14:40:05.815764 poetry_plugin_export-1.3.1/tests/fixtures/simple_project/README.rst
+-rw-r--r--   0        0        0     1106 2023-04-17 14:40:05.815764 poetry_plugin_export-1.3.1/tests/fixtures/simple_project/dist/simple-project-1.2.3.tar.gz
+-rw-r--r--   0        0        0     1320 2023-04-17 14:40:05.815764 poetry_plugin_export-1.3.1/tests/fixtures/simple_project/dist/simple_project-1.2.3-py2.py3-none-any.whl
+-rw-r--r--   0        0        0      771 2023-04-17 14:40:05.815764 poetry_plugin_export-1.3.1/tests/fixtures/simple_project/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-17 14:40:05.815764 poetry_plugin_export-1.3.1/tests/fixtures/simple_project/simple_project/__init__.py
+-rw-r--r--   0        0        0     3174 2023-04-17 14:40:05.815764 poetry_plugin_export-1.3.1/tests/helpers.py
+-rw-r--r--   0        0        0     1262 2023-04-17 14:40:05.815764 poetry_plugin_export-1.3.1/tests/markers.py
+-rw-r--r--   0        0        0    84039 2023-04-17 14:40:05.815764 poetry_plugin_export-1.3.1/tests/test_exporter.py
+-rw-r--r--   0        0        0      995 2023-04-17 14:40:05.815764 poetry_plugin_export-1.3.1/tests/test_walker.py
+-rw-r--r--   0        0        0     1010 2023-04-17 14:40:05.815764 poetry_plugin_export-1.3.1/tests/types.py
+-rw-r--r--   0        0        0     2629 1970-01-01 00:00:00.000000 poetry_plugin_export-1.3.1/PKG-INFO
```

### Comparing `poetry_plugin_export-1.3.0/LICENSE` & `poetry_plugin_export-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_plugin_export-1.3.0/README.md` & `poetry_plugin_export-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `poetry_plugin_export-1.3.0/pyproject.toml` & `poetry_plugin_export-1.3.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-plugin-export"
-version = "1.3.0"
+version = "1.3.1"
 description = "Poetry plugin to export the dependencies to various formats"
 authors = ["Sébastien Eustace <sebastien@eustace.io>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://python-poetry.org/"
 repository = "https://github.com/python-poetry/poetry-plugin-export"
```

### Comparing `poetry_plugin_export-1.3.0/src/poetry_plugin_export/command.py` & `poetry_plugin_export-1.3.1/src/poetry_plugin_export/command.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,16 +14,18 @@
     name = "export"
     description = "Exports the lock file to alternative formats."
 
     options = [
         option(
             "format",
             "f",
-            "Format to export to. Currently, only constraints.txt and requirements.txt"
-            " are supported.",
+            (
+                "Format to export to. Currently, only constraints.txt and"
+                " requirements.txt are supported."
+            ),
             flag=False,
             default=Exporter.FORMAT_REQUIREMENTS_TXT,
         ),
         option("output", "o", "The name of the output file.", flag=False),
         option("without-hashes", None, "Exclude hashes from the exported file."),
         option(
             "without-urls",
```

### Comparing `poetry_plugin_export-1.3.0/src/poetry_plugin_export/exporter.py` & `poetry_plugin_export-1.3.1/src/poetry_plugin_export/exporter.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_export-1.3.0/src/poetry_plugin_export/plugins.py` & `poetry_plugin_export-1.3.1/src/poetry_plugin_export/plugins.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_export-1.3.0/src/poetry_plugin_export/walker.py` & `poetry_plugin_export-1.3.1/src/poetry_plugin_export/walker.py`

 * *Files 6% similar despite different names*

```diff
@@ -238,14 +238,31 @@
         if package.python_constraint.allows_all(dependency.python_constraint)
         and dependency.constraint.allows(package.version)
         and (dependency.source_type is None or dependency.is_same_source_as(package))
     ]
 
     # If we have an overlapping candidate, we must use it.
     if overlapping_candidates:
-        compatible_candidates = [
+        filtered_compatible_candidates = [
             package
             for package in compatible_candidates
             if package in overlapping_candidates
         ]
 
+        if not filtered_compatible_candidates:
+            # TODO: Support this case:
+            # https://github.com/python-poetry/poetry-plugin-export/issues/183
+            raise DependencyWalkerError(
+                f"The `{dependency.name}` package has the following compatible"
+                f" candidates `{compatible_candidates}`;  but, the exporter dependency"
+                f" walker previously elected `{overlapping_candidates.pop()}` which is"
+                f" not compatible with the dependency `{dependency}`. Please contribute"
+                " to `poetry-plugin-export` to solve this problem."
+            )
+
+        compatible_candidates = filtered_compatible_candidates
+
     return next(iter(compatible_candidates), None)
+
+
+class DependencyWalkerError(Exception):
+    pass
```

### Comparing `poetry_plugin_export-1.3.0/tests/command/conftest.py` & `poetry_plugin_export-1.3.1/tests/command/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,14 @@
                 poetry.package,
                 poetry.locker,
                 poetry.pool,
                 poetry.config,
                 executor=executor
                 or TestExecutor(env, poetry.pool, poetry.config, tester.io),
             )
-            installer.use_executor(True)
             cmd.set_installer(installer)
 
         return tester
 
     return _tester
```

### Comparing `poetry_plugin_export-1.3.0/tests/command/test_command_export.py` & `poetry_plugin_export-1.3.1/tests/command/test_command_export.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_export-1.3.0/tests/conftest.py` & `poetry_plugin_export-1.3.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_export-1.3.0/tests/fixtures/distributions/demo-0.1.0-py2.py3-none-any.whl` & `poetry_plugin_export-1.3.1/tests/fixtures/distributions/demo-0.1.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry_plugin_export-1.3.0/tests/fixtures/distributions/demo-0.1.0.tar.gz` & `poetry_plugin_export-1.3.1/tests/fixtures/distributions/demo-0.1.0.tar.gz`

 * *Files identical despite different names*

### Comparing `poetry_plugin_export-1.3.0/tests/fixtures/sample_project/pyproject.toml` & `poetry_plugin_export-1.3.1/tests/fixtures/sample_project/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tool.poetry]
-name = "my-package"
+name = "sample-project"
 version = "1.2.3"
 description = "Some description."
 authors = [
     "Sébastien Eustace <sebastien@eustace.io>"
 ]
 license = "MIT"
 
@@ -47,12 +47,12 @@
 db = [ "orator" ]
 
 [tool.poetry.dev-dependencies]
 pytest = "~3.4"
 
 
 [tool.poetry.scripts]
-my-script = "my_package:main"
+my-script = "sample_project:main"
 
 
 [tool.poetry.plugins."blogtool.parsers"]
 ".rst" = "some_module::SomeClass"
```

### Comparing `poetry_plugin_export-1.3.0/tests/fixtures/simple_project/dist/simple-project-1.2.3.tar.gz` & `poetry_plugin_export-1.3.1/tests/fixtures/simple_project/dist/simple-project-1.2.3.tar.gz`

 * *Files identical despite different names*

### Comparing `poetry_plugin_export-1.3.0/tests/fixtures/simple_project/dist/simple_project-1.2.3-py2.py3-none-any.whl` & `poetry_plugin_export-1.3.1/tests/fixtures/simple_project/dist/simple_project-1.2.3-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry_plugin_export-1.3.0/tests/fixtures/simple_project/pyproject.toml` & `poetry_plugin_export-1.3.1/tests/fixtures/simple_project/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry_plugin_export-1.3.0/tests/helpers.py` & `poetry_plugin_export-1.3.1/tests/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         self._poetry.set_config(poetry.config)
         self._poetry.set_locker(
             TestLocker(poetry.locker.lock, self._poetry.local_config)
         )
 
 
 class TestLocker(Locker):
-    def __init__(self, lock: str | Path, local_config: dict[str, Any]) -> None:
+    def __init__(self, lock: Path, local_config: dict[str, Any]) -> None:
         super().__init__(lock, local_config)
         self._locked = False
         self._write = False
         self._contains_credential = False
 
     def write(self, write: bool = True) -> None:
         self._write = write
```

### Comparing `poetry_plugin_export-1.3.0/tests/markers.py` & `poetry_plugin_export-1.3.1/tests/markers.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_export-1.3.0/tests/test_exporter.py` & `poetry_plugin_export-1.3.1/tests/test_exporter.py`

 * *Files 10% similar despite different names*

```diff
@@ -76,22 +76,25 @@
 def poetry(fixture_root: Path, locker: Locker) -> Poetry:
     p = Factory().create_poetry(fixture_root / "sample_project")
     p._locker = locker
 
     return p
 
 
-def set_package_requires(poetry: Poetry, skip: set[str] | None = None) -> None:
+def set_package_requires(
+    poetry: Poetry, skip: set[str] | None = None, dev: set[str] | None = None
+) -> None:
     skip = skip or set()
+    dev = dev or set()
     packages = poetry.locker.locked_repository().packages
     package = poetry.package.with_dependency_groups([], only=True)
     for pkg in packages:
         if pkg.name not in skip:
             dep = pkg.to_dependency()
-            if pkg.category == "dev":
+            if pkg.name in dev:
                 dep._groups = frozenset(["dev"])
             package.add_dependency(dep)
 
     poetry._package = package
 
 
 def test_exporter_can_export_requirements_txt_with_standard_packages(
@@ -99,22 +102,20 @@
 ) -> None:
     poetry.locker.mock_lock_data(  # type: ignore[attr-defined]
         {
             "package": [
                 {
                     "name": "foo",
                     "version": "1.2.3",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                 },
                 {
                     "name": "bar",
                     "version": "4.5.6",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                 },
             ],
             "metadata": {
                 "python-versions": "*",
                 "content-hash": "123456789",
@@ -143,31 +144,28 @@
 ) -> None:
     poetry.locker.mock_lock_data(  # type: ignore[attr-defined]
         {
             "package": [
                 {
                     "name": "foo",
                     "version": "1.2.3",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                     "marker": "python_version < '3.7'",
                 },
                 {
                     "name": "bar",
                     "version": "4.5.6",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                     "marker": "extra =='foo'",
                 },
                 {
                     "name": "baz",
                     "version": "7.8.9",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                     "marker": "sys_platform == 'win32'",
                 },
             ],
             "metadata": {
                 "python-versions": "*",
@@ -200,60 +198,54 @@
 
     poetry.locker.mock_lock_data(  # type: ignore[attr-defined]
         {
             "package": [
                 {
                     "name": "poetry",
                     "version": "1.1.4",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                     "dependencies": {"keyring": "*"},
                 },
                 {
                     "name": "junit-xml",
                     "version": "1.9",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                     "dependencies": {"six": "*"},
                 },
                 {
                     "name": "keyring",
                     "version": "21.8.0",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                     "dependencies": {
                         "SecretStorage": {
                             "version": "*",
                             "markers": "sys_platform == 'linux'",
                         }
                     },
                 },
                 {
                     "name": "secretstorage",
                     "version": "3.3.0",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                     "dependencies": {"cryptography": "*"},
                 },
                 {
                     "name": "cryptography",
                     "version": "3.2",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                     "dependencies": {"six": "*"},
                 },
                 {
                     "name": "six",
                     "version": "1.15.0",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                 },
             ],
             "metadata": {
                 "python-versions": "*",
                 "content-hash": "123456789",
@@ -321,36 +313,33 @@
 
     poetry.locker.mock_lock_data(  # type: ignore[attr-defined]
         {
             "package": [
                 {
                     "name": "pyinstaller",
                     "version": "4.0",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                     "dependencies": {
                         "altgraph": "*",
                         "macholib": {
                             "version": "*",
                             "markers": "sys_platform == 'darwin'",
                         },
                     },
                 },
                 {
                     "name": "altgraph",
                     "version": "0.17",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                 },
                 {
                     "name": "macholib",
                     "version": "1.8",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                     "dependencies": {"altgraph": ">=0.15"},
                 },
             ],
             "metadata": {
                 "python-versions": "*",
@@ -401,42 +390,38 @@
 ) -> None:
     poetry.locker.mock_lock_data(  # type: ignore[attr-defined]
         {
             "package": [
                 {
                     "name": "a",
                     "version": "1.2.3",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                     "marker": "python_version < '3.7'",
                     "dependencies": {"b": ">=0.0.0", "c": ">=0.0.0"},
                 },
                 {
                     "name": "b",
                     "version": "4.5.6",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                     "marker": "platform_system == 'Windows'",
                     "dependencies": {"d": ">=0.0.0"},
                 },
                 {
                     "name": "c",
                     "version": "7.8.9",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                     "marker": "sys_platform == 'win32'",
                     "dependencies": {"d": ">=0.0.0"},
                 },
                 {
                     "name": "d",
                     "version": "0.0.1",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                 },
             ],
             "metadata": {
                 "python-versions": "*",
                 "content-hash": "123456789",
@@ -496,22 +481,20 @@
 ) -> None:
     poetry.locker.mock_lock_data(  # type: ignore[attr-defined]
         {
             "package": [
                 {
                     "name": "a",
                     "version": "1.2.3",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                 },
                 {
                     "name": "b",
                     "version": "4.5.6",
-                    "category": "dev",
                     "optional": False,
                     "python-versions": "*",
                     "dependencies": {"a": ">=1.2.3"},
                 },
             ],
             "metadata": {
                 "python-versions": "*",
@@ -550,22 +533,20 @@
 ) -> None:
     poetry.locker.mock_lock_data(  # type: ignore[attr-defined]
         {
             "package": [
                 {
                     "name": "foo",
                     "version": "1.2.3",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                 },
                 {
                     "name": "bar",
                     "version": "4.5.6",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                 },
             ],
             "metadata": {
                 "python-versions": "*",
                 "content-hash": "123456789",
@@ -599,22 +580,20 @@
 ) -> None:
     poetry.locker.mock_lock_data(  # type: ignore[attr-defined]
         {
             "package": [
                 {
                     "name": "foo",
                     "version": "1.2.3",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                 },
                 {
                     "name": "bar",
                     "version": "4.5.6",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                 },
             ],
             "metadata": {
                 "python-versions": "*",
                 "content-hash": "123456789",
@@ -656,22 +635,20 @@
 ) -> None:
     poetry.locker.mock_lock_data(  # type: ignore[attr-defined]
         {
             "package": [
                 {
                     "name": "foo",
                     "version": "1.2.3",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                 },
                 {
                     "name": "bar",
                     "version": "4.5.6",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                 },
             ],
             "metadata": {
                 "python-versions": "*",
                 "content-hash": "123456789",
@@ -704,37 +681,35 @@
 ) -> None:
     poetry.locker.mock_lock_data(  # type: ignore[attr-defined]
         {
             "package": [
                 {
                     "name": "foo",
                     "version": "1.2.3",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                 },
                 {
                     "name": "bar",
                     "version": "4.5.6",
-                    "category": "dev",
                     "optional": False,
                     "python-versions": "*",
                 },
             ],
             "metadata": {
                 "python-versions": "*",
                 "content-hash": "123456789",
                 "files": {
                     "foo": [{"name": "foo.whl", "hash": "12345"}],
                     "bar": [{"name": "bar.whl", "hash": "67890"}],
                 },
             },
         }
     )
-    set_package_requires(poetry)
+    set_package_requires(poetry, dev={"bar"})
 
     exporter = Exporter(poetry, NullIO())
     exporter.export("requirements.txt", tmp_path, "requirements.txt")
 
     with (tmp_path / "requirements.txt").open(encoding="utf-8") as f:
         content = f.read()
 
@@ -751,37 +726,35 @@
 ) -> None:
     poetry.locker.mock_lock_data(  # type: ignore[attr-defined]
         {
             "package": [
                 {
                     "name": "foo",
                     "version": "1.2.3",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                 },
                 {
                     "name": "bar",
                     "version": "4.5.6",
-                    "category": "dev",
                     "optional": False,
                     "python-versions": "*",
                 },
             ],
             "metadata": {
                 "python-versions": "*",
                 "content-hash": "123456789",
                 "files": {
                     "foo": [{"name": "foo.whl", "hash": "12345"}],
                     "bar": [{"name": "bar.whl", "hash": "67890"}],
                 },
             },
         }
     )
-    set_package_requires(poetry)
+    set_package_requires(poetry, dev={"bar"})
 
     exporter = Exporter(poetry, NullIO())
     exporter.only_groups([MAIN_GROUP, "dev"])
     exporter.export("requirements.txt", tmp_path, "requirements.txt")
 
     with (tmp_path / "requirements.txt").open(encoding="utf-8") as f:
         content = f.read()
@@ -801,37 +774,35 @@
 ) -> None:
     poetry.locker.mock_lock_data(  # type: ignore[attr-defined]
         {
             "package": [
                 {
                     "name": "foo",
                     "version": "1.2.3",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                 },
                 {
                     "name": "bar",
                     "version": "4.5.6",
-                    "category": "dev",
                     "optional": False,
                     "python-versions": "*",
                 },
             ],
             "metadata": {
                 "python-versions": "*",
                 "content-hash": "123456789",
                 "files": {
                     "foo": [{"name": "foo.whl", "hash": "12345"}],
                     "bar": [{"name": "bar.whl", "hash": "67890"}],
                 },
             },
         }
     )
-    set_package_requires(poetry)
+    set_package_requires(poetry, dev={"bar"})
 
     exporter = Exporter(poetry, NullIO())
     exporter.only_groups([])
     exporter.export("requirements.txt", tmp_path, "requirements.txt")
 
     with (tmp_path / "requirements.txt").open(encoding="utf-8") as f:
         content = f.read()
@@ -844,37 +815,35 @@
 ) -> None:
     poetry.locker.mock_lock_data(  # type: ignore[attr-defined]
         {
             "package": [
                 {
                     "name": "foo",
                     "version": "1.2.3",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                 },
                 {
                     "name": "bar",
                     "version": "4.5.6",
-                    "category": "dev",
                     "optional": True,
                     "python-versions": "*",
                 },
             ],
             "metadata": {
                 "python-versions": "*",
                 "content-hash": "123456789",
                 "files": {
                     "foo": [{"name": "foo.whl", "hash": "12345"}],
                     "bar": [{"name": "bar.whl", "hash": "67890"}],
                 },
             },
         }
     )
-    set_package_requires(poetry)
+    set_package_requires(poetry, dev={"bar"})
 
     exporter = Exporter(poetry, NullIO())
     exporter.only_groups([MAIN_GROUP, "dev"])
     exporter.export("requirements.txt", tmp_path, "requirements.txt")
 
     with (tmp_path / "requirements.txt").open(encoding="utf-8") as f:
         content = f.read()
@@ -908,30 +877,27 @@
 ) -> None:
     poetry.locker.mock_lock_data(  # type: ignore[attr-defined]
         {
             "package": [
                 {
                     "name": "foo",
                     "version": "1.2.3",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                 },
                 {
                     "name": "bar",
                     "version": "4.5.6",
-                    "category": "main",
                     "optional": True,
                     "python-versions": "*",
                     "dependencies": {"spam": ">=0.1"},
                 },
                 {
                     "name": "spam",
                     "version": "0.1.0",
-                    "category": "main",
                     "optional": True,
                     "python-versions": "*",
                 },
             ],
             "metadata": {
                 "python-versions": "*",
                 "content-hash": "123456789",
@@ -969,15 +935,14 @@
 ) -> None:
     poetry.locker.mock_lock_data(  # type: ignore[attr-defined]
         {
             "package": [
                 {
                     "name": "foo",
                     "version": "1.2.3",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                     "source": {
                         "type": "git",
                         "url": "https://github.com/foo/foo.git",
                         "reference": "123456",
                     },
@@ -1010,27 +975,25 @@
 ) -> None:
     poetry.locker.mock_lock_data(  # type: ignore[attr-defined]
         {
             "package": [
                 {
                     "name": "foo",
                     "version": "1.2.3",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                     "source": {
                         "type": "git",
                         "url": "https://github.com/foo/foo.git",
                         "reference": "123456",
                     },
                 },
                 {
                     "name": "bar",
                     "version": "4.5.6",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                     "dependencies": {
                         "foo": {
                             "git": "https://github.com/foo/foo.git",
                             "rev": "123456",
                         }
@@ -1065,31 +1028,28 @@
 ) -> None:
     poetry.locker.mock_lock_data(  # type: ignore[attr-defined]
         {
             "package": [
                 {
                     "name": "foo",
                     "version": "1.2.3",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                     "dependencies": {"bar": {"version": "4.5.6"}},
                 },
                 {
                     "name": "bar",
                     "version": "4.5.6",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                     "dependencies": {"baz": {"version": "7.8.9"}},
                 },
                 {
                     "name": "baz",
                     "version": "7.8.9",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                     "dependencies": {"foo": {"version": "1.2.3"}},
                 },
             ],
             "metadata": {
                 "python-versions": "*",
@@ -1120,15 +1080,14 @@
 ) -> None:
     poetry.locker.mock_lock_data(  # type: ignore[attr-defined]
         {
             "package": [
                 {
                     "name": "foo",
                     "version": "1.2.3",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                     "dependencies": {poetry.package.pretty_name: {"version": "1.2.3"}},
                 },
             ],
             "metadata": {
                 "python-versions": "*",
@@ -1157,15 +1116,14 @@
 ) -> None:
     poetry.locker.mock_lock_data(  # type: ignore[attr-defined]
         {
             "package": [
                 {
                     "name": "foo",
                     "version": "1.2.3",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                     "dependencies": {
                         "bar": [
                             {
                                 "version": ">=1.2.3,<7.8.10",
                                 "markers": 'platform_system != "Windows"',
@@ -1176,28 +1134,26 @@
                             },
                         ]
                     },
                 },
                 {
                     "name": "bar",
                     "version": "7.8.9",
-                    "category": "main",
                     "optional": True,
                     "python-versions": "*",
                     "dependencies": {
                         "baz": {
                             "version": "!=10.11.12",
                             "markers": 'platform_system == "Windows"',
                         }
                     },
                 },
                 {
                     "name": "baz",
                     "version": "10.11.13",
-                    "category": "main",
                     "optional": True,
                     "python-versions": "*",
                 },
             ],
             "metadata": {
                 "python-versions": "*",
                 "content-hash": "123456789",
@@ -1231,15 +1187,14 @@
 ) -> None:
     poetry.locker.mock_lock_data(  # type: ignore[attr-defined]
         {
             "package": [
                 {
                     "name": "foo",
                     "version": "1.2.3",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                     "marker": "python_version < '3.7'",
                     "source": {
                         "type": "git",
                         "url": "https://github.com/foo/foo.git",
                         "reference": "123456",
@@ -1273,15 +1228,14 @@
 ) -> None:
     poetry.locker.mock_lock_data(  # type: ignore[attr-defined]
         {
             "package": [
                 {
                     "name": "foo",
                     "version": "1.2.3",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                     "source": {
                         "type": "directory",
                         "url": "sample_project",
                         "reference": "",
                     },
@@ -1314,39 +1268,36 @@
 ) -> None:
     poetry.locker.mock_lock_data(  # type: ignore[attr-defined]
         {
             "package": [
                 {
                     "name": "foo",
                     "version": "1.2.3",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                     "source": {
                         "type": "directory",
                         "url": "sample_project",
                         "reference": "",
                     },
                 },
                 {
                     "name": "bar",
                     "version": "4.5.6",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                     "source": {
                         "type": "directory",
                         "url": "sample_project/../project_with_nested_local/bar",
                         "reference": "",
                     },
                 },
                 {
                     "name": "baz",
                     "version": "7.8.9",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                     "source": {
                         "type": "directory",
                         "url": "sample_project/../project_with_nested_local/bar/..",
                         "reference": "",
                     },
@@ -1381,15 +1332,14 @@
 ) -> None:
     poetry.locker.mock_lock_data(  # type: ignore[attr-defined]
         {
             "package": [
                 {
                     "name": "foo",
                     "version": "1.2.3",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                     "marker": "python_version < '3.7'",
                     "source": {
                         "type": "directory",
                         "url": "sample_project",
                         "reference": "",
@@ -1424,15 +1374,14 @@
 ) -> None:
     poetry.locker.mock_lock_data(  # type: ignore[attr-defined]
         {
             "package": [
                 {
                     "name": "foo",
                     "version": "1.2.3",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                     "source": {
                         "type": "file",
                         "url": "distributions/demo-0.1.0.tar.gz",
                         "reference": "",
                     },
@@ -1466,15 +1415,14 @@
 ) -> None:
     poetry.locker.mock_lock_data(  # type: ignore[attr-defined]
         {
             "package": [
                 {
                     "name": "foo",
                     "version": "1.2.3",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                     "marker": "python_version < '3.7'",
                     "source": {
                         "type": "file",
                         "url": "distributions/demo-0.1.0.tar.gz",
                         "reference": "",
@@ -1515,22 +1463,20 @@
     )
     poetry.locker.mock_lock_data(  # type: ignore[attr-defined]
         {
             "package": [
                 {
                     "name": "foo",
                     "version": "1.2.3",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                 },
                 {
                     "name": "bar",
                     "version": "4.5.6",
-                    "category": "dev",
                     "optional": False,
                     "python-versions": "*",
                     "source": {
                         "type": "legacy",
                         "url": "https://example.com/simple",
                         "reference": "",
                     },
@@ -1542,15 +1488,15 @@
                 "files": {
                     "foo": [{"name": "foo.whl", "hash": "12345"}],
                     "bar": [{"name": "bar.whl", "hash": "67890"}],
                 },
             },
         }
     )
-    set_package_requires(poetry)
+    set_package_requires(poetry, dev={"bar"})
 
     exporter = Exporter(poetry, NullIO())
     exporter.only_groups([MAIN_GROUP, "dev"])
     exporter.export("requirements.txt", tmp_path, "requirements.txt")
 
     with (tmp_path / "requirements.txt").open(encoding="utf-8") as f:
         content = f.read()
@@ -1578,22 +1524,20 @@
     )
     poetry.locker.mock_lock_data(  # type: ignore[attr-defined]
         {
             "package": [
                 {
                     "name": "foo",
                     "version": "1.2.3",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                 },
                 {
                     "name": "bar",
                     "version": "4.5.6",
-                    "category": "dev",
                     "optional": False,
                     "python-versions": "*",
                     "source": {
                         "type": "legacy",
                         "url": "https://example.com/simple",
                         "reference": "",
                     },
@@ -1605,15 +1549,15 @@
                 "files": {
                     "foo": [{"name": "foo.whl", "hash": "12345"}],
                     "bar": [{"name": "bar.whl", "hash": "67890"}],
                 },
             },
         }
     )
-    set_package_requires(poetry)
+    set_package_requires(poetry, dev={"bar"})
 
     exporter = Exporter(poetry, NullIO())
     exporter.only_groups([MAIN_GROUP, "dev"])
     exporter.with_urls(False)
     exporter.export("requirements.txt", tmp_path, "requirements.txt")
 
     with (tmp_path / "requirements.txt").open(encoding="utf-8") as f:
@@ -1640,15 +1584,14 @@
     )
     poetry.locker.mock_lock_data(  # type: ignore[attr-defined]
         {
             "package": [
                 {
                     "name": "bar",
                     "version": "4.5.6",
-                    "category": "dev",
                     "optional": False,
                     "python-versions": "*",
                     "source": {
                         "type": "legacy",
                         "url": "http://example.com/simple",
                         "reference": "",
                     },
@@ -1659,15 +1602,15 @@
                 "content-hash": "123456789",
                 "files": {
                     "bar": [{"name": "bar.whl", "hash": "67890"}],
                 },
             },
         }
     )
-    set_package_requires(poetry)
+    set_package_requires(poetry, dev={"bar"})
     exporter = Exporter(poetry, NullIO())
     exporter.only_groups([MAIN_GROUP, "dev"])
     exporter.export("requirements.txt", tmp_path, "requirements.txt")
 
     with (tmp_path / "requirements.txt").open(encoding="utf-8") as f:
         content = f.read()
 
@@ -1707,49 +1650,46 @@
 ) -> None:
     poetry.locker.mock_lock_data(  # type: ignore[attr-defined]
         {
             "package": [
                 {
                     "name": "foo",
                     "version": "1.2.1",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                 },
                 {
                     "name": "bar",
                     "version": "1.2.2",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                     "dependencies": {
                         "baz": {
                             "version": ">=0.1.0",
                             "optional": True,
                             "markers": "extra == 'baz'",
                         }
                     },
                     "extras": {"baz": ["baz (>=0.1.0)"]},
                 },
                 {
                     "name": "baz",
                     "version": "1.2.3",
-                    "category": "dev",
                     "optional": False,
                     "python-versions": "*",
                 },
             ],
             "metadata": {
                 "python-versions": "*",
                 "content-hash": "123456789",
                 "files": {"foo": [], "bar": [], "baz": []},
             },
         }
     )
-    set_package_requires(poetry)
+    set_package_requires(poetry, dev={"baz"})
 
     exporter = Exporter(poetry, NullIO())
     if dev:
         exporter.only_groups([MAIN_GROUP, "dev"])
     exporter.export("requirements.txt", tmp_path, "requirements.txt")
 
     with (tmp_path / "requirements.txt").open(encoding="utf-8") as f:
@@ -1775,39 +1715,36 @@
     )
     poetry.locker.mock_lock_data(  # type: ignore[attr-defined]
         {
             "package": [
                 {
                     "name": "foo",
                     "version": "1.2.3",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                     "source": {
                         "type": "legacy",
                         "url": "https://example.com/simple",
                         "reference": "",
                     },
                 },
                 {
                     "name": "bar",
                     "version": "4.5.6",
-                    "category": "dev",
                     "optional": False,
                     "python-versions": "*",
                     "source": {
                         "type": "legacy",
                         "url": "https://example.com/simple",
                         "reference": "",
                     },
                 },
                 {
                     "name": "baz",
                     "version": "7.8.9",
-                    "category": "dev",
                     "optional": False,
                     "python-versions": "*",
                     "source": {
                         "type": "legacy",
                         "url": "https://foobaz.com/simple",
                         "reference": "",
                     },
@@ -1820,15 +1757,15 @@
                     "foo": [{"name": "foo.whl", "hash": "12345"}],
                     "bar": [{"name": "bar.whl", "hash": "67890"}],
                     "baz": [{"name": "baz.whl", "hash": "24680"}],
                 },
             },
         }
     )
-    set_package_requires(poetry)
+    set_package_requires(poetry, dev={"bar", "baz"})
 
     exporter = Exporter(poetry, NullIO())
     exporter.only_groups([MAIN_GROUP, "dev"])
     exporter.export("requirements.txt", tmp_path, "requirements.txt")
 
     with (tmp_path / "requirements.txt").open(encoding="utf-8") as f:
         content = f.read()
@@ -1882,39 +1819,36 @@
     )
     poetry.locker.mock_lock_data(  # type: ignore[attr-defined]
         {
             "package": [
                 {
                     "name": "foo",
                     "version": "1.2.3",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                     "source": {
                         "type": "legacy",
                         "url": "https://a.example.com/simple",
                         "reference": "",
                     },
                 },
                 {
                     "name": "bar",
                     "version": "4.5.6",
-                    "category": "dev",
                     "optional": False,
                     "python-versions": "*",
                     "source": {
                         "type": "legacy",
                         "url": "https://b.example.com/simple",
                         "reference": "",
                     },
                 },
                 {
                     "name": "baz",
                     "version": "7.8.9",
-                    "category": "dev",
                     "optional": False,
                     "python-versions": "*",
                     "source": {
                         "type": "legacy",
                         "url": "https://b.example.com/simple",
                         "reference": "",
                     },
@@ -1927,15 +1861,15 @@
                     "foo": [{"name": "foo.whl", "hash": "12345"}],
                     "bar": [{"name": "bar.whl", "hash": "67890"}],
                     "baz": [{"name": "baz.whl", "hash": "24680"}],
                 },
             },
         }
     )
-    set_package_requires(poetry)
+    set_package_requires(poetry, dev={"bar", "baz"})
 
     exporter = Exporter(poetry, NullIO())
     exporter.only_groups([MAIN_GROUP, "dev"])
     exporter.with_credentials()
     exporter.export("requirements.txt", tmp_path, "requirements.txt")
 
     with (tmp_path / "requirements.txt").open(encoding="utf-8") as f:
@@ -1970,22 +1904,20 @@
     )
     poetry.locker.mock_lock_data(  # type: ignore[attr-defined]
         {
             "package": [
                 {
                     "name": "foo",
                     "version": "1.2.3",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                 },
                 {
                     "name": "bar",
                     "version": "4.5.6",
-                    "category": "dev",
                     "optional": False,
                     "python-versions": "*",
                     "source": {
                         "type": "legacy",
                         "url": "https://example.com/simple",
                         "reference": "",
                     },
@@ -1997,15 +1929,15 @@
                 "files": {
                     "foo": [{"name": "foo.whl", "hash": "12345"}],
                     "bar": [{"name": "bar.whl", "hash": "67890"}],
                 },
             },
         }
     )
-    set_package_requires(poetry)
+    set_package_requires(poetry, dev={"bar"})
 
     exporter = Exporter(poetry, NullIO())
     exporter.only_groups([MAIN_GROUP, "dev"])
     exporter.with_credentials()
     exporter.export(
         "requirements.txt",
         tmp_path,
@@ -2032,22 +1964,20 @@
 ) -> None:
     poetry.locker.mock_lock_data(  # type: ignore[attr-defined]
         {
             "package": [
                 {
                     "name": "foo",
                     "version": "1.2.3",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                 },
                 {
                     "name": "bar",
                     "version": "4.5.6",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                 },
             ],
             "metadata": {
                 "python-versions": "*",
                 "content-hash": "123456789",
@@ -2075,72 +2005,65 @@
     # Testcase derived from <https://github.com/python-poetry/poetry/issues/5141>.
     poetry.locker.mock_lock_data(  # type: ignore[attr-defined]
         {
             "package": [
                 {
                     "name": "celery",
                     "version": "5.1.2",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "<3.7",
                     "dependencies": {
                         "click": ">=7.0,<8.0",
                         "click-didyoumean": ">=0.0.3",
                         "click-plugins": ">=1.1.1",
                     },
                 },
                 {
                     "name": "celery",
                     "version": "5.2.3",
-                    "category": "main",
                     "optional": False,
                     "python-versions": ">=3.7",
                     "dependencies": {
                         "click": ">=8.0.3,<9.0",
                         "click-didyoumean": ">=0.0.3",
                         "click-plugins": ">=1.1.1",
                     },
                 },
                 {
                     "name": "click",
                     "version": "7.1.2",
-                    "category": "main",
                     "optional": False,
                     "python-versions": (
                         ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*"
                     ),
                 },
                 {
                     "name": "click",
                     "version": "8.0.3",
-                    "category": "main",
                     "optional": False,
                     "python-versions": ">=3.6",
                     "dependencies": {},
                 },
                 {
                     "name": "click-didyoumean",
                     "version": "0.0.3",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                     "dependencies": {"click": "*"},
                 },
                 {
                     "name": "click-didyoumean",
                     "version": "0.3.0",
-                    "category": "main",
                     "optional": False,
                     "python-versions": ">=3.6.2,<4.0.0",
                     "dependencies": {"click": ">=7"},
                 },
                 {
                     "name": "click-plugins",
                     "version": "1.1.1",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                     "dependencies": {"click": ">=4.0"},
                 },
             ],
             "metadata": {
                 "lock-version": "1.1",
@@ -2206,15 +2129,14 @@
     poetry.locker.mock_lock_data(  # type: ignore[attr-defined]
         {
             "package": [
                 {
                     "name": "localstack",
                     "python-versions": "*",
                     "version": "1.0.0",
-                    "category": "main",
                     "optional": False,
                     "dependencies": {
                         "localstack-ext": [
                             {"version": ">=1.0.0"},
                             {
                                 "version": ">=1.0.0",
                                 "extras": ["bar"],
@@ -2224,15 +2146,14 @@
                     },
                     "extras": {"foo": ["localstack-ext[bar] (>=1.0.0)"]},
                 },
                 {
                     "name": "localstack-ext",
                     "python-versions": "*",
                     "version": "1.0.0",
-                    "category": "main",
                     "optional": False,
                     "dependencies": {
                         "something": "*",
                         "something-else": {
                             "version": ">=1.0.0",
                             "markers": 'extra == "bar"',
                         },
@@ -2246,31 +2167,28 @@
                         "baz": ["another-thing (>=1.0.0)"],
                     },
                 },
                 {
                     "name": "something",
                     "python-versions": "*",
                     "version": "1.0.0",
-                    "category": "main",
                     "optional": False,
                     "dependencies": {},
                 },
                 {
                     "name": "something-else",
                     "python-versions": "*",
                     "version": "1.0.0",
-                    "category": "main",
                     "optional": False,
                     "dependencies": {},
                 },
                 {
                     "name": "another-thing",
                     "python-versions": "*",
                     "version": "1.0.0",
-                    "category": "main",
                     "optional": False,
                     "dependencies": {},
                 },
             ],
             "metadata": {
                 "lock-version": "1.1",
                 "python-versions": "^3.6",
@@ -2319,31 +2237,28 @@
     poetry.locker.mock_lock_data(  # type: ignore[attr-defined]
         {
             "package": [
                 {
                     "name": "ipython",
                     "python-versions": ">=3.6",
                     "version": "7.16.3",
-                    "category": "main",
                     "optional": False,
                     "dependencies": {},
                 },
                 {
                     "name": "ipython",
                     "python-versions": ">=3.7",
                     "version": "7.34.0",
-                    "category": "main",
                     "optional": False,
                     "dependencies": {},
                 },
                 {
                     "name": "slash",
                     "python-versions": ">=3.6.*",
                     "version": "1.13.0",
-                    "category": "main",
                     "optional": False,
                     "dependencies": {
                         "ipython": [
                             {
                                 "version": "*",
                                 "markers": (
                                     'python_version >= "3.6" and implementation_name !='
@@ -2433,24 +2348,22 @@
     poetry.locker.mock_lock_data(  # type: ignore[attr-defined]
         {
             "package": [
                 {
                     "name": "foo",
                     "python-versions": ">=3.6",
                     "version": "1.0.0",
-                    "category": "main",
                     "optional": False,
                     "dependencies": {"pytest": {"version": "^6.2.4", "optional": True}},
                     "extras": {"test": ["pytest (>=6.2.4,<7.0.0)"]},
                 },
                 {
                     "name": "pytest",
                     "python-versions": ">=3.6",
                     "version": "6.24.0",
-                    "category": "dev",
                     "optional": False,
                     "dependencies": {},
                 },
             ],
             "metadata": {
                 "lock-version": "1.1",
                 "python-versions": "^3.6",
@@ -2517,43 +2430,40 @@
 ) -> None:
     poetry.locker.mock_lock_data(  # type: ignore[attr-defined]
         {
             "package": [
                 {
                     "name": "foo",
                     "version": "1.2.3",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                     "dependencies": {
                         "bar": {
                             "extras": ["baz"],
                             "version": ">=0.1.0",
                         }
                     },
                 },
                 {
                     "name": "bar",
                     "version": "4.5.6",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                     "dependencies": {
                         "baz": {
                             "version": ">=0.1.0",
                             "optional": True,
                             "markers": "extra == 'baz'",
                         }
                     },
                     "extras": {"baz": ["baz (>=0.1.0)"]},
                 },
                 {
                     "name": "baz",
                     "version": "7.8.9",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                 },
             ],
             "metadata": {
                 "python-versions": "*",
                 "content-hash": "123456789",
@@ -2577,35 +2487,32 @@
 ) -> None:
     poetry.locker.mock_lock_data(  # type: ignore[attr-defined]
         {
             "package": [
                 {
                     "name": "foo",
                     "version": "1.2.3",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                     "source": {
                         "type": "git",
                         "url": "https://github.com/foo/foo.git",
                         "reference": "123456",
                     },
                     "develop": True,
                 },
                 {
                     "name": "bar",
                     "version": "7.8.9",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                 },
                 {
                     "name": "baz",
                     "version": "4.5.6",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                     "source": {
                         "type": "directory",
                         "url": "sample_project",
                         "reference": "",
                     },
@@ -2644,27 +2551,25 @@
     poetry.locker.mock_lock_data(  # type: ignore[attr-defined]
         {
             "package": [
                 {
                     "name": "foo",
                     "python-versions": ">=3.6",
                     "version": "1.0.0",
-                    "category": "main",
                     "optional": False,
                     "dependencies": {},
                     "source": {
                         "type": "url",
                         "url": "https://example.com/foo-darwin.whl",
                     },
                 },
                 {
                     "name": "foo",
                     "python-versions": ">=3.6",
                     "version": "1.0.0",
-                    "category": "main",
                     "optional": False,
                     "dependencies": {},
                     "source": {
                         "type": "url",
                         "url": "https://example.com/foo-linux.whl",
                     },
                 },
@@ -2720,30 +2625,28 @@
     # extra.
     poetry.locker.mock_lock_data(  # type: ignore[attr-defined]
         {
             "package": [
                 {
                     "name": "foo",
                     "version": "1.2.3",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                     "dependencies": {
                         "bar": {
                             "version": ">=0.1.0",
                             "optional": True,
                             "markers": "extra == 'bar'",
                         }
                     },
                     "extras": {"bar": ["bar (>=0.1.0)"]},
                 },
                 {
                     "name": "bar",
                     "version": "4.5.6",
-                    "category": "main",
                     "optional": False,
                     "python-versions": "*",
                 },
             ],
             "metadata": {
                 "python-versions": "*",
                 "content-hash": "123456789",
```

### Comparing `poetry_plugin_export-1.3.0/tests/types.py` & `poetry_plugin_export-1.3.1/tests/types.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_export-1.3.0/setup.py` & `poetry_plugin_export-1.3.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,74 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: poetry-plugin-export
+Version: 1.3.1
+Summary: Poetry plugin to export the dependencies to various formats
+Home-page: https://python-poetry.org/
+License: MIT
+Author: Sébastien Eustace
+Author-email: sebastien@eustace.io
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: poetry (>=1.3.0,<2.0.0)
+Requires-Dist: poetry-core (>=1.3.0,<2.0.0)
+Project-URL: Repository, https://github.com/python-poetry/poetry-plugin-export
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': 'src'}
+# Poetry Plugin: Export
 
-packages = \
-['poetry_plugin_export']
+This package is a plugin that allows the export of locked packages to various formats.
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['poetry-core>=1.3.0,<2.0.0', 'poetry>=1.3.0,<2.0.0']
-
-entry_points = \
-{'poetry.application.plugin': ['export = '
-                               'poetry_plugin_export.plugins:ExportApplicationPlugin']}
-
-setup_kwargs = {
-    'name': 'poetry-plugin-export',
-    'version': '1.3.0',
-    'description': 'Poetry plugin to export the dependencies to various formats',
-    'long_description': '# Poetry Plugin: Export\n\nThis package is a plugin that allows the export of locked packages to various formats.\n\n**Note**: For now, only the `constraints.txt` and `requirements.txt` formats are available.\n\nThis plugin provides the same features as the existing `export` command of Poetry which it will eventually replace.\n\n\n## Installation\n\nThe easiest way to install the `export` plugin is via the `self add` command of Poetry.\n\n```bash\npoetry self add poetry-plugin-export\n```\n\nIf you used `pipx` to install Poetry you can add the plugin via the `pipx inject` command.\n\n```bash\npipx inject poetry poetry-plugin-export\n```\n\nOtherwise, if you used `pip` to install Poetry you can add the plugin packages via the `pip install` command.\n\n```bash\npip install poetry-plugin-export\n```\n\n\n## Usage\n\nThe plugin provides an `export` command to export to the desired format.\n\n```bash\npoetry export -f requirements.txt --output requirements.txt\n```\n\n**Note**: Only the `constraints.txt` and `requirements.txt` formats are currently supported.\n\n### Available options\n\n* `--format (-f)`: The format to export to (default: `requirements.txt`). Currently, only `constraints.txt` and `requirements.txt` are supported.\n* `--output (-o)`: The name of the output file.  If omitted, print to standard output.\n* `--without`: The dependency groups to ignore when exporting.\n* `--with`: The optional dependency groups to include when exporting.\n* `--only`: The only dependency groups to include when exporting.\n* `--default`: Only export the main dependencies. (**Deprecated**)\n* `--dev`: Include development dependencies. (**Deprecated**)\n* `--extras (-E)`: Extra sets of dependencies to include.\n* `--without-hashes`: Exclude hashes from the exported file.\n* `--with-credentials`: Include credentials for extra indices.\n',
-    'author': 'Sébastien Eustace',
-    'author_email': 'sebastien@eustace.io',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://python-poetry.org/',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
+**Note**: For now, only the `constraints.txt` and `requirements.txt` formats are available.
 
+This plugin provides the same features as the existing `export` command of Poetry which it will eventually replace.
+
+
+## Installation
+
+The easiest way to install the `export` plugin is via the `self add` command of Poetry.
+
+```bash
+poetry self add poetry-plugin-export
+```
+
+If you used `pipx` to install Poetry you can add the plugin via the `pipx inject` command.
+
+```bash
+pipx inject poetry poetry-plugin-export
+```
+
+Otherwise, if you used `pip` to install Poetry you can add the plugin packages via the `pip install` command.
+
+```bash
+pip install poetry-plugin-export
+```
+
+
+## Usage
+
+The plugin provides an `export` command to export to the desired format.
+
+```bash
+poetry export -f requirements.txt --output requirements.txt
+```
+
+**Note**: Only the `constraints.txt` and `requirements.txt` formats are currently supported.
+
+### Available options
+
+* `--format (-f)`: The format to export to (default: `requirements.txt`). Currently, only `constraints.txt` and `requirements.txt` are supported.
+* `--output (-o)`: The name of the output file.  If omitted, print to standard output.
+* `--without`: The dependency groups to ignore when exporting.
+* `--with`: The optional dependency groups to include when exporting.
+* `--only`: The only dependency groups to include when exporting.
+* `--default`: Only export the main dependencies. (**Deprecated**)
+* `--dev`: Include development dependencies. (**Deprecated**)
+* `--extras (-E)`: Extra sets of dependencies to include.
+* `--without-hashes`: Exclude hashes from the exported file.
+* `--with-credentials`: Include credentials for extra indices.
 
-setup(**setup_kwargs)
```

