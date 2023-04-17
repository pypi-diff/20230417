# Comparing `tmp/steam-pysigma-2023.4.7.tar.gz` & `tmp/steam-pysigma-2023.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\steam-pysigma-2023.4.7.tar", last modified: Wed Apr 12 08:24:29 2023, max compression
+gzip compressed data, was "dist\steam-pysigma-2023.4.8.tar", last modified: Thu Apr 13 08:17:06 2023, max compression
```

## Comparing `steam-pysigma-2023.4.7.tar` & `steam-pysigma-2023.4.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 08:24:29.961576 steam-pysigma-2023.4.7/
--rw-rw-rw-   0        0        0     1030 2023-04-12 08:24:29.955576 steam-pysigma-2023.4.7/PKG-INFO
--rw-rw-rw-   0        0        0      616 2023-02-22 13:16:40.000000 steam-pysigma-2023.4.7/README.md
--rw-rw-rw-   0        0        0       42 2023-04-12 08:24:29.962577 steam-pysigma-2023.4.7/setup.cfg
--rw-rw-rw-   0        0        0      867 2023-04-12 08:13:33.000000 steam-pysigma-2023.4.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-12 08:24:29.907576 steam-pysigma-2023.4.7/steam_pysigma/
--rw-rw-rw-   0        0        0        0 2023-02-02 13:16:25.000000 steam-pysigma-2023.4.7/steam_pysigma/__init__.py
--rw-rw-rw-   0        0        0    10881 2023-04-05 08:23:05.000000 steam-pysigma-2023.4.7/steam_pysigma/helpers.py
--rw-rw-rw-   0        0        0     8355 2023-04-05 08:56:51.000000 steam-pysigma-2023.4.7/steam_pysigma/pysigma.py
-drwxrwxrwx   0        0        0        0 2023-04-12 08:24:29.952576 steam-pysigma-2023.4.7/steam_pysigma.egg-info/
--rw-rw-rw-   0        0        0     1030 2023-04-12 08:24:29.000000 steam-pysigma-2023.4.7/steam_pysigma.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2023-04-12 08:24:29.000000 steam-pysigma-2023.4.7/steam_pysigma.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 08:24:29.000000 steam-pysigma-2023.4.7/steam_pysigma.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      237 2023-04-12 08:24:29.000000 steam-pysigma-2023.4.7/steam_pysigma.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-12 08:24:29.000000 steam-pysigma-2023.4.7/steam_pysigma.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 08:17:06.453145 steam-pysigma-2023.4.8/
+-rw-rw-rw-   0        0        0     1030 2023-04-13 08:17:06.445145 steam-pysigma-2023.4.8/PKG-INFO
+-rw-rw-rw-   0        0        0      616 2023-02-22 13:16:40.000000 steam-pysigma-2023.4.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-13 08:17:06.453145 steam-pysigma-2023.4.8/setup.cfg
+-rw-rw-rw-   0        0        0      876 2023-04-13 08:14:39.000000 steam-pysigma-2023.4.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 08:17:06.427146 steam-pysigma-2023.4.8/steam_pysigma/
+-rw-rw-rw-   0        0        0        0 2023-02-02 13:16:25.000000 steam-pysigma-2023.4.8/steam_pysigma/__init__.py
+-rw-rw-rw-   0        0        0    10881 2023-04-05 08:23:05.000000 steam-pysigma-2023.4.8/steam_pysigma/helpers.py
+-rw-rw-rw-   0        0        0     8356 2023-04-12 09:10:53.000000 steam-pysigma-2023.4.8/steam_pysigma/pysigma.py
+drwxrwxrwx   0        0        0        0 2023-04-13 08:17:06.443145 steam-pysigma-2023.4.8/steam_pysigma.egg-info/
+-rw-rw-rw-   0        0        0     1030 2023-04-13 08:17:01.000000 steam-pysigma-2023.4.8/steam_pysigma.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2023-04-13 08:17:01.000000 steam-pysigma-2023.4.8/steam_pysigma.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 08:17:01.000000 steam-pysigma-2023.4.8/steam_pysigma.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      237 2023-04-13 08:17:01.000000 steam-pysigma-2023.4.8/steam_pysigma.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-13 08:17:01.000000 steam-pysigma-2023.4.8/steam_pysigma.egg-info/top_level.txt
```

### Comparing `steam-pysigma-2023.4.7/PKG-INFO` & `steam-pysigma-2023.4.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: steam-pysigma
-Version: 2023.4.7
+Version: 2023.4.8
 Summary: This is python wrapper of STEAM SIGMA code
 Home-page: https://gitlab.cern.ch/steam/steam_pysigma
 Author: STEAM Team
 Author-email: steam-team@cern.ch
 License: UNKNOWN
-Keywords: STEAM,CERN,SIGMA
+Keywords: CERN,SIGMA,STEAM
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # STEAM PySIGMA
```

### Comparing `steam-pysigma-2023.4.7/README.md` & `steam-pysigma-2023.4.8/README.md`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.4.7/setup.py` & `steam-pysigma-2023.4.8/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,24 +5,24 @@
     long_description = fh.read()
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='steam-pysigma',
-    version="2023.4.7",
+    version="2023.4.8",
     author="STEAM Team",
     author_email="steam-team@cern.ch",
     description="This is python wrapper of STEAM SIGMA code",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://gitlab.cern.ch/steam/steam_pysigma",
     keywords={'STEAM', 'SIGMA', 'CERN'},
     install_requires=required,
     python_requires='>=3.8',
-    package_data={'': ['steam-sigma.jar']},
+    package_data={'': ['steam-sigma-2023.4.7.jar']},
     include_package_data=True,
     packages=find_packages(exclude=["tests"]),
     classifiers=[
         "Programming Language :: Python :: 3.8"
         ],
 )
```

### Comparing `steam-pysigma-2023.4.7/steam_pysigma/helpers.py` & `steam-pysigma-2023.4.8/steam_pysigma/helpers.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.4.7/steam_pysigma/pysigma.py` & `steam-pysigma-2023.4.8/steam_pysigma/pysigma.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         self.MagnetMPHBuilder = self.gateway.jvm.comsol.MagnetMPHBuilder
         self.QuenchHeaterMPHBuilder = self.gateway.jvm.comsol.QuenchHeaterMPHBuilder
         self.Cable = self.gateway.jvm.model.geometry.coil.Cable
         self.Winding = self.gateway.jvm.model.geometry.coil.Winding
         self.Pole = self.gateway.jvm.model.geometry.coil.Pole
         self.Coil = self.gateway.jvm.model.geometry.coil.Coil
         self.Magnet_T0_QH = self.gateway.jvm.input.OthersT0.Magnet_T0_QH
-        self.Magnet_T1_QH = self.gateway.jvm.input.OthersT0.Magnet_T1_QH
+        #self.Magnet_T1_QH = self.gateway.jvm.input.OthersT0.Magnet_T1_QH
 
         self.StudyAPI = self.gateway.jvm.comsol.api.StudyAPI
         self.ResultsAPI = self.gateway.jvm.comsol.api.ResultsAPI
         self.constants = self.gateway.jvm.comsol.constants.MPHC
     # def __del__(self):
     #     self.gateway.shutdown()
```

### Comparing `steam-pysigma-2023.4.7/steam_pysigma.egg-info/PKG-INFO` & `steam-pysigma-2023.4.8/steam_pysigma.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: steam-pysigma
-Version: 2023.4.7
+Version: 2023.4.8
 Summary: This is python wrapper of STEAM SIGMA code
 Home-page: https://gitlab.cern.ch/steam/steam_pysigma
 Author: STEAM Team
 Author-email: steam-team@cern.ch
 License: UNKNOWN
-Keywords: STEAM,CERN,SIGMA
+Keywords: CERN,SIGMA,STEAM
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # STEAM PySIGMA
```

