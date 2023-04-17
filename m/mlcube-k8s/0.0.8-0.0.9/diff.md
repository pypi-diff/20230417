# Comparing `tmp/mlcube_k8s-0.0.8.tar.gz` & `tmp/mlcube_k8s-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlcube_k8s-0.0.8.tar", last modified: Wed Sep 21 22:31:30 2022, max compression
+gzip compressed data, was "mlcube_k8s-0.0.9.tar", last modified: Mon Apr 17 18:11:35 2023, max compression
```

## Comparing `mlcube_k8s-0.0.8.tar` & `mlcube_k8s-0.0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 22:31:30.428161 mlcube_k8s-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-09-21 22:31:30.428161 mlcube_k8s-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      875 2022-09-21 22:31:22.000000 mlcube_k8s-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 22:31:30.424161 mlcube_k8s-0.0.8/mlcube_k8s/
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-09-21 22:31:22.000000 mlcube_k8s-0.0.8/mlcube_k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6177 2022-09-21 22:31:22.000000 mlcube_k8s-0.0.8/mlcube_k8s/k8s_run.py
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-09-21 22:31:22.000000 mlcube_k8s-0.0.8/mlcube_k8s/main.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 22:31:30.424161 mlcube_k8s-0.0.8/mlcube_k8s/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 22:31:22.000000 mlcube_k8s-0.0.8/mlcube_k8s/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 22:31:30.424161 mlcube_k8s-0.0.8/mlcube_k8s/tests/test_data/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 22:31:30.424161 mlcube_k8s-0.0.8/mlcube_k8s/tests/test_data/test_cube/
--rw-r--r--   0 runner    (1001) docker     (121)      185 2022-09-21 22:31:22.000000 mlcube_k8s-0.0.8/mlcube_k8s/tests/test_data/test_cube/mlcube.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 22:31:30.428161 mlcube_k8s-0.0.8/mlcube_k8s/tests/test_data/test_cube/platforms/
--rw-r--r--   0 runner    (1001) docker     (121)      137 2022-09-21 22:31:22.000000 mlcube_k8s-0.0.8/mlcube_k8s/tests/test_data/test_cube/platforms/docker.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 22:31:30.428161 mlcube_k8s-0.0.8/mlcube_k8s/tests/test_data/test_cube/run/
--rw-r--r--   0 runner    (1001) docker     (121)      249 2022-09-21 22:31:22.000000 mlcube_k8s-0.0.8/mlcube_k8s/tests/test_data/test_cube/run/kubernetes.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      172 2022-09-21 22:31:22.000000 mlcube_k8s-0.0.8/mlcube_k8s/tests/test_mlcube_k8s_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 22:31:30.424161 mlcube_k8s-0.0.8/mlcube_k8s.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-09-21 22:31:30.000000 mlcube_k8s-0.0.8/mlcube_k8s.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      522 2022-09-21 22:31:30.000000 mlcube_k8s-0.0.8/mlcube_k8s.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-21 22:31:30.000000 mlcube_k8s-0.0.8/mlcube_k8s.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-09-21 22:31:30.000000 mlcube_k8s-0.0.8/mlcube_k8s.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-09-21 22:31:30.000000 mlcube_k8s-0.0.8/mlcube_k8s.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-09-21 22:31:30.000000 mlcube_k8s-0.0.8/mlcube_k8s.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-21 22:31:30.428161 mlcube_k8s-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1330 2022-09-21 22:31:22.000000 mlcube_k8s-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:11:35.967893 mlcube_k8s-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-17 18:11:35.967893 mlcube_k8s-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-17 18:11:23.000000 mlcube_k8s-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:11:35.963893 mlcube_k8s-0.0.9/mlcube_k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-17 18:11:23.000000 mlcube_k8s-0.0.9/mlcube_k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-04-17 18:11:23.000000 mlcube_k8s-0.0.9/mlcube_k8s/k8s_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-17 18:11:23.000000 mlcube_k8s-0.0.9/mlcube_k8s/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:11:35.967893 mlcube_k8s-0.0.9/mlcube_k8s/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:11:23.000000 mlcube_k8s-0.0.9/mlcube_k8s/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:11:35.959893 mlcube_k8s-0.0.9/mlcube_k8s/tests/test_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:11:35.967893 mlcube_k8s-0.0.9/mlcube_k8s/tests/test_data/test_cube/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-17 18:11:23.000000 mlcube_k8s-0.0.9/mlcube_k8s/tests/test_data/test_cube/mlcube.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:11:35.967893 mlcube_k8s-0.0.9/mlcube_k8s/tests/test_data/test_cube/platforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-17 18:11:23.000000 mlcube_k8s-0.0.9/mlcube_k8s/tests/test_data/test_cube/platforms/docker.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:11:35.967893 mlcube_k8s-0.0.9/mlcube_k8s/tests/test_data/test_cube/run/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-17 18:11:23.000000 mlcube_k8s-0.0.9/mlcube_k8s/tests/test_data/test_cube/run/kubernetes.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-17 18:11:23.000000 mlcube_k8s-0.0.9/mlcube_k8s/tests/test_get_runner_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:11:35.963893 mlcube_k8s-0.0.9/mlcube_k8s.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-17 18:11:35.000000 mlcube_k8s-0.0.9/mlcube_k8s.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-17 18:11:35.000000 mlcube_k8s-0.0.9/mlcube_k8s.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 18:11:35.000000 mlcube_k8s-0.0.9/mlcube_k8s.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-17 18:11:35.000000 mlcube_k8s-0.0.9/mlcube_k8s.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-17 18:11:35.000000 mlcube_k8s-0.0.9/mlcube_k8s.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-17 18:11:35.000000 mlcube_k8s-0.0.9/mlcube_k8s.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 18:11:35.967893 mlcube_k8s-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-17 18:11:23.000000 mlcube_k8s-0.0.9/setup.py
```

### Comparing `mlcube_k8s-0.0.8/README.md` & `mlcube_k8s-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `mlcube_k8s-0.0.8/mlcube_k8s/k8s_run.py` & `mlcube_k8s-0.0.9/mlcube_k8s/k8s_run.py`

 * *Files identical despite different names*

### Comparing `mlcube_k8s-0.0.8/mlcube_k8s.egg-info/SOURCES.txt` & `mlcube_k8s-0.0.9/mlcube_k8s.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -6,11 +6,11 @@
 mlcube_k8s.egg-info/PKG-INFO
 mlcube_k8s.egg-info/SOURCES.txt
 mlcube_k8s.egg-info/dependency_links.txt
 mlcube_k8s.egg-info/entry_points.txt
 mlcube_k8s.egg-info/requires.txt
 mlcube_k8s.egg-info/top_level.txt
 mlcube_k8s/tests/__init__.py
-mlcube_k8s/tests/test_mlcube_k8s_cli.py
+mlcube_k8s/tests/test_get_runner_class.py
 mlcube_k8s/tests/test_data/test_cube/mlcube.yaml
 mlcube_k8s/tests/test_data/test_cube/platforms/docker.yaml
 mlcube_k8s/tests/test_data/test_cube/run/kubernetes.yaml
```

### Comparing `mlcube_k8s-0.0.8/setup.py` & `mlcube_k8s-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 
 extra_files = schemas()
 
 
 setup(
     name="mlcube_k8s",
-    version="0.0.8",
+    version="0.0.9",
     packages=find_packages(exclude=["tests"]),
     license="Apache 2.0",
     entry_points='''
         [console_scripts]
         mlcube_k8s=mlcube_k8s.main:cli
     ''',
     install_requires=requires,
```

