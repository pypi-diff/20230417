# Comparing `tmp/graphicle-0.2.8.tar.gz` & `tmp/graphicle-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphicle-0.2.8.tar", last modified: Fri Mar 17 17:36:08 2023, max compression
+gzip compressed data, was "graphicle-0.2.9.tar", last modified: Fri Mar 31 09:59:54 2023, max compression
```

## Comparing `graphicle-0.2.8.tar` & `graphicle-0.2.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 17:36:08.693530 graphicle-0.2.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 17:36:08.689530 graphicle-0.2.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 17:36:08.689530 graphicle-0.2.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-03-17 17:35:54.000000 graphicle-0.2.8/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-03-17 17:35:54.000000 graphicle-0.2.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-03-17 17:35:54.000000 graphicle-0.2.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-03-17 17:35:54.000000 graphicle-0.2.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-03-17 17:35:54.000000 graphicle-0.2.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9244 2023-03-17 17:36:08.693530 graphicle-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8668 2023-03-17 17:35:54.000000 graphicle-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 17:36:08.689530 graphicle-0.2.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-03-17 17:35:54.000000 graphicle-0.2.8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-03-17 17:35:54.000000 graphicle-0.2.8/docs/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-03-17 17:35:54.000000 graphicle-0.2.8/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-17 17:35:54.000000 graphicle-0.2.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 17:36:08.689530 graphicle-0.2.8/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 17:36:08.689530 graphicle-0.2.8/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 17:35:54.000000 graphicle-0.2.8/docs/source/_static/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 17:36:08.689530 graphicle-0.2.8/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 17:35:54.000000 graphicle-0.2.8/docs/source/_templates/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-03-17 17:35:54.000000 graphicle-0.2.8/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-03-17 17:35:54.000000 graphicle-0.2.8/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-03-17 17:35:54.000000 graphicle-0.2.8/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 17:36:08.693530 graphicle-0.2.8/graphicle/
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-03-17 17:35:54.000000 graphicle-0.2.8/graphicle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-17 17:36:08.000000 graphicle-0.2.8/graphicle/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-03-17 17:35:54.000000 graphicle-0.2.8/graphicle/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-03-17 17:35:54.000000 graphicle-0.2.8/graphicle/calculate.py
--rw-r--r--   0 runner    (1001) docker     (123)    75143 2023-03-17 17:35:54.000000 graphicle-0.2.8/graphicle/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7368 2023-03-17 17:35:54.000000 graphicle-0.2.8/graphicle/matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 17:35:54.000000 graphicle-0.2.8/graphicle/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    38655 2023-03-17 17:35:54.000000 graphicle-0.2.8/graphicle/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-03-17 17:35:54.000000 graphicle-0.2.8/graphicle/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 17:36:08.693530 graphicle-0.2.8/graphicle.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9244 2023-03-17 17:36:08.000000 graphicle-0.2.8/graphicle.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-03-17 17:36:08.000000 graphicle-0.2.8/graphicle.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 17:36:08.000000 graphicle-0.2.8/graphicle.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-03-17 17:36:08.000000 graphicle-0.2.8/graphicle.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-17 17:36:08.000000 graphicle-0.2.8/graphicle.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-03-17 17:35:54.000000 graphicle-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-03-17 17:36:08.693530 graphicle-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-17 17:35:54.000000 graphicle-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 17:36:08.693530 graphicle-0.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-03-17 17:35:54.000000 graphicle-0.2.8/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-03-17 17:35:54.000000 graphicle-0.2.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 09:59:54.245954 graphicle-0.2.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 09:59:54.241954 graphicle-0.2.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 09:59:54.245954 graphicle-0.2.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-03-31 09:59:44.000000 graphicle-0.2.9/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-03-31 09:59:44.000000 graphicle-0.2.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-03-31 09:59:44.000000 graphicle-0.2.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-03-31 09:59:44.000000 graphicle-0.2.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-03-31 09:59:44.000000 graphicle-0.2.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9244 2023-03-31 09:59:54.245954 graphicle-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8668 2023-03-31 09:59:44.000000 graphicle-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 09:59:54.245954 graphicle-0.2.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-03-31 09:59:44.000000 graphicle-0.2.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-03-31 09:59:44.000000 graphicle-0.2.9/docs/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-03-31 09:59:44.000000 graphicle-0.2.9/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-31 09:59:44.000000 graphicle-0.2.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 09:59:54.245954 graphicle-0.2.9/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 09:59:54.245954 graphicle-0.2.9/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 09:59:44.000000 graphicle-0.2.9/docs/source/_static/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 09:59:54.245954 graphicle-0.2.9/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 09:59:44.000000 graphicle-0.2.9/docs/source/_templates/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-03-31 09:59:44.000000 graphicle-0.2.9/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-03-31 09:59:44.000000 graphicle-0.2.9/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-03-31 09:59:44.000000 graphicle-0.2.9/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 09:59:54.245954 graphicle-0.2.9/graphicle/
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-03-31 09:59:44.000000 graphicle-0.2.9/graphicle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-31 09:59:54.000000 graphicle-0.2.9/graphicle/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-03-31 09:59:44.000000 graphicle-0.2.9/graphicle/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-03-31 09:59:44.000000 graphicle-0.2.9/graphicle/calculate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75120 2023-03-31 09:59:44.000000 graphicle-0.2.9/graphicle/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7368 2023-03-31 09:59:44.000000 graphicle-0.2.9/graphicle/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 09:59:44.000000 graphicle-0.2.9/graphicle/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    39037 2023-03-31 09:59:44.000000 graphicle-0.2.9/graphicle/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-03-31 09:59:44.000000 graphicle-0.2.9/graphicle/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 09:59:54.245954 graphicle-0.2.9/graphicle.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9244 2023-03-31 09:59:54.000000 graphicle-0.2.9/graphicle.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-03-31 09:59:54.000000 graphicle-0.2.9/graphicle.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 09:59:54.000000 graphicle-0.2.9/graphicle.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-03-31 09:59:54.000000 graphicle-0.2.9/graphicle.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-31 09:59:54.000000 graphicle-0.2.9/graphicle.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-03-31 09:59:44.000000 graphicle-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-03-31 09:59:54.249954 graphicle-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-31 09:59:44.000000 graphicle-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 09:59:54.245954 graphicle-0.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-03-31 09:59:44.000000 graphicle-0.2.9/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-03-31 09:59:44.000000 graphicle-0.2.9/tox.ini
```

### Comparing `graphicle-0.2.8/.github/workflows/publish-to-pypi.yml` & `graphicle-0.2.9/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `graphicle-0.2.8/.gitignore` & `graphicle-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `graphicle-0.2.8/.pre-commit-config.yaml` & `graphicle-0.2.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `graphicle-0.2.8/LICENSE.txt` & `graphicle-0.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `graphicle-0.2.8/PKG-INFO` & `graphicle-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphicle
-Version: 0.2.8
+Version: 0.2.9
 Summary: Encode particle physics data onto graph structures.
 Home-page: https://github.com/jacanchaplais/graphicle
 Author: Jacan Chaplais
 Author-email: jacanchaplais@gmail.com
 License: BSD 3-Clause License
 Project-URL: Documentation, https://graphicle.readthedocs.io
 Classifier: Programming Language :: Python :: 3
```

### Comparing `graphicle-0.2.8/README.md` & `graphicle-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `graphicle-0.2.8/docs/Makefile` & `graphicle-0.2.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `graphicle-0.2.8/docs/make.bat` & `graphicle-0.2.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `graphicle-0.2.8/docs/source/api.rst` & `graphicle-0.2.9/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `graphicle-0.2.8/docs/source/conf.py` & `graphicle-0.2.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `graphicle-0.2.8/docs/source/index.rst` & `graphicle-0.2.9/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `graphicle-0.2.8/graphicle/__init__.py` & `graphicle-0.2.9/graphicle/__init__.py`

 * *Files identical despite different names*

### Comparing `graphicle-0.2.8/graphicle/base.py` & `graphicle-0.2.9/graphicle/base.py`

 * *Files identical despite different names*

### Comparing `graphicle-0.2.8/graphicle/calculate.py` & `graphicle-0.2.9/graphicle/calculate.py`

 * *Files identical despite different names*

### Comparing `graphicle-0.2.8/graphicle/data.py` & `graphicle-0.2.9/graphicle/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -438,15 +438,15 @@
     def __array_wrap__(cls, array: base.BoolVector) -> "MaskArray":
         return cls(array)
 
     def __array_ufunc__(self, ufunc, method, *inputs, **kwargs):
         return _array_ufunc(self, ufunc, method, *inputs, **kwargs)
 
     def __iter__(self) -> ty.Iterator[bool]:
-        yield from map(bool, self.data)
+        return map(bool, self.data)
 
     def copy(self) -> "MaskArray":
         return self.__class__(self._data.copy())
 
     def __repr__(self) -> str:
         return _array_repr(self)
 
@@ -701,14 +701,16 @@
         if not isinstance(key, str):
             raise KeyError("Key must be string.")
         if not isinstance(mask, (MaskArray, type(self))):
             mask = MaskArray(mask)
         self._mask_arrays.update({key: mask})
 
     def __bool__(self) -> bool:
+        if len(self) == 0:
+            return False
         if np.shape(self.data)[0] == 0:
             return False
         return True
 
     def __len__(self) -> int:
         return len(self._mask_arrays)
 
@@ -1172,15 +1174,15 @@
 
     @classmethod
     def __array_wrap__(cls, array: base.AnyVector) -> "MomentumArray":
         return cls(array)
 
     def __iter__(self) -> ty.Iterator[MomentumElement]:
         flat_vals = map(float, self._data.flatten())
-        elems = zip(*(flat_vals,) * 4, strict=True)  # type: ignore
+        elems = zip(*(flat_vals,) * 4)  # type: ignore
         yield from it.starmap(MomentumElement, elems)
 
     def __len__(self) -> int:
         return self._data.shape[0]
 
     def __array__(self) -> base.VoidVector:
         return self.data
@@ -1375,15 +1377,15 @@
         return self.data
 
     def __repr__(self) -> str:
         return _array_repr(self)
 
     def __iter__(self) -> ty.Iterator[ColorElement]:
         flat_vals = map(int, it.chain.from_iterable(self.data))
-        elems = zip(*(flat_vals,) * 2, strict=True)  # type: ignore
+        elems = zip(*(flat_vals,) * 2)
         yield from it.starmap(ColorElement, elems)
 
     @property
     def data(self) -> base.VoidVector:
         """Structured array containing ``('color', 'anticolor')``
         values for particle set.
         """
@@ -1853,15 +1855,15 @@
         return cls(array)
 
     def __repr__(self) -> str:
         return _array_repr(self)
 
     def __iter__(self) -> ty.Iterator[VertexPair]:
         flat_vals = map(int, it.chain.from_iterable(self._data))
-        elems = zip(*(flat_vals,) * 2, strict=True)  # type: ignore
+        elems = zip(*(flat_vals,) * 2)
         yield from it.starmap(VertexPair, elems)
 
     def __len__(self) -> int:
         return len(self._data)
 
     def __bool__(self) -> bool:
         return _truthy(self)
```

### Comparing `graphicle-0.2.8/graphicle/matrix.py` & `graphicle-0.2.9/graphicle/matrix.py`

 * *Files identical despite different names*

### Comparing `graphicle-0.2.8/graphicle/select.py` & `graphicle-0.2.9/graphicle/select.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,24 @@
 DistFunc = ty.Callable[
     [gcl.MomentumArray, gcl.MomentumArray], base.DoubleVector
 ]
 MaskType = ty.Union[gcl.MaskArray, gcl.MaskGroup]
 MaskGeneric = ty.TypeVar("MaskGeneric", gcl.MaskGroup, gcl.MaskArray, MaskType)
 
 
+def _param_check(
+    param: ty.Any, name: str, expected: ty.Type
+) -> ty.Optional[ty.NoReturn]:
+    if not isinstance(param, expected):
+        received = type(param)
+        raise ValueError(
+            f"Expected {name} to be {expected}. Received {received}."
+        )
+
+
 def fastjet_clusters(
     pmu: gcl.MomentumArray,
     radius: float,
     p_val: float,
     pt_cut: ty.Optional[float] = None,
     eta_cut: ty.Optional[float] = None,
     top_k: ty.Optional[int] = None,
@@ -91,14 +101,15 @@
         clustering, in order of descending :math:`p_T`.
 
     Notes
     -----
     ``p_val`` set to ``-1`` gives **anti-kT**, ``0`` gives
     **Cambridge-Aachen**, and ``1`` gives **kT** clusterings.
     """
+    _param_check(pmu, "pmu", gcl.MomentumArray)
     pmu_pyjet = pmu.data[["e", "x", "y", "z"]]
     pmu_pyjet.dtype.names = "E", "px", "py", "pz"
     pmu_pyjet_idx = rfn.append_fields(
         pmu_pyjet, "idx", np.arange(len(pmu_pyjet))
     )
     sequence: ClusterSequence = pyjet.cluster(
         pmu_pyjet_idx, R=radius, p=p_val, ep=True
@@ -921,14 +932,15 @@
 
     Returns
     -------
     MaskArray
         Mask which retains only the particles within ``radius`` of the
         centroid.
     """
+    _param_check(pmu, "pmu", gcl.MomentumArray)
     if mask is not None:
         pmu = pmu[mask]
         event_mask = np.zeros_like(mask, "<?")
     if centre is None:
         eta_mid = (pmu.eta * pmu.pt).sum() / pmu.pt.sum()
         phi_sum_ = (pmu._xy_pol * pmu.pt).sum()
         phi_mid_ = phi_sum_ / np.abs(phi_sum_)
@@ -1093,14 +1105,14 @@
     )
     colored_leaves, colored_leaves_ = it.tee(colored_leaves, 2)
     hard_mask = graph.hard_mask["outgoing"]
     parton_masks = map(op.and_, it.repeat(hard_mask), colored_leaves_)
     parton_pmus = map(op.getitem, it.repeat(graph.pmu), parton_masks)
     parton_centroids = map(op.attrgetter("eta", "phi"), parton_pmus)
     for leaf, centroid in zip(colored_leaves, parton_centroids):
-        leaf[...] = centroid_prune(graph.pmu, radius, leaf, centroid)
+        leaf.data[...] = centroid_prune(graph.pmu, radius, leaf, centroid).data
     hier.recursive_drop(inplace=True)
     flat_hier = hier.flatten("rise")
     flat_hier_final = map(op.itemgetter(graph.final), flat_hier.values())
     return gcl.MaskGroup(
         cl.OrderedDict(zip(flat_hier.keys(), flat_hier_final)), agg_op="or"
     )
```

### Comparing `graphicle-0.2.8/graphicle/transform.py` & `graphicle-0.2.9/graphicle/transform.py`

 * *Files identical despite different names*

### Comparing `graphicle-0.2.8/graphicle.egg-info/PKG-INFO` & `graphicle-0.2.9/graphicle.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphicle
-Version: 0.2.8
+Version: 0.2.9
 Summary: Encode particle physics data onto graph structures.
 Home-page: https://github.com/jacanchaplais/graphicle
 Author: Jacan Chaplais
 Author-email: jacanchaplais@gmail.com
 License: BSD 3-Clause License
 Project-URL: Documentation, https://graphicle.readthedocs.io
 Classifier: Programming Language :: Python :: 3
```

### Comparing `graphicle-0.2.8/graphicle.egg-info/SOURCES.txt` & `graphicle-0.2.9/graphicle.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `graphicle-0.2.8/pyproject.toml` & `graphicle-0.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `graphicle-0.2.8/setup.cfg` & `graphicle-0.2.9/setup.cfg`

 * *Files identical despite different names*

