# Comparing `tmp/remoteit-ssh-0.3.0.tar.gz` & `tmp/remoteit-ssh-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remoteit-ssh-0.3.0.tar", last modified: Thu Mar 23 12:24:00 2023, max compression
+gzip compressed data, was "remoteit-ssh-0.3.1.tar", last modified: Mon Apr 17 15:10:52 2023, max compression
```

## Comparing `remoteit-ssh-0.3.0.tar` & `remoteit-ssh-0.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:24:00.580314 remoteit-ssh-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-03-23 12:24:00.580314 remoteit-ssh-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-03-23 12:23:50.000000 remoteit-ssh-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:24:00.580314 remoteit-ssh-0.3.0/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-03-23 12:23:50.000000 remoteit-ssh-0.3.0/resources/post_install_script.sh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 12:24:00.580314 remoteit-ssh-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-03-23 12:23:50.000000 remoteit-ssh-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:24:00.580314 remoteit-ssh-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:24:00.580314 remoteit-ssh-0.3.0/src/remoteit_ssh/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:23:50.000000 remoteit-ssh-0.3.0/src/remoteit_ssh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-03-23 12:23:50.000000 remoteit-ssh-0.3.0/src/remoteit_ssh/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:24:00.580314 remoteit-ssh-0.3.0/src/remoteit_ssh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-03-23 12:24:00.000000 remoteit-ssh-0.3.0/src/remoteit_ssh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-03-23 12:24:00.000000 remoteit-ssh-0.3.0/src/remoteit_ssh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 12:24:00.000000 remoteit-ssh-0.3.0/src/remoteit_ssh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-23 12:24:00.000000 remoteit-ssh-0.3.0/src/remoteit_ssh.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-23 12:24:00.000000 remoteit-ssh-0.3.0/src/remoteit_ssh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-23 12:24:00.000000 remoteit-ssh-0.3.0/src/remoteit_ssh.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:10:52.089005 remoteit-ssh-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-17 15:10:52.089005 remoteit-ssh-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-17 15:10:39.000000 remoteit-ssh-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:10:52.085005 remoteit-ssh-0.3.1/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-17 15:10:39.000000 remoteit-ssh-0.3.1/resources/post_install_script.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 15:10:52.089005 remoteit-ssh-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-17 15:10:39.000000 remoteit-ssh-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:10:52.085005 remoteit-ssh-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:10:52.085005 remoteit-ssh-0.3.1/src/remoteit_ssh/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 15:10:39.000000 remoteit-ssh-0.3.1/src/remoteit_ssh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-04-17 15:10:39.000000 remoteit-ssh-0.3.1/src/remoteit_ssh/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:10:52.089005 remoteit-ssh-0.3.1/src/remoteit_ssh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-17 15:10:51.000000 remoteit-ssh-0.3.1/src/remoteit_ssh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-17 15:10:52.000000 remoteit-ssh-0.3.1/src/remoteit_ssh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 15:10:51.000000 remoteit-ssh-0.3.1/src/remoteit_ssh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-17 15:10:51.000000 remoteit-ssh-0.3.1/src/remoteit_ssh.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-17 15:10:51.000000 remoteit-ssh-0.3.1/src/remoteit_ssh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-17 15:10:51.000000 remoteit-ssh-0.3.1/src/remoteit_ssh.egg-info/top_level.txt
```

### Comparing `remoteit-ssh-0.3.0/setup.py` & `remoteit-ssh-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 INSTALL_REQUIRES = [
     'requests-http-signature==v0.1.0'
 ]
 
 setup(
     name='remoteit-ssh',
     description='Opens an SSH connection to a remoteit device by name.',
-    version='0.3.0',
+    version='0.3.1',
     url='https://github.com/conor-f/remoteit-ssh',
     python_requires='>=3.6',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     install_requires=INSTALL_REQUIRES,
     entry_points={
         'console_scripts': [
```

### Comparing `remoteit-ssh-0.3.0/src/remoteit_ssh/client.py` & `remoteit-ssh-0.3.1/src/remoteit_ssh/client.py`

 * *Files identical despite different names*

