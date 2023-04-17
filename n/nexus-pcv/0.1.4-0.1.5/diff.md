# Comparing `tmp/nexus_pcv-0.1.4.tar.gz` & `tmp/nexus_pcv-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nexus_pcv-0.1.4.tar", max compression
+gzip compressed data, was "nexus_pcv-0.1.5.tar", max compression
```

## Comparing `nexus_pcv-0.1.4.tar` & `nexus_pcv-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    16295 2023-04-09 14:07:25.117517 nexus_pcv-0.1.4/LICENSE
--rw-r--r--   0        0        0     4292 2023-04-09 14:07:25.117517 nexus_pcv-0.1.4/README.md
--rw-r--r--   0        0        0      394 2023-04-09 14:07:25.117517 nexus_pcv-0.1.4/nexus_pcv/__init__.py
--rw-r--r--   0        0        0      169 2023-04-09 14:07:25.117517 nexus_pcv-0.1.4/nexus_pcv/__main__.py
--rw-r--r--   0        0        0     5464 2023-04-09 14:07:25.117517 nexus_pcv-0.1.4/nexus_pcv/apic.py
--rw-r--r--   0        0        0        0 2023-04-09 14:07:25.117517 nexus_pcv-0.1.4/nexus_pcv/cli/__init__.py
--rw-r--r--   0        0        0     2488 2023-04-09 14:07:25.117517 nexus_pcv-0.1.4/nexus_pcv/cli/main.py
--rw-r--r--   0        0        0     4210 2023-04-09 14:07:25.117517 nexus_pcv-0.1.4/nexus_pcv/cli/options.py
--rw-r--r--   0        0        0     5696 2023-04-09 14:07:25.117517 nexus_pcv-0.1.4/nexus_pcv/const.py
--rw-r--r--   0        0        0    11189 2023-04-09 14:07:25.121517 nexus_pcv-0.1.4/nexus_pcv/nae.py
--rw-r--r--   0        0        0     8460 2023-04-09 14:07:25.121517 nexus_pcv-0.1.4/nexus_pcv/ndi.py
--rw-r--r--   0        0        0    10017 2023-04-09 14:07:25.121517 nexus_pcv-0.1.4/nexus_pcv/pcv.py
--rw-r--r--   0        0        0     1914 2023-04-09 14:07:25.121517 nexus_pcv-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     5430 1970-01-01 00:00:00.000000 nexus_pcv-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    16295 2023-04-17 07:02:38.207021 nexus_pcv-0.1.5/LICENSE
+-rw-r--r--   0        0        0     4292 2023-04-17 07:02:38.207021 nexus_pcv-0.1.5/README.md
+-rw-r--r--   0        0        0      394 2023-04-17 07:02:38.207021 nexus_pcv-0.1.5/nexus_pcv/__init__.py
+-rw-r--r--   0        0        0      169 2023-04-17 07:02:38.207021 nexus_pcv-0.1.5/nexus_pcv/__main__.py
+-rw-r--r--   0        0        0     5464 2023-04-17 07:02:38.207021 nexus_pcv-0.1.5/nexus_pcv/apic.py
+-rw-r--r--   0        0        0        0 2023-04-17 07:02:38.207021 nexus_pcv-0.1.5/nexus_pcv/cli/__init__.py
+-rw-r--r--   0        0        0     2488 2023-04-17 07:02:38.207021 nexus_pcv-0.1.5/nexus_pcv/cli/main.py
+-rw-r--r--   0        0        0     4210 2023-04-17 07:02:38.207021 nexus_pcv-0.1.5/nexus_pcv/cli/options.py
+-rw-r--r--   0        0        0     5879 2023-04-17 07:02:38.207021 nexus_pcv-0.1.5/nexus_pcv/const.py
+-rw-r--r--   0        0        0    11189 2023-04-17 07:02:38.207021 nexus_pcv-0.1.5/nexus_pcv/nae.py
+-rw-r--r--   0        0        0     8460 2023-04-17 07:02:38.207021 nexus_pcv-0.1.5/nexus_pcv/ndi.py
+-rw-r--r--   0        0        0    10017 2023-04-17 07:02:38.207021 nexus_pcv-0.1.5/nexus_pcv/pcv.py
+-rw-r--r--   0        0        0     1914 2023-04-17 07:02:38.207021 nexus_pcv-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     5430 1970-01-01 00:00:00.000000 nexus_pcv-0.1.5/PKG-INFO
```

### Comparing `nexus_pcv-0.1.4/LICENSE` & `nexus_pcv-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nexus_pcv-0.1.4/README.md` & `nexus_pcv-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `nexus_pcv-0.1.4/nexus_pcv/apic.py` & `nexus_pcv-0.1.5/nexus_pcv/apic.py`

 * *Files identical despite different names*

### Comparing `nexus_pcv-0.1.4/nexus_pcv/cli/main.py` & `nexus_pcv-0.1.5/nexus_pcv/cli/main.py`

 * *Files identical despite different names*

### Comparing `nexus_pcv-0.1.4/nexus_pcv/cli/options.py` & `nexus_pcv-0.1.5/nexus_pcv/cli/options.py`

 * *Files identical despite different names*

### Comparing `nexus_pcv-0.1.4/nexus_pcv/const.py` & `nexus_pcv-0.1.5/nexus_pcv/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,8 +273,17 @@
         "keys": [
             {
                 "attribute": "name",
                 "regex": ".*",
             }
         ],
     },
+    "format": {
+        "class": "datetimeFormat",
+        "keys": [
+            {
+                "attribute": "name",
+                "regex": ".*",
+            }
+        ],
+    },
 }
```

### Comparing `nexus_pcv-0.1.4/nexus_pcv/nae.py` & `nexus_pcv-0.1.5/nexus_pcv/nae.py`

 * *Files identical despite different names*

### Comparing `nexus_pcv-0.1.4/nexus_pcv/ndi.py` & `nexus_pcv-0.1.5/nexus_pcv/ndi.py`

 * *Files identical despite different names*

### Comparing `nexus_pcv-0.1.4/nexus_pcv/pcv.py` & `nexus_pcv-0.1.5/nexus_pcv/pcv.py`

 * *Files identical despite different names*

### Comparing `nexus_pcv-0.1.4/pyproject.toml` & `nexus_pcv-0.1.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 documentation = "https://github.com/netascode/nexus-pcv"
 homepage = "https://github.com/netascode/nexus-pcv"
 license = "LICENSE"
 maintainers = ["Daniel Schmidt <danischm@cisco.com>"]
 name = "nexus-pcv"
 readme = "README.md"
 repository = "https://github.com/netascode/nexus-pcv"
-version = "0.1.4"
+version = "0.1.5"
 
 [tool.poetry.scripts]
 nexus-pcv = "nexus_pcv.cli.main:main"
 
 [tool.poetry.dependencies]
 click = "^8.1.3"
 errorhandler = "^2.0.1"
```

### Comparing `nexus_pcv-0.1.4/PKG-INFO` & `nexus_pcv-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexus-pcv
-Version: 0.1.4
+Version: 0.1.5
 Summary: A CLI tool to perform a pre-change validation on Nexus Dashboard Insights or Network Assurance Engine.
 Home-page: https://github.com/netascode/nexus-pcv
 License: LICENSE
 Author: Daniel Schmidt
 Author-email: danischm@cisco.com
 Maintainer: Daniel Schmidt
 Maintainer-email: danischm@cisco.com
```

