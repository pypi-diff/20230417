# Comparing `tmp/kadalu-quotad-1.0.1.tar.gz` & `tmp/kadalu-quotad-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kadalu-quotad-1.0.1.tar", last modified: Thu Mar 30 02:26:59 2023, max compression
+gzip compressed data, was "kadalu-quotad-1.1.0.tar", last modified: Mon Apr 17 18:07:19 2023, max compression
```

## Comparing `kadalu-quotad-1.0.1.tar` & `kadalu-quotad-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 02:26:59.303073 kadalu-quotad-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-30 02:26:40.000000 kadalu-quotad-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-03-30 02:26:59.303073 kadalu-quotad-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-03-30 02:26:40.000000 kadalu-quotad-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-30 02:26:58.000000 kadalu-quotad-1.0.1/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 02:26:59.303073 kadalu-quotad-1.0.1/kadalu_quotad/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 02:26:40.000000 kadalu-quotad-1.0.1/kadalu_quotad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-03-30 02:26:40.000000 kadalu-quotad-1.0.1/kadalu_quotad/glusterutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12824 2023-03-30 02:26:58.000000 kadalu-quotad-1.0.1/kadalu_quotad/kadalulib.py
--rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-03-30 02:26:40.000000 kadalu-quotad-1.0.1/kadalu_quotad/quotad.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 02:26:59.303073 kadalu-quotad-1.0.1/kadalu_quotad.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-03-30 02:26:59.000000 kadalu-quotad-1.0.1/kadalu_quotad.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-03-30 02:26:59.000000 kadalu-quotad-1.0.1/kadalu_quotad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 02:26:59.000000 kadalu-quotad-1.0.1/kadalu_quotad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-30 02:26:59.000000 kadalu-quotad-1.0.1/kadalu_quotad.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 02:26:59.000000 kadalu-quotad-1.0.1/kadalu_quotad.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-30 02:26:59.000000 kadalu-quotad-1.0.1/kadalu_quotad.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-30 02:26:59.000000 kadalu-quotad-1.0.1/kadalu_quotad.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 02:26:59.303073 kadalu-quotad-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-03-30 02:26:40.000000 kadalu-quotad-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:07:19.556137 kadalu-quotad-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-17 18:06:53.000000 kadalu-quotad-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-17 18:07:19.556137 kadalu-quotad-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-17 18:06:53.000000 kadalu-quotad-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-17 18:07:19.000000 kadalu-quotad-1.1.0/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:07:19.556137 kadalu-quotad-1.1.0/kadalu_quotad/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:06:53.000000 kadalu-quotad-1.1.0/kadalu_quotad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-04-17 18:06:53.000000 kadalu-quotad-1.1.0/kadalu_quotad/glusterutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13733 2023-04-17 18:07:19.000000 kadalu-quotad-1.1.0/kadalu_quotad/kadalulib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-04-17 18:06:53.000000 kadalu-quotad-1.1.0/kadalu_quotad/quotad.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:07:19.556137 kadalu-quotad-1.1.0/kadalu_quotad.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-17 18:07:19.000000 kadalu-quotad-1.1.0/kadalu_quotad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-17 18:07:19.000000 kadalu-quotad-1.1.0/kadalu_quotad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 18:07:19.000000 kadalu-quotad-1.1.0/kadalu_quotad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-17 18:07:19.000000 kadalu-quotad-1.1.0/kadalu_quotad.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 18:07:19.000000 kadalu-quotad-1.1.0/kadalu_quotad.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-17 18:07:19.000000 kadalu-quotad-1.1.0/kadalu_quotad.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-17 18:07:19.000000 kadalu-quotad-1.1.0/kadalu_quotad.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 18:07:19.556137 kadalu-quotad-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-17 18:06:53.000000 kadalu-quotad-1.1.0/setup.py
```

### Comparing `kadalu-quotad-1.0.1/PKG-INFO` & `kadalu-quotad-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kadalu-quotad
-Version: 1.0.1
+Version: 1.1.0
 Summary: Kadalu Quota Daemon
 Home-page: https://github.com/kadalu/kadalu
 Author: Kadalu Authors
 Author-email: support@kadalu.io
 License: Apache-2.0
 Keywords: kadalu,container,kubernetes,kubectl,storage
 Platform: linux
```

### Comparing `kadalu-quotad-1.0.1/README.md` & `kadalu-quotad-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `kadalu-quotad-1.0.1/kadalu_quotad/glusterutils.py` & `kadalu-quotad-1.1.0/kadalu_quotad/glusterutils.py`

 * *Files identical despite different names*

### Comparing `kadalu-quotad-1.0.1/kadalu_quotad/kadalulib.py` & `kadalu-quotad-1.1.0/kadalu_quotad/kadalulib.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,16 +75,46 @@
                           stderr=None,
                           stdout=None,
                           universal_newlines=True) as proc:
         proc.communicate()
         return proc.returncode == 0
 
 
+def is_server_pod_reachable(hosts, port=24007, timeout=20):
+    """
+    Return True if atleast one of server pods(internal hosts),
+    are reachable at port 24007.
+    Retries every 30 seconds if the server pod is not reachable.
+    Returns False server pods are not reachable even after the timeout.
+    """
+
+    socket.setdefaulttimeout(timeout)
+
+    for host in hosts:
+        retry_count = 0
+        while retry_count < 4:
+            try:
+                sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+                sock.connect((host, port))
+                sock.close()
+                return True
+            except socket.error:
+                logging.info(logf(
+                    "Waiting for the server pod to come up...",
+                    server_pod=host,
+                    retry_count=retry_count+1
+                ))
+                time.sleep(30)
+                retry_count += 1
+    return False
+
+
 def is_host_reachable(hosts, port):
     """Check if glusterd is reachable in the given node"""
+
     timeout = 5
     sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
     sock.settimeout(timeout)
     for host in hosts:
         try:
             sock.connect((host, int(port)))
             sock.shutdown(socket.SHUT_RDWR)
@@ -415,15 +445,14 @@
 
                 for _, state in self.procs.items():
                     self.monitor_proc(state, terminating)
 
                 if terminating:
                     logging.info("Terminating Monitor process")
                     sys.exit(0)
-                    break
 
                 time.sleep(1)
         except KeyboardInterrupt:
             self.terminating = True
             sys.exit(1)
```

### Comparing `kadalu-quotad-1.0.1/kadalu_quotad/quotad.py` & `kadalu-quotad-1.1.0/kadalu_quotad/quotad.py`

 * *Files identical despite different names*

### Comparing `kadalu-quotad-1.0.1/kadalu_quotad.egg-info/PKG-INFO` & `kadalu-quotad-1.1.0/kadalu_quotad.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kadalu-quotad
-Version: 1.0.1
+Version: 1.1.0
 Summary: Kadalu Quota Daemon
 Home-page: https://github.com/kadalu/kadalu
 Author: Kadalu Authors
 Author-email: support@kadalu.io
 License: Apache-2.0
 Keywords: kadalu,container,kubernetes,kubectl,storage
 Platform: linux
```

### Comparing `kadalu-quotad-1.0.1/setup.py` & `kadalu-quotad-1.1.0/setup.py`

 * *Files identical despite different names*

