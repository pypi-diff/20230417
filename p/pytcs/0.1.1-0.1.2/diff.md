# Comparing `tmp/pytcs-0.1.1.tar.gz` & `tmp/pytcs-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytcs-0.1.1.tar", last modified: Tue Apr  4 09:37:13 2023, max compression
+gzip compressed data, was "pytcs-0.1.2.tar", last modified: Mon Apr 17 13:02:54 2023, max compression
```

## Comparing `pytcs-0.1.1.tar` & `pytcs-0.1.2.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 jupyter-cfabry  (1001) jupyter-cfabry  (1003)        0 2023-04-04 09:37:13.020129 pytcs-0.1.1/
-drwxr-xr-x   0 jupyter-cfabry  (1001) jupyter-cfabry  (1003)        0 2023-04-04 09:37:13.016129 pytcs-0.1.1/.github/
--rw-r--r--   0 jupyter-cfabry  (1001) jupyter-cfabry  (1003)       21 2023-01-31 11:44:57.000000 pytcs-0.1.1/.github/CODEOWNERS
-drwxr-xr-x   0 jupyter-cfabry  (1001) jupyter-cfabry  (1003)        0 2023-04-04 09:37:13.020129 pytcs-0.1.1/.github/workflows/
--rw-r--r--   0 jupyter-cfabry  (1001) jupyter-cfabry  (1003)     3491 2023-04-04 09:34:40.000000 pytcs-0.1.1/.github/workflows/build.yml
--rw-r--r--   0 jupyter-cfabry  (1001) jupyter-cfabry  (1003)     1156 2023-02-01 11:11:37.000000 pytcs-0.1.1/.github/workflows/pytest.yml
--rw-r--r--   0 jupyter-cfabry  (1001) jupyter-cfabry  (1003)      346 2023-02-01 11:11:37.000000 pytcs-0.1.1/.github/workflows/static_analysis.yml
--rw-r--r--   0 jupyter-cfabry  (1001) jupyter-cfabry  (1003)     1868 2022-11-17 12:15:09.000000 pytcs-0.1.1/.gitignore
--rw-r--r--   0 jupyter-cfabry  (1001) jupyter-cfabry  (1003)     1264 2023-01-31 11:44:57.000000 pytcs-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 jupyter-cfabry  (1001) jupyter-cfabry  (1003)     1520 2022-11-17 12:15:09.000000 pytcs-0.1.1/LICENSE
--rw-r--r--   0 jupyter-cfabry  (1001) jupyter-cfabry  (1003)       28 2023-04-04 09:34:40.000000 pytcs-0.1.1/MANIFEST.in
--rw-r--r--   0 jupyter-cfabry  (1001) jupyter-cfabry  (1003)    10459 2023-04-04 09:37:13.020129 pytcs-0.1.1/PKG-INFO
--rw-------   0 jupyter-cfabry  (1001) jupyter-cfabry  (1003)     7654 2023-04-04 09:08:58.000000 pytcs-0.1.1/README.md
-drwxr-xr-x   0 jupyter-cfabry  (1001) jupyter-cfabry  (1003)        0 2023-04-04 09:37:13.016129 pytcs-0.1.1/devtools/
-drwxr-xr-x   0 jupyter-cfabry  (1001) jupyter-cfabry  (1003)        0 2023-04-04 09:37:13.020129 pytcs-0.1.1/devtools/conda.recipe/
--rw-r--r--   0 jupyter-cfabry  (1001) jupyter-cfabry  (1003)      214 2023-04-04 09:34:40.000000 pytcs-0.1.1/devtools/conda.recipe/build_env.yml
--rw-r--r--   0 jupyter-cfabry  (1001) jupyter-cfabry  (1003)     1491 2023-04-04 09:34:40.000000 pytcs-0.1.1/devtools/conda.recipe/meta.yaml
--rw-r--r--   0 jupyter-cfabry  (1001) jupyter-cfabry  (1003)     3051 2023-04-04 09:34:40.000000 pytcs-0.1.1/pyproject.toml
-drwxr-xr-x   0 jupyter-cfabry  (1001) jupyter-cfabry  (1003)        0 2023-04-04 09:37:13.020129 pytcs-0.1.1/pytcs/
--rw-r--r--   0 jupyter-cfabry  (1001) jupyter-cfabry  (1003)      114 2022-11-17 12:15:09.000000 pytcs-0.1.1/pytcs/__init__.py
--rw-r--r--   0 jupyter-cfabry  (1001) jupyter-cfabry  (1003)      160 2023-04-04 09:37:12.000000 pytcs-0.1.1/pytcs/_version.py
--rw-r--r--   0 jupyter-cfabry  (1001) jupyter-cfabry  (1003)     3767 2023-01-31 11:44:57.000000 pytcs-0.1.1/pytcs/helpers.py
--rw-r--r--   0 jupyter-cfabry  (1001) jupyter-cfabry  (1003)    24997 2023-02-01 11:50:49.000000 pytcs-0.1.1/pytcs/pytcs.py
-drwxr-xr-x   0 jupyter-cfabry  (1001) jupyter-cfabry  (1003)        0 2023-04-04 09:37:13.020129 pytcs-0.1.1/pytcs.egg-info/
--rw-r--r--   0 jupyter-cfabry  (1001) jupyter-cfabry  (1003)    10459 2023-04-04 09:37:12.000000 pytcs-0.1.1/pytcs.egg-info/PKG-INFO
--rw-r--r--   0 jupyter-cfabry  (1001) jupyter-cfabry  (1003)      483 2023-04-04 09:37:13.000000 pytcs-0.1.1/pytcs.egg-info/SOURCES.txt
--rw-r--r--   0 jupyter-cfabry  (1001) jupyter-cfabry  (1003)        1 2023-04-04 09:37:12.000000 pytcs-0.1.1/pytcs.egg-info/dependency_links.txt
--rw-r--r--   0 jupyter-cfabry  (1001) jupyter-cfabry  (1003)      161 2023-04-04 09:37:12.000000 pytcs-0.1.1/pytcs.egg-info/requires.txt
--rw-r--r--   0 jupyter-cfabry  (1001) jupyter-cfabry  (1003)       36 2023-04-04 09:37:12.000000 pytcs-0.1.1/pytcs.egg-info/top_level.txt
--rw-r--r--   0 jupyter-cfabry  (1001) jupyter-cfabry  (1003)       38 2023-04-04 09:37:13.020129 pytcs-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:02:54.250518 pytcs-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:02:54.250518 pytcs-0.1.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-17 13:02:31.000000 pytcs-0.1.2/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:02:54.250518 pytcs-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-04-17 13:02:31.000000 pytcs-0.1.2/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-17 13:02:31.000000 pytcs-0.1.2/.github/workflows/pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-17 13:02:31.000000 pytcs-0.1.2/.github/workflows/static_analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-04-17 13:02:31.000000 pytcs-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-17 13:02:31.000000 pytcs-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-17 13:02:31.000000 pytcs-0.1.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-17 13:02:31.000000 pytcs-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-17 13:02:31.000000 pytcs-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10459 2023-04-17 13:02:54.250518 pytcs-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7654 2023-04-17 13:02:31.000000 pytcs-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:02:54.250518 pytcs-0.1.2/devtools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:02:54.250518 pytcs-0.1.2/devtools/conda.recipe/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-17 13:02:31.000000 pytcs-0.1.2/devtools/conda.recipe/build_env.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-17 13:02:31.000000 pytcs-0.1.2/devtools/conda.recipe/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-04-17 13:02:31.000000 pytcs-0.1.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:02:54.250518 pytcs-0.1.2/pytcs/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-17 13:02:31.000000 pytcs-0.1.2/pytcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-17 13:02:54.000000 pytcs-0.1.2/pytcs/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-04-17 13:02:31.000000 pytcs-0.1.2/pytcs/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26074 2023-04-17 13:02:31.000000 pytcs-0.1.2/pytcs/pytcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:02:54.250518 pytcs-0.1.2/pytcs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10459 2023-04-17 13:02:54.000000 pytcs-0.1.2/pytcs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-17 13:02:54.000000 pytcs-0.1.2/pytcs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 13:02:54.000000 pytcs-0.1.2/pytcs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-17 13:02:54.000000 pytcs-0.1.2/pytcs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-17 13:02:54.000000 pytcs-0.1.2/pytcs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 13:02:54.250518 pytcs-0.1.2/setup.cfg
```

### Comparing `pytcs-0.1.1/.github/workflows/build.yml` & `pytcs-0.1.2/.github/workflows/build.yml`

 * *Files 4% similar despite different names*

```diff
@@ -98,20 +98,20 @@
 
       - name: pip dist install
         run: |
           pip install ${{ env.SDIST_FILE }}[all,test]
       - name: run pytest
         run: |
           pytest
-#      - name: set pypi test repo defaults
-#        run: |
-#          echo "pypi_repo=testpypi" >> $GITHUB_ENV
-#          echo "pypi_token=${{ secrets.TESTPYPI_UPLOAD }}" >> $GITHUB_ENV
-#      - name: set pypi main repo for release
-#        if: github.event_name == 'release'
-#        run: |
-#          echo "pypi_repo=pypi" >> $GITHUB_ENV
-#          echo "pypi_token=${{ secrets.PYPI_UPLOAD }}" >> $GITHUB_ENV
-#      - name: pypi release
-#        if: startsWith(github.ref, 'refs/tags/') || (github.event_name == 'release')
-#        run: |
-#          python -m twine upload --repository $pypi_repo dist/* -u __token__ -p $pypi_token
+      - name: set pypi test repo defaults
+        run: |
+          echo "pypi_repo=testpypi" >> $GITHUB_ENV
+          echo "pypi_token=${{ secrets.TESTPYPI_UPLOAD }}" >> $GITHUB_ENV
+      - name: set pypi main repo for release
+        if: github.event_name == 'release'
+        run: |
+          echo "pypi_repo=pypi" >> $GITHUB_ENV
+          echo "pypi_token=${{ secrets.PYPI_UPLOAD }}" >> $GITHUB_ENV
+      - name: pypi release
+        if: startsWith(github.ref, 'refs/tags/') || (github.event_name == 'release')
+        run: |
+          python -m twine upload --repository $pypi_repo dist/* -u __token__ -p $pypi_token
```

### Comparing `pytcs-0.1.1/.github/workflows/pytest.yml` & `pytcs-0.1.2/.github/workflows/pytest.yml`

 * *Files 18% similar despite different names*

```diff
@@ -14,14 +14,22 @@
     name: pytest
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-latest]
         py: ['3.8', '3.9', '3.10', '3.11']
+        pandas: [ '1.*' ]
+        include:
+          - os: ubuntu-latest
+            py: '3.10'
+            pandas: '1.3'
+          - os: ubuntu-latest
+            py: '3.10'
+            pandas: '1.4'
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: '0' # Fetch all history for all tags and branches
 
       - uses: CagtayFabry/pydeps2env@main
         with:
```

### Comparing `pytcs-0.1.1/.gitignore` & `pytcs-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pytcs-0.1.1/.pre-commit-config.yaml` & `pytcs-0.1.2/.pre-commit-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -23,25 +23,25 @@
       - id: mdformat
         additional_dependencies:
           - mdformat-gfm
           - mdformat-black
           - mdformat-config
   # ----- Python formatting -----
   - repo: https://github.com/psf/black
-    rev: 22.12.0
+    rev: 23.3.0
     hooks:
       - id: black
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.238
+    rev: v0.0.261
     hooks:
       - id: ruff
         args:
           - --quiet
           - --fix
   - repo: https://github.com/tox-dev/pyproject-fmt
-    rev: 0.6.0
+    rev: 0.9.2
     hooks:
       - id: pyproject-fmt
   - repo: https://github.com/abravalheri/validate-pyproject
-    rev: v0.12.1
+    rev: v0.12.2
     hooks:
       - id: validate-pyproject
```

### Comparing `pytcs-0.1.1/LICENSE` & `pytcs-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytcs-0.1.1/PKG-INFO` & `pytcs-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytcs
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python API for processing TwinCAT Scope data files
 Author-email: Cagtay Fabry <cagtay.fabry@bam.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Cagtay Fabry
         All rights reserved.
```

### Comparing `pytcs-0.1.1/README.md` & `pytcs-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pytcs-0.1.1/devtools/conda.recipe/meta.yaml` & `pytcs-0.1.2/devtools/conda.recipe/meta.yaml`

 * *Files identical despite different names*

### Comparing `pytcs-0.1.1/pytcs/helpers.py` & `pytcs-0.1.2/pytcs/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,32 +29,32 @@
         # "STRING_255": (, ),
         # "IMAGE": (, ),
     }
     return tc3_dtypes
 
 
 # list of channel metadata keys
-_channel_meta_keys = dict(
-    SymbolComment="symbol_comment",
-    DataType="data_type",
-    SampleTime="sample_time",
-    VariableSize="variable_size",
-    SymbolBased="symbol_based",
-    IndexGroup="index_group",
-    IndexOffset="index_offset",
-    SymbolName="symbol_name",
-    NetID="net_id",
-    Port="port",
-    Offset="offset",
-    ScaleFactor="scale_factor",
-    BitMask="bit_mask",
-    Unit="unit",
-    UnitScaleFactor="unit_scale_factor",
-    UnitOffset="unit_offset",
-)
+_channel_meta_keys = {
+    "SymbolComment": "symbol_comment",
+    "DataType": "data_type",
+    "SampleTime": "sample_time",
+    "VariableSize": "variable_size",
+    "SymbolBased": "symbol_based",
+    "IndexGroup": "index_group",
+    "IndexOffset": "index_offset",
+    "SymbolName": "symbol_name",
+    "NetID": "net_id",
+    "Port": "port",
+    "Offset": "offset",
+    "ScaleFactor": "scale_factor",
+    "BitMask": "bit_mask",
+    "Unit": "unit",
+    "UnitScaleFactor": "unit_scale_factor",
+    "UnitOffset": "unit_offset",
+}
 _channel_meta_keys = bidict(_channel_meta_keys)
 
 # Offset from filetime-Origin to 1970-1-1 00.00:00 in MS filetime units
 MS_FILETIME_OFFSET = int(116444736000000000)
 
 
 def filetime_to_dt(ft: int) -> datetime:
```

### Comparing `pytcs-0.1.1/pytcs/pytcs.py` & `pytcs-0.1.2/pytcs/pytcs.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """pytcs - Python API for reading TwinCAT Scope Files."""
 from __future__ import annotations
 
 import gzip
 from collections.abc import ItemsView, Iterator, ValuesView
 from dataclasses import dataclass, field
 from datetime import datetime
+from io import BytesIO, IOBase, StringIO
 from itertools import chain
 from pathlib import Path
 from typing import TYPE_CHECKING, KeysView, Union
 from warnings import warn
 
 import numpy as np
 import pandas as pd
@@ -75,14 +76,15 @@
         """Channel as xarray dataarray."""
         import xarray as xr
 
         if not (lt := len(self.time)) == (lv := len(self.values)):
             warn(
                 f"Mismatch in time and value length for channel {self.name}",
                 UserWarning,
+                stacklevel=2,
             )
             return xr.DataArray(
                 data=self.values[: min(lt, lv)],
                 dims=["time"],
                 coords={"time": self.time[: min(lt, lv)]},
                 name=self.name,
             )
@@ -138,18 +140,19 @@
 
 
 class ScopeFile:
     """Class for reading TwinCAT Scope files."""
 
     def __init__(
         self,
-        filepath_or_buffer: Union[Path, str],
+        filepath_or_buffer: Union[Path, str, StringIO, BytesIO],
         delimiter: str = None,
         decimal: str = None,
         encoding: str = "utf-8",
+        compression: str = "infer",
     ):
         """Open a TwinCAT Scope file.
 
         Parameters
         ----------
         filepath_or_buffer
             The file or buffer to open.
@@ -159,30 +162,40 @@
             The column delimiter used in the file.
             If no explicit value is given this is inferred form the file header.
         decimal
             The decimal delimiter used in the file.
             If no explicit value is given this is inferred form the file header.
         encoding
             File encoding (default: 'utf-8')
+        compression
+            File or data compression (default: 'infer' / autodetect)
 
         """
         self._delimiter: str = delimiter
         self._decimal: str = decimal
 
         self._file = filepath_or_buffer  # file handle, buffer etc.
         self._encoding: str = encoding
+        self._compression = compression
         self._meta: dict = {}
         self.start_time: datetime = None
         self.run_time: timedelta = None
 
         self._channels: dict[str, ScopeChannel] = {}
 
         self._data: dict[int, np.ndarray] = {}  # column data
 
-        if Path(filepath_or_buffer).suffix in [".gz", ".gzip"]:
+        # determine correct way to open file
+        if isinstance(filepath_or_buffer, StringIO):
+            self._read_header(filepath_or_buffer)
+            return
+
+        if isinstance(filepath_or_buffer, BytesIO) or Path(
+            filepath_or_buffer
+        ).suffix in [".gz", ".gzip"]:
             fopen = gzip.open
         else:
             fopen = open
 
         with fopen(self._file, "rt", encoding=self._encoding) as f:
             self._read_header(f)
 
@@ -215,14 +228,15 @@
         if backend == "pandas":
             data_dict = self._read_pandas(usecols, native_dtypes)
         elif backend == "datatable":
             if native_dtypes:
                 warn(
                     "Ignoring option 'native_dtypes' with datatable backend.",
                     UserWarning,
+                    stacklevel=2,
                 )
             data_dict = self._read_datatable(usecols)
         else:
             raise ValueError(f"Unknown CSV backend: '{backend}'.")
 
         self._data.update(data_dict)
         self._update_time_links()
@@ -232,16 +246,16 @@
     def as_dict(self) -> dict:
         """Convert scope file into regular Python dict."""
         sf_dict = {
             "scope_name": self._meta["ScopeName"],
             "file": self._meta["File"],
             "start_time": self.start_time,
             "run_time": self.run_time,
+            "channels": {k: v.as_dict() for k, v in self.items()},
         }
-        sf_dict["channels"] = {k: v.as_dict() for k, v in self.items()}
         return sf_dict
 
     def as_pandas(
         self,
         channels: list[str] = None,
         time_fmt: str = "timestamp",
     ) -> pd.DataFrame:
@@ -288,15 +302,15 @@
             c = self[n]
             t_col = self._time_mapping[c.time_col]
 
             _dict[t_col] = _dict[t_col].assign(**{c.name: c.values[: _l[t_col]]})
 
         _list = [v for v in _dict.values() if not v.empty]
 
-        df = pd.DataFrame().join(_list, how="outer")
+        df = pd.DataFrame().join(_list, how="outer", sort=True)
 
         if time_fmt == "timedelta":
             df.index = pd.TimedeltaIndex((df.index * 1e6).astype(np.int64))
         else:
             df.index = to_datetime_from_ms(df.index, self.start_time)
 
         return df
@@ -449,16 +463,22 @@
         if not self._decimal:
             self._decimal = self._get_decimal_from_line(line, delimiter)
             while not self._decimal:
                 self._decimal = self._get_decimal_from_line(f.readline(), delimiter)
 
         # determine the number of header rows
         f.seek(0)
-        _header = f.buffer.read(data_block_search_index)  # read binary from buffer
-        self._header_lines = _header.count(b"\n")
+        if isinstance(f, StringIO):  # we navigate characters
+            _header = f.read(data_block_search_index)
+            self._header_lines = _header.count("\n")
+        else:
+            _header = f.buffer.read(
+                data_block_search_index
+            )  # read to binary position from buffer
+            self._header_lines = _header.count(b"\n")
 
         # build the time column mappings
         self._build_time_mapping(f.readline(), f.readline())
 
         # cleanup channels without name (legacy file exports)
         self._channels = {k: v for k, v in self._channels.items() if v.name}
 
@@ -549,28 +569,32 @@
         self._time_offset = {c: _time_meta[i][0] for i, c in enumerate(time_indx)}
         self._time_sample_time = {c: _time_meta[i][1] for i, c in enumerate(time_indx)}
 
     def _read_pandas(
         self, usecols: list[int], native_dtypes: bool
     ) -> dict[str, np.ndarray]:
         """Read data into dictionary using the pandas backend."""
+        if isinstance(self._file, IOBase):  # read open streams from beginning
+            self._file.seek(0)
+
         df = pd.read_csv(
             self._file,
             delimiter=self._delimiter,
             skiprows=self._header_lines,
             decimal=self._decimal,
             header=None,
             usecols=usecols,
             names=self._get_cols(),
             index_col=False,
-            encoding="utf-8",
+            encoding=self._encoding,
             na_values=[" ", "EOF"],
             skip_blank_lines=True,
             engine="c",
             low_memory=False,
+            compression=self._compression,
         )
 
         # self._df = df  # debug
 
         if native_dtypes:
             tc3_dtypes = get_tc3_dtypes()
             dtypes_np = {
@@ -586,15 +610,19 @@
         return data_dict
 
     def _read_datatable(self, usecols: list[int]) -> dict[str, np.ndarray]:
         """Read data into dictionary using the datatable backend."""
         try:
             import datatable
         except ModuleNotFoundError:
-            warn("'datatable' backend not found, using pandas.", UserWarning)
+            warn(
+                "'datatable' backend not found, using pandas.",
+                UserWarning,
+                stacklevel=2,
+            )
             return self._read_pandas(usecols)
 
         columns = [
             i in usecols
             for i in range(len(self._get_cols()) + self._line_end_delimiter)
         ]
 
@@ -631,15 +659,17 @@
         """
         if isinstance(channels, str):
             channels = [channels]
         if channels is None:
             channels = self._channels.keys()
 
         if diff := (set(channels) - self._channels.keys()):
-            warn(f"Cannot find the following channels: {diff}", UserWarning)
+            warn(
+                f"Cannot find the following channels: {diff}", UserWarning, stacklevel=2
+            )
             channels = self._channels.keys() - channels
         channels = list(channels)
 
         s = self._get_cols(channels) - self._data.keys()
         return sorted({self._time_mapping.get(i, i) for i in s})
 
     def _update_data_refs(self):
@@ -665,14 +695,15 @@
         values = list(chain(*values))  # flatten
 
         if not len(self._channels.keys()) == len(values):
             if key == "SymbolComment":
                 warn(
                     "Wrong format in 'SymbolComment' header line, skipping.",
                     UserWarning,
+                    stacklevel=2,
                 )
                 return
             else:
                 raise ValueError(
                     f"wrong metadata count for {key}"
                     f": {len(self._channels.keys())}, {len(values)}"
                 )
```

### Comparing `pytcs-0.1.1/pytcs.egg-info/PKG-INFO` & `pytcs-0.1.2/pytcs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytcs
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python API for processing TwinCAT Scope data files
 Author-email: Cagtay Fabry <cagtay.fabry@bam.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Cagtay Fabry
         All rights reserved.
```

