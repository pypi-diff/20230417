# Comparing `tmp/kubetools-9.1.tar.gz` & `tmp/kubetools-9.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kubetools-9.1.tar", last modified: Tue Jun 11 15:11:50 2019, max compression
+gzip compressed data, was "dist/kubetools-9.1.1.tar", last modified: Wed Aug 28 09:06:03 2019, max compression
```

## Comparing `kubetools-9.1.tar` & `kubetools-9.1.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2019-06-11 15:11:50.000000 kubetools-9.1/
--rw-r--r--   0 nick       (501) staff       (20)      315 2019-06-11 15:11:15.000000 kubetools-9.1/CHANGELOG.md
--rw-r--r--   0 nick       (501) staff       (20)       21 2019-03-15 13:54:56.000000 kubetools-9.1/MANIFEST.in
--rw-r--r--   0 nick       (501) staff       (20)      269 2019-06-11 15:11:50.000000 kubetools-9.1/PKG-INFO
--rw-r--r--   0 nick       (501) staff       (20)      476 2019-03-20 15:31:55.000000 kubetools-9.1/README.md
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2019-06-11 15:11:50.000000 kubetools-9.1/kubetools.egg-info/
--rw-r--r--   0 nick       (501) staff       (20)      269 2019-06-11 15:11:50.000000 kubetools-9.1/kubetools.egg-info/PKG-INFO
--rw-r--r--   0 nick       (501) staff       (20)     1003 2019-06-11 15:11:50.000000 kubetools-9.1/kubetools.egg-info/SOURCES.txt
--rw-r--r--   0 nick       (501) staff       (20)        1 2019-06-11 15:11:50.000000 kubetools-9.1/kubetools.egg-info/dependency_links.txt
--rw-r--r--   0 nick       (501) staff       (20)      107 2019-06-11 15:11:50.000000 kubetools-9.1/kubetools.egg-info/entry_points.txt
--rw-r--r--   0 nick       (501) staff       (20)       95 2019-06-11 15:11:50.000000 kubetools-9.1/kubetools.egg-info/requires.txt
--rw-r--r--   0 nick       (501) staff       (20)       17 2019-06-11 15:11:50.000000 kubetools-9.1/kubetools.egg-info/top_level.txt
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2019-06-11 15:11:50.000000 kubetools-9.1/kubetools_client/
--rw-r--r--   0 nick       (501) staff       (20)      144 2019-03-15 13:54:56.000000 kubetools-9.1/kubetools_client/__init__.py
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2019-06-11 15:11:50.000000 kubetools-9.1/kubetools_client/cli/
--rw-r--r--   0 nick       (501) staff       (20)      999 2019-03-15 13:54:56.000000 kubetools-9.1/kubetools_client/cli/__init__.py
--rwxr-xr-x   0 nick       (501) staff       (20)      249 2019-03-15 13:54:56.000000 kubetools-9.1/kubetools_client/cli/__main__.py
--rw-r--r--   0 nick       (501) staff       (20)     7048 2019-03-15 13:54:56.000000 kubetools-9.1/kubetools_client/cli/generate.py
--rw-r--r--   0 nick       (501) staff       (20)      954 2019-03-15 13:54:56.000000 kubetools-9.1/kubetools_client/cli/jobs.py
--rw-r--r--   0 nick       (501) staff       (20)     8007 2019-03-15 13:54:56.000000 kubetools-9.1/kubetools_client/cli/lists.py
--rw-r--r--   0 nick       (501) staff       (20)     3858 2019-03-15 13:54:56.000000 kubetools-9.1/kubetools_client/cli/wait.py
--rw-r--r--   0 nick       (501) staff       (20)     2228 2019-03-15 13:54:56.000000 kubetools-9.1/kubetools_client/cli/wait_util.py
--rw-r--r--   0 nick       (501) staff       (20)    10042 2019-03-15 13:54:56.000000 kubetools-9.1/kubetools_client/client.py
--rw-r--r--   0 nick       (501) staff       (20)     8325 2019-06-11 15:11:15.000000 kubetools-9.1/kubetools_client/config.py
--rw-r--r--   0 nick       (501) staff       (20)     4013 2019-03-15 13:54:56.000000 kubetools-9.1/kubetools_client/config_legacy.py
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2019-06-11 15:11:50.000000 kubetools-9.1/kubetools_client/dev/
--rw-r--r--   0 nick       (501) staff       (20)      925 2019-03-15 13:54:56.000000 kubetools-9.1/kubetools_client/dev/__init__.py
--rwxr-xr-x   0 nick       (501) staff       (20)      239 2019-03-15 13:54:56.000000 kubetools-9.1/kubetools_client/dev/__main__.py
--rw-r--r--   0 nick       (501) staff       (20)     7574 2019-03-15 13:54:56.000000 kubetools-9.1/kubetools_client/dev/config.py
--rw-r--r--   0 nick       (501) staff       (20)     2179 2019-03-15 13:54:56.000000 kubetools-9.1/kubetools_client/dev/container.py
--rw-r--r--   0 nick       (501) staff       (20)    12394 2019-03-15 13:54:56.000000 kubetools-9.1/kubetools_client/dev/container_util.py
--rw-r--r--   0 nick       (501) staff       (20)    10139 2019-03-20 15:31:55.000000 kubetools-9.1/kubetools_client/dev/docker_util.py
--rw-r--r--   0 nick       (501) staff       (20)     7165 2019-06-11 15:11:15.000000 kubetools-9.1/kubetools_client/dev/environment.py
--rw-r--r--   0 nick       (501) staff       (20)     1828 2019-03-15 13:54:56.000000 kubetools-9.1/kubetools_client/dev/logs.py
--rw-r--r--   0 nick       (501) staff       (20)     2829 2019-03-15 13:54:56.000000 kubetools-9.1/kubetools_client/dev/scripts.py
--rw-r--r--   0 nick       (501) staff       (20)      499 2019-03-15 13:54:56.000000 kubetools-9.1/kubetools_client/exceptions.py
--rw-r--r--   0 nick       (501) staff       (20)     2094 2019-03-15 13:54:56.000000 kubetools-9.1/kubetools_client/log.py
--rw-r--r--   0 nick       (501) staff       (20)     1617 2019-03-15 13:54:56.000000 kubetools-9.1/kubetools_client/main.py
--rw-r--r--   0 nick       (501) staff       (20)     2292 2019-03-15 13:54:56.000000 kubetools-9.1/kubetools_client/settings.py
--rw-r--r--   0 nick       (501) staff       (20)      195 2019-06-11 15:11:50.000000 kubetools-9.1/setup.cfg
--rw-r--r--   0 nick       (501) staff       (20)     1413 2019-03-20 15:40:59.000000 kubetools-9.1/setup.py
+drwxrwxr-x   0 germain   (1000) germain   (1000)        0 2019-08-28 09:06:03.000000 kubetools-9.1.1/
+-rw-rw-r--   0 germain   (1000) germain   (1000)     1436 2019-08-28 09:06:03.000000 kubetools-9.1.1/setup.py
+drwxrwxr-x   0 germain   (1000) germain   (1000)        0 2019-08-28 09:06:03.000000 kubetools-9.1.1/kubetools_client/
+-rw-rw-r--   0 germain   (1000) germain   (1000)     4013 2019-08-28 09:06:03.000000 kubetools-9.1.1/kubetools_client/config_legacy.py
+drwxrwxr-x   0 germain   (1000) germain   (1000)        0 2019-08-28 09:06:03.000000 kubetools-9.1.1/kubetools_client/cli/
+-rw-rw-r--   0 germain   (1000) germain   (1000)     7048 2019-08-28 09:06:03.000000 kubetools-9.1.1/kubetools_client/cli/generate.py
+-rwxrwxr-x   0 germain   (1000) germain   (1000)      249 2019-08-28 09:06:03.000000 kubetools-9.1.1/kubetools_client/cli/__main__.py
+-rw-rw-r--   0 germain   (1000) germain   (1000)      954 2019-08-28 09:06:03.000000 kubetools-9.1.1/kubetools_client/cli/jobs.py
+-rw-rw-r--   0 germain   (1000) germain   (1000)     8007 2019-08-28 09:06:03.000000 kubetools-9.1.1/kubetools_client/cli/lists.py
+-rw-rw-r--   0 germain   (1000) germain   (1000)      999 2019-08-28 09:06:03.000000 kubetools-9.1.1/kubetools_client/cli/__init__.py
+-rw-rw-r--   0 germain   (1000) germain   (1000)     3858 2019-08-28 09:06:03.000000 kubetools-9.1.1/kubetools_client/cli/wait.py
+-rw-rw-r--   0 germain   (1000) germain   (1000)     2228 2019-08-28 09:06:03.000000 kubetools-9.1.1/kubetools_client/cli/wait_util.py
+-rw-rw-r--   0 germain   (1000) germain   (1000)     1617 2019-08-28 09:06:03.000000 kubetools-9.1.1/kubetools_client/main.py
+-rw-rw-r--   0 germain   (1000) germain   (1000)      499 2019-08-28 09:06:03.000000 kubetools-9.1.1/kubetools_client/exceptions.py
+-rw-rw-r--   0 germain   (1000) germain   (1000)    10042 2019-08-28 09:06:03.000000 kubetools-9.1.1/kubetools_client/client.py
+-rw-rw-r--   0 germain   (1000) germain   (1000)     8325 2019-08-28 09:06:03.000000 kubetools-9.1.1/kubetools_client/config.py
+drwxrwxr-x   0 germain   (1000) germain   (1000)        0 2019-08-28 09:06:03.000000 kubetools-9.1.1/kubetools_client/dev/
+-rw-rw-r--   0 germain   (1000) germain   (1000)     2179 2019-08-28 09:06:03.000000 kubetools-9.1.1/kubetools_client/dev/container.py
+-rw-rw-r--   0 germain   (1000) germain   (1000)    10139 2019-08-28 09:06:03.000000 kubetools-9.1.1/kubetools_client/dev/docker_util.py
+-rw-rw-r--   0 germain   (1000) germain   (1000)     1828 2019-08-28 09:06:03.000000 kubetools-9.1.1/kubetools_client/dev/logs.py
+-rwxrwxr-x   0 germain   (1000) germain   (1000)      239 2019-08-28 09:06:03.000000 kubetools-9.1.1/kubetools_client/dev/__main__.py
+-rw-rw-r--   0 germain   (1000) germain   (1000)    12519 2019-08-28 09:06:03.000000 kubetools-9.1.1/kubetools_client/dev/container_util.py
+-rw-rw-r--   0 germain   (1000) germain   (1000)     7165 2019-08-28 09:06:03.000000 kubetools-9.1.1/kubetools_client/dev/environment.py
+-rw-rw-r--   0 germain   (1000) germain   (1000)     7574 2019-08-28 09:06:03.000000 kubetools-9.1.1/kubetools_client/dev/config.py
+-rw-rw-r--   0 germain   (1000) germain   (1000)      925 2019-08-28 09:06:03.000000 kubetools-9.1.1/kubetools_client/dev/__init__.py
+-rw-rw-r--   0 germain   (1000) germain   (1000)     2829 2019-08-28 09:06:03.000000 kubetools-9.1.1/kubetools_client/dev/scripts.py
+-rw-rw-r--   0 germain   (1000) germain   (1000)      144 2019-08-28 09:06:03.000000 kubetools-9.1.1/kubetools_client/__init__.py
+-rw-rw-r--   0 germain   (1000) germain   (1000)     2094 2019-08-28 09:06:03.000000 kubetools-9.1.1/kubetools_client/log.py
+-rw-rw-r--   0 germain   (1000) germain   (1000)     2292 2019-08-28 09:06:03.000000 kubetools-9.1.1/kubetools_client/settings.py
+-rw-rw-r--   0 germain   (1000) germain   (1000)      195 2019-08-28 09:06:03.000000 kubetools-9.1.1/setup.cfg
+drwxrwxr-x   0 germain   (1000) germain   (1000)        0 2019-08-28 09:06:03.000000 kubetools-9.1.1/kubetools.egg-info/
+-rw-rw-r--   0 germain   (1000) germain   (1000)      107 2019-08-28 09:06:03.000000 kubetools-9.1.1/kubetools.egg-info/entry_points.txt
+-rw-rw-r--   0 germain   (1000) germain   (1000)       17 2019-08-28 09:06:03.000000 kubetools-9.1.1/kubetools.egg-info/top_level.txt
+-rw-rw-r--   0 germain   (1000) germain   (1000)      118 2019-08-28 09:06:03.000000 kubetools-9.1.1/kubetools.egg-info/requires.txt
+-rw-rw-r--   0 germain   (1000) germain   (1000)        1 2019-08-28 09:06:03.000000 kubetools-9.1.1/kubetools.egg-info/dependency_links.txt
+-rw-rw-r--   0 germain   (1000) germain   (1000)     1003 2019-08-28 09:06:03.000000 kubetools-9.1.1/kubetools.egg-info/SOURCES.txt
+-rw-rw-r--   0 germain   (1000) germain   (1000)      271 2019-08-28 09:06:03.000000 kubetools-9.1.1/kubetools.egg-info/PKG-INFO
+-rw-rw-r--   0 germain   (1000) germain   (1000)       21 2019-08-28 09:06:03.000000 kubetools-9.1.1/MANIFEST.in
+-rw-rw-r--   0 germain   (1000) germain   (1000)      385 2019-08-28 09:06:03.000000 kubetools-9.1.1/CHANGELOG.md
+-rw-rw-r--   0 germain   (1000) germain   (1000)      476 2019-08-28 09:06:03.000000 kubetools-9.1.1/README.md
+-rw-rw-r--   0 germain   (1000) germain   (1000)      271 2019-08-28 09:06:03.000000 kubetools-9.1.1/PKG-INFO
```

### Comparing `kubetools-9.1/kubetools.egg-info/SOURCES.txt` & `kubetools-9.1.1/kubetools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kubetools-9.1/kubetools_client/cli/__init__.py` & `kubetools-9.1.1/kubetools_client/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `kubetools-9.1/kubetools_client/cli/generate.py` & `kubetools-9.1.1/kubetools_client/cli/generate.py`

 * *Files identical despite different names*

### Comparing `kubetools-9.1/kubetools_client/cli/jobs.py` & `kubetools-9.1.1/kubetools_client/cli/jobs.py`

 * *Files identical despite different names*

### Comparing `kubetools-9.1/kubetools_client/cli/lists.py` & `kubetools-9.1.1/kubetools_client/cli/lists.py`

 * *Files identical despite different names*

### Comparing `kubetools-9.1/kubetools_client/cli/wait.py` & `kubetools-9.1.1/kubetools_client/cli/wait.py`

 * *Files identical despite different names*

### Comparing `kubetools-9.1/kubetools_client/cli/wait_util.py` & `kubetools-9.1.1/kubetools_client/cli/wait_util.py`

 * *Files identical despite different names*

### Comparing `kubetools-9.1/kubetools_client/client.py` & `kubetools-9.1.1/kubetools_client/client.py`

 * *Files identical despite different names*

### Comparing `kubetools-9.1/kubetools_client/config.py` & `kubetools-9.1.1/kubetools_client/config.py`

 * *Files identical despite different names*

### Comparing `kubetools-9.1/kubetools_client/config_legacy.py` & `kubetools-9.1.1/kubetools_client/config_legacy.py`

 * *Files identical despite different names*

### Comparing `kubetools-9.1/kubetools_client/dev/__init__.py` & `kubetools-9.1.1/kubetools_client/dev/__init__.py`

 * *Files identical despite different names*

### Comparing `kubetools-9.1/kubetools_client/dev/config.py` & `kubetools-9.1.1/kubetools_client/dev/config.py`

 * *Files identical despite different names*

### Comparing `kubetools-9.1/kubetools_client/dev/container.py` & `kubetools-9.1.1/kubetools_client/dev/container.py`

 * *Files identical despite different names*

### Comparing `kubetools-9.1/kubetools_client/dev/container_util.py` & `kubetools-9.1.1/kubetools_client/dev/container_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,28 +115,30 @@
 
     status = get_container_status(kubetools_config, name)
 
     # Check for readinessProbe or probes (probes = readiness + liveness)
     probe = config.get('readinessProbe', config.get('probes'))
     if probe:
         timeout = probe.get('timeoutSeconds', 5)
+        retries = probe.get('failureThreshold', 5)
 
         # Execute a command to check for container up?
         if 'exec' in probe:
             ready_command = probe['exec']['command']
 
             click.echo('--> Waiting for {0} to be ready with {1}'.format(
                 name, click.style(' '.join(ready_command), bold=True),
             ))
 
             command = ['exec', '-T', name]
             command.extend(ready_command)
 
             run_with_retry = retry(
                 KubeDevError,
+                num_retries=retries,
                 timeout=timeout,
             )(run_compose_process)
 
             run_with_retry(kubetools_config, command)
 
         # Check HTTP status to check for container up?
         if 'httpGet' in probe:
@@ -158,14 +160,15 @@
 
             http_url = 'http://{0}:{1}{2}'.format(
                 settings.DEV_HOST, target_port, http_path,
             )
 
             get_with_retry = retry(
                 KubeDevError,
+                num_retries=retries,
                 timeout=timeout,
             )(http_get)
 
             logger.debug('Executing HTTP check: {0}'.format(http_url))
             get_with_retry(http_url, timeout)
 
     # No probe? Sleep 2s and check it's still up as a super basic check
```

### Comparing `kubetools-9.1/kubetools_client/dev/docker_util.py` & `kubetools-9.1.1/kubetools_client/dev/docker_util.py`

 * *Files identical despite different names*

### Comparing `kubetools-9.1/kubetools_client/dev/environment.py` & `kubetools-9.1.1/kubetools_client/dev/environment.py`

 * *Files identical despite different names*

### Comparing `kubetools-9.1/kubetools_client/dev/logs.py` & `kubetools-9.1.1/kubetools_client/dev/logs.py`

 * *Files identical despite different names*

### Comparing `kubetools-9.1/kubetools_client/dev/scripts.py` & `kubetools-9.1.1/kubetools_client/dev/scripts.py`

 * *Files identical despite different names*

### Comparing `kubetools-9.1/kubetools_client/log.py` & `kubetools-9.1.1/kubetools_client/log.py`

 * *Files identical despite different names*

### Comparing `kubetools-9.1/kubetools_client/main.py` & `kubetools-9.1.1/kubetools_client/main.py`

 * *Files identical despite different names*

### Comparing `kubetools-9.1/kubetools_client/settings.py` & `kubetools-9.1.1/kubetools_client/settings.py`

 * *Files identical despite different names*

### Comparing `kubetools-9.1/setup.py` & `kubetools-9.1.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,20 +34,20 @@
                 'kubetools=kubetools_client.cli.__main__:main',
                 # ktd dev commands
                 'ktd=kubetools_client.dev.__main__:main',
             ),
         },
         install_requires=(
             'click>=7',
-            'docker>=2',
+            'docker>=3.7,<4.0',
             'docker-compose',
-            'pyyaml',
+            'pyyaml>=3,<4.3',
             'pydash',
             'pyretry',
-            'requests>=2',
+            'requests>2.18,<2.21',
             'six',
             'setuptools',
         ),
         extras_require={
             'dev': (
                 'ipdb',
             ),
```

