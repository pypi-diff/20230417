# Comparing `tmp/dab-1.0.0.tar.gz` & `tmp/dab-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dab-1.0.0.tar", last modified: Wed May 26 13:53:25 2021, max compression
+gzip compressed data, was "dab-1.0.1.tar", last modified: Mon Apr 17 13:43:53 2023, max compression
```

## Comparing `dab-1.0.0.tar` & `dab-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxr-x   0 lph       (1000) lph       (1000)        0 2021-05-26 13:53:25.620359 dab-1.0.0/
--rw-rw-r--   0 lph       (1000) lph       (1000)      202 2021-05-26 13:53:25.620359 dab-1.0.0/PKG-INFO
-drwxrwxr-x   0 lph       (1000) lph       (1000)        0 2021-05-26 13:53:25.620359 dab-1.0.0/dab/
--rw-rw-r--   0 lph       (1000) lph       (1000)      910 2021-05-26 13:43:43.000000 dab-1.0.0/dab/__init__.py
--rwxrwxr-x   0 lph       (1000) lph       (1000)     1801 2021-05-26 13:43:43.000000 dab-1.0.0/dab/__main__.py
--rw-rw-r--   0 lph       (1000) lph       (1000)     5531 2021-05-26 13:43:43.000000 dab-1.0.0/dab/core.py
--rw-rw-r--   0 lph       (1000) lph       (1000)     1803 2021-05-26 13:43:43.000000 dab-1.0.0/dab/dns.py
--rw-rw-r--   0 lph       (1000) lph       (1000)     6907 2021-05-26 13:43:43.000000 dab-1.0.0/dab/netbios.py
--rw-rw-r--   0 lph       (1000) lph       (1000)     2134 2021-05-26 13:43:43.000000 dab-1.0.0/dab/ssh.py
-drwxrwxr-x   0 lph       (1000) lph       (1000)        0 2021-05-26 13:53:25.620359 dab-1.0.0/dab.egg-info/
--rw-rw-r--   0 lph       (1000) lph       (1000)      202 2021-05-26 13:53:25.000000 dab-1.0.0/dab.egg-info/PKG-INFO
--rw-rw-r--   0 lph       (1000) lph       (1000)      253 2021-05-26 13:53:25.000000 dab-1.0.0/dab.egg-info/SOURCES.txt
--rw-rw-r--   0 lph       (1000) lph       (1000)        1 2021-05-26 13:53:25.000000 dab-1.0.0/dab.egg-info/dependency_links.txt
--rw-rw-r--   0 lph       (1000) lph       (1000)       43 2021-05-26 13:53:25.000000 dab-1.0.0/dab.egg-info/entry_points.txt
--rw-rw-r--   0 lph       (1000) lph       (1000)       47 2021-05-26 13:53:25.000000 dab-1.0.0/dab.egg-info/requires.txt
--rw-rw-r--   0 lph       (1000) lph       (1000)        4 2021-05-26 13:53:25.000000 dab-1.0.0/dab.egg-info/top_level.txt
--rw-rw-r--   0 lph       (1000) lph       (1000)       38 2021-05-26 13:53:25.620359 dab-1.0.0/setup.cfg
--rw-rw-r--   0 lph       (1000) lph       (1000)      395 2021-05-26 13:52:36.000000 dab-1.0.0/setup.py
+drwxrwxr-x   0 lph       (1000) lph       (1000)        0 2023-04-17 13:43:53.534783 dab-1.0.1/
+-rw-rw-r--   0 lph       (1000) lph       (1000)      880 2021-05-26 13:43:43.000000 dab-1.0.1/LICENSE
+-rw-rw-r--   0 lph       (1000) lph       (1000)      175 2023-04-17 13:43:53.534783 dab-1.0.1/PKG-INFO
+drwxrwxr-x   0 lph       (1000) lph       (1000)        0 2023-04-17 13:43:53.534783 dab-1.0.1/dab/
+-rw-rw-r--   0 lph       (1000) lph       (1000)      910 2021-05-26 13:43:43.000000 dab-1.0.1/dab/__init__.py
+-rwxrwxr-x   0 lph       (1000) lph       (1000)     1801 2021-05-26 13:43:43.000000 dab-1.0.1/dab/__main__.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     5801 2023-04-17 13:39:09.000000 dab-1.0.1/dab/core.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     1803 2021-05-26 13:43:43.000000 dab-1.0.1/dab/dns.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     6907 2021-05-26 13:43:43.000000 dab-1.0.1/dab/netbios.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     2134 2021-05-26 13:43:43.000000 dab-1.0.1/dab/ssh.py
+drwxrwxr-x   0 lph       (1000) lph       (1000)        0 2023-04-17 13:43:53.534783 dab-1.0.1/dab.egg-info/
+-rw-rw-r--   0 lph       (1000) lph       (1000)      175 2023-04-17 13:43:53.000000 dab-1.0.1/dab.egg-info/PKG-INFO
+-rw-rw-r--   0 lph       (1000) lph       (1000)      261 2023-04-17 13:43:53.000000 dab-1.0.1/dab.egg-info/SOURCES.txt
+-rw-rw-r--   0 lph       (1000) lph       (1000)        1 2023-04-17 13:43:53.000000 dab-1.0.1/dab.egg-info/dependency_links.txt
+-rw-rw-r--   0 lph       (1000) lph       (1000)       43 2023-04-17 13:43:53.000000 dab-1.0.1/dab.egg-info/entry_points.txt
+-rw-rw-r--   0 lph       (1000) lph       (1000)       47 2023-04-17 13:43:53.000000 dab-1.0.1/dab.egg-info/requires.txt
+-rw-rw-r--   0 lph       (1000) lph       (1000)        4 2023-04-17 13:43:53.000000 dab-1.0.1/dab.egg-info/top_level.txt
+-rw-rw-r--   0 lph       (1000) lph       (1000)       38 2023-04-17 13:43:53.534783 dab-1.0.1/setup.cfg
+-rw-rw-r--   0 lph       (1000) lph       (1000)      395 2023-04-17 13:43:26.000000 dab-1.0.1/setup.py
```

### Comparing `dab-1.0.0/dab/__init__.py` & `dab-1.0.1/dab/__init__.py`

 * *Files identical despite different names*

### Comparing `dab-1.0.0/dab/__main__.py` & `dab-1.0.1/dab/__main__.py`

 * *Files identical despite different names*

### Comparing `dab-1.0.0/dab/core.py` & `dab-1.0.1/dab/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,20 +55,23 @@
     SSH_PORTS = [22]
 
     # TLS-enabled Ports
     TLS_PORTS = [443, 5002]
 
     alternative_names = re.compile(r'DNS:(?P<name>[^,\s]+)')
 
-    def __init__(self, address, netbios_client=None, dns_client=None, ssh_client=None):
+    def __init__(self, address, *,
+                 netbios_client=None, dns_client=None, ssh_client=None,
+                 per_port_timeout=2.0):
         self.address = address
         self.fingerprints = set()
         self.netbios_client = netbios_client or NetBIOS()
         self.dns_client = dns_client or DNS()
         self.ssh_client = ssh_client or SSH()
+        self.per_port_timeout = per_port_timeout
 
     def add_fingerprint(self, type, value):
         if value:  # Skip empty values from the result
             type = re.sub(r'[^\w+]', '_', type).lower()
             self.fingerprints.add(Fingerprint(type=type, value=value))
 
     async def fingerprint(self):
@@ -90,17 +93,20 @@
         await self._nbt_read_response()
 
     async def _apply_on_open_ports(self, ports, callback):
         rv = []
         for port in ports:
             is_open = await self.is_open(port)
             if is_open:
-                result = await callback(port)
-                if result:
-                    rv = rv + result
+                try:
+                    result = await asyncio.wait_for(callback(port), timeout=self.per_port_timeout)
+                    if result:
+                        rv = rv + result
+                except asyncio.TimeoutError:
+                    pass
 
         return rv
 
     async def _ssl_fingerprint(self, port):
         fingerprint = await self._ssl_process(port, [], ['-fingerprint'])
         if fingerprint:
             fingerprint = fingerprint.strip('\n')
@@ -147,12 +153,12 @@
         writer = None
 
         try:
             future = asyncio.open_connection(self.address, port)
             reader, writer = await asyncio.wait_for(future, timeout=0.5)
 
             return True
-        except:
+        except Exception:
             return False
         finally:
             if writer:
                 writer.close()
```

### Comparing `dab-1.0.0/dab/dns.py` & `dab-1.0.1/dab/dns.py`

 * *Files identical despite different names*

### Comparing `dab-1.0.0/dab/netbios.py` & `dab-1.0.1/dab/netbios.py`

 * *Files identical despite different names*

### Comparing `dab-1.0.0/dab/ssh.py` & `dab-1.0.1/dab/ssh.py`

 * *Files identical despite different names*

