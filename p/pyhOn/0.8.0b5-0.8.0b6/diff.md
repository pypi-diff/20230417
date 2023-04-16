# Comparing `tmp/pyhOn-0.8.0b5.tar.gz` & `tmp/pyhOn-0.8.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhOn-0.8.0b5.tar", last modified: Sun Apr 16 11:59:58 2023, max compression
+gzip compressed data, was "pyhOn-0.8.0b6.tar", last modified: Sun Apr 16 22:11:10 2023, max compression
```

## Comparing `pyhOn-0.8.0b5.tar` & `pyhOn-0.8.0b6.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:59:58.600005 pyhOn-0.8.0b5/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-04-16 11:59:58.600005 pyhOn-0.8.0b5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:59:58.596005 pyhOn-0.8.0b5/pyhOn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-04-16 11:59:58.000000 pyhOn-0.8.0b5/pyhOn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-16 11:59:58.000000 pyhOn-0.8.0b5/pyhOn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 11:59:58.000000 pyhOn-0.8.0b5/pyhOn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-16 11:59:58.000000 pyhOn-0.8.0b5/pyhOn.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-16 11:59:58.000000 pyhOn-0.8.0b5/pyhOn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-16 11:59:58.000000 pyhOn-0.8.0b5/pyhOn.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:59:58.596005 pyhOn-0.8.0b5/pyhon/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/pyhon/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3251 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/pyhon/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/pyhon/appliance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:59:58.596005 pyhOn-0.8.0b5/pyhon/appliances/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/pyhon/appliances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/pyhon/appliances/dw.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/pyhon/appliances/td.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/pyhon/appliances/wd.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/pyhon/appliances/wm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/pyhon/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:59:58.596005 pyhOn-0.8.0b5/pyhon/connection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/pyhon/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/pyhon/connection/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10539 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/pyhon/connection/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/pyhon/connection/device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:59:58.596005 pyhOn-0.8.0b5/pyhon/connection/handler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/pyhon/connection/handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/pyhon/connection/handler/anonym.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/pyhon/connection/handler/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/pyhon/connection/handler/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/pyhon/connection/handler/hon.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/pyhon/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/pyhon/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/pyhon/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/pyhon/hon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:59:58.600005 pyhOn-0.8.0b5/pyhon/parameter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/pyhon/parameter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/pyhon/parameter/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/pyhon/parameter/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/pyhon/parameter/fixed.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/pyhon/parameter/program.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/pyhon/parameter/range.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 11:59:58.600005 pyhOn-0.8.0b5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-16 11:59:47.000000 pyhOn-0.8.0b5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:11:10.256554 pyhOn-0.8.0b6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-16 22:10:55.000000 pyhOn-0.8.0b6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-04-16 22:11:10.256554 pyhOn-0.8.0b6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-04-16 22:10:55.000000 pyhOn-0.8.0b6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:11:10.252554 pyhOn-0.8.0b6/pyhOn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-04-16 22:11:10.000000 pyhOn-0.8.0b6/pyhOn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-16 22:11:10.000000 pyhOn-0.8.0b6/pyhOn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 22:11:10.000000 pyhOn-0.8.0b6/pyhOn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-16 22:11:10.000000 pyhOn-0.8.0b6/pyhOn.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-16 22:11:10.000000 pyhOn-0.8.0b6/pyhOn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-16 22:11:10.000000 pyhOn-0.8.0b6/pyhOn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:11:10.256554 pyhOn-0.8.0b6/pyhon/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-16 22:10:55.000000 pyhOn-0.8.0b6/pyhon/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3251 2023-04-16 22:10:55.000000 pyhOn-0.8.0b6/pyhon/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-04-16 22:10:55.000000 pyhOn-0.8.0b6/pyhon/appliance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:11:10.256554 pyhOn-0.8.0b6/pyhon/appliances/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 22:10:55.000000 pyhOn-0.8.0b6/pyhon/appliances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-16 22:10:55.000000 pyhOn-0.8.0b6/pyhon/appliances/dw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-16 22:10:55.000000 pyhOn-0.8.0b6/pyhon/appliances/td.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-16 22:10:55.000000 pyhOn-0.8.0b6/pyhon/appliances/wd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-16 22:10:55.000000 pyhOn-0.8.0b6/pyhon/appliances/wm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-04-16 22:10:55.000000 pyhOn-0.8.0b6/pyhon/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:11:10.256554 pyhOn-0.8.0b6/pyhon/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 22:10:55.000000 pyhOn-0.8.0b6/pyhon/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-04-16 22:10:55.000000 pyhOn-0.8.0b6/pyhon/connection/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10539 2023-04-16 22:10:55.000000 pyhOn-0.8.0b6/pyhon/connection/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-16 22:10:55.000000 pyhOn-0.8.0b6/pyhon/connection/device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:11:10.256554 pyhOn-0.8.0b6/pyhon/connection/handler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 22:10:55.000000 pyhOn-0.8.0b6/pyhon/connection/handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-16 22:10:55.000000 pyhOn-0.8.0b6/pyhon/connection/handler/anonym.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-16 22:10:55.000000 pyhOn-0.8.0b6/pyhon/connection/handler/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-04-16 22:10:55.000000 pyhOn-0.8.0b6/pyhon/connection/handler/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-04-16 22:10:55.000000 pyhOn-0.8.0b6/pyhon/connection/handler/hon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-16 22:10:55.000000 pyhOn-0.8.0b6/pyhon/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-16 22:10:55.000000 pyhOn-0.8.0b6/pyhon/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-04-16 22:10:55.000000 pyhOn-0.8.0b6/pyhon/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-04-16 22:10:55.000000 pyhOn-0.8.0b6/pyhon/hon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:11:10.256554 pyhOn-0.8.0b6/pyhon/parameter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 22:10:55.000000 pyhOn-0.8.0b6/pyhon/parameter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-16 22:10:55.000000 pyhOn-0.8.0b6/pyhon/parameter/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-04-16 22:10:55.000000 pyhOn-0.8.0b6/pyhon/parameter/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-16 22:10:55.000000 pyhOn-0.8.0b6/pyhon/parameter/fixed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-16 22:10:55.000000 pyhOn-0.8.0b6/pyhon/parameter/program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-16 22:10:55.000000 pyhOn-0.8.0b6/pyhon/parameter/range.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 22:11:10.256554 pyhOn-0.8.0b6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-16 22:10:55.000000 pyhOn-0.8.0b6/setup.py
```

### Comparing `pyhOn-0.8.0b5/LICENSE` & `pyhOn-0.8.0b6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.0b5/PKG-INFO` & `pyhOn-0.8.0b6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhOn
-Version: 0.8.0b5
+Version: 0.8.0b6
 Summary: Control hOn devices with python
 Author: Andre Basche
 License: MIT
 Project-URL: GitHub, https://github.com/Andre0512/pyhOn
 Project-URL: PyPI, https://pypi.org/project/pyhOn
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyhOn-0.8.0b5/README.md` & `pyhOn-0.8.0b6/README.md`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.0b5/pyhOn.egg-info/PKG-INFO` & `pyhOn-0.8.0b6/pyhOn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhOn
-Version: 0.8.0b5
+Version: 0.8.0b6
 Summary: Control hOn devices with python
 Author: Andre Basche
 License: MIT
 Project-URL: GitHub, https://github.com/Andre0512/pyhOn
 Project-URL: PyPI, https://pypi.org/project/pyhOn
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyhOn-0.8.0b5/pyhOn.egg-info/SOURCES.txt` & `pyhOn-0.8.0b6/pyhOn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.0b5/pyhon/__main__.py` & `pyhOn-0.8.0b6/pyhon/__main__.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.0b5/pyhon/appliance.py` & `pyhOn-0.8.0b6/pyhon/appliance.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.0b5/pyhon/commands.py` & `pyhOn-0.8.0b6/pyhon/commands.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,19 +58,18 @@
         return self._parameters
 
     @property
     def ancillary_parameters(self) -> Dict[str, HonParameter]:
         return self._ancillary_parameters
 
     async def send(self) -> bool:
-        parameters = {
-            name: parameter.value for name, parameter in self._parameters.items()
-        }
+        params = {k: v.value for k, v in self._parameters.items()}
+        ancillary_params = {k: v.value for k, v in self._ancillary_parameters.items()}
         return await self._api.send_command(
-            self._appliance, self._name, parameters, self.ancillary_parameters
+            self._appliance, self._name, params, ancillary_params
         )
 
     @property
     def programs(self) -> Dict[str, "HonCommand"]:
         if self._programs is None:
             return {}
         return self._programs
```

### Comparing `pyhOn-0.8.0b5/pyhon/connection/api.py` & `pyhOn-0.8.0b6/pyhon/connection/api.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.0b5/pyhon/connection/auth.py` & `pyhOn-0.8.0b6/pyhon/connection/auth.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.0b5/pyhon/connection/device.py` & `pyhOn-0.8.0b6/pyhon/connection/device.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.0b5/pyhon/connection/handler/anonym.py` & `pyhOn-0.8.0b6/pyhon/connection/handler/anonym.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.0b5/pyhon/connection/handler/auth.py` & `pyhOn-0.8.0b6/pyhon/connection/handler/auth.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.0b5/pyhon/connection/handler/base.py` & `pyhOn-0.8.0b6/pyhon/connection/handler/base.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.0b5/pyhon/connection/handler/hon.py` & `pyhOn-0.8.0b6/pyhon/connection/handler/hon.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.0b5/pyhon/helper.py` & `pyhOn-0.8.0b6/pyhon/helper.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.0b5/pyhon/hon.py` & `pyhOn-0.8.0b6/pyhon/hon.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.0b5/pyhon/parameter/base.py` & `pyhOn-0.8.0b6/pyhon/parameter/base.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.0b5/pyhon/parameter/enum.py` & `pyhOn-0.8.0b6/pyhon/parameter/enum.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.0b5/pyhon/parameter/fixed.py` & `pyhOn-0.8.0b6/pyhon/parameter/fixed.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.0b5/pyhon/parameter/program.py` & `pyhOn-0.8.0b6/pyhon/parameter/program.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.0b5/pyhon/parameter/range.py` & `pyhOn-0.8.0b6/pyhon/parameter/range.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.0b5/setup.py` & `pyhOn-0.8.0b6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="pyhOn",
-    version="0.8.0b5",
+    version="0.8.0b6",
     author="Andre Basche",
     description="Control hOn devices with python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     project_urls={
         "GitHub": "https://github.com/Andre0512/pyhOn",
         "PyPI": "https://pypi.org/project/pyhOn",
```

