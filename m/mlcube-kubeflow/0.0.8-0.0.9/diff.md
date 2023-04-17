# Comparing `tmp/mlcube_kubeflow-0.0.8.tar.gz` & `tmp/mlcube_kubeflow-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlcube_kubeflow-0.0.8.tar", last modified: Wed Sep 21 22:31:31 2022, max compression
+gzip compressed data, was "mlcube_kubeflow-0.0.9.tar", last modified: Mon Apr 17 18:11:37 2023, max compression
```

## Comparing `mlcube_kubeflow-0.0.8.tar` & `mlcube_kubeflow-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 22:31:31.161749 mlcube_kubeflow-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)      167 2022-09-21 22:31:31.161749 mlcube_kubeflow-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-09-21 22:31:21.000000 mlcube_kubeflow-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 22:31:31.161749 mlcube_kubeflow-0.0.8/mlcube_kubeflow/
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-09-21 22:31:21.000000 mlcube_kubeflow-0.0.8/mlcube_kubeflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4187 2022-09-21 22:31:21.000000 mlcube_kubeflow-0.0.8/mlcube_kubeflow/kubeflow_run.py
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-09-21 22:31:21.000000 mlcube_kubeflow-0.0.8/mlcube_kubeflow/main.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 22:31:31.161749 mlcube_kubeflow-0.0.8/mlcube_kubeflow/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 22:31:21.000000 mlcube_kubeflow-0.0.8/mlcube_kubeflow/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      174 2022-09-21 22:31:21.000000 mlcube_kubeflow-0.0.8/mlcube_kubeflow/tests/test_mlcube_kubeflow_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 22:31:31.161749 mlcube_kubeflow-0.0.8/mlcube_kubeflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      167 2022-09-21 22:31:31.000000 mlcube_kubeflow-0.0.8/mlcube_kubeflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      422 2022-09-21 22:31:31.000000 mlcube_kubeflow-0.0.8/mlcube_kubeflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-21 22:31:31.000000 mlcube_kubeflow-0.0.8/mlcube_kubeflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-09-21 22:31:31.000000 mlcube_kubeflow-0.0.8/mlcube_kubeflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-09-21 22:31:31.000000 mlcube_kubeflow-0.0.8/mlcube_kubeflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-09-21 22:31:31.000000 mlcube_kubeflow-0.0.8/mlcube_kubeflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-21 22:31:31.161749 mlcube_kubeflow-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1348 2022-09-21 22:31:21.000000 mlcube_kubeflow-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:11:37.435853 mlcube_kubeflow-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-17 18:11:37.435853 mlcube_kubeflow-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-17 18:11:21.000000 mlcube_kubeflow-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:11:37.431853 mlcube_kubeflow-0.0.9/mlcube_kubeflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-17 18:11:21.000000 mlcube_kubeflow-0.0.9/mlcube_kubeflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-17 18:11:21.000000 mlcube_kubeflow-0.0.9/mlcube_kubeflow/kubeflow_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-17 18:11:21.000000 mlcube_kubeflow-0.0.9/mlcube_kubeflow/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:11:37.431853 mlcube_kubeflow-0.0.9/mlcube_kubeflow/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:11:21.000000 mlcube_kubeflow-0.0.9/mlcube_kubeflow/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-17 18:11:21.000000 mlcube_kubeflow-0.0.9/mlcube_kubeflow/tests/test_get_runner_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:11:37.431853 mlcube_kubeflow-0.0.9/mlcube_kubeflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-17 18:11:37.000000 mlcube_kubeflow-0.0.9/mlcube_kubeflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-17 18:11:37.000000 mlcube_kubeflow-0.0.9/mlcube_kubeflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 18:11:37.000000 mlcube_kubeflow-0.0.9/mlcube_kubeflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-17 18:11:37.000000 mlcube_kubeflow-0.0.9/mlcube_kubeflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-17 18:11:37.000000 mlcube_kubeflow-0.0.9/mlcube_kubeflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-17 18:11:37.000000 mlcube_kubeflow-0.0.9/mlcube_kubeflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 18:11:37.435853 mlcube_kubeflow-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-17 18:11:21.000000 mlcube_kubeflow-0.0.9/setup.py
```

### Comparing `mlcube_kubeflow-0.0.8/README.md` & `mlcube_kubeflow-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `mlcube_kubeflow-0.0.8/mlcube_kubeflow/kubeflow_run.py` & `mlcube_kubeflow-0.0.9/mlcube_kubeflow/kubeflow_run.py`

 * *Files identical despite different names*

### Comparing `mlcube_kubeflow-0.0.8/setup.py` & `mlcube_kubeflow-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 
 extra_files = schemas()
 
 
 setup(
     name="mlcube_kubeflow",
-    version="0.0.8",
+    version="0.0.9",
     packages=find_packages(exclude=["tests"]),
     license="Apache 2.0",
     entry_points='''
         [console_scripts]
         mlcube_kubeflow=mlcube_kubeflow.main:cli
     ''',
     install_requires=requires,
```

