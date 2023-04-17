# Comparing `tmp/psd_export-1.0.3.tar.gz` & `tmp/psd_export-1.0.4.tar.gz`

## Comparing `psd_export-1.0.3.tar` & `psd_export-1.0.4.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 psd_export-1.0.3/blend_analyze.py
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 psd_export-1.0.3/numba-blur-test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 psd_export-1.0.3/src/psd_export/__init__.py
--rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 psd_export-1.0.3/src/psd_export/blendfuncs.py
--rw-r--r--   0        0        0    19861 2020-02-02 00:00:00.000000 psd_export-1.0.3/src/psd_export/composite.py
--rw-r--r--   0        0        0     7606 2020-02-02 00:00:00.000000 psd_export-1.0.3/src/psd_export/export.py
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 psd_export-1.0.3/src/psd_export/filters.py
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 psd_export-1.0.3/src/psd_export/util.py
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 psd_export-1.0.3/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 psd_export-1.0.3/LICENSE
--rw-r--r--   0        0        0     8583 2020-02-02 00:00:00.000000 psd_export-1.0.3/README.md
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 psd_export-1.0.3/pyproject.toml
--rw-r--r--   0        0        0    10610 2020-02-02 00:00:00.000000 psd_export-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 psd_export-1.0.4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 psd_export-1.0.4/src/psd_export/__init__.py
+-rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 psd_export-1.0.4/src/psd_export/blendfuncs.py
+-rw-r--r--   0        0        0    20326 2020-02-02 00:00:00.000000 psd_export-1.0.4/src/psd_export/composite.py
+-rw-r--r--   0        0        0     7606 2020-02-02 00:00:00.000000 psd_export-1.0.4/src/psd_export/export.py
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 psd_export-1.0.4/src/psd_export/filters.py
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 psd_export-1.0.4/src/psd_export/util.py
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 psd_export-1.0.4/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 psd_export-1.0.4/LICENSE
+-rw-r--r--   0        0        0     8583 2020-02-02 00:00:00.000000 psd_export-1.0.4/README.md
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 psd_export-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0    10610 2020-02-02 00:00:00.000000 psd_export-1.0.4/PKG-INFO
```

### Comparing `psd_export-1.0.3/numba-blur-test.py` & `psd_export-1.0.4/src/psd_export/filters.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,61 +1,69 @@
-import numba
-from numba.typed import Dict
+import cv2
 import numpy as np
 
-@numba.njit
-def get_gaussian_kernel(size, kernels):
-    kernel = kernels.get(size)
-    if kernel is not None:
-        return kernel
-    ax = np.linspace(-(size - 1) / 2., (size - 1) / 2., size)
-    gauss = np.exp(-0.5 * np.square(ax) / np.square(size))
-    kernel = np.outer(gauss, gauss)
-    kernel /= np.sum(kernel)
-    kernels[size] = kernel
-    return kernel
-
-@numba.njit(inline='always')
-def clamp(val, min_val, max_val):
-    return max(min_val, min(max_val, val))
-
-@numba.njit
-def get_clamped(data, y, x):
-    h, w = data.shape[:2]
-    y = clamp(y, 0, h - 1)
-    x = clamp(x, 0, w - 1)
-    return data[y, x]
-
-@numba.njit
-def convolve(data, y, x, kernel, result):
-    kh, kw = kernel.shape
-    total = kh * kw
-    kh2, kw2 = kh // 2, kw // 2
-    dy = y - kh2
-    for ky in range(kh):
-        dx = x - kw2
-        for kx in range(kw):
-            result[y, x] += get_clamped(data, dy, dx) * kernel[ky, kx]
-            dx += 1
-        dy += 1
-
-@numba.njit()
-def variable_blur(color, alpha, size, kernels):
-    alpha_k = (alpha * size).astype(np.int16).reshape(alpha.shape[:2])
-    h, w = color.shape[:2]
-    result = np.empty_like(color)
-    for y in range(h):
-        for x in range(w):
-            k = alpha_k[y, x]
-            if k > 0:
-                convolve(color, y, x, get_gaussian_kernel(k, kernels), result)
-    return result
-
-kernel_cache = Dict.empty(
-    key_type=numba.int16,
-    value_type=numba.float64[:,:],
-)
+from . import util
 
-def variable_blur_op(color, alpha, size=50, *_):
+filter_names = {}
+
+def filter(name):
+    def wrap(func):
+        filter_names[name] = func
+        return func
+    return wrap
+
+def get_filter(name):
+    return filter_names.get(name, None)
+
+def compose_ops(ops):
+    if not ops:
+        return None
+    def c(color, alpha):
+        for op in ops:
+            color, alpha = op(color, alpha)
+        return color, alpha
+    return c
+
+def mosaic(image, mosaic_factor):
+    original_size = util.swap(image.shape[:2])
+    min_dim = min(original_size) // mosaic_factor
+    min_dim = max(4, min_dim)
+    scale_dimension = (original_size[0] // min_dim, original_size[1] // min_dim)
+    mosaic_image = cv2.resize(image, scale_dimension, interpolation=cv2.INTER_AREA)
+    return cv2.resize(mosaic_image, original_size, interpolation=cv2.INTER_NEAREST)
+
+mosaic_factor_default = 100
+
+@filter('censor')
+def mosaic_op(color, alpha, mosaic_factor=None, apply_to_alpha=False, *_):
+    if mosaic_factor is None:
+        mosaic_factor = mosaic_factor_default
+    mosaic_factor = int(mosaic_factor)
+    color = mosaic(color, mosaic_factor)
+    if apply_to_alpha:
+        alpha = mosaic(alpha, mosaic_factor)
+    return color, alpha
+
+@filter('blur')
+def blur_op(color, alpha, size=50, apply_to_alpha=False, *_):
+    size = float(size)
+    color = cv2.GaussianBlur(color, ksize=(0, 0), sigmaX=size, dst=color, borderType=cv2.BORDER_REPLICATE)
+    if apply_to_alpha:
+        alpha = cv2.GaussianBlur(alpha, ksize=(0, 0), sigmaX=size, dst=alpha, borderType=cv2.BORDER_REPLICATE)
+    return color, alpha
+
+def motion_blur(data, angle, size):
+    kernel = np.zeros((size, size))
+    kernel[(size - 1) // 2] = 1
+    rotation = cv2.getRotationMatrix2D((size / 2, size / 2), np.degrees(angle), 1.0)
+    kernel = cv2.warpAffine(kernel, rotation, (size, size))
+    kernel *= (1.0 / np.sum(kernel))
+    return cv2.filter2D(data, -1, kernel)
+
+@filter('motion-blur')
+def motion_blur_op(color, alpha, angle=0, size=50, apply_to_alpha=False, *_):
+    angle = float(angle)
     size = int(size)
-    color = variable_blur(color, alpha, size, kernel_cache)
-    return color, alpha
+    color = motion_blur(color, angle, size)
+    if apply_to_alpha:
+        alpha = motion_blur(alpha, angle, size).reshape(alpha.shape)
+    return color, alpha
```

### Comparing `psd_export-1.0.3/src/psd_export/blendfuncs.py` & `psd_export-1.0.4/src/psd_export/blendfuncs.py`

 * *Files identical despite different names*

### Comparing `psd_export-1.0.3/src/psd_export/composite.py` & `psd_export-1.0.4/src/psd_export/composite.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,18 +99,19 @@
 
 def blit(dst, src, offset):
     dst, src = get_overlap_tiles(dst, src, offset)
     np.copyto(dst, src)
 
 def get_visibility_all_children(layer:WrappedLayer, visited, visit_all):
     if layer.visible or visit_all:
-        visited.add(layer)
-        if layer.layer.is_group():
-            for sublayer in layer.flat_children:
-                get_visibility_all_children(sublayer, visited, visit_all)
+        tags = [not tag.ignore for tag in layer.tags]
+        if any(tags):
+            visited.add(layer)
+        for sublayer in layer.flat_children:
+            get_visibility_all_children(sublayer, visited, visit_all)
     return visited
 
 def get_visibility_dependency_sub(layer:WrappedLayer, visited, visit_all):
     if layer.parent == None:
         return
     if layer in visited:
         return
@@ -122,25 +123,22 @@
             get_visibility_all_children(sublayer, visited, visit_all)
     if layer.parent.parent != None and layer.parent.layer.blend_mode == BlendMode.PASS_THROUGH:
         get_visibility_dependency_sub(layer.parent, visited, visit_all)
 
 def get_visibility_dependency(layer:WrappedLayer, visit_all=False):
     visited = set()
     get_visibility_dependency_sub(layer, visited, visit_all)
-    for sublayer in layer.clip_layers:
-        get_visibility_all_children(sublayer, visited, visit_all)
     return frozenset(visited)
 
 def set_layer_extra_data(layer:WrappedLayer, tile_count, size):
     set_tag_dependency(layer)
     for sublayer in layer.descendants():
         sublayer.worker_counter = tile_count
         sublayer.cache_hit = ''
-        if sublayer.visible:
-            sublayer.visibility_dependency = get_visibility_dependency(sublayer)
+        sublayer.visibility_dependency = get_visibility_dependency(sublayer)
         if sublayer.custom_op is not None:
             sublayer.custom_op_barrier = asyncio.Barrier(tile_count)
             sublayer.custom_op_condition = asyncio.Condition()
             sublayer.custom_op_finished = False
             sublayer.custom_op_color = np.zeros(size + (3,))
             sublayer.custom_op_alpha = np.zeros(size + (1,))
 
@@ -149,46 +147,49 @@
         layer.composite_cache[offset] = {}
     return layer.composite_cache[offset]
 
 def get_cached_composite(layer:WrappedLayer, offset):
     return get_tile_cache(layer, offset).get(layer.visibility_dependency, None)
 
 def set_cached_composite(layer:WrappedLayer, offset, tile_data):
-    if not layer.tag_dependency or layer.tags:
-        get_tile_cache(layer, offset)[layer.visibility_dependency] = tile_data
+    get_tile_cache(layer, offset)[layer.visibility_dependency] = tile_data
 
 def clear_all_caches(layer:WrappedLayer):
     layer.composite_cache.clear()
     layer.data_cache.clear()
     for sublayer in layer.descendants():
         sublayer.composite_cache.clear()
-        layer.data_cache.clear()
+        sublayer.data_cache.clear()
 
-def clear_descendants_composite_cache(layer:WrappedLayer):
+def clear_descendants_caches(layer:WrappedLayer):
     for sublayer in layer.descendants():
         sublayer.composite_cache.clear()
+        sublayer.data_cache.clear()
 
 def set_tag_dependency(layer:WrappedLayer):
     for sublayer in layer.descendants():
         if sublayer.tag_dependency is None:
             v = get_visibility_dependency(sublayer, True)
             sublayer.tag_dependency = False
             for v_layer in v:
-                if v_layer.tags:
+                tags = [not tag.ignore for tag in v_layer.tags]
+                if any(tags):
                     sublayer.tag_dependency = True
                     break
 
 def set_skip_to_last_untagged(layer:WrappedLayer):
     skip = False
     for child in reversed(layer.children):
         if not child.tag_dependency and not skip:
             skip = True
             continue
         if skip and child.composite_cache:
             child.skip = True
+            child.data_cache.clear()
+            child.composite_cache.clear()
 
 def set_skips(layer:WrappedLayer):
     for sublayer in layer.descendants():
         set_skip_to_last_untagged(sublayer)
 
 def get_cached_layer_data(layer:WrappedLayer, channel):
     with layer.data_cache_lock:
@@ -323,16 +324,24 @@
                 color_src, alpha_src = await get_pixel_layer_data(sublayer, size, offset)
 
             # Empty tile, can just ignore.
             if color_src is None:
                 set_cached_composite(sublayer, offset, (color_dst, alpha_dst))
                 if sublayer.custom_op is not None:
                     await barrier_skip(sublayer.custom_op_barrier)
+                # Need to enter the clip layers to make sure any barriers are hit.
+                if sublayer.clip_layers:
+                    await composite_group_layer(sublayer.clip_layers, size, offset)
                 continue
 
+            # Copy group output to prevent mutated cache tiles
+            if sublayer.layer.is_group():
+                color_src = color_src.copy()
+                alpha_src = alpha_src.copy()
+
             # Perform custom filter over the current color_dst
             if sublayer.custom_op is not None:
                 if not np.isscalar(color_dst):
                     await peval(lambda: blit(sublayer.custom_op_color, color_dst, offset))
                     await peval(lambda: blit(sublayer.custom_op_alpha, alpha_src, offset))
                 await sublayer.custom_op_barrier.wait()
                 if not sublayer.custom_op_condition.locked():
@@ -409,29 +418,31 @@
                 alpha_dst = await peval(lambda: blendfuncs.normal_alpha(alpha_dst, alpha_src))
 
             set_cached_composite(sublayer, offset, (color_dst, alpha_dst))
         finally:
             sublayer.worker_counter -= 1
             if sublayer.worker_counter == 0 and not sublayer.tag_dependency:
                 sublayer.data_cache.clear()
-                clear_descendants_composite_cache(sublayer)
+                clear_descendants_caches(sublayer)
 
     if np.isscalar(color_dst):
         return None, None
 
     return color_dst, alpha_dst
 
 debug_path = pathlib.Path('')
+debug_run = 0
 
 def debug_layer(name, offset, data):
+    data = (data * 255).astype(np.uint8)
     if data.shape[2] == 1:
         data = data.reshape(data.shape[:2])
-    data = (data * 255).astype(np.uint8)
-    data = cv2.cvtColor(data, cv2.COLOR_RGB2BGR)
-    path = debug_path / f'{name}-{offset}.png'
+    else:
+        data = cv2.cvtColor(data, cv2.COLOR_RGB2BGR)
+    path = debug_path /  f'{name}-{offset}-{debug_run}.png'
     cv2.imwrite(str(path), data)
 
 async def composite_tile(psd:WrappedLayer, size, offset, color, alpha):
     tile_color, tile_alpha = await composite_group_layer(psd, size, offset)
     if tile_color is not None:
         await peval(lambda: blit(color, tile_color, offset))
         await peval(lambda: blit(alpha, tile_alpha, offset))
```

### Comparing `psd_export-1.0.3/src/psd_export/export.py` & `psd_export-1.0.4/src/psd_export/export.py`

 * *Files identical despite different names*

### Comparing `psd_export-1.0.3/src/psd_export/util.py` & `psd_export-1.0.4/src/psd_export/util.py`

 * *Files identical despite different names*

### Comparing `psd_export-1.0.3/.gitignore` & `psd_export-1.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `psd_export-1.0.3/LICENSE` & `psd_export-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `psd_export-1.0.3/README.md` & `psd_export-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `psd_export-1.0.3/pyproject.toml` & `psd_export-1.0.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "psd-export"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
     { name = "cromachina" }
 ]
 license = { file = "LICENSE" }
 description = "Fast exporting of PSDs with [tagged] layers for variants."
 readme = "README.md"
 requires-python = ">=3.0"
```

### Comparing `psd_export-1.0.3/PKG-INFO` & `psd_export-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psd-export
-Version: 1.0.3
+Version: 1.0.4
 Summary: Fast exporting of PSDs with [tagged] layers for variants.
 Project-URL: Homepage, https://github.com/cromachina/psd-export
 Author: cromachina
 License: MIT License
         
         Copyright (c) 2022 cromachina
```

