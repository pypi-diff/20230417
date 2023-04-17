# Comparing `tmp/ops.manifest-1.1.1.tar.gz` & `tmp/ops.manifest-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ops.manifest-1.1.1.tar", last modified: Thu Apr  6 19:05:56 2023, max compression
+gzip compressed data, was "ops.manifest-1.1.2.tar", last modified: Mon Apr 17 18:42:27 2023, max compression
```

## Comparing `ops.manifest-1.1.1.tar` & `ops.manifest-1.1.2.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxr-x   0 addyess   (1000) addyess   (1000)        0 2023-04-06 19:05:56.840496 ops.manifest-1.1.1/
--rw-rw-r--   0 addyess   (1000) addyess   (1000)    11357 2023-02-06 20:40:33.000000 ops.manifest-1.1.1/LICENSE
--rw-rw-r--   0 addyess   (1000) addyess   (1000)    23732 2023-04-06 19:05:56.840496 ops.manifest-1.1.1/PKG-INFO
--rw-rw-r--   0 addyess   (1000) addyess   (1000)    10740 2022-08-26 13:28:24.000000 ops.manifest-1.1.1/README.md
-drwxrwxr-x   0 addyess   (1000) addyess   (1000)        0 2023-04-06 19:05:56.836496 ops.manifest-1.1.1/ops/
-drwxrwxr-x   0 addyess   (1000) addyess   (1000)        0 2023-04-06 19:05:56.840496 ops.manifest-1.1.1/ops/manifests/
--rw-rw-r--   0 addyess   (1000) addyess   (1000)      522 2023-02-06 17:02:56.000000 ops.manifest-1.1.1/ops/manifests/__init__.py
--rw-rw-r--   0 addyess   (1000) addyess   (1000)     6614 2023-02-06 17:02:56.000000 ops.manifest-1.1.1/ops/manifests/collector.py
--rw-rw-r--   0 addyess   (1000) addyess   (1000)      197 2023-02-06 17:02:56.000000 ops.manifest-1.1.1/ops/manifests/exceptions.py
--rw-rw-r--   0 addyess   (1000) addyess   (1000)    11154 2023-04-06 19:02:14.000000 ops.manifest-1.1.1/ops/manifests/manifest.py
--rw-rw-r--   0 addyess   (1000) addyess   (1000)     9932 2023-03-10 16:45:29.000000 ops.manifest-1.1.1/ops/manifests/manipulations.py
-drwxrwxr-x   0 addyess   (1000) addyess   (1000)        0 2023-04-06 19:05:56.840496 ops.manifest-1.1.1/ops.manifest.egg-info/
--rw-rw-r--   0 addyess   (1000) addyess   (1000)    23732 2023-04-06 19:05:56.000000 ops.manifest-1.1.1/ops.manifest.egg-info/PKG-INFO
--rw-rw-r--   0 addyess   (1000) addyess   (1000)      399 2023-04-06 19:05:56.000000 ops.manifest-1.1.1/ops.manifest.egg-info/SOURCES.txt
--rw-rw-r--   0 addyess   (1000) addyess   (1000)        1 2023-04-06 19:05:56.000000 ops.manifest-1.1.1/ops.manifest.egg-info/dependency_links.txt
--rw-rw-r--   0 addyess   (1000) addyess   (1000)       40 2023-04-06 19:05:56.000000 ops.manifest-1.1.1/ops.manifest.egg-info/requires.txt
--rw-rw-r--   0 addyess   (1000) addyess   (1000)        4 2023-04-06 19:05:56.000000 ops.manifest-1.1.1/ops.manifest.egg-info/top_level.txt
--rw-rw-r--   0 addyess   (1000) addyess   (1000)        1 2023-02-06 18:03:47.000000 ops.manifest-1.1.1/ops.manifest.egg-info/zip-safe
--rw-rw-r--   0 addyess   (1000) addyess   (1000)       80 2023-02-06 20:40:33.000000 ops.manifest-1.1.1/pyproject.toml
--rw-rw-r--   0 addyess   (1000) addyess   (1000)      979 2023-04-06 19:05:56.840496 ops.manifest-1.1.1/setup.cfg
--rw-rw-r--   0 addyess   (1000) addyess   (1000)      116 2023-02-06 20:40:33.000000 ops.manifest-1.1.1/setup.py
+drwxrwxr-x   0 addyess   (1000) addyess   (1000)        0 2023-04-17 18:42:27.598874 ops.manifest-1.1.2/
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)     1460 2023-04-17 18:41:57.000000 ops.manifest-1.1.2/CHANGELOG.md
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)    11357 2023-02-06 20:40:33.000000 ops.manifest-1.1.2/LICENSE
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)    24345 2023-04-17 18:42:27.598874 ops.manifest-1.1.2/PKG-INFO
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)    10740 2022-08-26 13:28:24.000000 ops.manifest-1.1.2/README.md
+drwxrwxr-x   0 addyess   (1000) addyess   (1000)        0 2023-04-17 18:42:27.598874 ops.manifest-1.1.2/ops/
+drwxrwxr-x   0 addyess   (1000) addyess   (1000)        0 2023-04-17 18:42:27.598874 ops.manifest-1.1.2/ops/manifests/
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)      522 2023-02-06 17:02:56.000000 ops.manifest-1.1.2/ops/manifests/__init__.py
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)     6614 2023-02-06 17:02:56.000000 ops.manifest-1.1.2/ops/manifests/collector.py
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)      197 2023-02-06 17:02:56.000000 ops.manifest-1.1.2/ops/manifests/exceptions.py
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)    11354 2023-04-17 18:31:24.000000 ops.manifest-1.1.2/ops/manifests/manifest.py
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)     9932 2023-03-10 16:45:29.000000 ops.manifest-1.1.2/ops/manifests/manipulations.py
+drwxrwxr-x   0 addyess   (1000) addyess   (1000)        0 2023-04-17 18:42:27.598874 ops.manifest-1.1.2/ops.manifest.egg-info/
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)    24345 2023-04-17 18:42:27.000000 ops.manifest-1.1.2/ops.manifest.egg-info/PKG-INFO
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)      412 2023-04-17 18:42:27.000000 ops.manifest-1.1.2/ops.manifest.egg-info/SOURCES.txt
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)        1 2023-04-17 18:42:27.000000 ops.manifest-1.1.2/ops.manifest.egg-info/dependency_links.txt
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)       40 2023-04-17 18:42:27.000000 ops.manifest-1.1.2/ops.manifest.egg-info/requires.txt
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)        4 2023-04-17 18:42:27.000000 ops.manifest-1.1.2/ops.manifest.egg-info/top_level.txt
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)        1 2023-02-06 18:03:47.000000 ops.manifest-1.1.2/ops.manifest.egg-info/zip-safe
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)       80 2023-02-06 20:40:33.000000 ops.manifest-1.1.2/pyproject.toml
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)      979 2023-04-17 18:42:27.602874 ops.manifest-1.1.2/setup.cfg
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)      116 2023-02-06 20:40:33.000000 ops.manifest-1.1.2/setup.py
```

### Comparing `ops.manifest-1.1.1/LICENSE` & `ops.manifest-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ops.manifest-1.1.1/PKG-INFO` & `ops.manifest-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ops.manifest
-Version: 1.1.1
+Version: 1.1.2
 Summary: "Kubernetes manifests for Operators"
 Home-page: https://github.com/canonical/ops-lib-manifest
 Author: Adam Dyess
 Author-email: adam.dyess@canonical.com
 License: Apache
 Keywords: juju,charming,kubernetes,operators,manifests,yaml
 Classifier: License :: OSI Approved :: Apache Software License
@@ -295,14 +295,37 @@
 Changelog
 =========
 
 Versions follow `Semantic Versioning <https://semver.org/>`_ (``<major>.<minor>.<patch>``).
 
 Backward incompatible (breaking) changes will only be introduced in major versions
 
+ops-lib-manifest 1.1.2 (2023-04-17)
+=========================
+
+Issues Resolved
+* [LP#2006619](https://launchpad.net/bugs/2006619)
+    - resolves status issues when trying to use a client
+      which cannot reach the API endpoint
+
+ops-lib-manifest 1.1.1 (2022-04-06)
+=========================
+
+Issues Resolved
+* [LP#1999427](https://launchpad.net/bugs/1999427)
+    - resolve issues when loading CRDs from an
+      unreachable API endpoint
+
+ops-lib-manifest 1.1.0 (2022-02-17)
+=========================
+
+Feature
+* Supports image manipulation of `Job`, `CronJob`,
+  `ReplicationController` and `ReplicaSet` objects
+
 
 ops-lib-manifest 1.0.0 (2022-12-14)
 =========================
 
 Issues Resolved
 * [LP#1999427](https://launchpad.net/bugs/1999427)
     - handles non-api errors from the client which are represented
```

### Comparing `ops.manifest-1.1.1/README.md` & `ops.manifest-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ops.manifest-1.1.1/ops/manifests/__init__.py` & `ops.manifest-1.1.2/ops/manifests/__init__.py`

 * *Files identical despite different names*

### Comparing `ops.manifest-1.1.1/ops/manifests/collector.py` & `ops.manifest-1.1.2/ops/manifests/collector.py`

 * *Files identical despite different names*

### Comparing `ops.manifest-1.1.1/ops/manifests/manifest.py` & `ops.manifest-1.1.2/ops/manifests/manifest.py`

 * *Files 1% similar despite different names*

```diff
@@ -231,14 +231,19 @@
         for obj in self.resources:
             try:
                 next_rsc = self.client.get(
                     type(obj.resource),
                     obj.name,
                     namespace=obj.namespace,
                 )
+            except ManifestClientError:
+                log.exception(
+                    f"Cannot connect to the api endpoint, marking ({obj}) as missing"
+                )
+                continue
             except (ApiError, HTTPError):
                 log.exception(f"Didn't find expected resource installed ({obj})")
                 continue
             result[HashableResource(next_rsc)] = None
         return frozenset(result.keys())
 
     def labelled_resources(self) -> FrozenSet[HashableResource]:
```

### Comparing `ops.manifest-1.1.1/ops/manifests/manipulations.py` & `ops.manifest-1.1.2/ops/manifests/manipulations.py`

 * *Files identical despite different names*

### Comparing `ops.manifest-1.1.1/ops.manifest.egg-info/PKG-INFO` & `ops.manifest-1.1.2/ops.manifest.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ops.manifest
-Version: 1.1.1
+Version: 1.1.2
 Summary: "Kubernetes manifests for Operators"
 Home-page: https://github.com/canonical/ops-lib-manifest
 Author: Adam Dyess
 Author-email: adam.dyess@canonical.com
 License: Apache
 Keywords: juju,charming,kubernetes,operators,manifests,yaml
 Classifier: License :: OSI Approved :: Apache Software License
@@ -295,14 +295,37 @@
 Changelog
 =========
 
 Versions follow `Semantic Versioning <https://semver.org/>`_ (``<major>.<minor>.<patch>``).
 
 Backward incompatible (breaking) changes will only be introduced in major versions
 
+ops-lib-manifest 1.1.2 (2023-04-17)
+=========================
+
+Issues Resolved
+* [LP#2006619](https://launchpad.net/bugs/2006619)
+    - resolves status issues when trying to use a client
+      which cannot reach the API endpoint
+
+ops-lib-manifest 1.1.1 (2022-04-06)
+=========================
+
+Issues Resolved
+* [LP#1999427](https://launchpad.net/bugs/1999427)
+    - resolve issues when loading CRDs from an
+      unreachable API endpoint
+
+ops-lib-manifest 1.1.0 (2022-02-17)
+=========================
+
+Feature
+* Supports image manipulation of `Job`, `CronJob`,
+  `ReplicationController` and `ReplicaSet` objects
+
 
 ops-lib-manifest 1.0.0 (2022-12-14)
 =========================
 
 Issues Resolved
 * [LP#1999427](https://launchpad.net/bugs/1999427)
     - handles non-api errors from the client which are represented
```

### Comparing `ops.manifest-1.1.1/setup.cfg` & `ops.manifest-1.1.2/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ops.manifest
-version = 1.1.1
+version = 1.1.2
 author = Adam Dyess
 author_email = adam.dyess@canonical.com
 description = "Kubernetes manifests for Operators"
 long_description = file: README.md, CHANGELOG.md, LICENSE
 long_description_content_type = text/markdown
 keywords = juju, charming, kubernetes, operators, manifests, yaml
 license = Apache
```

