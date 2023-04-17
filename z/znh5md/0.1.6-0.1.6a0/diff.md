# Comparing `tmp/znh5md-0.1.6.tar.gz` & `tmp/znh5md-0.1.6a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "znh5md-0.1.6.tar", max compression
+gzip compressed data, was "znh5md-0.1.6a0.tar", max compression
```

## Comparing `znh5md-0.1.6.tar` & `znh5md-0.1.6a0.tar`

### file list

```diff
@@ -1,15 +1,12 @@
--rw-r--r--   0        0        0    13575 2023-02-10 13:53:08.586838 znh5md-0.1.6/LICENSE
--rw-r--r--   0        0        0     2955 2023-04-17 20:41:06.339576 znh5md-0.1.6/README.md
--rw-r--r--   0        0        0     1166 2023-04-17 20:41:06.349576 znh5md-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      450 2023-04-17 20:41:06.349576 znh5md-0.1.6/znh5md/__init__.py
--rw-r--r--   0        0        0     1404 2023-04-17 20:41:06.349576 znh5md-0.1.6/znh5md/cli.py
--rw-r--r--   0        0        0     3638 2023-04-17 21:18:33.805011 znh5md-0.1.6/znh5md/format/__init__.py
--rw-r--r--   0        0        0      249 2023-03-26 13:37:32.418733 znh5md-0.1.6/znh5md/io/__init__.py
--rw-r--r--   0        0        0     9426 2023-04-03 11:34:58.032893 znh5md-0.1.6/znh5md/io/base.py
--rw-r--r--   0        0        0     7467 2023-04-17 21:18:33.805011 znh5md-0.1.6/znh5md/io/reader.py
--rw-r--r--   0        0        0      179 2023-03-26 12:05:45.108922 znh5md-0.1.6/znh5md/utils.py
--rw-r--r--   0        0        0      268 2023-04-17 20:41:06.349576 znh5md-0.1.6/znh5md/znh5md/__init__.py
--rw-r--r--   0        0        0      366 2023-04-17 20:41:06.349576 znh5md-0.1.6/znh5md/znh5md/base.py
--rw-r--r--   0        0        0     4431 2023-04-17 21:18:33.805011 znh5md-0.1.6/znh5md/znh5md/h5ase.py
--rw-r--r--   0        0        0     7391 2023-04-17 20:41:06.349576 znh5md-0.1.6/znh5md/znh5md/h5dask.py
--rw-r--r--   0        0        0     3719 1970-01-01 00:00:00.000000 znh5md-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    13575 2023-02-10 13:53:08.586838 znh5md-0.1.6a0/LICENSE
+-rw-r--r--   0        0        0     2613 2023-03-28 13:29:46.018406 znh5md-0.1.6a0/README.md
+-rw-r--r--   0        0        0     1083 2023-04-03 14:36:35.844540 znh5md-0.1.6a0/pyproject.toml
+-rw-r--r--   0        0        0      299 2023-03-26 12:05:45.098922 znh5md-0.1.6a0/znh5md/__init__.py
+-rw-r--r--   0        0        0     1404 2023-04-03 11:34:58.022893 znh5md-0.1.6a0/znh5md/cli.py
+-rw-r--r--   0        0        0     3589 2023-04-03 13:19:42.924739 znh5md-0.1.6a0/znh5md/format/__init__.py
+-rw-r--r--   0        0        0      249 2023-03-26 13:37:32.418733 znh5md-0.1.6a0/znh5md/io/__init__.py
+-rw-r--r--   0        0        0     9426 2023-04-03 11:34:58.032893 znh5md-0.1.6a0/znh5md/io/base.py
+-rw-r--r--   0        0        0     7142 2023-04-03 11:34:58.032893 znh5md-0.1.6a0/znh5md/io/reader.py
+-rw-r--r--   0        0        0      179 2023-03-26 12:05:45.108922 znh5md-0.1.6a0/znh5md/utils.py
+-rw-r--r--   0        0        0     9109 2023-04-03 14:33:48.496359 znh5md-0.1.6a0/znh5md/znh5md/__init__.py
+-rw-r--r--   0        0        0     3335 1970-01-01 00:00:00.000000 znh5md-0.1.6a0/PKG-INFO
```

### Comparing `znh5md-0.1.6/LICENSE` & `znh5md-0.1.6a0/LICENSE`

 * *Files identical despite different names*

### Comparing `znh5md-0.1.6/README.md` & `znh5md-0.1.6a0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -2,18 +2,14 @@
 [![Coverage Status](https://coveralls.io/repos/github/zincware/ZnH5MD/badge.svg?branch=main)](https://coveralls.io/github/zincware/ZnH5MD?branch=main)
 [![PyPI version](https://badge.fury.io/py/znh5md.svg)](https://badge.fury.io/py/znh5md)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/zincware/ZnH5MD/HEAD)
 
 # ZnH5MD - High Performance Interface for H5MD Trajectories
 
 ZnH5MD allows easy access to simulation results from H5MD trajectories.
-It provides a Python interface and can convert existing data to H5MD files as well as export to other formats.
-```
-pip install znh5md["daskk"]
-```
 
 ## Example
 In the following example we investigate an H5MD dump from LAMMPS with 1000 atoms and 201 configurations:
 
 ```python
 import znh5md
 
@@ -63,10 +59,7 @@
 
 ## CLI
 ZnH5MD provides a small set of CLI tools:
 
 - `znh5md view <file.h5>` to view the File using `ase.visualize`
 - `znh5md export <file.h5> <file.xyz>` to export the file to `.xyz` or any other supported file format
 - `znh5md convert <file.xyz> <file.h5>` to save a `file.xyz` as `file.h5` in the H5MD standard.
-
-## More examples
-A complete documentation is still work in progress. In the meantime, I can recommend looking at the tests, especially `test_znh5md.py` to learn more about slicing and batching.
```

### Comparing `znh5md-0.1.6/pyproject.toml` & `znh5md-0.1.6a0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "znh5md"
-version = "0.1.6"
+version = "0.1.6a0"
 description = "High Performance Interface for H5MD Trajectories"
 authors = ["zincwarecode <zincwarecode@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 h5py = "^3.7.0"
-dask = {extras = ["array"], version = "^2022.11.1", optional = true}
+dask = {extras = ["array"], version = "^2022.11.1"}
 ase = "^3.22.1"
 tqdm = "^4.65.0"
-typer = {extras = ["all"], version = "^0.7.0"}
+typer = "^0.7.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 isort = "^5.12.0"
 ruff = "^0.0.256"
 pytest = "^7.2.0"
 graphviz = "^0.20.1"
@@ -27,17 +27,14 @@
 
 [tool.poetry.group.notebook.dependencies]
 jupyterlab = "^3.5.0"
 
 [tool.poetry.scripts]
 znh5md = 'znh5md.cli:app'
 
-[tool.poetry.extras]
-dask = ["dask"]
-
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 90
 preview = true
```

### Comparing `znh5md-0.1.6/znh5md/cli.py` & `znh5md-0.1.6a0/znh5md/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
     data = znh5md.ASEH5MD(file)
     ase.visualize.view(data.get_atoms_list())
 
 
 @app.command()
 def export(file: str, output: str):
-    """Export a H5MD File into the output file."""
+    """export a H5MD File into the output file."""
     import znh5md
 
     data = znh5md.ASEH5MD(file)
     for atom in tqdm.tqdm(data.get_atoms_list(), ncols=120):
         ase.io.write(output, atom, append=True)
```

### Comparing `znh5md-0.1.6/znh5md/format/__init__.py` & `znh5md-0.1.6a0/znh5md/format/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,14 @@
     boundary: str = "boundary"
     position: str = "position"
     energy: str = "energy"
     species: str = "species"
     forces: str = "forces"
     stress: str = "stress"
     velocity: str = "velocity"
-    momentum: str = "momentum"
     pbc: str = "pbc"
     dimension: str = "dimension"
 
     @staticmethod
     def encode_boundary(value) -> np.ndarray:
         return np.array(
             [
@@ -53,15 +52,14 @@
 
 
 PARTICLES_GRP = [
     GRP.position,
     GRP.species,
     GRP.forces,
     GRP.velocity,
-    GRP.momentum,
     GRP.pbc,
     GRP.dimension,
     GRP.edges,
     GRP.boundary,
 ]
 
 OBSERVABLES_GRP = [GRP.energy, GRP.stress]
```

### Comparing `znh5md-0.1.6/znh5md/io/base.py` & `znh5md-0.1.6a0/znh5md/io/base.py`

 * *Files identical despite different names*

### Comparing `znh5md-0.1.6/znh5md/io/reader.py` & `znh5md-0.1.6a0/znh5md/io/reader.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,21 +73,14 @@
     def _get_forces(self, atoms: list[ase.Atoms]) -> np.ndarray:
         data = [x.get_forces() for x in atoms]
         try:
             return np.array(data).astype(float)
         except ValueError:
             return self._fill_with_nan(data).astype(float)
 
-    def _get_momenta(self, atoms: list[ase.Atoms]) -> np.ndarray:
-        data = [x.arrays["momenta"] for x in atoms]
-        try:
-            return np.array(data).astype(float)
-        except ValueError:
-            return self._fill_with_nan(data).astype(float)
-
     def _get_stress(self, atoms: list[ase.Atoms]) -> np.ndarray:
         return np.array([x.get_stress() for x in atoms]).astype(float)
 
     def _get_edges(self, atoms: list[ase.Atoms]) -> np.ndarray:
         return np.array([x.get_cell() for x in atoms]).astype(float)
 
     def _get_pbc(self, atoms: list[ase.Atoms]) -> np.ndarray:
@@ -116,15 +109,14 @@
                 GRP.position: self._get_positions,
                 GRP.energy: self._get_energy,
                 GRP.species: self._get_species,
                 GRP.forces: self._get_forces,
                 GRP.stress: self._get_stress,
                 GRP.edges: self._get_edges,
                 GRP.boundary: self._get_boundary,
-                GRP.momentum: self._get_momenta,
             }
             if self.use_pbc_group:
                 functions[GRP.pbc] = self._get_pbc
 
             for name in group_names or functions:
                 if name not in functions:
                     raise ValueError(f"Value {name} not supported")
@@ -132,15 +124,15 @@
                 try:
                     value = functions[name](self.atoms[start_index:stop_index])
                     data[name] = FixedStepTimeChunk(
                         value=value,
                         step=self.step,
                         time=self.time,
                     )
-                except (PropertyNotImplementedError, RuntimeError, KeyError) as err:
+                except (PropertyNotImplementedError, RuntimeError) as err:
                     if group_names is not None:
                         # if the property was specifically selected, raise the error
                         raise err
                     else:
                         log.debug(f"Skipping {name} because {err}")
 
             if self.atoms[0].calc is not None and self.save_atoms_results:
```

### Comparing `znh5md-0.1.6/PKG-INFO` & `znh5md-0.1.6a0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,35 @@
 Metadata-Version: 2.1
 Name: znh5md
-Version: 0.1.6
+Version: 0.1.6a0
 Summary: High Performance Interface for H5MD Trajectories
 License: Apache-2.0
 Author: zincwarecode
 Author-email: zincwarecode@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Provides-Extra: dask
 Requires-Dist: ase (>=3.22.1,<4.0.0)
-Requires-Dist: dask[array] (>=2022.11.1,<2023.0.0) ; extra == "dask"
+Requires-Dist: dask[array] (>=2022.11.1,<2023.0.0)
 Requires-Dist: h5py (>=3.7.0,<4.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
-Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
+Requires-Dist: typer (>=0.7.0,<0.8.0)
 Description-Content-Type: text/markdown
 
 [![zincware](https://img.shields.io/badge/Powered%20by-zincware-darkcyan)](https://github.com/zincware)
 [![Coverage Status](https://coveralls.io/repos/github/zincware/ZnH5MD/badge.svg?branch=main)](https://coveralls.io/github/zincware/ZnH5MD?branch=main)
 [![PyPI version](https://badge.fury.io/py/znh5md.svg)](https://badge.fury.io/py/znh5md)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/zincware/ZnH5MD/HEAD)
 
 # ZnH5MD - High Performance Interface for H5MD Trajectories
 
 ZnH5MD allows easy access to simulation results from H5MD trajectories.
-It provides a Python interface and can convert existing data to H5MD files as well as export to other formats.
-```
-pip install znh5md["daskk"]
-```
 
 ## Example
 In the following example we investigate an H5MD dump from LAMMPS with 1000 atoms and 201 configurations:
 
 ```python
 import znh5md
 
@@ -85,10 +80,7 @@
 ## CLI
 ZnH5MD provides a small set of CLI tools:
 
 - `znh5md view <file.h5>` to view the File using `ase.visualize`
 - `znh5md export <file.h5> <file.xyz>` to export the file to `.xyz` or any other supported file format
 - `znh5md convert <file.xyz> <file.h5>` to save a `file.xyz` as `file.h5` in the H5MD standard.
 
-## More examples
-A complete documentation is still work in progress. In the meantime, I can recommend looking at the tests, especially `test_znh5md.py` to learn more about slicing and batching.
-
```

