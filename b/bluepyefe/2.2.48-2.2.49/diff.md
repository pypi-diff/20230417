# Comparing `tmp/bluepyefe-2.2.48.tar.gz` & `tmp/bluepyefe-2.2.49.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluepyefe-2.2.48.tar", last modified: Fri Apr 14 15:12:48 2023, max compression
+gzip compressed data, was "bluepyefe-2.2.49.tar", last modified: Mon Apr 17 07:29:53 2023, max compression
```

## Comparing `bluepyefe-2.2.48.tar` & `bluepyefe-2.2.49.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:12:48.092910 bluepyefe-2.2.48/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-14 15:12:45.000000 bluepyefe-2.2.48/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-14 15:12:45.000000 bluepyefe-2.2.48/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-14 15:12:45.000000 bluepyefe-2.2.48/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-14 15:12:48.092910 bluepyefe-2.2.48/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-04-14 15:12:45.000000 bluepyefe-2.2.48/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:12:48.092910 bluepyefe-2.2.48/bluepyefe/
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-14 15:12:45.000000 bluepyefe-2.2.48/bluepyefe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-14 15:12:48.092910 bluepyefe-2.2.48/bluepyefe/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-04-14 15:12:45.000000 bluepyefe-2.2.48/bluepyefe/auto_targets.py
--rw-r--r--   0 runner    (1001) docker     (123)     9582 2023-04-14 15:12:45.000000 bluepyefe-2.2.48/bluepyefe/cell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:12:48.092910 bluepyefe-2.2.48/bluepyefe/ecode/
--rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-04-14 15:12:45.000000 bluepyefe-2.2.48/bluepyefe/ecode/DeHyperPol.py
--rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-04-14 15:12:45.000000 bluepyefe-2.2.48/bluepyefe/ecode/HyperDePol.py
--rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-04-14 15:12:45.000000 bluepyefe-2.2.48/bluepyefe/ecode/SpikeRec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-04-14 15:12:45.000000 bluepyefe-2.2.48/bluepyefe/ecode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-04-14 15:12:45.000000 bluepyefe-2.2.48/bluepyefe/ecode/negCheops.py
--rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-04-14 15:12:45.000000 bluepyefe-2.2.48/bluepyefe/ecode/posCheops.py
--rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-04-14 15:12:45.000000 bluepyefe-2.2.48/bluepyefe/ecode/ramp.py
--rw-r--r--   0 runner    (1001) docker     (123)     9741 2023-04-14 15:12:45.000000 bluepyefe-2.2.48/bluepyefe/ecode/sAHP.py
--rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-04-14 15:12:45.000000 bluepyefe-2.2.48/bluepyefe/ecode/sineSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-04-14 15:12:45.000000 bluepyefe-2.2.48/bluepyefe/ecode/step.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-14 15:12:45.000000 bluepyefe-2.2.48/bluepyefe/ecode/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    34969 2023-04-14 15:12:45.000000 bluepyefe-2.2.48/bluepyefe/extract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:12:48.092910 bluepyefe-2.2.48/bluepyefe/igorpy/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3976 2023-04-14 15:12:45.000000 bluepyefe-2.2.48/bluepyefe/igorpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9498 2023-04-14 15:12:45.000000 bluepyefe-2.2.48/bluepyefe/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-04-14 15:12:45.000000 bluepyefe-2.2.48/bluepyefe/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)    10086 2023-04-14 15:12:45.000000 bluepyefe-2.2.48/bluepyefe/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    15562 2023-04-14 15:12:45.000000 bluepyefe-2.2.48/bluepyefe/recording.py
--rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-04-14 15:12:45.000000 bluepyefe-2.2.48/bluepyefe/rheobase.py
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-04-14 15:12:45.000000 bluepyefe-2.2.48/bluepyefe/target.py
--rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-04-14 15:12:45.000000 bluepyefe-2.2.48/bluepyefe/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-04-14 15:12:45.000000 bluepyefe-2.2.48/bluepyefe/translate_legacy_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:12:48.088910 bluepyefe-2.2.48/bluepyefe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-14 15:12:48.000000 bluepyefe-2.2.48/bluepyefe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-14 15:12:48.000000 bluepyefe-2.2.48/bluepyefe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 15:12:48.000000 bluepyefe-2.2.48/bluepyefe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-14 15:12:48.000000 bluepyefe-2.2.48/bluepyefe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-14 15:12:48.000000 bluepyefe-2.2.48/bluepyefe.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:12:48.092910 bluepyefe-2.2.48/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-14 15:12:45.000000 bluepyefe-2.2.48/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-14 15:12:48.092910 bluepyefe-2.2.48/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-04-14 15:12:45.000000 bluepyefe-2.2.48/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    69513 2023-04-14 15:12:45.000000 bluepyefe-2.2.48/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:29:53.348635 bluepyefe-2.2.49/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-17 07:29:45.000000 bluepyefe-2.2.49/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-17 07:29:45.000000 bluepyefe-2.2.49/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-17 07:29:45.000000 bluepyefe-2.2.49/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-17 07:29:53.348635 bluepyefe-2.2.49/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-04-17 07:29:45.000000 bluepyefe-2.2.49/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:29:53.348635 bluepyefe-2.2.49/bluepyefe/
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-17 07:29:45.000000 bluepyefe-2.2.49/bluepyefe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-17 07:29:53.348635 bluepyefe-2.2.49/bluepyefe/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-04-17 07:29:45.000000 bluepyefe-2.2.49/bluepyefe/auto_targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9582 2023-04-17 07:29:45.000000 bluepyefe-2.2.49/bluepyefe/cell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:29:53.348635 bluepyefe-2.2.49/bluepyefe/ecode/
+-rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-04-17 07:29:45.000000 bluepyefe-2.2.49/bluepyefe/ecode/DeHyperPol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-04-17 07:29:45.000000 bluepyefe-2.2.49/bluepyefe/ecode/HyperDePol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-04-17 07:29:45.000000 bluepyefe-2.2.49/bluepyefe/ecode/SpikeRec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-04-17 07:29:45.000000 bluepyefe-2.2.49/bluepyefe/ecode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-04-17 07:29:45.000000 bluepyefe-2.2.49/bluepyefe/ecode/negCheops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-04-17 07:29:45.000000 bluepyefe-2.2.49/bluepyefe/ecode/posCheops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-04-17 07:29:45.000000 bluepyefe-2.2.49/bluepyefe/ecode/ramp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9741 2023-04-17 07:29:45.000000 bluepyefe-2.2.49/bluepyefe/ecode/sAHP.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-04-17 07:29:45.000000 bluepyefe-2.2.49/bluepyefe/ecode/sineSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-04-17 07:29:45.000000 bluepyefe-2.2.49/bluepyefe/ecode/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-17 07:29:45.000000 bluepyefe-2.2.49/bluepyefe/ecode/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34969 2023-04-17 07:29:45.000000 bluepyefe-2.2.49/bluepyefe/extract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:29:53.348635 bluepyefe-2.2.49/bluepyefe/igorpy/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3976 2023-04-17 07:29:45.000000 bluepyefe-2.2.49/bluepyefe/igorpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9498 2023-04-17 07:29:45.000000 bluepyefe-2.2.49/bluepyefe/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-04-17 07:29:45.000000 bluepyefe-2.2.49/bluepyefe/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10064 2023-04-17 07:29:45.000000 bluepyefe-2.2.49/bluepyefe/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15562 2023-04-17 07:29:45.000000 bluepyefe-2.2.49/bluepyefe/recording.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-04-17 07:29:45.000000 bluepyefe-2.2.49/bluepyefe/rheobase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-04-17 07:29:45.000000 bluepyefe-2.2.49/bluepyefe/target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-04-17 07:29:45.000000 bluepyefe-2.2.49/bluepyefe/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-04-17 07:29:45.000000 bluepyefe-2.2.49/bluepyefe/translate_legacy_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:29:53.348635 bluepyefe-2.2.49/bluepyefe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-17 07:29:53.000000 bluepyefe-2.2.49/bluepyefe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-17 07:29:53.000000 bluepyefe-2.2.49/bluepyefe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 07:29:53.000000 bluepyefe-2.2.49/bluepyefe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-17 07:29:53.000000 bluepyefe-2.2.49/bluepyefe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-17 07:29:53.000000 bluepyefe-2.2.49/bluepyefe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:29:53.348635 bluepyefe-2.2.49/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-17 07:29:45.000000 bluepyefe-2.2.49/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-17 07:29:53.348635 bluepyefe-2.2.49/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-04-17 07:29:45.000000 bluepyefe-2.2.49/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69513 2023-04-17 07:29:45.000000 bluepyefe-2.2.49/versioneer.py
```

### Comparing `bluepyefe-2.2.48/LICENSE.txt` & `bluepyefe-2.2.49/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.48/PKG-INFO` & `bluepyefe-2.2.49/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: bluepyefe
-Version: 2.2.48
+Version: 2.2.49
 Summary: Blue Brain Python E-feature extraction
 Home-page: https://github.com/BlueBrain/BluePyEfe
 Author: BlueBrain Project, EPFL
 License: LGPLv3
 Description: The Blue Brain Python E-feature extraction Library (BluePyEfe) aims at easing the process of reading experimental recordings and extracting batches of electrical features from them. To do so, it combines trace reading functions and features extraction functions from the eFel library. BluePyEfe outputs protocols and features files in a format that can then be used by BluePyOpt for electrical model building purposes.
 Keywords: neuroscience,BlueBrainProject
 Platform: UNKNOWN
```

### Comparing `bluepyefe-2.2.48/README.md` & `bluepyefe-2.2.49/README.md`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.48/bluepyefe/__init__.py` & `bluepyefe-2.2.49/bluepyefe/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.48/bluepyefe/auto_targets.py` & `bluepyefe-2.2.49/bluepyefe/auto_targets.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.48/bluepyefe/cell.py` & `bluepyefe-2.2.49/bluepyefe/cell.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.48/bluepyefe/ecode/DeHyperPol.py` & `bluepyefe-2.2.49/bluepyefe/ecode/DeHyperPol.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.48/bluepyefe/ecode/HyperDePol.py` & `bluepyefe-2.2.49/bluepyefe/ecode/HyperDePol.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.48/bluepyefe/ecode/SpikeRec.py` & `bluepyefe-2.2.49/bluepyefe/ecode/SpikeRec.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.48/bluepyefe/ecode/__init__.py` & `bluepyefe-2.2.49/bluepyefe/ecode/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.48/bluepyefe/ecode/negCheops.py` & `bluepyefe-2.2.49/bluepyefe/ecode/negCheops.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.48/bluepyefe/ecode/posCheops.py` & `bluepyefe-2.2.49/bluepyefe/ecode/posCheops.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.48/bluepyefe/ecode/ramp.py` & `bluepyefe-2.2.49/bluepyefe/ecode/ramp.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.48/bluepyefe/ecode/sAHP.py` & `bluepyefe-2.2.49/bluepyefe/ecode/sAHP.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.48/bluepyefe/ecode/sineSpec.py` & `bluepyefe-2.2.49/bluepyefe/ecode/sineSpec.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.48/bluepyefe/ecode/step.py` & `bluepyefe-2.2.49/bluepyefe/ecode/step.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.48/bluepyefe/ecode/tools.py` & `bluepyefe-2.2.49/bluepyefe/ecode/tools.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.48/bluepyefe/extract.py` & `bluepyefe-2.2.49/bluepyefe/extract.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.48/bluepyefe/igorpy/__init__.py` & `bluepyefe-2.2.49/bluepyefe/igorpy/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.48/bluepyefe/plotting.py` & `bluepyefe-2.2.49/bluepyefe/plotting.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.48/bluepyefe/protocol.py` & `bluepyefe-2.2.49/bluepyefe/protocol.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.48/bluepyefe/reader.py` & `bluepyefe-2.2.49/bluepyefe/reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,15 +116,15 @@
         voltage, current = current, voltage
         notes_v, notes_i = notes_i, notes_v
 
     # Extract data
     trace_data = {}
     trace_data["voltage"] = numpy.asarray(voltage)
     trace_data["v_unit"] = str(notes_v.dUnits).replace(" ", "")
-    trace_data["dt"] = str(notes_v.dx).replace(" ", "")
+    trace_data["dt"] = notes_v.dx
     trace_data["current"] = numpy.asarray(current)
     trace_data["i_unit"] = str(notes_i.dUnits).replace(" ", "")
 
     return [trace_data]
 
 
 def read_matlab(in_data):
```

### Comparing `bluepyefe-2.2.48/bluepyefe/recording.py` & `bluepyefe-2.2.49/bluepyefe/recording.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.48/bluepyefe/rheobase.py` & `bluepyefe-2.2.49/bluepyefe/rheobase.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.48/bluepyefe/target.py` & `bluepyefe-2.2.49/bluepyefe/target.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.48/bluepyefe/tools.py` & `bluepyefe-2.2.49/bluepyefe/tools.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.48/bluepyefe/translate_legacy_config.py` & `bluepyefe-2.2.49/bluepyefe/translate_legacy_config.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.48/bluepyefe.egg-info/PKG-INFO` & `bluepyefe-2.2.49/bluepyefe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: bluepyefe
-Version: 2.2.48
+Version: 2.2.49
 Summary: Blue Brain Python E-feature extraction
 Home-page: https://github.com/BlueBrain/BluePyEfe
 Author: BlueBrain Project, EPFL
 License: LGPLv3
 Description: The Blue Brain Python E-feature extraction Library (BluePyEfe) aims at easing the process of reading experimental recordings and extracting batches of electrical features from them. To do so, it combines trace reading functions and features extraction functions from the eFel library. BluePyEfe outputs protocols and features files in a format that can then be used by BluePyOpt for electrical model building purposes.
 Keywords: neuroscience,BlueBrainProject
 Platform: UNKNOWN
```

### Comparing `bluepyefe-2.2.48/bluepyefe.egg-info/SOURCES.txt` & `bluepyefe-2.2.49/bluepyefe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.48/examples/__init__.py` & `bluepyefe-2.2.49/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.48/setup.py` & `bluepyefe-2.2.49/setup.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.48/versioneer.py` & `bluepyefe-2.2.49/versioneer.py`

 * *Files identical despite different names*

