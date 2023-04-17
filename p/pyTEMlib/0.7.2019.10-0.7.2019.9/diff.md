# Comparing `tmp/pyTEMlib-0.7.2019.10.tar.gz` & `tmp/pyTEMlib-0.7.2019.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyTEMlib-0.7.2019.10.tar", last modified: Wed Oct 30 20:18:06 2019, max compression
+gzip compressed data, was "dist\pyTEMlib-0.7.2019.9.tar", last modified: Wed Oct 16 20:14:45 2019, max compression
```

## Comparing `pyTEMlib-0.7.2019.10.tar` & `pyTEMlib-0.7.2019.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2019-10-30 20:18:06.000000 pyTEMlib-0.7.2019.10/
--rw-rw-rw-   0        0        0      356 2019-10-30 20:18:06.000000 pyTEMlib-0.7.2019.10/PKG-INFO
--rw-rw-rw-   0        0        0      431 2019-05-14 21:08:55.000000 pyTEMlib-0.7.2019.10/README.md
-drwxrwxrwx   0        0        0        0 2019-10-30 20:18:06.000000 pyTEMlib-0.7.2019.10/pyTEMlib/
--rw-rw-rw-   0        0        0    68860 2019-06-19 23:13:24.000000 pyTEMlib-0.7.2019.10/pyTEMlib/EELS_tools.py
--rw-rw-rw-   0        0        0   114750 2019-07-08 18:31:52.000000 pyTEMlib-0.7.2019.10/pyTEMlib/KinsCat.py
--rw-rw-rw-   0        0        0      192 2019-05-14 21:08:55.000000 pyTEMlib-0.7.2019.10/pyTEMlib/__init__.py
--rw-rw-rw-   0        0        0       55 2019-10-30 20:16:26.000000 pyTEMlib-0.7.2019.10/pyTEMlib/__version__.py
--rw-rw-rw-   0        0        0     5947 2019-05-14 21:08:55.000000 pyTEMlib-0.7.2019.10/pyTEMlib/chksanity.py
--rw-rw-rw-   0        0        0     2305 2019-05-14 21:08:55.000000 pyTEMlib-0.7.2019.10/pyTEMlib/config_dir.py
--rw-rw-rw-   0        0        0     3896 2019-05-14 21:08:55.000000 pyTEMlib-0.7.2019.10/pyTEMlib/defaults_parser.py
--rw-rw-rw-   0        0        0    15319 2019-08-02 19:57:56.000000 pyTEMlib-0.7.2019.10/pyTEMlib/dftregistration.py
--rw-rw-rw-   0        0        0    12944 2019-07-29 18:36:43.000000 pyTEMlib-0.7.2019.10/pyTEMlib/dftregistration2.py
--rw-rw-rw-   0        0        0    26528 2019-09-27 19:39:12.000000 pyTEMlib-0.7.2019.10/pyTEMlib/dm3lib_v1_0b.py
--rw-rw-rw-   0        0        0     2749 2019-05-14 21:08:55.000000 pyTEMlib-0.7.2019.10/pyTEMlib/edges_db.py
--rw-rw-rw-   0        0        0   112723 2019-10-16 21:13:21.000000 pyTEMlib-0.7.2019.10/pyTEMlib/file_tools.py
--rw-rw-rw-   0        0        0    71728 2019-09-18 20:42:17.000000 pyTEMlib-0.7.2019.10/pyTEMlib/image_tools.py
--rw-rw-rw-   0        0        0    74476 2019-05-24 22:12:09.000000 pyTEMlib-0.7.2019.10/pyTEMlib/image_tools1.py
--rw-rw-rw-   0        0        0    11633 2019-05-14 21:08:55.000000 pyTEMlib-0.7.2019.10/pyTEMlib/structure_tools.py
-drwxrwxrwx   0        0        0        0 2019-10-30 20:18:06.000000 pyTEMlib-0.7.2019.10/pyTEMlib.egg-info/
--rw-rw-rw-   0        0        0      356 2019-10-30 20:18:06.000000 pyTEMlib-0.7.2019.10/pyTEMlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      576 2019-10-30 20:18:06.000000 pyTEMlib-0.7.2019.10/pyTEMlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2019-10-30 20:18:06.000000 pyTEMlib-0.7.2019.10/pyTEMlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2019-10-30 20:18:06.000000 pyTEMlib-0.7.2019.10/pyTEMlib.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       50 2019-10-30 20:18:06.000000 pyTEMlib-0.7.2019.10/pyTEMlib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2019-10-30 20:18:06.000000 pyTEMlib-0.7.2019.10/pyTEMlib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2019-10-30 20:18:06.000000 pyTEMlib-0.7.2019.10/setup.cfg
--rw-rw-rw-   0        0        0     1023 2019-10-30 20:16:56.000000 pyTEMlib-0.7.2019.10/setup.py
+drwxrwxrwx   0        0        0        0 2019-10-16 20:14:45.000000 pyTEMlib-0.7.2019.9/
+-rw-rw-rw-   0        0        0      355 2019-10-16 20:14:45.000000 pyTEMlib-0.7.2019.9/PKG-INFO
+-rw-rw-rw-   0        0        0      431 2019-05-14 21:08:55.000000 pyTEMlib-0.7.2019.9/README.md
+drwxrwxrwx   0        0        0        0 2019-10-16 20:14:45.000000 pyTEMlib-0.7.2019.9/pyTEMlib/
+-rw-rw-rw-   0        0        0    68860 2019-06-19 23:13:24.000000 pyTEMlib-0.7.2019.9/pyTEMlib/EELS_tools.py
+-rw-rw-rw-   0        0        0   114750 2019-07-08 18:31:52.000000 pyTEMlib-0.7.2019.9/pyTEMlib/KinsCat.py
+-rw-rw-rw-   0        0        0      192 2019-05-14 21:08:55.000000 pyTEMlib-0.7.2019.9/pyTEMlib/__init__.py
+-rw-rw-rw-   0        0        0       55 2019-10-16 20:14:05.000000 pyTEMlib-0.7.2019.9/pyTEMlib/__version__.py
+-rw-rw-rw-   0        0        0     5947 2019-05-14 21:08:55.000000 pyTEMlib-0.7.2019.9/pyTEMlib/chksanity.py
+-rw-rw-rw-   0        0        0     2305 2019-05-14 21:08:55.000000 pyTEMlib-0.7.2019.9/pyTEMlib/config_dir.py
+-rw-rw-rw-   0        0        0     3896 2019-05-14 21:08:55.000000 pyTEMlib-0.7.2019.9/pyTEMlib/defaults_parser.py
+-rw-rw-rw-   0        0        0    15319 2019-08-02 19:57:56.000000 pyTEMlib-0.7.2019.9/pyTEMlib/dftregistration.py
+-rw-rw-rw-   0        0        0    12944 2019-07-29 18:36:43.000000 pyTEMlib-0.7.2019.9/pyTEMlib/dftregistration2.py
+-rw-rw-rw-   0        0        0    26528 2019-09-27 19:39:12.000000 pyTEMlib-0.7.2019.9/pyTEMlib/dm3lib_v1_0b.py
+-rw-rw-rw-   0        0        0     2749 2019-05-14 21:08:55.000000 pyTEMlib-0.7.2019.9/pyTEMlib/edges_db.py
+-rw-rw-rw-   0        0        0   112650 2019-09-27 15:01:09.000000 pyTEMlib-0.7.2019.9/pyTEMlib/file_tools.py
+-rw-rw-rw-   0        0        0    71728 2019-09-18 20:42:17.000000 pyTEMlib-0.7.2019.9/pyTEMlib/image_tools.py
+-rw-rw-rw-   0        0        0    74476 2019-05-24 22:12:09.000000 pyTEMlib-0.7.2019.9/pyTEMlib/image_tools1.py
+-rw-rw-rw-   0        0        0    11633 2019-05-14 21:08:55.000000 pyTEMlib-0.7.2019.9/pyTEMlib/structure_tools.py
+drwxrwxrwx   0        0        0        0 2019-10-16 20:14:45.000000 pyTEMlib-0.7.2019.9/pyTEMlib.egg-info/
+-rw-rw-rw-   0        0        0      355 2019-10-16 20:14:39.000000 pyTEMlib-0.7.2019.9/pyTEMlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      576 2019-10-16 20:14:40.000000 pyTEMlib-0.7.2019.9/pyTEMlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2019-10-16 20:14:39.000000 pyTEMlib-0.7.2019.9/pyTEMlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2019-10-16 20:14:39.000000 pyTEMlib-0.7.2019.9/pyTEMlib.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       50 2019-10-16 20:14:39.000000 pyTEMlib-0.7.2019.9/pyTEMlib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2019-10-16 20:14:39.000000 pyTEMlib-0.7.2019.9/pyTEMlib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2019-10-16 20:14:45.000000 pyTEMlib-0.7.2019.9/setup.cfg
+-rw-rw-rw-   0        0        0     1022 2019-10-16 20:13:38.000000 pyTEMlib-0.7.2019.9/setup.py
```

### Comparing `pyTEMlib-0.7.2019.10/pyTEMlib/EELS_tools.py` & `pyTEMlib-0.7.2019.9/pyTEMlib/EELS_tools.py`

 * *Files identical despite different names*

### Comparing `pyTEMlib-0.7.2019.10/pyTEMlib/KinsCat.py` & `pyTEMlib-0.7.2019.9/pyTEMlib/KinsCat.py`

 * *Files identical despite different names*

### Comparing `pyTEMlib-0.7.2019.10/pyTEMlib/chksanity.py` & `pyTEMlib-0.7.2019.9/pyTEMlib/chksanity.py`

 * *Files identical despite different names*

### Comparing `pyTEMlib-0.7.2019.10/pyTEMlib/config_dir.py` & `pyTEMlib-0.7.2019.9/pyTEMlib/config_dir.py`

 * *Files identical despite different names*

### Comparing `pyTEMlib-0.7.2019.10/pyTEMlib/defaults_parser.py` & `pyTEMlib-0.7.2019.9/pyTEMlib/defaults_parser.py`

 * *Files identical despite different names*

### Comparing `pyTEMlib-0.7.2019.10/pyTEMlib/dftregistration.py` & `pyTEMlib-0.7.2019.9/pyTEMlib/dftregistration.py`

 * *Files identical despite different names*

### Comparing `pyTEMlib-0.7.2019.10/pyTEMlib/dftregistration2.py` & `pyTEMlib-0.7.2019.9/pyTEMlib/dftregistration2.py`

 * *Files identical despite different names*

### Comparing `pyTEMlib-0.7.2019.10/pyTEMlib/dm3lib_v1_0b.py` & `pyTEMlib-0.7.2019.9/pyTEMlib/dm3lib_v1_0b.py`

 * *Files identical despite different names*

### Comparing `pyTEMlib-0.7.2019.10/pyTEMlib/edges_db.py` & `pyTEMlib-0.7.2019.9/pyTEMlib/edges_db.py`

 * *Files identical despite different names*

### Comparing `pyTEMlib-0.7.2019.10/pyTEMlib/file_tools.py` & `pyTEMlib-0.7.2019.9/pyTEMlib/file_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -1401,21 +1401,20 @@
         if 'ImageScanned' in  key: ## Nion type file read out relevant parameters
             if 'EHT' in key:
                 out_tags['acceleration_voltage'] = float(si.tags[key])
                 if out_tags['acceleration_voltage'] >100000:
                     out_tags['microscope'] = 'UltraSTEM 200'
                 else:
                     out_tags['microscope'] = 'UltraSTEM 100'
-            if 'detector_type' in channel_tags:
-                if 'HAADF' in channel_tags['detector_type']:
-                    if 'PMTDF_gain' in key:
-                        out_tags['detector_gain'] = si.tags[key]
-                else:
-                    if 'PMTBF_gain' in key:
-                        out_tags['detector_gain'] = si.tags[key]
+            if 'HAADF' in channel_tags['detector_type']:
+                if 'PMTDF_gain' in key:
+                    out_tags['detector_gain'] = si.tags[key]
+            else:
+                if 'PMTBF_gain' in key:
+                    out_tags['detector_gain'] = si.tags[key]
             if 'StageOutX' in key:
                 out_tags['stage_x'] =  si.tags[key]
             if 'StageOutY' in key:
                 out_tags['stage_y'] =  si.tags[key]
             if 'StageOutZ' in key:
                 out_tags['stage_z'] =  si.tags[key]
             if 'StageOutA' in key:
```

### Comparing `pyTEMlib-0.7.2019.10/pyTEMlib/image_tools.py` & `pyTEMlib-0.7.2019.9/pyTEMlib/image_tools.py`

 * *Files identical despite different names*

### Comparing `pyTEMlib-0.7.2019.10/pyTEMlib/image_tools1.py` & `pyTEMlib-0.7.2019.9/pyTEMlib/image_tools1.py`

 * *Files identical despite different names*

### Comparing `pyTEMlib-0.7.2019.10/pyTEMlib/structure_tools.py` & `pyTEMlib-0.7.2019.9/pyTEMlib/structure_tools.py`

 * *Files identical despite different names*

### Comparing `pyTEMlib-0.7.2019.10/pyTEMlib.egg-info/SOURCES.txt` & `pyTEMlib-0.7.2019.9/pyTEMlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyTEMlib-0.7.2019.10/setup.py` & `pyTEMlib-0.7.2019.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 with open(os.path.join(here, 'pyTEMlib/__version__.py')) as f:
     __version__ = f.read().split("'")[1]
     
 setuptools.setup(
     name="pyTEMlib",
-    version="0.7.2019.10",
+    version="0.7.2019.9",
     author="Gerd Duscher",
     author_email="gduscher@utk.edu",
     description="pyTEM: TEM Data Quantification library through a Model Based Approach",
     #long_description=open("README.rst").read(),
     url="https://web.utk.edu/~gduscher/Quantifit/",
     packages=["pyTEMlib"],
     package_data={"pyTEMlib": ["data/*"]},
```

