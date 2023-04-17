# Comparing `tmp/promexp-1.0.2.tar.gz` & `tmp/promexp-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/promexp-1.0.2.tar", last modified: Tue May 25 07:37:08 2021, max compression
+gzip compressed data, was "promexp-1.0.3.tar", last modified: Mon Apr 17 13:55:27 2023, max compression
```

## Comparing `promexp-1.0.2.tar` & `promexp-1.0.3.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxrwxr-x   0 martas    (1000) martas    (1000)        0 2021-05-25 07:37:08.000000 promexp-1.0.2/
-drwxrwxr-x   0 martas    (1000) martas    (1000)        0 2021-05-25 07:37:08.000000 promexp-1.0.2/promexp.egg-info/
--rw-rw-r--   0 martas    (1000) martas    (1000)     9792 2021-05-25 07:37:08.000000 promexp-1.0.2/promexp.egg-info/PKG-INFO
--rw-rw-r--   0 martas    (1000) martas    (1000)      646 2021-05-25 07:37:08.000000 promexp-1.0.2/promexp.egg-info/SOURCES.txt
--rw-rw-r--   0 martas    (1000) martas    (1000)        1 2021-05-25 07:37:08.000000 promexp-1.0.2/promexp.egg-info/dependency_links.txt
--rw-rw-r--   0 martas    (1000) martas    (1000)        8 2021-05-25 07:37:08.000000 promexp-1.0.2/promexp.egg-info/top_level.txt
--rw-rw-r--   0 martas    (1000) martas    (1000)     9792 2021-05-25 07:37:08.000000 promexp-1.0.2/PKG-INFO
--rw-rw-r--   0 martas    (1000) martas    (1000)       38 2021-05-25 07:37:08.000000 promexp-1.0.2/setup.cfg
--rw-rw-r--   0 martas    (1000) martas    (1000)     7509 2021-02-11 09:10:33.000000 promexp-1.0.2/README.md
--rw-rw-r--   0 martas    (1000) martas    (1000)      966 2021-05-25 07:34:50.000000 promexp-1.0.2/setup.py
-drwxrwxr-x   0 martas    (1000) martas    (1000)        0 2021-05-25 07:37:08.000000 promexp-1.0.2/promexp/
--rw-rw-r--   0 martas    (1000) martas    (1000)     1960 2021-02-15 13:33:55.000000 promexp-1.0.2/promexp/metrics.py
--rw-rw-r--   0 martas    (1000) martas    (1000)     1294 2021-02-15 13:33:55.000000 promexp-1.0.2/promexp/__init__.py
--rw-rw-r--   0 martas    (1000) martas    (1000)      809 2021-02-09 14:44:27.000000 promexp-1.0.2/promexp/provider.py
-drwxrwxr-x   0 martas    (1000) martas    (1000)        0 2021-05-25 07:37:08.000000 promexp-1.0.2/promexp/providers/
-drwxrwxr-x   0 martas    (1000) martas    (1000)        0 2021-05-25 07:37:08.000000 promexp-1.0.2/promexp/providers/casparcg/
--rw-rw-r--   0 martas    (1000) martas    (1000)     5111 2021-05-25 07:27:21.000000 promexp-1.0.2/promexp/providers/casparcg/__init__.py
--rw-rw-r--   0 martas    (1000) martas    (1000)     1890 2021-01-12 16:29:28.000000 promexp-1.0.2/promexp/providers/casparcg/ntp.py
--rw-rw-r--   0 martas    (1000) martas    (1000)     4136 2021-01-12 16:29:28.000000 promexp-1.0.2/promexp/providers/casparcg/message.py
--rw-rw-r--   0 martas    (1000) martas    (1000)     3459 2021-01-12 16:29:28.000000 promexp-1.0.2/promexp/providers/casparcg/bundle.py
--rw-rw-r--   0 martas    (1000) martas    (1000)      971 2021-01-12 16:29:28.000000 promexp-1.0.2/promexp/providers/casparcg/osc_server.py
--rw-rw-r--   0 martas    (1000) martas    (1000)     2424 2021-01-12 16:29:28.000000 promexp-1.0.2/promexp/providers/casparcg/packet.py
--rw-rw-r--   0 martas    (1000) martas    (1000)    11024 2021-01-12 16:29:28.000000 promexp-1.0.2/promexp/providers/casparcg/osc_types.py
--rw-rw-r--   0 martas    (1000) martas    (1000)      378 2021-02-08 21:50:14.000000 promexp-1.0.2/promexp/providers/__init__.py
--rw-rw-r--   0 martas    (1000) martas    (1000)     2316 2021-02-09 12:47:38.000000 promexp-1.0.2/promexp/providers/nvidia.py
--rw-rw-r--   0 martas    (1000) martas    (1000)     1808 2021-02-05 20:54:33.000000 promexp-1.0.2/promexp/providers/storage.py
--rw-rw-r--   0 martas    (1000) martas    (1000)     2404 2021-02-09 14:44:27.000000 promexp-1.0.2/promexp/providers/storagespaces.py
--rw-rw-r--   0 martas    (1000) martas    (1000)     1257 2021-05-25 06:49:11.000000 promexp-1.0.2/promexp/providers/psutil.py
--rw-rw-r--   0 martas    (1000) martas    (1000)     1395 2021-02-05 20:54:33.000000 promexp-1.0.2/promexp/providers/network.py
+drwxrwxr-x   0 martas    (1000) martas    (1000)        0 2023-04-17 13:55:27.902385 promexp-1.0.3/
+-rw-r--r--   0 martas    (1000) martas    (1000)     1068 2021-02-05 20:54:33.000000 promexp-1.0.3/LICENSE
+-rw-rw-r--   0 martas    (1000) martas    (1000)     8195 2023-04-17 13:55:27.902385 promexp-1.0.3/PKG-INFO
+-rw-r--r--   0 martas    (1000) martas    (1000)     7509 2021-02-11 09:10:33.000000 promexp-1.0.3/README.md
+drwxrwxr-x   0 martas    (1000) martas    (1000)        0 2023-04-17 13:55:27.902385 promexp-1.0.3/promexp/
+-rw-r--r--   0 martas    (1000) martas    (1000)     1323 2023-04-17 13:55:01.000000 promexp-1.0.3/promexp/__init__.py
+-rw-r--r--   0 martas    (1000) martas    (1000)     1991 2023-04-17 13:54:44.000000 promexp-1.0.3/promexp/metrics.py
+-rw-r--r--   0 martas    (1000) martas    (1000)      834 2023-04-17 13:54:47.000000 promexp-1.0.3/promexp/provider.py
+drwxrwxr-x   0 martas    (1000) martas    (1000)        0 2023-04-17 13:55:27.902385 promexp-1.0.3/promexp/providers/
+-rw-r--r--   0 martas    (1000) martas    (1000)      378 2023-04-17 13:54:28.000000 promexp-1.0.3/promexp/providers/__init__.py
+drwxrwxr-x   0 martas    (1000) martas    (1000)        0 2023-04-17 13:55:27.902385 promexp-1.0.3/promexp/providers/casparcg/
+-rw-r--r--   0 martas    (1000) martas    (1000)     5111 2021-05-25 07:27:21.000000 promexp-1.0.3/promexp/providers/casparcg/__init__.py
+-rw-r--r--   0 martas    (1000) martas    (1000)     3459 2021-01-12 16:29:28.000000 promexp-1.0.3/promexp/providers/casparcg/bundle.py
+-rw-r--r--   0 martas    (1000) martas    (1000)     4136 2021-01-12 16:29:28.000000 promexp-1.0.3/promexp/providers/casparcg/message.py
+-rw-r--r--   0 martas    (1000) martas    (1000)     1890 2021-01-12 16:29:28.000000 promexp-1.0.3/promexp/providers/casparcg/ntp.py
+-rw-r--r--   0 martas    (1000) martas    (1000)      971 2021-01-12 16:29:28.000000 promexp-1.0.3/promexp/providers/casparcg/osc_server.py
+-rw-r--r--   0 martas    (1000) martas    (1000)    11024 2021-01-12 16:29:28.000000 promexp-1.0.3/promexp/providers/casparcg/osc_types.py
+-rw-r--r--   0 martas    (1000) martas    (1000)     2424 2021-01-12 16:29:28.000000 promexp-1.0.3/promexp/providers/casparcg/packet.py
+-rw-r--r--   0 martas    (1000) martas    (1000)     1395 2023-04-17 13:54:31.000000 promexp-1.0.3/promexp/providers/network.py
+-rw-r--r--   0 martas    (1000) martas    (1000)     2316 2023-04-17 13:54:34.000000 promexp-1.0.3/promexp/providers/nvidia.py
+-rw-r--r--   0 martas    (1000) martas    (1000)     1257 2023-04-17 13:54:36.000000 promexp-1.0.3/promexp/providers/psutil.py
+-rw-r--r--   0 martas    (1000) martas    (1000)     2210 2023-04-17 13:53:49.000000 promexp-1.0.3/promexp/providers/storage.py
+-rw-r--r--   0 martas    (1000) martas    (1000)     2405 2023-04-17 13:54:39.000000 promexp-1.0.3/promexp/providers/storagespaces.py
+drwxrwxr-x   0 martas    (1000) martas    (1000)        0 2023-04-17 13:55:27.902385 promexp-1.0.3/promexp.egg-info/
+-rw-r--r--   0 martas    (1000) martas    (1000)     8195 2023-04-17 13:55:27.000000 promexp-1.0.3/promexp.egg-info/PKG-INFO
+-rw-r--r--   0 martas    (1000) martas    (1000)      654 2023-04-17 13:55:27.000000 promexp-1.0.3/promexp.egg-info/SOURCES.txt
+-rw-r--r--   0 martas    (1000) martas    (1000)        1 2023-04-17 13:55:27.000000 promexp-1.0.3/promexp.egg-info/dependency_links.txt
+-rw-r--r--   0 martas    (1000) martas    (1000)        8 2023-04-17 13:55:27.000000 promexp-1.0.3/promexp.egg-info/top_level.txt
+-rw-rw-r--   0 martas    (1000) martas    (1000)       38 2023-04-17 13:55:27.902385 promexp-1.0.3/setup.cfg
+-rw-r--r--   0 martas    (1000) martas    (1000)      952 2023-04-17 13:54:56.000000 promexp-1.0.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `promexp-1.0.2/promexp.egg-info/SOURCES.txt` & `promexp-1.0.3/promexp.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 promexp/__init__.py
 promexp/metrics.py
 promexp/provider.py
 promexp.egg-info/PKG-INFO
 promexp.egg-info/SOURCES.txt
```

### Comparing `promexp-1.0.2/README.md` & `promexp-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `promexp-1.0.2/setup.py` & `promexp-1.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import os
 from setuptools import setup
 
+
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
+
 setup(
-    name = "promexp",
-    version = "1.0.2",
-    author = "Martin Wacker",
-    author_email = "martas@imm.cz",
-    description = "A simple system metrics exporter for Prometheus",
-    license = "MIT",
-    keywords = "metrics devops prometheus",
-    url = "https://github.com/immstudios/promexp",
-    packages=['promexp', 'promexp.providers', 'promexp.providers.casparcg'],
-    long_description=read('README.md'),
-    long_description_content_type='text/markdown',
+    name="promexp",
+    version="1.0.3",
+    author="Martin Wacker",
+    author_email="martas@imm.cz",
+    description="A simple system metrics exporter for Prometheus",
+    license="MIT",
+    keywords="metrics devops prometheus",
+    url="https://github.com/immstudios/promexp",
+    packages=["promexp", "promexp.providers", "promexp.providers.casparcg"],
+    long_description=read("README.md"),
+    long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: POSIX :: Linux",
```

### Comparing `promexp-1.0.2/promexp/metrics.py` & `promexp-1.0.3/promexp/metrics.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import collections.abc
 
+
 class frozendict(collections.abc.Mapping):
     dict_cls = dict
 
     def __init__(self, *args, **kwargs):
         self._dict = self.dict_cls(*args, **kwargs)
         self._hash = None
 
@@ -30,19 +31,19 @@
             h = 0
             for key, value in self._dict.items():
                 h ^= hash((key, value))
             self._hash = h
         return self._hash
 
 
-class Metrics():
+class Metrics:
     def __init__(self):
         self.data = {}
 
-    def add(self, metric_name:str, value:float, **tags) -> bool:
+    def add(self, metric_name: str, value: float, **tags) -> bool:
         """Add a metric to the pool"""
         if type(value) not in [int, float]:
             return False
         key = (metric_name, frozendict(**tags))
         self.data[key] = value
         return True
 
@@ -51,18 +52,19 @@
         return [[key[0], key[1]._dict, value] for key, value in self.data.items()]
 
     def load(self, data):
         """Loads data from a list created previously using dump method"""
         for name, tags, value in data:
             self.add(name, value, **tags)
 
-    def render(self, prefix:str="", **kwargs):
+    def render(self, prefix: str = "", **kwargs):
         """Returns metrics in Prometheus format"""
         if prefix:
             prefix += "_"
         result = ""
         for key, value in self.data.items():
             name, tags = key
-            tstring = ", ".join(f"{k}=\"{v}\"" for k, v in {**tags._dict, **kwargs}.items())
+            tstring = ", ".join(
+                f'{k}="{v}"' for k, v in {**tags._dict, **kwargs}.items()
+            )
             result += f"{prefix}{name}{{{tstring}}} {value}\n"
         return result
-
```

### Comparing `promexp-1.0.2/promexp/__init__.py` & `promexp-1.0.3/promexp/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 import logging
 
 from .metrics import Metrics
 from .providers import registry
 
-class Promexp():
+
+class Promexp:
     def __init__(self, prefix="", tags={}, provider_settings={}, logger=None):
         self.prefix = prefix
         self.tags = tags
         self.providers = {}
         self._logger = logger
         self.metrics = Metrics()
         for pclass in registry:
             self.add_provider(pclass, provider_settings.get(pclass.name, {}))
 
     def add_provider(self, pclass, psettings={}):
         if psettings is None:
             return False
 
         if pclass.name in self.providers:
-            self.logger.warning(f"Duplicate provider name {pclass.name}. Skipping initialization.")
+            self.logger.warning(
+                f"Duplicate provider name {pclass.name}. Skipping initialization."
+            )
             return False
 
         self.providers[pclass.name] = pclass(self, psettings)
 
         if self.providers[pclass.name].enabled:
             self.logger.info(f"Enabling {pclass.name} provider")
 
     @property
     def logger(self):
-        if self._logger == None:
+        if self._logger is None:
             self._logger = logging.getLogger("promexp")
         return self._logger
 
     def collect(self):
         for name, provider in self.providers.items():
             if provider.enabled:
                 provider.collect()
```

### Comparing `promexp-1.0.2/promexp/provider.py` & `promexp-1.0.3/promexp/provider.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-class BaseProvider():
+class BaseProvider:
     name = "base"
 
     def __init__(self, parent, settings):
         self.parent = parent
         self.logger = parent.logger
         self.enabled = settings is not None
         if type(settings) == dict:
             self.settings = settings
         else:
-            self.logger.warning(f"Incorrect settings for {self.name} provider. Ignoring")
+            self.logger.warning(
+                f"Incorrect settings for {self.name} provider. Ignoring"
+            )
             self.settings = {}
 
     def __getitem__(self, key):
         return self.settings.get(key, None)
 
     def get(self, key, default):
         return self.settings.get(key, default)
@@ -24,10 +26,7 @@
         self.enabled = True
 
     def add(self, metric_name, value, **tags):
         self.parent.metrics.add(metric_name, value, **tags)
 
     def collect(self):
         pass
-
-
-
```

### Comparing `promexp-1.0.2/promexp/providers/casparcg/__init__.py` & `promexp-1.0.3/promexp/providers/casparcg/__init__.py`

 * *Files identical despite different names*

### Comparing `promexp-1.0.2/promexp/providers/casparcg/ntp.py` & `promexp-1.0.3/promexp/providers/casparcg/ntp.py`

 * *Files identical despite different names*

### Comparing `promexp-1.0.2/promexp/providers/casparcg/message.py` & `promexp-1.0.3/promexp/providers/casparcg/message.py`

 * *Files identical despite different names*

### Comparing `promexp-1.0.2/promexp/providers/casparcg/bundle.py` & `promexp-1.0.3/promexp/providers/casparcg/bundle.py`

 * *Files identical despite different names*

### Comparing `promexp-1.0.2/promexp/providers/casparcg/osc_server.py` & `promexp-1.0.3/promexp/providers/casparcg/osc_server.py`

 * *Files identical despite different names*

### Comparing `promexp-1.0.2/promexp/providers/casparcg/packet.py` & `promexp-1.0.3/promexp/providers/casparcg/packet.py`

 * *Files identical despite different names*

### Comparing `promexp-1.0.2/promexp/providers/casparcg/osc_types.py` & `promexp-1.0.3/promexp/providers/casparcg/osc_types.py`

 * *Files identical despite different names*

### Comparing `promexp-1.0.2/promexp/providers/nvidia.py` & `promexp-1.0.3/promexp/providers/nvidia.py`

 * *Files identical despite different names*

### Comparing `promexp-1.0.2/promexp/providers/storage.py` & `promexp-1.0.3/promexp/providers/storage.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,43 +6,66 @@
 
 
 class StorageProvider(BaseProvider):
     name = "storage"
 
     def __init__(self, parent, settings):
         super(StorageProvider, self).__init__(parent, settings)
-        mountpoint_blacklist = ["/run", "/proc", "/sys", "/dev", "/snap", "/var/lib", "/tmp/snap", "/boot"]
+        mountpoint_blacklist = [
+            "/run",
+            "/proc",
+            "/sys",
+            "/dev",
+            "/snap",
+            "/var/lib",
+            "/tmp/snap",
+            "/boot",
+        ]
         mountpoint_whitelist = self.get("storages", [])
-        
+
         self.storages = []
         for storage in psutil.disk_partitions(all=True):
-            if not all([not storage.mountpoint.startswith(b) for b in mountpoint_blacklist]):
+            if not all(
+                [not storage.mountpoint.startswith(b) for b in mountpoint_blacklist]
+            ):
                 continue
 
             if mountpoint_whitelist:
-                if not any([storage.mountpoint == b if b == "/" else storage.mountpoint.lower().startswith(b.lower()) for b in mountpoint_whitelist ]):
+                if not any(
+                    [
+                        storage.mountpoint == b
+                        if b == "/"
+                        else storage.mountpoint.lower().startswith(b.lower())
+                        for b in mountpoint_whitelist
+                    ]
+                ):
                     continue
 
-            self.storages.append({
-                    "device" : storage.device,
-                    "mountpoint" : storage.mountpoint,
-                    "fstype" : storage.fstype,
-                })
-
+            self.storages.append(
+                {
+                    "device": storage.device,
+                    "mountpoint": storage.mountpoint,
+                    "fstype": storage.fstype,
+                }
+            )
 
     def collect(self):
         for storage in self.storages:
             if storage.get("disabled"):
                 continue
             try:
                 usage = psutil.disk_usage(storage["mountpoint"])
             except PermissionError:
-                self.logger.warning(f"Disabling {storage['mountpoint']} check due to permission error")
+                self.logger.warning(
+                    f"Disabling {storage['mountpoint']} check due to permission error"
+                )
                 storage["disabled"] = True
                 continue
+            except Exception:
+                continue
             tags = {
-                "mountpoint" : storage["mountpoint"].replace("\\", "/"),
-                "fstype" : storage["fstype"],
+                "mountpoint": storage["mountpoint"].replace("\\", "/"),
+                "fstype": storage["fstype"],
             }
             self.add("storage_bytes_total", usage.total, **tags)
             self.add("storage_bytes_free", usage.free, **tags)
-            self.add("storage_usage", usage.percent, **tags)
+            self.add("storage_usage", usage.percent, **tags)
```

### Comparing `promexp-1.0.2/promexp/providers/storagespaces.py` & `promexp-1.0.3/promexp/providers/storagespaces.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -92,8 +92,8 @@
             status = []
 
         for sspace in status:
             tags = {
                 "name" : sspace["title"],
                 "mode" : sspace["mode"]
             }
-            self.add("storage_space_healthy", int(sspace["health"] == "Healthy"), **tags)
+            self.add("storage_space_healthy", int(sspace["health"] == "Healthy"), **tags)
```

### Comparing `promexp-1.0.2/promexp/providers/psutil.py` & `promexp-1.0.3/promexp/providers/psutil.py`

 * *Files identical despite different names*

### Comparing `promexp-1.0.2/promexp/providers/network.py` & `promexp-1.0.3/promexp/providers/network.py`

 * *Files identical despite different names*

