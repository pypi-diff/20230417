# Comparing `tmp/kannon-0.1.2.tar.gz` & `tmp/kannon-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kannon-0.1.2.tar", max compression
+gzip compressed data, was "kannon-0.1.3.tar", max compression
```

## Comparing `kannon-0.1.2.tar` & `kannon-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1065 2023-04-13 01:33:16.999551 kannon-0.1.2/LICENSE
--rw-r--r--   0        0        0     5988 2023-04-13 01:33:16.999551 kannon-0.1.2/README.md
--rw-r--r--   0        0        0       70 2023-04-13 01:33:16.999551 kannon-0.1.2/kannon/__init__.py
--rw-r--r--   0        0        0     1229 2023-04-13 01:33:16.999551 kannon-0.1.2/kannon/kube_util.py
--rw-r--r--   0        0        0     6850 2023-04-13 01:33:16.999551 kannon-0.1.2/kannon/master.py
--rw-r--r--   0        0        0       64 2023-04-13 01:33:16.999551 kannon-0.1.2/kannon/task.py
--rw-r--r--   0        0        0     1173 2023-04-13 01:33:32.055549 kannon-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     6826 1970-01-01 00:00:00.000000 kannon-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-17 06:07:59.924958 kannon-0.1.3/LICENSE
+-rw-r--r--   0        0        0     6109 2023-04-17 06:07:59.924958 kannon-0.1.3/README.md
+-rw-r--r--   0        0        0       70 2023-04-17 06:07:59.924958 kannon-0.1.3/kannon/__init__.py
+-rw-r--r--   0        0        0     1229 2023-04-17 06:07:59.924958 kannon-0.1.3/kannon/kube_util.py
+-rw-r--r--   0        0        0     6858 2023-04-17 06:07:59.924958 kannon-0.1.3/kannon/master.py
+-rw-r--r--   0        0        0       64 2023-04-17 06:07:59.924958 kannon-0.1.3/kannon/task.py
+-rw-r--r--   0        0        0     1264 2023-04-17 06:08:14.869369 kannon-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     6947 1970-01-01 00:00:00.000000 kannon-0.1.3/PKG-INFO
```

### Comparing `kannon-0.1.2/LICENSE` & `kannon-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kannon-0.1.2/README.md` & `kannon-0.1.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 # Install
 Kannon can be installed via `pip`.
 
 ```bash
 pip install kannon
 ```
 
+# [Quick Starter](./example/README.md)
+An easy and self-contained tutorial can be found in [here](./example/README.md)!
+
 # Usage
 It is required for users to prepare following two scripts and copy them into a docker container:
 - A script to start task pipeline on master job.
 - A script for child jobs to run assigned tasks.
 
 Easy and self-contained quick starter will be available soon!
```

### Comparing `kannon-0.1.2/kannon/kube_util.py` & `kannon-0.1.3/kannon/kube_util.py`

 * *Files identical despite different names*

### Comparing `kannon-0.1.2/kannon/master.py` & `kannon-0.1.3/kannon/master.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         self.path_child_script = path_child_script
         if env_to_inherit is None:
             env_to_inherit = ["TASK_WORKSPACE_DIRECTORY"]
         self.env_to_inherit = env_to_inherit
 
         self.task_id_to_job_name: Dict[str, str] = dict()
 
-    def build(self, root_task: gokart.TaskOnKart):
+    def build(self, root_task: gokart.TaskOnKart) -> None:
         # push tasks into queue
         logger.info("Creating task queue...")
         task_queue = self._create_task_queue(root_task)
 
         # consume task queue
         launched_task_ids: Set[str] = set()
         logger.info("Consuming task queue...")
```

### Comparing `kannon-0.1.2/pyproject.toml` & `kannon-0.1.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kannon"
-version = "0.1.2"
+version = "0.1.3"
 description = "Kannon is a wrapper for the gokart library that allows gokart tasks to be easily executed in a distributed and parallel manner on multiple kubernetes jobs."
 authors = ["M3, inc."]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/m3dev/kannon"
 repository = "https://github.com/m3dev/kannon"
 
@@ -41,19 +41,21 @@
 based_on_style = "pep8"
 column_limit = 160
 
 [tool.yapfignore]
 ignore_patterns = [
   ".venv/*",
   ".tox/*",
-  "examples/*"
 ]
 
 [tool.isort]
 line_length = 160
 
 [tool.mypy]
+strict = true
+disallow_subclassing_any = false  # revert strict
+implicit_reexport = true  # revert strict
 ignore_missing_imports = true
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `kannon-0.1.2/PKG-INFO` & `kannon-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kannon
-Version: 0.1.2
+Version: 0.1.3
 Summary: Kannon is a wrapper for the gokart library that allows gokart tasks to be easily executed in a distributed and parallel manner on multiple kubernetes jobs.
 Home-page: https://github.com/m3dev/kannon
 License: MIT
 Author: M3, inc.
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -25,14 +25,17 @@
 # Install
 Kannon can be installed via `pip`.
 
 ```bash
 pip install kannon
 ```
 
+# [Quick Starter](./example/README.md)
+An easy and self-contained tutorial can be found in [here](./example/README.md)!
+
 # Usage
 It is required for users to prepare following two scripts and copy them into a docker container:
 - A script to start task pipeline on master job.
 - A script for child jobs to run assigned tasks.
 
 Easy and self-contained quick starter will be available soon!
```

