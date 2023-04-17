# Comparing `tmp/mlcube_ssh-0.0.8.tar.gz` & `tmp/mlcube_ssh-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlcube_ssh-0.0.8.tar", last modified: Wed Sep 21 22:31:38 2022, max compression
+gzip compressed data, was "mlcube_ssh-0.0.9.tar", last modified: Mon Apr 17 18:11:33 2023, max compression
```

## Comparing `mlcube_ssh-0.0.8.tar` & `mlcube_ssh-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 22:31:38.313244 mlcube_ssh-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-09-21 22:31:38.313244 mlcube_ssh-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      192 2022-09-21 22:31:28.000000 mlcube_ssh-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 22:31:38.313244 mlcube_ssh-0.0.8/mlcube_ssh/
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-09-21 22:31:28.000000 mlcube_ssh-0.0.8/mlcube_ssh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-09-21 22:31:28.000000 mlcube_ssh-0.0.8/mlcube_ssh/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7115 2022-09-21 22:31:28.000000 mlcube_ssh-0.0.8/mlcube_ssh/ssh_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     6374 2022-09-21 22:31:28.000000 mlcube_ssh-0.0.8/mlcube_ssh/ssh_run.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 22:31:38.313244 mlcube_ssh-0.0.8/mlcube_ssh/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 22:31:28.000000 mlcube_ssh-0.0.8/mlcube_ssh/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 22:31:38.313244 mlcube_ssh-0.0.8/mlcube_ssh/tests/test_data/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 22:31:38.313244 mlcube_ssh-0.0.8/mlcube_ssh/tests/test_data/platforms/
--rw-r--r--   0 runner    (1001) docker     (121)      665 2022-09-21 22:31:28.000000 mlcube_ssh-0.0.8/mlcube_ssh/tests/test_data/platforms/platform_01.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      691 2022-09-21 22:31:28.000000 mlcube_ssh-0.0.8/mlcube_ssh/tests/test_data/platforms/platform_02.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-09-21 22:31:28.000000 mlcube_ssh-0.0.8/mlcube_ssh/tests/test_mlcube_ssh_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     2509 2022-09-21 22:31:28.000000 mlcube_ssh-0.0.8/mlcube_ssh/tests/test_python_interpreters.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 22:31:38.313244 mlcube_ssh-0.0.8/mlcube_ssh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-09-21 22:31:38.000000 mlcube_ssh-0.0.8/mlcube_ssh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      541 2022-09-21 22:31:38.000000 mlcube_ssh-0.0.8/mlcube_ssh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-21 22:31:38.000000 mlcube_ssh-0.0.8/mlcube_ssh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-09-21 22:31:38.000000 mlcube_ssh-0.0.8/mlcube_ssh.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-09-21 22:31:38.000000 mlcube_ssh-0.0.8/mlcube_ssh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-09-21 22:31:38.000000 mlcube_ssh-0.0.8/mlcube_ssh.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-21 22:31:38.313244 mlcube_ssh-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1361 2022-09-21 22:31:28.000000 mlcube_ssh-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:11:33.878172 mlcube_ssh-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-17 18:11:33.878172 mlcube_ssh-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-17 18:11:20.000000 mlcube_ssh-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:11:33.878172 mlcube_ssh-0.0.9/mlcube_ssh/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-17 18:11:20.000000 mlcube_ssh-0.0.9/mlcube_ssh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-17 18:11:20.000000 mlcube_ssh-0.0.9/mlcube_ssh/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7115 2023-04-17 18:11:20.000000 mlcube_ssh-0.0.9/mlcube_ssh/ssh_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-04-17 18:11:20.000000 mlcube_ssh-0.0.9/mlcube_ssh/ssh_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:11:33.878172 mlcube_ssh-0.0.9/mlcube_ssh/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:11:20.000000 mlcube_ssh-0.0.9/mlcube_ssh/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:11:33.878172 mlcube_ssh-0.0.9/mlcube_ssh/tests/test_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:11:33.878172 mlcube_ssh-0.0.9/mlcube_ssh/tests/test_data/platforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-17 18:11:20.000000 mlcube_ssh-0.0.9/mlcube_ssh/tests/test_data/platforms/platform_01.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-17 18:11:20.000000 mlcube_ssh-0.0.9/mlcube_ssh/tests/test_data/platforms/platform_02.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-04-17 18:11:20.000000 mlcube_ssh-0.0.9/mlcube_ssh/tests/test_python_interpreters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:11:33.878172 mlcube_ssh-0.0.9/mlcube_ssh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-17 18:11:33.000000 mlcube_ssh-0.0.9/mlcube_ssh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-17 18:11:33.000000 mlcube_ssh-0.0.9/mlcube_ssh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 18:11:33.000000 mlcube_ssh-0.0.9/mlcube_ssh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-17 18:11:33.000000 mlcube_ssh-0.0.9/mlcube_ssh.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-17 18:11:33.000000 mlcube_ssh-0.0.9/mlcube_ssh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-17 18:11:33.000000 mlcube_ssh-0.0.9/mlcube_ssh.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 18:11:33.878172 mlcube_ssh-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-17 18:11:20.000000 mlcube_ssh-0.0.9/setup.py
```

### Comparing `mlcube_ssh-0.0.8/mlcube_ssh/ssh_metadata.py` & `mlcube_ssh-0.0.9/mlcube_ssh/ssh_metadata.py`

 * *Files identical despite different names*

### Comparing `mlcube_ssh-0.0.8/mlcube_ssh/ssh_run.py` & `mlcube_ssh-0.0.9/mlcube_ssh/ssh_run.py`

 * *Files identical despite different names*

### Comparing `mlcube_ssh-0.0.8/mlcube_ssh/tests/test_data/platforms/platform_01.yaml` & `mlcube_ssh-0.0.9/mlcube_ssh/tests/test_data/platforms/platform_01.yaml`

 * *Files identical despite different names*

### Comparing `mlcube_ssh-0.0.8/mlcube_ssh/tests/test_data/platforms/platform_02.yaml` & `mlcube_ssh-0.0.9/mlcube_ssh/tests/test_data/platforms/platform_02.yaml`

 * *Files identical despite different names*

### Comparing `mlcube_ssh-0.0.8/mlcube_ssh/tests/test_python_interpreters.py` & `mlcube_ssh-0.0.9/mlcube_ssh/tests/test_python_interpreters.py`

 * *Files identical despite different names*

### Comparing `mlcube_ssh-0.0.8/setup.py` & `mlcube_ssh-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 
 extra_files = schemas()
 
 
 setup(
     name="mlcube_ssh",
-    version="0.0.8",
+    version="0.0.9",
     packages=find_packages(exclude=["tests"]),
     license="Apache 2.0",
     entry_points='''
         [console_scripts]
         mlcube_ssh=mlcube_ssh.__main__:cli
     ''',
     install_requires=requires,
```

