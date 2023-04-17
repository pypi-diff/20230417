# Comparing `tmp/atlas-ftag-tools-0.0.8.tar.gz` & `tmp/atlas-ftag-tools-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atlas-ftag-tools-0.0.8.tar", last modified: Thu Apr  6 13:18:14 2023, max compression
+gzip compressed data, was "atlas-ftag-tools-0.0.9.tar", last modified: Mon Apr 17 13:48:56 2023, max compression
```

## Comparing `atlas-ftag-tools-0.0.8.tar` & `atlas-ftag-tools-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:18:14.730051 atlas-ftag-tools-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-06 13:17:54.000000 atlas-ftag-tools-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-06 13:18:14.730051 atlas-ftag-tools-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-06 13:17:54.000000 atlas-ftag-tools-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:18:14.730051 atlas-ftag-tools-0.0.8/atlas_ftag_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-06 13:18:14.000000 atlas-ftag-tools-0.0.8/atlas_ftag_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-06 13:18:14.000000 atlas-ftag-tools-0.0.8/atlas_ftag_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 13:18:14.000000 atlas-ftag-tools-0.0.8/atlas_ftag_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 13:18:14.000000 atlas-ftag-tools-0.0.8/atlas_ftag_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-06 13:18:14.000000 atlas-ftag-tools-0.0.8/atlas_ftag_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-06 13:18:14.000000 atlas-ftag-tools-0.0.8/atlas_ftag_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:18:14.730051 atlas-ftag-tools-0.0.8/ftag/
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-06 13:17:54.000000 atlas-ftag-tools-0.0.8/ftag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-04-06 13:17:54.000000 atlas-ftag-tools-0.0.8/ftag/cuts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-04-06 13:17:54.000000 atlas-ftag-tools-0.0.8/ftag/flavour.py
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-04-06 13:17:54.000000 atlas-ftag-tools-0.0.8/ftag/flavours.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:18:14.730051 atlas-ftag-tools-0.0.8/ftag/hdf5/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-06 13:17:54.000000 atlas-ftag-tools-0.0.8/ftag/hdf5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8446 2023-04-06 13:17:54.000000 atlas-ftag-tools-0.0.8/ftag/hdf5/h5reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-04-06 13:17:54.000000 atlas-ftag-tools-0.0.8/ftag/hdf5/h5utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-06 13:17:54.000000 atlas-ftag-tools-0.0.8/ftag/hdf5/h5writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-04-06 13:17:54.000000 atlas-ftag-tools-0.0.8/ftag/mock.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-06 13:17:54.000000 atlas-ftag-tools-0.0.8/ftag/region.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-06 13:17:54.000000 atlas-ftag-tools-0.0.8/ftag/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-04-06 13:17:54.000000 atlas-ftag-tools-0.0.8/ftag/vds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-06 13:17:54.000000 atlas-ftag-tools-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 13:18:14.730051 atlas-ftag-tools-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:48:56.110608 atlas-ftag-tools-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-17 13:48:35.000000 atlas-ftag-tools-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-17 13:48:56.110608 atlas-ftag-tools-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-04-17 13:48:35.000000 atlas-ftag-tools-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:48:56.110608 atlas-ftag-tools-0.0.9/atlas_ftag_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-17 13:48:56.000000 atlas-ftag-tools-0.0.9/atlas_ftag_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-17 13:48:56.000000 atlas-ftag-tools-0.0.9/atlas_ftag_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 13:48:56.000000 atlas-ftag-tools-0.0.9/atlas_ftag_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-17 13:48:56.000000 atlas-ftag-tools-0.0.9/atlas_ftag_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-17 13:48:56.000000 atlas-ftag-tools-0.0.9/atlas_ftag_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-17 13:48:56.000000 atlas-ftag-tools-0.0.9/atlas_ftag_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:48:56.110608 atlas-ftag-tools-0.0.9/ftag/
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-17 13:48:35.000000 atlas-ftag-tools-0.0.9/ftag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-04-17 13:48:35.000000 atlas-ftag-tools-0.0.9/ftag/cuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-04-17 13:48:35.000000 atlas-ftag-tools-0.0.9/ftag/flavour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-04-17 13:48:35.000000 atlas-ftag-tools-0.0.9/ftag/flavours.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:48:56.110608 atlas-ftag-tools-0.0.9/ftag/hdf5/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-17 13:48:35.000000 atlas-ftag-tools-0.0.9/ftag/hdf5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8446 2023-04-17 13:48:35.000000 atlas-ftag-tools-0.0.9/ftag/hdf5/h5reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-04-17 13:48:35.000000 atlas-ftag-tools-0.0.9/ftag/hdf5/h5utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-17 13:48:35.000000 atlas-ftag-tools-0.0.9/ftag/hdf5/h5writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-04-17 13:48:35.000000 atlas-ftag-tools-0.0.9/ftag/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-17 13:48:35.000000 atlas-ftag-tools-0.0.9/ftag/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-17 13:48:35.000000 atlas-ftag-tools-0.0.9/ftag/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-04-17 13:48:35.000000 atlas-ftag-tools-0.0.9/ftag/vds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-17 13:48:35.000000 atlas-ftag-tools-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 13:48:56.114608 atlas-ftag-tools-0.0.9/setup.cfg
```

### Comparing `atlas-ftag-tools-0.0.8/README.md` & `atlas-ftag-tools-0.0.9/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -35,7 +35,31 @@
 See the [h5py documentation](https://docs.h5py.org/en/stable/vds.html) for more information on virtual datasets.
 
 The script is `vds.py` and can be run after installing this package with
 
 ```
 vds <pattern> <output path>
 ```
+
+The `<pattern>` argument should be a quotes enclosed [glob pattern](https://en.wikipedia.org/wiki/Glob_(programming)), for example `"dsid/path/*.h5"`
+
+
+## Calculate WPs
+
+This package contains a script to calculate tagger working points (WPs).
+The script is `working_points.py` and can be run after installing this package with
+
+```
+wps \
+    --ttbar "path/to/ttbar/*.h5" \
+    --tagger GN120220509 \
+    --fx 0.1
+```
+
+Both the `--tagger` and `--fx` options accept a list if you want to get the WPs for multiple taggers.
+
+If you want to use the `ttbar` WPs get the efficiencies and rejections for the `zprime` sample, you can add `--zprime "path/to/zprime/*.h5"` to the command.
+Note that a default selection of $p_T > 250 ~GeV$ to jets in the `zprime` sample.
+
+By default the working points are printed to the terminal, but you can save the results to a YAML file with the `--outfile` option.
+
+Use `--help` for more options and information.
```

### Comparing `atlas-ftag-tools-0.0.8/ftag/cuts.py` & `atlas-ftag-tools-0.0.9/ftag/cuts.py`

 * *Files identical despite different names*

### Comparing `atlas-ftag-tools-0.0.8/ftag/flavour.py` & `atlas-ftag-tools-0.0.9/ftag/flavour.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 from __future__ import annotations
 
 from collections.abc import Generator
 from dataclasses import dataclass
+from pathlib import Path
+
+import yaml
 
 from ftag.cuts import Cuts
 
 
 def remove_suffix(string: str, suffix: str) -> str:
     if string.endswith(suffix):
         return string[: -len(suffix)]
@@ -70,7 +73,14 @@
     def from_cuts(self, cuts: list | Cuts) -> Flavour:
         if isinstance(cuts, list):
             cuts = Cuts.from_list(cuts)
         for flavour in self:
             if flavour.cuts == cuts:
                 return flavour
         raise KeyError(f"Flavour with {cuts} not found")
+
+
+with open(Path(__file__).parent / "flavours.yaml") as f:
+    flavours_yaml = yaml.safe_load(f)
+flavours_dict = {f["name"]: Flavour(cuts=Cuts.from_list(f.pop("cuts")), **f) for f in flavours_yaml}
+assert len(flavours_dict) == len(flavours_yaml), "Duplicate flavour names detected"
+Flavours = FlavourContainer(flavours_dict)
```

### Comparing `atlas-ftag-tools-0.0.8/ftag/flavours.yaml` & `atlas-ftag-tools-0.0.9/ftag/flavours.yaml`

 * *Files identical despite different names*

### Comparing `atlas-ftag-tools-0.0.8/ftag/hdf5/h5reader.py` & `atlas-ftag-tools-0.0.9/ftag/hdf5/h5reader.py`

 * *Files identical despite different names*

### Comparing `atlas-ftag-tools-0.0.8/ftag/hdf5/h5utils.py` & `atlas-ftag-tools-0.0.9/ftag/hdf5/h5utils.py`

 * *Files identical despite different names*

### Comparing `atlas-ftag-tools-0.0.8/ftag/hdf5/h5writer.py` & `atlas-ftag-tools-0.0.9/ftag/hdf5/h5writer.py`

 * *Files identical despite different names*

### Comparing `atlas-ftag-tools-0.0.8/ftag/mock.py` & `atlas-ftag-tools-0.0.9/ftag/mock.py`

 * *Files identical despite different names*

### Comparing `atlas-ftag-tools-0.0.8/ftag/sample.py` & `atlas-ftag-tools-0.0.9/ftag/sample.py`

 * *Files identical despite different names*

### Comparing `atlas-ftag-tools-0.0.8/ftag/vds.py` & `atlas-ftag-tools-0.0.9/ftag/vds.py`

 * *Files 12% similar despite different names*

```diff
@@ -61,17 +61,19 @@
 
     return out_fname
 
 
 def main():
     import argparse
 
-    parser = argparse.ArgumentParser(description="Create a virtual dataset from a glob pattern")
-    parser.add_argument("pattern", type=Path, help="Glob pattern of files to merge")
-    parser.add_argument("output", type=Path, help="Output file name")
+    parser = argparse.ArgumentParser(
+        description="Create a lightweight wrapper around a set of h5 files"
+    )
+    parser.add_argument("pattern", type=Path, help="quotes-enclosed glob pattern of files to merge")
+    parser.add_argument("output", type=Path, help="path to output virtual file")
     args = parser.parse_args()
 
     print(f"Globbing {args.pattern}...")
     create_virtual_file(args.pattern, args.output, overwrite=True)
     with h5py.File(args.output) as f:
         key = list(f.keys())[0]
         num = len(f[key])
```

### Comparing `atlas-ftag-tools-0.0.8/pyproject.toml` & `atlas-ftag-tools-0.0.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,15 @@
   "pytest-cov==4.0.0",
   "pytest_notebook==0.8.1",
   "ipykernel==6.21.3",
 ]
 
 [project.scripts]
 vds = "ftag.vds:main"
+wps = "ftag.wps.working_points:main"
 
 [tool.setuptools]
 packages = ["ftag", "ftag.hdf5"]
 include-package-data = true
 
 [tool.setuptools.dynamic]
 version = {attr = "ftag.__version__"}
```

