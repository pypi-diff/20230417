# Comparing `tmp/kerchunk-0.1.0.tar.gz` & `tmp/kerchunk-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kerchunk-0.1.0.tar", last modified: Thu Jan 19 01:23:08 2023, max compression
+gzip compressed data, was "kerchunk-0.1.1.tar", last modified: Mon Apr 17 13:29:33 2023, max compression
```

## Comparing `kerchunk-0.1.0.tar` & `kerchunk-0.1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-01-19 01:23:08.843685 kerchunk-0.1.0/
--rw-r--r--   0 mdurant    (502) staff       (20)     1063 2022-09-18 01:28:32.000000 kerchunk-0.1.0/LICENSE
--rw-r--r--   0 mdurant    (502) staff       (20)      155 2022-09-18 01:28:32.000000 kerchunk-0.1.0/MANIFEST.in
--rw-r--r--   0 mdurant    (502) staff       (20)     2883 2023-01-19 01:23:08.843754 kerchunk-0.1.0/PKG-INFO
--rw-r--r--   0 mdurant    (502) staff       (20)     2433 2022-09-23 18:01:10.000000 kerchunk-0.1.0/README.md
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-01-19 01:23:08.844446 kerchunk-0.1.0/kerchunk/
--rw-r--r--   0 mdurant    (502) staff       (20)      142 2022-09-18 01:28:32.000000 kerchunk-0.1.0/kerchunk/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)      497 2023-01-19 01:23:08.844499 kerchunk-0.1.0/kerchunk/_version.py
--rw-r--r--   0 mdurant    (502) staff       (20)     6014 2023-01-15 19:25:10.000000 kerchunk-0.1.0/kerchunk/codecs.py
--rw-r--r--   0 mdurant    (502) staff       (20)    26805 2023-01-17 18:22:52.000000 kerchunk-0.1.0/kerchunk/combine.py
--rw-r--r--   0 mdurant    (502) staff       (20)     4392 2023-01-19 01:22:26.000000 kerchunk-0.1.0/kerchunk/df.py
--rw-r--r--   0 mdurant    (502) staff       (20)     8985 2022-10-31 16:19:59.000000 kerchunk-0.1.0/kerchunk/fits.py
--rw-r--r--   0 mdurant    (502) staff       (20)     9429 2023-01-16 14:32:53.000000 kerchunk-0.1.0/kerchunk/grib2.py
--rw-r--r--   0 mdurant    (502) staff       (20)    21998 2023-01-19 01:22:26.000000 kerchunk-0.1.0/kerchunk/hdf.py
--rw-r--r--   0 mdurant    (502) staff       (20)     9882 2022-12-09 18:27:45.000000 kerchunk-0.1.0/kerchunk/netCDF3.py
--rw-r--r--   0 mdurant    (502) staff       (20)     3589 2022-12-09 18:27:45.000000 kerchunk-0.1.0/kerchunk/tiff.py
--rw-r--r--   0 mdurant    (502) staff       (20)    12231 2023-01-16 14:32:57.000000 kerchunk-0.1.0/kerchunk/utils.py
--rw-r--r--   0 mdurant    (502) staff       (20)      963 2022-12-09 18:27:45.000000 kerchunk-0.1.0/kerchunk/zarr.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-01-19 01:23:08.843558 kerchunk-0.1.0/kerchunk.egg-info/
--rw-r--r--   0 mdurant    (502) staff       (20)     2883 2023-01-19 01:23:08.000000 kerchunk-0.1.0/kerchunk.egg-info/PKG-INFO
--rw-r--r--   0 mdurant    (502) staff       (20)      523 2023-01-19 01:23:08.000000 kerchunk-0.1.0/kerchunk.egg-info/SOURCES.txt
--rw-r--r--   0 mdurant    (502) staff       (20)        1 2023-01-19 01:23:08.000000 kerchunk-0.1.0/kerchunk.egg-info/dependency_links.txt
--rw-r--r--   0 mdurant    (502) staff       (20)      244 2023-01-19 01:23:08.000000 kerchunk-0.1.0/kerchunk.egg-info/entry_points.txt
--rw-r--r--   0 mdurant    (502) staff       (20)        1 2022-09-21 14:47:57.000000 kerchunk-0.1.0/kerchunk.egg-info/not-zip-safe
--rw-r--r--   0 mdurant    (502) staff       (20)      118 2023-01-19 01:23:08.000000 kerchunk-0.1.0/kerchunk.egg-info/requires.txt
--rw-r--r--   0 mdurant    (502) staff       (20)        9 2023-01-19 01:23:08.000000 kerchunk-0.1.0/kerchunk.egg-info/top_level.txt
--rw-r--r--   0 mdurant    (502) staff       (20)       34 2022-09-18 01:28:32.000000 kerchunk-0.1.0/requirements.txt
--rw-r--r--   0 mdurant    (502) staff       (20)      724 2023-01-19 01:23:08.844126 kerchunk-0.1.0/setup.cfg
--rw-r--r--   0 mdurant    (502) staff       (20)     1247 2023-01-19 01:22:26.000000 kerchunk-0.1.0/setup.py
--rw-r--r--   0 mdurant    (502) staff       (20)    70238 2022-09-18 01:28:32.000000 kerchunk-0.1.0/versioneer.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-04-17 13:29:33.971612 kerchunk-0.1.1/
+-rw-r--r--   0 mdurant    (502) staff       (20)     1063 2022-09-18 01:28:32.000000 kerchunk-0.1.1/LICENSE
+-rw-r--r--   0 mdurant    (502) staff       (20)      155 2022-09-18 01:28:32.000000 kerchunk-0.1.1/MANIFEST.in
+-rw-r--r--   0 mdurant    (502) staff       (20)     2883 2023-04-17 13:29:33.971686 kerchunk-0.1.1/PKG-INFO
+-rw-r--r--   0 mdurant    (502) staff       (20)     2433 2022-09-23 18:01:10.000000 kerchunk-0.1.1/README.md
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-04-17 13:29:33.972353 kerchunk-0.1.1/kerchunk/
+-rw-r--r--   0 mdurant    (502) staff       (20)      142 2022-09-18 01:28:32.000000 kerchunk-0.1.1/kerchunk/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      497 2023-04-17 13:29:33.972405 kerchunk-0.1.1/kerchunk/_version.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     6203 2023-04-17 13:28:40.000000 kerchunk-0.1.1/kerchunk/codecs.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    28247 2023-04-17 13:28:40.000000 kerchunk-0.1.1/kerchunk/combine.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     8840 2023-03-13 19:21:13.000000 kerchunk-0.1.1/kerchunk/df.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     8985 2022-10-31 16:19:59.000000 kerchunk-0.1.1/kerchunk/fits.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     9429 2023-01-16 14:32:53.000000 kerchunk-0.1.1/kerchunk/grib2.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    22133 2023-04-12 17:06:54.000000 kerchunk-0.1.1/kerchunk/hdf.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     9882 2022-12-09 18:27:45.000000 kerchunk-0.1.1/kerchunk/netCDF3.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     3589 2023-03-13 14:06:07.000000 kerchunk-0.1.1/kerchunk/tiff.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    12231 2023-02-28 15:06:36.000000 kerchunk-0.1.1/kerchunk/utils.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      963 2022-12-09 18:27:45.000000 kerchunk-0.1.1/kerchunk/zarr.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-04-17 13:29:33.971493 kerchunk-0.1.1/kerchunk.egg-info/
+-rw-r--r--   0 mdurant    (502) staff       (20)     2883 2023-04-17 13:29:33.000000 kerchunk-0.1.1/kerchunk.egg-info/PKG-INFO
+-rw-r--r--   0 mdurant    (502) staff       (20)      523 2023-04-17 13:29:33.000000 kerchunk-0.1.1/kerchunk.egg-info/SOURCES.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)        1 2023-04-17 13:29:33.000000 kerchunk-0.1.1/kerchunk.egg-info/dependency_links.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)      244 2023-04-17 13:29:33.000000 kerchunk-0.1.1/kerchunk.egg-info/entry_points.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)        1 2022-09-21 14:47:57.000000 kerchunk-0.1.1/kerchunk.egg-info/not-zip-safe
+-rw-r--r--   0 mdurant    (502) staff       (20)      118 2023-04-17 13:29:33.000000 kerchunk-0.1.1/kerchunk.egg-info/requires.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)        9 2023-04-17 13:29:33.000000 kerchunk-0.1.1/kerchunk.egg-info/top_level.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)       34 2022-09-18 01:28:32.000000 kerchunk-0.1.1/requirements.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)      724 2023-04-17 13:29:33.972010 kerchunk-0.1.1/setup.cfg
+-rw-r--r--   0 mdurant    (502) staff       (20)     1247 2023-01-19 21:15:29.000000 kerchunk-0.1.1/setup.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    70238 2022-09-18 01:28:32.000000 kerchunk-0.1.1/versioneer.py
```

### Comparing `kerchunk-0.1.0/LICENSE` & `kerchunk-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kerchunk-0.1.0/PKG-INFO` & `kerchunk-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kerchunk
-Version: 0.1.0
+Version: 0.1.1
 Summary: Functions to make reference descriptions for ReferenceFileSystem
 Home-page: https://github.com/fsspec/kerchunk
 Author: Martin Durant
 Author-email: martin.durant@alumni.utoronto.ca
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `kerchunk-0.1.0/README.md` & `kerchunk-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `kerchunk-0.1.0/kerchunk/codecs.py` & `kerchunk-0.1.1/kerchunk/codecs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import ast
 import numcodecs
 from numcodecs.abc import Codec
 import numpy as np
+import threading
 
 
 class FillStringsCodec(Codec):
     """Sets fixed-length string fields to empty
 
     To be used with HDF fields of strings, to fill in the valules of the opaque
     16-byte string IDs.
@@ -67,14 +68,16 @@
 
 
 class GRIBCodec(numcodecs.abc.Codec):
     """
     Read GRIB stream of bytes as a message using eccodes
     """
 
+    eclock = threading.RLock()
+
     codec_id = "grib"
 
     def __init__(self, var, dtype=None):
         self.var = var
         self.dtype = dtype
 
     def encode(self, buf):
@@ -86,26 +89,29 @@
 
         if self.var in ["latitude", "longitude"]:
             var = self.var + "s"
             dt = self.dtype or "float64"
         else:
             var = "values"
             dt = self.dtype or "float32"
-        mid = eccodes.codes_new_from_message(bytes(buf))
-        try:
-            data = eccodes.codes_get_array(mid, var)
-        finally:
-            eccodes.codes_release(mid)
-
-        if var == "values" and eccodes.codes_get_string(mid, "missingValue"):
-            data[data == float(eccodes.codes_get_string(mid, "missingValue"))] = np.nan
-        if out is not None:
-            return numcodecs.compat.ndarray_copy(data, out)
-        else:
-            return data.astype(dt)
+        with self.eclock:
+            mid = eccodes.codes_new_from_message(bytes(buf))
+            try:
+                data = eccodes.codes_get_array(mid, var)
+                if var == "values" and eccodes.codes_get_string(mid, "missingValue"):
+                    data[
+                        data == float(eccodes.codes_get_string(mid, "missingValue"))
+                    ] = np.nan
+                if out is not None:
+                    return numcodecs.compat.ndarray_copy(data, out)
+                else:
+                    return data.astype(dt)
+
+            finally:
+                eccodes.codes_release(mid)
 
 
 numcodecs.register_codec(GRIBCodec, "grib")
 
 
 class AsciiTableCodec(numcodecs.abc.Codec):
     """Decodes ASCII-TABLE extensions in FITS files"""
```

### Comparing `kerchunk-0.1.0/kerchunk/combine.py` & `kerchunk-0.1.1/kerchunk/combine.py`

 * *Files 3% similar despite different names*

```diff
@@ -149,15 +149,17 @@
         if self._fss is None:
             logger.debug("setup filesystems")
             if self._indicts is not None:
                 fo_list = self._indicts
                 self._paths = self.path
             elif isinstance(self.path[0], collections.abc.Mapping):
                 fo_list = self.path
-                self._paths = [None] * len(fo_list)
+                self._paths = []
+                for path in self.path:
+                    self._paths.append(path.get("templates", {}).get("u", None))
             else:
                 self._paths = []
                 for of in fsspec.open_files(self.path, **self.target_options):
                     self._paths.append(of.full_name)
                 fs = fsspec.core.url_to_fs(self.path[0], **self.target_options)[0]
                 fo_list = fs.cat(self.path)
                 fo_list = [ujson.loads(v) for v in fo_list.values()]
@@ -189,15 +191,15 @@
         """
         selector = self.coo_map[var]
         if isinstance(selector, collections.abc.Callable):
             o = selector(index, z, var, fn)
         elif isinstance(selector, list):
             o = selector[index]
         elif isinstance(selector, re.Pattern):
-            o = selector.match(fn).groups()[0]  # may raise
+            o = selector.search(fn).groups()[0]
         elif not isinstance(selector, str):
             # constant, should be int or float
             o = selector
         elif selector == "VARNAME":
             # used for merging variable names across datasets
             o = [_ for _ in z if _ not in self.concat_dims + self.identical_dims]
             if len(o) > 1:
@@ -429,14 +431,17 @@
 
                     zarray["shape"] = shape
                     zarray["chunks"] = ch
                     zattrs["_ARRAY_DIMENSIONS"] = coord_order
                     self.out[f"{var or v}/.zarray"] = ujson.dumps(zarray)
                     # other attributes copied as-is from first occurrence of this array
                     self.out[f"{var or v}/.zattrs"] = ujson.dumps(zattrs)
+                else:
+                    k = self.out[f"{var or v}/.zarray"]
+                    ch = ujson.loads(k)["chunks"]
 
                 for fn in fs.ls(v, detail=False):
                     # loop over the chunks and copy the references
                     if ".z" in fn:
                         continue
                     key_parts = fn.split("/")[-1].split(".")
                     key = f"{var or v}/"
@@ -562,40 +567,74 @@
     """
     out = {}
     if path is None:
         path = ""
     else:
         path = "/".join(path.rstrip(".").rstrip("/").split(".")) + "/"
 
+    def _replace(l: list, i: int, v) -> list:
+        l = l.copy()
+        l[i] = v
+        return l
+
+    n_files = len(files)
+
+    chunks_offset = 0
     for i, fn in enumerate(files):
         fs = fsspec.filesystem("reference", fo=fn, **(storage_options or {}))
-        zdata = ujson.load(fs.open(f"{path}.zarray"))
+        zarray = ujson.load(fs.open(f"{path}.zarray"))
+        shape = zarray["shape"]
+        chunks = zarray["chunks"]
+        n_chunks, rem = divmod(shape[axis], chunks[axis])
+        n_chunks += rem > 0
+
         if i == 0:
-            shape = zdata["shape"]
-            chunks = zdata["chunks"]
-            chunks_per_file = int(shape[axis] / chunks[axis])
-            shape[axis] *= len(files)
-            zdata["shape"] = shape
-            out[f"{path}.zarray"] = ujson.dumps(zdata)
+            base_shape = _replace(shape, axis, None)
+            base_chunks = chunks
+            # result_* are modified in-place
+            result_zarray = zarray
+            result_shape = shape
             for name in [".zgroup", ".zattrs", f"{path}.zattrs"]:
                 if name in fs.references:
                     out[name] = fs.references[name]
+        else:
+            result_shape[axis] += shape[axis]
+
+        # Safety checks
         if check_arrays:
-            if shape != zdata["shape"]:
-                raise ValueError(f"Incompatible array shapes at {fn}")
-            if chunks != zdata["chunks"]:
-                raise ValueError(f"Incompatible array chunks at {fn}")
+            if _replace(shape, axis, None) != base_shape:
+                expected_shape = (
+                    f"[{', '.join(map(str, _replace(base_shape, axis, '*')))}]"
+                )
+                raise ValueError(
+                    f"Incompatible array shape at index {i}. Expected {expected_shape}, got {shape}."
+                )
+            if chunks != base_chunks:
+                raise ValueError(
+                    f"Incompatible array chunks at index {i}. Expected {base_chunks}, got {chunks}."
+                )
+            if i < (n_files - 1) and rem != 0:
+                raise ValueError(
+                    f"Array at index {i} has irregular chunking at its boundary. "
+                    "This is only allowed for the final array."
+                )
+
+        # Referencing the offset chunks
         for key in fs.find(""):
             if key.startswith(f"{path}.z") or not key.startswith(path):
                 continue
             parts = key.lstrip(path).split(key_seperator)
-            parts[axis] = str(int(parts[axis]) + i * chunks_per_file)
+            parts[axis] = str(int(parts[axis]) + chunks_offset)
             key2 = path + key_seperator.join(parts)
             out[key2] = fs.references[key]
 
+        chunks_offset += n_chunks
+
+    out[f"{path}.zarray"] = ujson.dumps(result_zarray)
+
     return consolidate(out)
 
 
 def auto_dask(
     urls: List[str],
     single_driver: str,
     single_kwargs: dict,
@@ -638,37 +677,45 @@
 
     # make delayed functions
     single_task = dask.delayed(lambda x: single_driver(x, **single_kwargs).translate())
     post = mzz_kwargs.pop("postprocess", None)
     inline = mzz_kwargs.pop("inline_threshold", None)
     # TODO: if single files produce list of reference sets (e.g., grib2)
     batch_task = dask.delayed(
-        lambda u, x: MultiZarrToZarr(u, indicts=x, **mzz_kwargs).translate()
+        lambda u, x: MultiZarrToZarr(
+            u,
+            indicts=x,
+            remote_protocol=remote_protocol,
+            remote_options=remote_options,
+            **mzz_kwargs,
+        ).translate()
     )
 
     # sort out kwargs
     dims = mzz_kwargs.get("concat_dims", [])
     dims += [k for k in mzz_kwargs.get("coo_map", []) if k not in dims]
     kwargs = {"concat_dims": dims}
     if post:
         kwargs["postprocess"] = post
     if inline:
         kwargs["inline_threshold"] = inline
     for field in ["remote_protocol", "remote_options", "coo_dtypes", "identical_dims"]:
         if field in mzz_kwargs:
             kwargs[field] = mzz_kwargs[field]
     final_task = dask.delayed(
-        lambda x: MultiZarrToZarr(x, **kwargs).translate(filename, output_options)
+        lambda x: MultiZarrToZarr(
+            x, remote_options=remote_options, remote_protocol=remote_protocol, **kwargs
+        ).translate(filename, output_options)
     )
 
     # make delayed calls
     tasks = [single_task(u) for u in urls]
-    tasks_per_batch = len(tasks) // n_batches
+    tasks_per_batch = -(-len(tasks) // n_batches)
     tasks2 = []
-    for batch in range(tasks_per_batch + 1):
+    for batch in range(n_batches):
         in_tasks = tasks[batch * tasks_per_batch : (batch + 1) * tasks_per_batch]
         u = urls[batch * tasks_per_batch : (batch + 1) * tasks_per_batch]
         if in_tasks:
             # skip if on last iteration and no remaining tasks
             tasks2.append(batch_task(u, in_tasks))
     return dask.compute(final_task(tasks2))[0]
```

### Comparing `kerchunk-0.1.0/kerchunk/fits.py` & `kerchunk-0.1.1/kerchunk/fits.py`

 * *Files identical despite different names*

### Comparing `kerchunk-0.1.0/kerchunk/grib2.py` & `kerchunk-0.1.1/kerchunk/grib2.py`

 * *Files identical despite different names*

### Comparing `kerchunk-0.1.0/kerchunk/hdf.py` & `kerchunk-0.1.1/kerchunk/hdf.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,15 +270,15 @@
                             }
                             kwargs["object_codec"] = FillStringsCodec(
                                 dtype="S16", id_map=mapping
                             )
                             fill = " "
                         else:
                             raise NotImplementedError
-                    elif _is_netcdf_datetime(h5obj):
+                    elif _is_netcdf_datetime(h5obj) or _is_netcdf_variable(h5obj):
                         fill = None
                     else:
                         fill = h5obj.fillvalue
                     if h5obj.dtype.kind == "V":
                         fill = None
                         if self.vlen == "encode":
                             assert len(cinfo) == 1
@@ -548,7 +548,11 @@
 def _is_netcdf_datetime(dataset: h5py.Dataset):
     units = dataset.attrs.get("units")
     if isinstance(units, bytes):
         units = units.decode("utf-8")
     # This is the same heuristic used by xarray
     # https://github.com/pydata/xarray/blob/f8bae5974ee2c3f67346298da12621af4cae8cf8/xarray/coding/times.py#L670
     return units and "since" in units
+
+
+def _is_netcdf_variable(dataset: h5py.Dataset):
+    return any("_Netcdf4" in _ for _ in dataset.attrs)
```

### Comparing `kerchunk-0.1.0/kerchunk/netCDF3.py` & `kerchunk-0.1.1/kerchunk/netCDF3.py`

 * *Files identical despite different names*

### Comparing `kerchunk-0.1.0/kerchunk/tiff.py` & `kerchunk-0.1.1/kerchunk/tiff.py`

 * *Files identical despite different names*

### Comparing `kerchunk-0.1.0/kerchunk/utils.py` & `kerchunk-0.1.1/kerchunk/utils.py`

 * *Files identical despite different names*

### Comparing `kerchunk-0.1.0/kerchunk/zarr.py` & `kerchunk-0.1.1/kerchunk/zarr.py`

 * *Files identical despite different names*

### Comparing `kerchunk-0.1.0/kerchunk.egg-info/PKG-INFO` & `kerchunk-0.1.1/kerchunk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kerchunk
-Version: 0.1.0
+Version: 0.1.1
 Summary: Functions to make reference descriptions for ReferenceFileSystem
 Home-page: https://github.com/fsspec/kerchunk
 Author: Martin Durant
 Author-email: martin.durant@alumni.utoronto.ca
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `kerchunk-0.1.0/kerchunk.egg-info/SOURCES.txt` & `kerchunk-0.1.1/kerchunk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kerchunk-0.1.0/setup.cfg` & `kerchunk-0.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `kerchunk-0.1.0/setup.py` & `kerchunk-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `kerchunk-0.1.0/versioneer.py` & `kerchunk-0.1.1/versioneer.py`

 * *Files identical despite different names*

