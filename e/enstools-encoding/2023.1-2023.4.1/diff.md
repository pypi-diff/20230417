# Comparing `tmp/enstools-encoding-2023.1.tar.gz` & `tmp/enstools-encoding-2023.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enstools-encoding-2023.1.tar", last modified: Wed Jan 18 16:32:02 2023, max compression
+gzip compressed data, was "enstools-encoding-2023.4.1.tar", last modified: Mon Apr 17 12:03:16 2023, max compression
```

## Comparing `enstools-encoding-2023.1.tar` & `enstools-encoding-2023.4.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 oriol.tinto (24207) ls-craig (11075)        0 2023-01-18 16:32:02.000000 enstools-encoding-2023.1/
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)    10898 2023-01-18 16:32:01.000000 enstools-encoding-2023.1/LICENSE
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)       15 2023-01-18 16:32:01.000000 enstools-encoding-2023.1/MANIFEST.in
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     2139 2023-01-18 16:32:02.000000 enstools-encoding-2023.1/PKG-INFO
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)        6 2023-01-18 16:32:01.000000 enstools-encoding-2023.1/VERSION
-drwxr-xr-x   0 oriol.tinto (24207) ls-craig (11075)        0 2023-01-18 16:32:02.000000 enstools-encoding-2023.1/enstools/
-drwxr-xr-x   0 oriol.tinto (24207) ls-craig (11075)        0 2023-01-18 16:32:02.000000 enstools-encoding-2023.1/enstools/encoding/
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)        0 2023-01-18 16:32:01.000000 enstools-encoding-2023.1/enstools/encoding/__init__.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)      267 2023-01-18 16:32:01.000000 enstools-encoding-2023.1/enstools/encoding/api.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     6373 2023-01-18 16:32:01.000000 enstools-encoding-2023.1/enstools/encoding/dataset_encoding.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     1680 2023-01-18 16:32:01.000000 enstools-encoding-2023.1/enstools/encoding/definitions.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)      126 2023-01-18 16:32:01.000000 enstools-encoding-2023.1/enstools/encoding/errors.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)      654 2023-01-18 16:32:01.000000 enstools-encoding-2023.1/enstools/encoding/rules.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)    12024 2023-01-18 16:32:01.000000 enstools-encoding-2023.1/enstools/encoding/variable_encoding.py
-drwxr-xr-x   0 oriol.tinto (24207) ls-craig (11075)        0 2023-01-18 16:32:02.000000 enstools-encoding-2023.1/enstools_encoding.egg-info/
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     2139 2023-01-18 16:32:02.000000 enstools-encoding-2023.1/enstools_encoding.egg-info/PKG-INFO
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)      531 2023-01-18 16:32:02.000000 enstools-encoding-2023.1/enstools_encoding.egg-info/SOURCES.txt
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)        1 2023-01-18 16:32:02.000000 enstools-encoding-2023.1/enstools_encoding.egg-info/dependency_links.txt
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)        9 2023-01-18 16:32:02.000000 enstools-encoding-2023.1/enstools_encoding.egg-info/namespace_packages.txt
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)       39 2023-01-18 16:32:02.000000 enstools-encoding-2023.1/enstools_encoding.egg-info/requires.txt
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)        9 2023-01-18 16:32:02.000000 enstools-encoding-2023.1/enstools_encoding.egg-info/top_level.txt
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)       38 2023-01-18 16:32:02.000000 enstools-encoding-2023.1/setup.cfg
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)      992 2023-01-18 16:32:01.000000 enstools-encoding-2023.1/setup.py
-drwxr-xr-x   0 oriol.tinto (24207) ls-craig (11075)        0 2023-01-18 16:32:02.000000 enstools-encoding-2023.1/test/
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)    15517 2023-01-18 16:32:01.000000 enstools-encoding-2023.1/test/test_classes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:03:16.562552 enstools-encoding-2023.4.1/
+-rw-rw-rw-   0 root         (0) root         (0)    10898 2023-01-18 16:11:59.000000 enstools-encoding-2023.4.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       15 2023-01-18 16:11:59.000000 enstools-encoding-2023.4.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2195 2023-04-17 12:03:16.562552 enstools-encoding-2023.4.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)        8 2023-04-17 11:52:31.000000 enstools-encoding-2023.4.1/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:03:16.559552 enstools-encoding-2023.4.1/enstools/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:03:16.561552 enstools-encoding-2023.4.1/enstools/encoding/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-18 16:11:59.000000 enstools-encoding-2023.4.1/enstools/encoding/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      267 2023-01-18 16:11:59.000000 enstools-encoding-2023.4.1/enstools/encoding/api.py
+-rw-rw-rw-   0 root         (0) root         (0)     9046 2023-04-17 09:53:42.000000 enstools-encoding-2023.4.1/enstools/encoding/dataset_encoding.py
+-rw-rw-rw-   0 root         (0) root         (0)     1680 2023-01-18 16:11:59.000000 enstools-encoding-2023.4.1/enstools/encoding/definitions.py
+-rw-rw-rw-   0 root         (0) root         (0)      126 2023-01-18 16:11:59.000000 enstools-encoding-2023.4.1/enstools/encoding/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)      654 2023-01-18 16:11:59.000000 enstools-encoding-2023.4.1/enstools/encoding/rules.py
+-rw-rw-rw-   0 root         (0) root         (0)    11435 2023-04-17 11:57:40.000000 enstools-encoding-2023.4.1/enstools/encoding/variable_encoding.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:03:16.561552 enstools-encoding-2023.4.1/enstools_encoding.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2195 2023-04-17 12:03:16.000000 enstools-encoding-2023.4.1/enstools_encoding.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      531 2023-04-17 12:03:16.000000 enstools-encoding-2023.4.1/enstools_encoding.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 12:03:16.000000 enstools-encoding-2023.4.1/enstools_encoding.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-04-17 12:03:16.000000 enstools-encoding-2023.4.1/enstools_encoding.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-04-17 12:03:16.000000 enstools-encoding-2023.4.1/enstools_encoding.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-04-17 12:03:16.000000 enstools-encoding-2023.4.1/enstools_encoding.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 12:03:16.562552 enstools-encoding-2023.4.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      992 2023-01-18 16:25:49.000000 enstools-encoding-2023.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:03:16.562552 enstools-encoding-2023.4.1/test/
+-rw-rw-rw-   0 root         (0) root         (0)    15517 2023-01-18 16:11:59.000000 enstools-encoding-2023.4.1/test/test_classes.py
```

### Comparing `enstools-encoding-2023.1/LICENSE` & `enstools-encoding-2023.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `enstools-encoding-2023.1/PKG-INFO` & `enstools-encoding-2023.4.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 Metadata-Version: 2.1
 Name: enstools-encoding
-Version: 2023.1
+Version: 2023.4.1
+Summary: UNKNOWN
 Home-page: https://github.com/wavestoweather/enstools-encoding
 Author: Oriol Tintó
 Author-email: oriol.tinto@lmu.de
+License: UNKNOWN
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # enstools-encoding [![Documentation Status](https://readthedocs.org/projects/enstools/badge/?version=latest)](https://enstools-encoding.readthedocs.io/en/latest/?badge=latest)
 
 Library to generate the encodings to write compressed files as easily as possible with **xarray** using **hdf5 filters**.
 
@@ -45,7 +48,9 @@
 Waves to Weather (SFB/TRR165) coordinated by the subproject 
 [Z2](https://www.wavestoweather.de/research_areas/phase2/z2) and funded by the
 German Research Foundation (DFG).
 
 A full list of code contributors can [CONTRIBUTORS.md](./CONTRIBUTORS.md).
 
 The code is released under an [Apache-2.0 licence](./LICENSE).
+
+
```

### Comparing `enstools-encoding-2023.1/enstools/encoding/dataset_encoding.py` & `enstools-encoding-2023.4.1/enstools/encoding/dataset_encoding.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,74 @@
 import os
 from copy import deepcopy
 from pathlib import Path
-from typing import Union, Dict
+from typing import Hashable, Union, Dict
 
 import xarray
 import yaml
+import numpy as np
 
 from . import rules
 from .errors import InvalidCompressionSpecification
 from .variable_encoding import _Mapping, parse_variable_specification, Encoding, \
     NullEncoding
 
 
-def compression_dictionary_to_string(compression_dictionary: dict) -> str:
+def convert_size(size_bytes):
+    import math
+    if size_bytes < 0:
+        prefix = "-"
+        size_bytes = -size_bytes
+    else:
+        prefix = ""
+
+    if size_bytes == 0:
+        return "0B"
+    size_name = ("B", "KB", "MB", "GB", "TB", "PB", "EB", "ZB", "YB")
+    i = int(math.floor(math.log(size_bytes, 1024)))
+    p = math.pow(1024, i)
+    s = round(size_bytes / p, 2)
+    return f"{prefix}{s}{size_name[i]}"
+
+
+def convert_to_bytes(size_string):
+    """
+    This function converts a given size string (e.g. '5MB') to the number of bytes.
+    
+    Args:
+    size_string (str): The size string to be converted (e.g. '5MB')
+    
+    Returns:
+    int: The number of bytes.
+    """
+    import re
+    size_string = size_string.upper()
+    digits = re.match(r'\d+(?:\.\d+)?', size_string)  # matches digits and optionally a dot followed by more digits
+    if digits:
+        digits = digits.group()  # get the matched digits
+    else:
+        raise ValueError(f"Invalid size string: {size_string}")
+    unit = size_string.replace(digits, "")
+    size_name_dict = {'B': 0, 'KB': 1, 'MB': 2, 'GB': 3, 'TB': 4, 'PB': 5, 'EB': 6, 'ZB': 7, 'YB': 8}
+    if unit in size_name_dict:
+        size_bytes = float(digits) * np.power(1024, size_name_dict[unit])
+    else:
+        raise ValueError(f"Invalid size string: {size_string}")
+    return int(size_bytes)
+
+
+def compression_dictionary_to_string(compression_dictionary: Dict[str, str]) -> str:
     """
     Convert a dictionary containing multiple entries to a single line specification
     """
     return rules.VARIABLE_SEPARATOR.join(
         [f"{key}{rules.VARIABLE_NAME_SEPARATOR}{value}" for key, value in compression_dictionary.items()])
 
 
-def parse_full_specification(spec: str) -> Dict[str, Encoding]:
+def parse_full_specification(spec: Union[str, None]) -> Dict[str, Encoding]:
     from enstools.encoding.rules import VARIABLE_SEPARATOR, VARIABLE_NAME_SEPARATOR, \
         DATA_DEFAULT_LABEL, DATA_DEFAULT_VALUE, COORD_LABEL, COORD_DEFAULT_VALUE
     result = {}
 
     if spec is None:
         spec = "None"
 
@@ -54,37 +98,37 @@
         # If the default is a NullSpecification, we'll use the same for the coordinates
         if isinstance(result[DATA_DEFAULT_LABEL], NullEncoding):
             result[COORD_LABEL] = result[DATA_DEFAULT_LABEL]
         else:
             result[COORD_LABEL] = parse_variable_specification(COORD_DEFAULT_VALUE)
 
     # For each specification, check that the specifications are valid.
-    for key, spec in result.items():
-        spec.check_validity()
+    for _, _spec in result.items():
+        _spec.check_validity()
 
     return result
 
 
 class DatasetEncoding(_Mapping):
     """
     Class to encapsulate compression specification parameters corresponding to a full dataset.
     The kind of encoding that xarray expects is a mapping between the variables and their corresponding h5py encoding.
     """
 
-    def __init__(self, dataset: xarray.Dataset, compression: Union[str, dict, None]):
+    def __init__(self, dataset: xarray.Dataset, compression: Union[str, Dict[str, str], Path, None]):
         self.dataset = dataset
 
         # Process the compression argument to get a single string with per-variable specifications
         compression = self.get_a_single_compression_string(compression)
 
         # Save it
         self.variable_encodings = parse_full_specification(compression)
 
     @staticmethod
-    def get_a_single_compression_string(compression: Union[str, dict, Path]) -> str:
+    def get_a_single_compression_string(compression: Union[str, Dict[str, str], Path, None]) -> Union[str, None]:
         # The compression parameter can be a string or a dictionary.
 
         # In case it is a string, it can be directly a compression specification or a yaml file.
         # If it is a file, convert it to a Path
         if isinstance(compression, str) and os.path.exists(compression):
             compression = Path(compression)
 
@@ -116,26 +160,43 @@
         # Set encoding for data variables
         data_variable_encodings = {
             str(var): deepcopy(self.variable_encodings[str(var)]) if var in self.variable_encodings else deepcopy(
                 data_default) for
             var
             in self.dataset.data_vars}
 
-        # Add chunking?
-        for variable in self.dataset.data_vars:
-            chunks = {k: v if k != "time" else 1 for k, v in self.dataset[variable].sizes.items()}
-            chunk_sizes = tuple(chunks.values())
-            # Ugly python magic to add chunk sizes into the encoding mapping object.
-            data_variable_encodings[variable]._kwargs._kwargs["chunksizes"] = chunk_sizes  # noqa
-
         # Merge
         all_encodings = {**coordinate_encodings, **data_variable_encodings}
 
+        # Need to specify chunk size, otherwise it breaks down.
+        self.chunk(encodings=all_encodings)
+
         return all_encodings
 
+    def chunk(self, encodings: Dict[Union[Hashable, str], Encoding], chunk_memory_size="10MB"):
+        """
+        Add a variable "chunksizes" to each variable encoding with the corresponding 
+
+        Args:
+            encodings (dict): Dictionary with the corresponding encoding for each variable.
+            chunk_memory_size (str): Desired chunk size in memory.
+        """
+
+        chunk_memory_size = convert_to_bytes(chunk_memory_size)
+
+        # Loop over all the variables
+        for variable in self.dataset.data_vars:
+            da = self.dataset[variable]
+            type_size = da.dtype.itemsize
+
+            optimal_chunk_size = chunk_memory_size / type_size
+            chunk_sizes = find_chunk_sizes(data_array=da, chunk_size=optimal_chunk_size)
+            chunk_sizes = tuple(chunk_sizes[d] for d in da.dims)
+            encodings[variable].set_chunk_sizes(chunk_sizes)
+
     @property
     def _kwargs(self):
         return self.encoding()
 
     def add_metadata(self):
         """
         Add the corresponding compression metadata to the dataset.
@@ -149,7 +210,25 @@
 
 def is_a_valid_dataset_compression_specification(specification):
     try:
         _ = parse_full_specification(specification)
         return True
     except InvalidCompressionSpecification:
         return False
+
+
+def find_chunk_sizes(data_array, chunk_size):
+    import math
+    total_points = np.prod(data_array.shape)
+    num_chunks = max(1, int(total_points // chunk_size))
+    chunk_sizes = {}
+    chunk_number = {}
+
+    # Sort dimensions by size
+    dims = sorted(data_array.dims, key=lambda x: data_array[x].shape)
+    pending_num_chunks = num_chunks
+    for dim in dims:
+        chunk_sizes[dim] = max(1, int(data_array[dim].size // pending_num_chunks))
+        chunk_number[dim] = data_array[dim].size // chunk_sizes[dim]
+
+        pending_num_chunks = math.ceil(pending_num_chunks / chunk_number[dim])
+    return chunk_sizes
```

### Comparing `enstools-encoding-2023.1/enstools/encoding/definitions.py` & `enstools-encoding-2023.4.1/enstools/encoding/definitions.py`

 * *Files identical despite different names*

### Comparing `enstools-encoding-2023.1/enstools/encoding/rules.py` & `enstools-encoding-2023.4.1/enstools/encoding/rules.py`

 * *Files identical despite different names*

### Comparing `enstools-encoding-2023.1/enstools/encoding/variable_encoding.py` & `enstools-encoding-2023.4.1/enstools/encoding/variable_encoding.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-from abc import ABC
 
 from .definitions import lossy_compressors_and_modes
 import logging
 
-from typing import Mapping, Union, Protocol
+from typing import Mapping, Union
 
 import hdf5plugin
 
 from enstools.encoding import rules, definitions
 from enstools.encoding.errors import InvalidCompressionSpecification
 from .rules import LOSSLESS_DEFAULT_BACKEND, LOSSLESS_DEFAULT_COMPRESSION_LEVEL
 
@@ -18,15 +17,18 @@
     loggers[key].setLevel(logging.WARNING)
 
 
 class _Mapping(Mapping):
     """
     Subclass to implement dunder methods that are mandatory for Mapping to avoid repeating the code everywhere.
     """
-    _kwargs: Mapping
+
+    def __init__(self) -> None:
+        super().__init__()
+        self._kwargs = {}
 
     def __getitem__(self, item):
         return self._kwargs[item]
 
     def __setitem__(self, key, value):
         self._kwargs[key] = value
 
@@ -48,14 +50,40 @@
         ...
 
     def description(self) -> str:
         ...
 
     def __repr__(self):
         return f"{self.__class__.__name__}({self.to_string()})"
+    
+    def set_chunk_sizes(self, chunk_sizes: tuple) -> None:
+        """
+        Method to add chunksizes into the encoding dictionary.
+        Parameters
+        ----------
+        chunk_sizes
+
+        Returns
+        -------
+
+        """
+        self._kwargs["chunksizes"] = chunk_sizes
+
+    def set_chunk_sizes(self, chunk_sizes: tuple) -> None:
+        """
+        Method to add chunksizes into the encoding dictionary.
+        Parameters
+        ----------
+        chunk_sizes
+
+        Returns
+        -------
+
+        """
+        self._kwargs["chunksizes"] = chunk_sizes
 
 
 class VariableEncoding(_Mapping):
     """
     Factory class to get the proper encoding depending on the arguments provided.
 
     To get an encoding from a specification:
@@ -78,14 +106,15 @@
     Or it is possible to specify the backend and the compression level.
 
     >>> VariableEncoding(backend="snappy")
 
     >>> VariableEncoding(backend="snappy", compression_level=9)
 
     """
+
     def __new__(cls,
                 specification: str = None,
                 compressor: str = None,
                 mode: str = None,
                 parameter: Union[str, float, int] = None,
                 backend: str = None,
                 compression_level: int = None,
@@ -111,20 +140,22 @@
 
     def description(self) -> str:
         return ""
 
 
 class LosslessEncoding(Encoding):
     def __init__(self, backend: str, compression_level: int):
+        super().__init__()
         self.backend = backend if backend is not None else rules.LOSSLESS_DEFAULT_BACKEND
         self.compression_level = compression_level if compression_level is not None \
             else rules.LOSSLESS_DEFAULT_COMPRESSION_LEVEL
 
         self.check_validity()
-        self._kwargs = self.encoding()
+        # Trying to convert it to a dictionary already here.
+        self._kwargs = dict(self.encoding())
 
     def check_validity(self) -> bool:
         if self.backend not in definitions.lossless_backends:
             raise InvalidCompressionSpecification(f"Backend {self.backend!r} is not a valid backend.")
         elif not (1 <= self.compression_level <= 9):
             raise InvalidCompressionSpecification(f"Compression level {self.compression_level} must be within 1 and 9.")
         else:
@@ -142,21 +173,24 @@
 
     def __repr__(self):
         return f"{self.__class__.__name__}(backend={self.backend}, compression_level={self.compression_level})"
 
 
 class LossyEncoding(Encoding):
     def __init__(self, compressor: str, mode: str, parameter: Union[float, int]):
+        super().__init__()
         self.compressor = compressor
         self.mode = mode
 
         self.parameter = parameter
 
         self.check_validity()
-        self._kwargs = self.encoding()
+
+        # Trying to convert it to a dictionary already here.
+        self._kwargs = dict(self.encoding())
 
     def check_validity(self):
         # Check compressor validity
         if self.compressor not in definitions.lossy_compressors_and_modes:
             raise InvalidCompressionSpecification(f"Invalid compressor {self.compressor}")
         # Check compression mode validity
         if self.mode not in definitions.lossy_compressors_and_modes[self.compressor]:
@@ -240,56 +274,14 @@
             raise InvalidCompressionSpecification(f"Could not cast {specification!r} to type {specification_type!r}")
         return LossyEncoding(compressor, mode, specification)
     else:
         # In case its not lossy nor lossless, raise an exception.
         raise InvalidCompressionSpecification(f"Invalid specification {var_spec!r}")
 
 
-# class VariableEncoding(_Mapping):
-#     """
-#     Class to encapsulate compression specification parameters for a single variable.
-#
-#     It stores the compressor, the mode and the parameter.
-#
-#     It has a method to create a new instance from a specification string,
-#     a method to get the corresponding specification string from an existing object
-#     and a method to obtain the corresponding mapping expected by h5py.
-#
-#     """
-#
-#     def __init__(self, specification: Specification):
-#         # Init basic components
-#         self.specification = specification
-#
-#         self._kwargs = self.filter_mapping()
-#
-#     @staticmethod
-#     def from_string(string: str) -> 'VariableEncoding':
-#         specification = parse_variable_specification(string)
-#         """
-#         Method to create a specification object from a specification string
-#         """
-#         return VariableEncoding(specification)
-#
-#     def to_string(self) -> str:
-#         """
-#         Method to obtain a specification string from a specification object
-#         """
-#         return self.specification.to_string()
-#
-#     def filter_mapping(self) -> Mapping:
-#         """
-#         Method to get the corresponding FilterRefBase expected by h5py/xarray
-#         """
-#
-#         return self.specification.encoding()
-#
-#     def description(self):
-#         self.specification.description()
-
 def get_variable_encoding(
         specification: str = None,
         compressor: str = None,
         mode: str = None,
         parameter: Union[str, float, int] = None,
         backend: str = None,
         compression_level: int = None,
```

### Comparing `enstools-encoding-2023.1/enstools_encoding.egg-info/PKG-INFO` & `enstools-encoding-2023.4.1/enstools_encoding.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 Metadata-Version: 2.1
 Name: enstools-encoding
-Version: 2023.1
+Version: 2023.4.1
+Summary: UNKNOWN
 Home-page: https://github.com/wavestoweather/enstools-encoding
 Author: Oriol Tintó
 Author-email: oriol.tinto@lmu.de
+License: UNKNOWN
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # enstools-encoding [![Documentation Status](https://readthedocs.org/projects/enstools/badge/?version=latest)](https://enstools-encoding.readthedocs.io/en/latest/?badge=latest)
 
 Library to generate the encodings to write compressed files as easily as possible with **xarray** using **hdf5 filters**.
 
@@ -45,7 +48,9 @@
 Waves to Weather (SFB/TRR165) coordinated by the subproject 
 [Z2](https://www.wavestoweather.de/research_areas/phase2/z2) and funded by the
 German Research Foundation (DFG).
 
 A full list of code contributors can [CONTRIBUTORS.md](./CONTRIBUTORS.md).
 
 The code is released under an [Apache-2.0 licence](./LICENSE).
+
+
```

### Comparing `enstools-encoding-2023.1/enstools_encoding.egg-info/SOURCES.txt` & `enstools-encoding-2023.4.1/enstools_encoding.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `enstools-encoding-2023.1/setup.py` & `enstools-encoding-2023.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `enstools-encoding-2023.1/test/test_classes.py` & `enstools-encoding-2023.4.1/test/test_classes.py`

 * *Files identical despite different names*

