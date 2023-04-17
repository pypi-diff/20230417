# Comparing `tmp/enstools-compression-2023.1.tar.gz` & `tmp/enstools-compression-2023.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enstools-compression-2023.1.tar", last modified: Wed Jan 18 17:53:24 2023, max compression
+gzip compressed data, was "enstools-compression-2023.4.1.tar", last modified: Mon Apr 17 16:08:59 2023, max compression
```

## Comparing `enstools-compression-2023.1.tar` & `enstools-compression-2023.4.1.tar`

### file list

```diff
@@ -1,42 +1,44 @@
-drwxr-xr-x   0 oriol.tinto (24207) ls-craig (11075)        0 2023-01-18 17:53:24.000000 enstools-compression-2023.1/
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)    10898 2023-01-18 17:53:22.000000 enstools-compression-2023.1/LICENSE
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)       15 2023-01-18 17:53:22.000000 enstools-compression-2023.1/MANIFEST.in
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     1660 2023-01-18 17:53:24.000000 enstools-compression-2023.1/PKG-INFO
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     1412 2023-01-18 17:53:22.000000 enstools-compression-2023.1/README.md
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)        7 2023-01-18 17:53:22.000000 enstools-compression-2023.1/VERSION
-drwxr-xr-x   0 oriol.tinto (24207) ls-craig (11075)        0 2023-01-18 17:53:24.000000 enstools-compression-2023.1/enstools/
-drwxr-xr-x   0 oriol.tinto (24207) ls-craig (11075)        0 2023-01-18 17:53:24.000000 enstools-compression-2023.1/enstools/compression/
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)      444 2023-01-18 17:53:22.000000 enstools-compression-2023.1/enstools/compression/__init__.py
-drwxr-xr-x   0 oriol.tinto (24207) ls-craig (11075)        0 2023-01-18 17:53:24.000000 enstools-compression-2023.1/enstools/compression/analyzer/
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     3099 2023-01-18 17:53:22.000000 enstools-compression-2023.1/enstools/compression/analyzer/AnalysisOptions.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)       53 2023-01-18 17:53:22.000000 enstools-compression-2023.1/enstools/compression/analyzer/__init__.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     6293 2023-01-18 17:53:22.000000 enstools-compression-2023.1/enstools/compression/analyzer/analyze_data_array.py
--rwxr-xr-x   0 oriol.tinto (24207) ls-craig (11075)    10373 2023-01-18 17:53:22.000000 enstools-compression-2023.1/enstools/compression/analyzer/analyzer.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     8194 2023-01-18 17:53:22.000000 enstools-compression-2023.1/enstools/compression/analyzer/analyzer_utils.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)      344 2023-01-18 17:53:22.000000 enstools-compression-2023.1/enstools/compression/api.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)    16861 2023-01-18 17:53:22.000000 enstools-compression-2023.1/enstools/compression/cli.py
--rwxr-xr-x   0 oriol.tinto (24207) ls-craig (11075)    11172 2023-01-18 17:53:22.000000 enstools-compression-2023.1/enstools/compression/compressor.py
--rwxr-xr-x   0 oriol.tinto (24207) ls-craig (11075)     3354 2023-01-18 17:53:22.000000 enstools-compression-2023.1/enstools/compression/emulation.py
-drwxr-xr-x   0 oriol.tinto (24207) ls-craig (11075)        0 2023-01-18 17:53:24.000000 enstools-compression-2023.1/enstools/compression/emulators/
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     1188 2023-01-18 17:53:22.000000 enstools-compression-2023.1/enstools/compression/emulators/EmulatorClass.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     2353 2023-01-18 17:53:22.000000 enstools-compression-2023.1/enstools/compression/emulators/FiltersEmulator.py
--rwxr-xr-x   0 oriol.tinto (24207) ls-craig (11075)     2885 2023-01-18 17:53:22.000000 enstools-compression-2023.1/enstools/compression/emulators/LibpressioEmulator.py
--rwxr-xr-x   0 oriol.tinto (24207) ls-craig (11075)     2036 2023-01-18 17:53:22.000000 enstools-compression-2023.1/enstools/compression/emulators/ZFPEmulator.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)      197 2023-01-18 17:53:22.000000 enstools-compression-2023.1/enstools/compression/emulators/__init__.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     2715 2023-01-18 17:53:22.000000 enstools-compression-2023.1/enstools/compression/evaluator.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)    11156 2023-01-18 17:53:22.000000 enstools-compression-2023.1/enstools/compression/metrics.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     4557 2023-01-18 17:53:22.000000 enstools-compression-2023.1/enstools/compression/pruner.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)    10801 2023-01-18 17:53:22.000000 enstools-compression-2023.1/enstools/compression/significant_bits.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)      910 2023-01-18 17:53:22.000000 enstools-compression-2023.1/enstools/compression/size_metrics.py
-drwxr-xr-x   0 oriol.tinto (24207) ls-craig (11075)        0 2023-01-18 17:53:24.000000 enstools-compression-2023.1/enstools/compression/xr_accessor/
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)       23 2023-01-18 17:53:22.000000 enstools-compression-2023.1/enstools/compression/xr_accessor/__init__.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     5314 2023-01-18 17:53:22.000000 enstools-compression-2023.1/enstools/compression/xr_accessor/accessor.py
-drwxr-xr-x   0 oriol.tinto (24207) ls-craig (11075)        0 2023-01-18 17:53:24.000000 enstools-compression-2023.1/enstools_compression.egg-info/
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     1660 2023-01-18 17:53:24.000000 enstools-compression-2023.1/enstools_compression.egg-info/PKG-INFO
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     1208 2023-01-18 17:53:24.000000 enstools-compression-2023.1/enstools_compression.egg-info/SOURCES.txt
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)        1 2023-01-18 17:53:24.000000 enstools-compression-2023.1/enstools_compression.egg-info/dependency_links.txt
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)       71 2023-01-18 17:53:24.000000 enstools-compression-2023.1/enstools_compression.egg-info/entry_points.txt
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)       74 2023-01-18 17:53:24.000000 enstools-compression-2023.1/enstools_compression.egg-info/requires.txt
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)        9 2023-01-18 17:53:24.000000 enstools-compression-2023.1/enstools_compression.egg-info/top_level.txt
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)       38 2023-01-18 17:53:24.000000 enstools-compression-2023.1/setup.cfg
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     1366 2023-01-18 17:53:22.000000 enstools-compression-2023.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:08:59.975639 enstools-compression-2023.4.1/
+-rw-rw-rw-   0 root         (0) root         (0)    10898 2023-01-18 16:33:07.000000 enstools-compression-2023.4.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       15 2023-01-18 16:33:07.000000 enstools-compression-2023.4.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1662 2023-04-17 16:08:59.975639 enstools-compression-2023.4.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1412 2023-01-18 16:33:07.000000 enstools-compression-2023.4.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        9 2023-04-17 15:51:33.000000 enstools-compression-2023.4.1/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:08:59.971639 enstools-compression-2023.4.1/enstools/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:08:59.973639 enstools-compression-2023.4.1/enstools/compression/
+-rw-rw-rw-   0 root         (0) root         (0)      444 2023-01-18 16:33:07.000000 enstools-compression-2023.4.1/enstools/compression/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:08:59.973639 enstools-compression-2023.4.1/enstools/compression/analyzer/
+-rw-rw-rw-   0 root         (0) root         (0)     3099 2023-01-18 16:33:07.000000 enstools-compression-2023.4.1/enstools/compression/analyzer/AnalysisOptions.py
+-rw-rw-rw-   0 root         (0) root         (0)       53 2023-01-18 16:33:07.000000 enstools-compression-2023.4.1/enstools/compression/analyzer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6293 2023-01-18 16:33:07.000000 enstools-compression-2023.4.1/enstools/compression/analyzer/analyze_data_array.py
+-rwxrwxrwx   0 root         (0) root         (0)    10373 2023-01-18 16:33:07.000000 enstools-compression-2023.4.1/enstools/compression/analyzer/analyzer.py
+-rw-rw-rw-   0 root         (0) root         (0)     8194 2023-01-18 16:33:07.000000 enstools-compression-2023.4.1/enstools/compression/analyzer/analyzer_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      344 2023-01-18 16:33:07.000000 enstools-compression-2023.4.1/enstools/compression/api.py
+-rw-rw-rw-   0 root         (0) root         (0)    16861 2023-01-18 16:33:07.000000 enstools-compression-2023.4.1/enstools/compression/cli.py
+-rwxrwxrwx   0 root         (0) root         (0)    11172 2023-01-18 16:33:07.000000 enstools-compression-2023.4.1/enstools/compression/compressor.py
+-rwxrwxrwx   0 root         (0) root         (0)     3354 2023-01-18 16:33:07.000000 enstools-compression-2023.4.1/enstools/compression/emulation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:08:59.974639 enstools-compression-2023.4.1/enstools/compression/emulators/
+-rw-rw-rw-   0 root         (0) root         (0)     1188 2023-01-18 16:33:07.000000 enstools-compression-2023.4.1/enstools/compression/emulators/EmulatorClass.py
+-rw-rw-rw-   0 root         (0) root         (0)     2565 2023-02-10 12:30:33.000000 enstools-compression-2023.4.1/enstools/compression/emulators/FiltersEmulator.py
+-rwxrwxrwx   0 root         (0) root         (0)     2885 2023-01-18 16:33:07.000000 enstools-compression-2023.4.1/enstools/compression/emulators/LibpressioEmulator.py
+-rwxrwxrwx   0 root         (0) root         (0)     2036 2023-01-18 16:33:07.000000 enstools-compression-2023.4.1/enstools/compression/emulators/ZFPEmulator.py
+-rw-rw-rw-   0 root         (0) root         (0)      197 2023-01-18 16:33:07.000000 enstools-compression-2023.4.1/enstools/compression/emulators/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2715 2023-01-18 16:33:07.000000 enstools-compression-2023.4.1/enstools/compression/evaluator.py
+-rw-rw-rw-   0 root         (0) root         (0)     3736 2023-02-10 12:30:33.000000 enstools-compression-2023.4.1/enstools/compression/h5netcdf_compressor.py
+-rw-rw-rw-   0 root         (0) root         (0)    11156 2023-01-18 16:33:07.000000 enstools-compression-2023.4.1/enstools/compression/metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     4557 2023-01-18 16:33:07.000000 enstools-compression-2023.4.1/enstools/compression/pruner.py
+-rw-rw-rw-   0 root         (0) root         (0)    10801 2023-01-18 16:33:07.000000 enstools-compression-2023.4.1/enstools/compression/significant_bits.py
+-rw-rw-rw-   0 root         (0) root         (0)      910 2023-01-18 16:33:07.000000 enstools-compression-2023.4.1/enstools/compression/size_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     7903 2023-02-10 12:30:33.000000 enstools-compression-2023.4.1/enstools/compression/slicing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:08:59.974639 enstools-compression-2023.4.1/enstools/compression/xr_accessor/
+-rw-rw-rw-   0 root         (0) root         (0)       23 2023-01-18 16:33:07.000000 enstools-compression-2023.4.1/enstools/compression/xr_accessor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5314 2023-01-18 16:33:07.000000 enstools-compression-2023.4.1/enstools/compression/xr_accessor/accessor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:08:59.975639 enstools-compression-2023.4.1/enstools_compression.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1662 2023-04-17 16:08:59.000000 enstools-compression-2023.4.1/enstools_compression.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1284 2023-04-17 16:08:59.000000 enstools-compression-2023.4.1/enstools_compression.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 16:08:59.000000 enstools-compression-2023.4.1/enstools_compression.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       71 2023-04-17 16:08:59.000000 enstools-compression-2023.4.1/enstools_compression.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       74 2023-04-17 16:08:59.000000 enstools-compression-2023.4.1/enstools_compression.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-04-17 16:08:59.000000 enstools-compression-2023.4.1/enstools_compression.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 16:08:59.975639 enstools-compression-2023.4.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1366 2023-01-18 16:33:07.000000 enstools-compression-2023.4.1/setup.py
```

### Comparing `enstools-compression-2023.1/LICENSE` & `enstools-compression-2023.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `enstools-compression-2023.1/PKG-INFO` & `enstools-compression-2023.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enstools-compression
-Version: 2023.1
+Version: 2023.4.1
 Home-page: https://github.com/wavestoweather/enstools-compression
 Author: Oriol Tintó
 Author-email: oriol.tinto@lmu.de
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # enstools-compression [![Documentation Status](https://readthedocs.org/projects/enstools/badge/?version=latest)](https://enstools-compression.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `enstools-compression-2023.1/README.md` & `enstools-compression-2023.4.1/README.md`

 * *Files identical despite different names*

### Comparing `enstools-compression-2023.1/enstools/compression/analyzer/AnalysisOptions.py` & `enstools-compression-2023.4.1/enstools/compression/analyzer/AnalysisOptions.py`

 * *Files identical despite different names*

### Comparing `enstools-compression-2023.1/enstools/compression/analyzer/analyze_data_array.py` & `enstools-compression-2023.4.1/enstools/compression/analyzer/analyze_data_array.py`

 * *Files identical despite different names*

### Comparing `enstools-compression-2023.1/enstools/compression/analyzer/analyzer.py` & `enstools-compression-2023.4.1/enstools/compression/analyzer/analyzer.py`

 * *Files identical despite different names*

### Comparing `enstools-compression-2023.1/enstools/compression/analyzer/analyzer_utils.py` & `enstools-compression-2023.4.1/enstools/compression/analyzer/analyzer_utils.py`

 * *Files identical despite different names*

### Comparing `enstools-compression-2023.1/enstools/compression/cli.py` & `enstools-compression-2023.4.1/enstools/compression/cli.py`

 * *Files identical despite different names*

### Comparing `enstools-compression-2023.1/enstools/compression/compressor.py` & `enstools-compression-2023.4.1/enstools/compression/compressor.py`

 * *Files identical despite different names*

### Comparing `enstools-compression-2023.1/enstools/compression/emulation.py` & `enstools-compression-2023.4.1/enstools/compression/emulation.py`

 * *Files identical despite different names*

### Comparing `enstools-compression-2023.1/enstools/compression/emulators/EmulatorClass.py` & `enstools-compression-2023.4.1/enstools/compression/emulators/EmulatorClass.py`

 * *Files identical despite different names*

### Comparing `enstools-compression-2023.1/enstools/compression/emulators/FiltersEmulator.py` & `enstools-compression-2023.4.1/enstools/compression/emulators/FiltersEmulator.py`

 * *Files 10% similar despite different names*

```diff
@@ -51,20 +51,25 @@
         # Create a temporary directory in the system memory
         
         dummy_var = "tmp"
 
         # Calculate uncompressed size
         uncompressed_size = uncompressed_data.dtype.itemsize * uncompressed_data.size
 
+        # If the key "chunksizes" is inside the encoding, we need to rename it.
+        encoding = dict(self.compression)
+        if "chunksizes" in encoding:
+            encoding["chunks"] = encoding.pop("chunksizes")
+
         # Initialize file object
         with io.BytesIO() as bio:
         
             # Compress data
             with h5py.File(bio, mode='w') as f:
-                f.create_dataset(dummy_var, data=uncompressed_data, **self.compression)
+                f.create_dataset(dummy_var, data=uncompressed_data, **encoding)
             
             # Get compressed file
             compressed_size = bio.getbuffer().nbytes
 
             # Decompress data
             with h5py.File(bio, mode="r") as f:
                 recovered_data = f[dummy_var][()]
```

### Comparing `enstools-compression-2023.1/enstools/compression/emulators/LibpressioEmulator.py` & `enstools-compression-2023.4.1/enstools/compression/emulators/LibpressioEmulator.py`

 * *Files identical despite different names*

### Comparing `enstools-compression-2023.1/enstools/compression/emulators/ZFPEmulator.py` & `enstools-compression-2023.4.1/enstools/compression/emulators/ZFPEmulator.py`

 * *Files identical despite different names*

### Comparing `enstools-compression-2023.1/enstools/compression/evaluator.py` & `enstools-compression-2023.4.1/enstools/compression/evaluator.py`

 * *Files identical despite different names*

### Comparing `enstools-compression-2023.1/enstools/compression/metrics.py` & `enstools-compression-2023.4.1/enstools/compression/metrics.py`

 * *Files identical despite different names*

### Comparing `enstools-compression-2023.1/enstools/compression/pruner.py` & `enstools-compression-2023.4.1/enstools/compression/pruner.py`

 * *Files identical despite different names*

### Comparing `enstools-compression-2023.1/enstools/compression/significant_bits.py` & `enstools-compression-2023.4.1/enstools/compression/significant_bits.py`

 * *Files identical despite different names*

### Comparing `enstools-compression-2023.1/enstools/compression/size_metrics.py` & `enstools-compression-2023.4.1/enstools/compression/size_metrics.py`

 * *Files identical despite different names*

### Comparing `enstools-compression-2023.1/enstools/compression/xr_accessor/accessor.py` & `enstools-compression-2023.4.1/enstools/compression/xr_accessor/accessor.py`

 * *Files identical despite different names*

### Comparing `enstools-compression-2023.1/enstools_compression.egg-info/PKG-INFO` & `enstools-compression-2023.4.1/enstools_compression.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enstools-compression
-Version: 2023.1
+Version: 2023.4.1
 Home-page: https://github.com/wavestoweather/enstools-compression
 Author: Oriol Tintó
 Author-email: oriol.tinto@lmu.de
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # enstools-compression [![Documentation Status](https://readthedocs.org/projects/enstools/badge/?version=latest)](https://enstools-compression.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `enstools-compression-2023.1/enstools_compression.egg-info/SOURCES.txt` & `enstools-compression-2023.4.1/enstools_compression.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,20 @@
 setup.py
 enstools/compression/__init__.py
 enstools/compression/api.py
 enstools/compression/cli.py
 enstools/compression/compressor.py
 enstools/compression/emulation.py
 enstools/compression/evaluator.py
+enstools/compression/h5netcdf_compressor.py
 enstools/compression/metrics.py
 enstools/compression/pruner.py
 enstools/compression/significant_bits.py
 enstools/compression/size_metrics.py
+enstools/compression/slicing.py
 enstools/compression/analyzer/AnalysisOptions.py
 enstools/compression/analyzer/__init__.py
 enstools/compression/analyzer/analyze_data_array.py
 enstools/compression/analyzer/analyzer.py
 enstools/compression/analyzer/analyzer_utils.py
 enstools/compression/emulators/EmulatorClass.py
 enstools/compression/emulators/FiltersEmulator.py
```

### Comparing `enstools-compression-2023.1/setup.py` & `enstools-compression-2023.4.1/setup.py`

 * *Files identical despite different names*

