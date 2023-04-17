# Comparing `tmp/psd_export-1.0.4.tar.gz` & `tmp/psd_export-1.0.5.tar.gz`

## Comparing `psd_export-1.0.4.tar` & `psd_export-1.0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 psd_export-1.0.4/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 psd_export-1.0.4/src/psd_export/__init__.py
--rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 psd_export-1.0.4/src/psd_export/blendfuncs.py
--rw-r--r--   0        0        0    20326 2020-02-02 00:00:00.000000 psd_export-1.0.4/src/psd_export/composite.py
--rw-r--r--   0        0        0     7606 2020-02-02 00:00:00.000000 psd_export-1.0.4/src/psd_export/export.py
--rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 psd_export-1.0.4/src/psd_export/filters.py
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 psd_export-1.0.4/src/psd_export/util.py
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 psd_export-1.0.4/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 psd_export-1.0.4/LICENSE
--rw-r--r--   0        0        0     8583 2020-02-02 00:00:00.000000 psd_export-1.0.4/README.md
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 psd_export-1.0.4/pyproject.toml
--rw-r--r--   0        0        0    10610 2020-02-02 00:00:00.000000 psd_export-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 psd_export-1.0.5/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 psd_export-1.0.5/src/psd_export/__init__.py
+-rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 psd_export-1.0.5/src/psd_export/blendfuncs.py
+-rw-r--r--   0        0        0    20244 2020-02-02 00:00:00.000000 psd_export-1.0.5/src/psd_export/composite.py
+-rw-r--r--   0        0        0     7606 2020-02-02 00:00:00.000000 psd_export-1.0.5/src/psd_export/export.py
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 psd_export-1.0.5/src/psd_export/filters.py
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 psd_export-1.0.5/src/psd_export/util.py
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 psd_export-1.0.5/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 psd_export-1.0.5/LICENSE
+-rw-r--r--   0        0        0     8583 2020-02-02 00:00:00.000000 psd_export-1.0.5/README.md
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 psd_export-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0    10610 2020-02-02 00:00:00.000000 psd_export-1.0.5/PKG-INFO
```

### Comparing `psd_export-1.0.4/.github/workflows/python-publish.yml` & `psd_export-1.0.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `psd_export-1.0.4/src/psd_export/blendfuncs.py` & `psd_export-1.0.5/src/psd_export/blendfuncs.py`

 * *Files identical despite different names*

### Comparing `psd_export-1.0.4/src/psd_export/composite.py` & `psd_export-1.0.5/src/psd_export/composite.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,14 +147,17 @@
         layer.composite_cache[offset] = {}
     return layer.composite_cache[offset]
 
 def get_cached_composite(layer:WrappedLayer, offset):
     return get_tile_cache(layer, offset).get(layer.visibility_dependency, None)
 
 def set_cached_composite(layer:WrappedLayer, offset, tile_data):
+    for data in tile_data:
+        if not np.isscalar(data):
+            data.flags.writeable = False
     get_tile_cache(layer, offset)[layer.visibility_dependency] = tile_data
 
 def clear_all_caches(layer:WrappedLayer):
     layer.composite_cache.clear()
     layer.data_cache.clear()
     for sublayer in layer.descendants():
         sublayer.composite_cache.clear()
@@ -329,19 +332,14 @@
                 if sublayer.custom_op is not None:
                     await barrier_skip(sublayer.custom_op_barrier)
                 # Need to enter the clip layers to make sure any barriers are hit.
                 if sublayer.clip_layers:
                     await composite_group_layer(sublayer.clip_layers, size, offset)
                 continue
 
-            # Copy group output to prevent mutated cache tiles
-            if sublayer.layer.is_group():
-                color_src = color_src.copy()
-                alpha_src = alpha_src.copy()
-
             # Perform custom filter over the current color_dst
             if sublayer.custom_op is not None:
                 if not np.isscalar(color_dst):
                     await peval(lambda: blit(sublayer.custom_op_color, color_dst, offset))
                     await peval(lambda: blit(sublayer.custom_op_alpha, alpha_src, offset))
                 await sublayer.custom_op_barrier.wait()
                 if not sublayer.custom_op_condition.locked():
@@ -423,15 +421,15 @@
             if sublayer.worker_counter == 0 and not sublayer.tag_dependency:
                 sublayer.data_cache.clear()
                 clear_descendants_caches(sublayer)
 
     if np.isscalar(color_dst):
         return None, None
 
-    return color_dst, alpha_dst
+    return color_dst.copy(), alpha_dst.copy()
 
 debug_path = pathlib.Path('')
 debug_run = 0
 
 def debug_layer(name, offset, data):
     data = (data * 255).astype(np.uint8)
     if data.shape[2] == 1:
```

### Comparing `psd_export-1.0.4/src/psd_export/export.py` & `psd_export-1.0.5/src/psd_export/export.py`

 * *Files identical despite different names*

### Comparing `psd_export-1.0.4/src/psd_export/filters.py` & `psd_export-1.0.5/src/psd_export/filters.py`

 * *Files identical despite different names*

### Comparing `psd_export-1.0.4/src/psd_export/util.py` & `psd_export-1.0.5/src/psd_export/util.py`

 * *Files identical despite different names*

### Comparing `psd_export-1.0.4/.gitignore` & `psd_export-1.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `psd_export-1.0.4/LICENSE` & `psd_export-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `psd_export-1.0.4/README.md` & `psd_export-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `psd_export-1.0.4/pyproject.toml` & `psd_export-1.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "psd-export"
-version = "1.0.4"
+version = "1.0.5"
 authors = [
     { name = "cromachina" }
 ]
 license = { file = "LICENSE" }
 description = "Fast exporting of PSDs with [tagged] layers for variants."
 readme = "README.md"
 requires-python = ">=3.0"
```

### Comparing `psd_export-1.0.4/PKG-INFO` & `psd_export-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psd-export
-Version: 1.0.4
+Version: 1.0.5
 Summary: Fast exporting of PSDs with [tagged] layers for variants.
 Project-URL: Homepage, https://github.com/cromachina/psd-export
 Author: cromachina
 License: MIT License
         
         Copyright (c) 2022 cromachina
```

