# Comparing `tmp/glean-cli-0.5.5.tar.gz` & `tmp/glean-cli-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glean-cli-0.5.5.tar", last modified: Wed Feb 15 23:41:29 2023, max compression
+gzip compressed data, was "glean-cli-0.5.6.tar", last modified: Mon Apr 17 15:30:26 2023, max compression
```

## Comparing `glean-cli-0.5.5.tar` & `glean-cli-0.5.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-02-15 23:41:29.342168 glean-cli-0.5.5/
--rw-r--r--   0 mark       (501) staff       (20)    11357 2022-10-25 19:35:41.000000 glean-cli-0.5.5/LICENSE
--rw-r--r--   0 mark       (501) staff       (20)     1283 2023-02-15 23:41:29.342233 glean-cli-0.5.5/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      832 2022-11-06 03:46:13.000000 glean-cli-0.5.5/README.md
--rw-r--r--   0 mark       (501) staff       (20)      103 2022-10-25 19:35:41.000000 glean-cli-0.5.5/pyproject.toml
--rw-r--r--   0 mark       (501) staff       (20)      793 2023-02-15 23:41:29.342522 glean-cli-0.5.5/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)       38 2022-10-25 19:35:41.000000 glean-cli-0.5.5/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-02-15 23:41:29.336891 glean-cli-0.5.5/src/
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-02-15 23:41:29.339407 glean-cli-0.5.5/src/glean/
--rw-r--r--   0 mark       (501) staff       (20)       18 2023-02-15 23:39:34.000000 glean-cli-0.5.5/src/glean/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)    19217 2023-02-06 20:27:45.000000 glean-cli-0.5.5/src/glean/cli.py
--rw-r--r--   0 mark       (501) staff       (20)     1598 2022-11-01 21:06:11.000000 glean-cli-0.5.5/src/glean/credentials.py
--rw-r--r--   0 mark       (501) staff       (20)     2048 2022-12-06 21:14:52.000000 glean-cli-0.5.5/src/glean/filesystem.py
--rw-r--r--   0 mark       (501) staff       (20)    12074 2023-02-06 21:20:55.000000 glean-cli-0.5.5/src/glean/glean_api.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-02-15 23:41:29.340369 glean-cli-0.5.5/src/glean/utils/
--rw-r--r--   0 mark       (501) staff       (20)        0 2022-11-01 21:06:11.000000 glean-cli-0.5.5/src/glean/utils/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)      509 2022-11-01 21:06:11.000000 glean-cli-0.5.5/src/glean/utils/cli.py
--rw-r--r--   0 mark       (501) staff       (20)     1583 2023-01-20 07:19:41.000000 glean-cli-0.5.5/src/glean/utils/grn.py
--rw-r--r--   0 mark       (501) staff       (20)     1035 2023-01-20 07:19:41.000000 glean-cli-0.5.5/src/glean/utils/validate_config.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-02-15 23:41:29.341257 glean-cli-0.5.5/src/glean_cli.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)     1283 2023-02-15 23:41:29.000000 glean-cli-0.5.5/src/glean_cli.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      588 2023-02-15 23:41:29.000000 glean-cli-0.5.5/src/glean_cli.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-02-15 23:41:29.000000 glean-cli-0.5.5/src/glean_cli.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)       41 2023-02-15 23:41:29.000000 glean-cli-0.5.5/src/glean_cli.egg-info/entry_points.txt
--rw-r--r--   0 mark       (501) staff       (20)       84 2023-02-15 23:41:29.000000 glean-cli-0.5.5/src/glean_cli.egg-info/requires.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-02-15 23:41:29.000000 glean-cli-0.5.5/src/glean_cli.egg-info/top_level.txt
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-02-15 23:41:29.342014 glean-cli-0.5.5/tests/
--rw-r--r--   0 mark       (501) staff       (20)      309 2022-11-01 21:06:11.000000 glean-cli-0.5.5/tests/test_cli.py
--rw-r--r--   0 mark       (501) staff       (20)     1652 2022-11-01 21:06:11.000000 glean-cli-0.5.5/tests/test_credentials.py
--rw-r--r--   0 mark       (501) staff       (20)     1715 2023-01-20 07:19:41.000000 glean-cli-0.5.5/tests/test_filesystem.py
--rw-r--r--   0 mark       (501) staff       (20)      666 2022-11-01 21:06:11.000000 glean-cli-0.5.5/tests/test_glean_api.py
+drwxr-xr-x   0 anixon     (501) staff       (20)        0 2023-04-17 15:30:26.938509 glean-cli-0.5.6/
+-rw-r--r--   0 anixon     (501) staff       (20)    11357 2022-12-17 00:47:55.000000 glean-cli-0.5.6/LICENSE
+-rw-r--r--   0 anixon     (501) staff       (20)     1283 2023-04-17 15:30:26.938568 glean-cli-0.5.6/PKG-INFO
+-rw-r--r--   0 anixon     (501) staff       (20)      832 2023-01-19 16:41:15.000000 glean-cli-0.5.6/README.md
+-rw-r--r--   0 anixon     (501) staff       (20)      103 2022-12-17 00:47:55.000000 glean-cli-0.5.6/pyproject.toml
+-rw-r--r--   0 anixon     (501) staff       (20)      793 2023-04-17 15:30:26.938846 glean-cli-0.5.6/setup.cfg
+-rw-r--r--   0 anixon     (501) staff       (20)       38 2022-12-17 00:47:55.000000 glean-cli-0.5.6/setup.py
+drwxr-xr-x   0 anixon     (501) staff       (20)        0 2023-04-17 15:30:26.934561 glean-cli-0.5.6/src/
+drwxr-xr-x   0 anixon     (501) staff       (20)        0 2023-04-17 15:30:26.936367 glean-cli-0.5.6/src/glean/
+-rw-r--r--   0 anixon     (501) staff       (20)       18 2023-04-17 15:29:18.000000 glean-cli-0.5.6/src/glean/__init__.py
+-rw-r--r--   0 anixon     (501) staff       (20)    19217 2023-04-11 21:15:13.000000 glean-cli-0.5.6/src/glean/cli.py
+-rw-r--r--   0 anixon     (501) staff       (20)     1598 2022-12-17 00:47:55.000000 glean-cli-0.5.6/src/glean/credentials.py
+-rw-r--r--   0 anixon     (501) staff       (20)     2048 2022-12-17 00:47:55.000000 glean-cli-0.5.6/src/glean/filesystem.py
+-rw-r--r--   0 anixon     (501) staff       (20)    12288 2023-04-17 15:29:18.000000 glean-cli-0.5.6/src/glean/glean_api.py
+drwxr-xr-x   0 anixon     (501) staff       (20)        0 2023-04-17 15:30:26.937120 glean-cli-0.5.6/src/glean/utils/
+-rw-r--r--   0 anixon     (501) staff       (20)        0 2022-12-17 00:47:55.000000 glean-cli-0.5.6/src/glean/utils/__init__.py
+-rw-r--r--   0 anixon     (501) staff       (20)      509 2023-01-03 16:54:54.000000 glean-cli-0.5.6/src/glean/utils/cli.py
+-rw-r--r--   0 anixon     (501) staff       (20)     1583 2023-01-19 16:41:15.000000 glean-cli-0.5.6/src/glean/utils/grn.py
+-rw-r--r--   0 anixon     (501) staff       (20)     1035 2023-01-19 16:41:15.000000 glean-cli-0.5.6/src/glean/utils/validate_config.py
+drwxr-xr-x   0 anixon     (501) staff       (20)        0 2023-04-17 15:30:26.937904 glean-cli-0.5.6/src/glean_cli.egg-info/
+-rw-r--r--   0 anixon     (501) staff       (20)     1283 2023-04-17 15:30:26.000000 glean-cli-0.5.6/src/glean_cli.egg-info/PKG-INFO
+-rw-r--r--   0 anixon     (501) staff       (20)      588 2023-04-17 15:30:26.000000 glean-cli-0.5.6/src/glean_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 anixon     (501) staff       (20)        1 2023-04-17 15:30:26.000000 glean-cli-0.5.6/src/glean_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 anixon     (501) staff       (20)       41 2023-04-17 15:30:26.000000 glean-cli-0.5.6/src/glean_cli.egg-info/entry_points.txt
+-rw-r--r--   0 anixon     (501) staff       (20)       84 2023-04-17 15:30:26.000000 glean-cli-0.5.6/src/glean_cli.egg-info/requires.txt
+-rw-r--r--   0 anixon     (501) staff       (20)        6 2023-04-17 15:30:26.000000 glean-cli-0.5.6/src/glean_cli.egg-info/top_level.txt
+drwxr-xr-x   0 anixon     (501) staff       (20)        0 2023-04-17 15:30:26.938408 glean-cli-0.5.6/tests/
+-rw-r--r--   0 anixon     (501) staff       (20)      309 2022-12-17 00:47:55.000000 glean-cli-0.5.6/tests/test_cli.py
+-rw-r--r--   0 anixon     (501) staff       (20)     1652 2022-12-17 00:47:55.000000 glean-cli-0.5.6/tests/test_credentials.py
+-rw-r--r--   0 anixon     (501) staff       (20)     1715 2023-01-19 16:41:15.000000 glean-cli-0.5.6/tests/test_filesystem.py
+-rw-r--r--   0 anixon     (501) staff       (20)      666 2022-12-17 00:47:55.000000 glean-cli-0.5.6/tests/test_glean_api.py
```

### Comparing `glean-cli-0.5.5/LICENSE` & `glean-cli-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `glean-cli-0.5.5/PKG-INFO` & `glean-cli-0.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glean-cli
-Version: 0.5.5
+Version: 0.5.6
 Summary: Command-line tools for interacting with Glean
 Home-page: https://glean.io/
 Author: Dan Eisenberg
 Author-email: dse@glean.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `glean-cli-0.5.5/README.md` & `glean-cli-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `glean-cli-0.5.5/setup.cfg` & `glean-cli-0.5.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `glean-cli-0.5.5/src/glean/cli.py` & `glean-cli-0.5.6/src/glean/cli.py`

 * *Files identical despite different names*

### Comparing `glean-cli-0.5.5/src/glean/credentials.py` & `glean-cli-0.5.6/src/glean/credentials.py`

 * *Files identical despite different names*

### Comparing `glean-cli-0.5.5/src/glean/filesystem.py` & `glean-cli-0.5.6/src/glean/filesystem.py`

 * *Files identical despite different names*

### Comparing `glean-cli-0.5.5/src/glean/glean_api.py` & `glean-cli-0.5.6/src/glean/glean_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,14 +31,19 @@
     if r.status_code >= 500:
         raise ClickException("Unexpected error initiating your Glean session.")
     elif r.status_code >= 400:
         raise ClickException("Your access key is invalid.")
     if not r.ok:
         raise ClickException("Unexpected error initiating your Glean session.")
 
+    click.echo()
+    click.echo("Successfully logged in to " + click.style(r.text, bold=True))
+    click.echo("Project id: " + credentials.project_id)
+    click.echo("Access key id: " + credentials.access_key_id)
+
     return credentials.project_id
 
 
 def create_build_from_git_revision(
     session: Session,
     project_id: str,
     git_revision: Optional[str],
```

### Comparing `glean-cli-0.5.5/src/glean/utils/grn.py` & `glean-cli-0.5.6/src/glean/utils/grn.py`

 * *Files identical despite different names*

### Comparing `glean-cli-0.5.5/src/glean/utils/validate_config.py` & `glean-cli-0.5.6/src/glean/utils/validate_config.py`

 * *Files identical despite different names*

### Comparing `glean-cli-0.5.5/src/glean_cli.egg-info/PKG-INFO` & `glean-cli-0.5.6/src/glean_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glean-cli
-Version: 0.5.5
+Version: 0.5.6
 Summary: Command-line tools for interacting with Glean
 Home-page: https://glean.io/
 Author: Dan Eisenberg
 Author-email: dse@glean.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `glean-cli-0.5.5/src/glean_cli.egg-info/SOURCES.txt` & `glean-cli-0.5.6/src/glean_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `glean-cli-0.5.5/tests/test_credentials.py` & `glean-cli-0.5.6/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `glean-cli-0.5.5/tests/test_filesystem.py` & `glean-cli-0.5.6/tests/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `glean-cli-0.5.5/tests/test_glean_api.py` & `glean-cli-0.5.6/tests/test_glean_api.py`

 * *Files identical despite different names*

