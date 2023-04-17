# Comparing `tmp/pynmrstar-3.3.1.tar.gz` & `tmp/pynmrstar-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynmrstar-3.3.1.tar", last modified: Wed Jul 27 18:26:10 2022, max compression
+gzip compressed data, was "pynmrstar-3.3.2.tar", last modified: Mon Apr 17 19:07:38 2023, max compression
```

## Comparing `pynmrstar-3.3.1.tar` & `pynmrstar-3.3.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 jon       (1001) jon       (1001)        0 2022-07-27 18:26:10.878465 pynmrstar-3.3.1/
--rw-rw-r--   0 jon       (1001) jon       (1001)       41 2021-04-29 22:04:53.000000 pynmrstar-3.3.1/MANIFEST.in
--rw-rw-r--   0 jon       (1001) jon       (1001)     2750 2022-07-27 18:26:10.878465 pynmrstar-3.3.1/PKG-INFO
--rw-rw-r--   0 jon       (1001) jon       (1001)     1236 2021-05-25 14:39:26.000000 pynmrstar-3.3.1/README.rst
-drwxrwxr-x   0 jon       (1001) jon       (1001)        0 2022-07-27 18:26:10.874465 pynmrstar-3.3.1/c/
--rw-rw-r--   0 jon       (1001) jon       (1001)    25233 2021-06-25 23:07:01.000000 pynmrstar-3.3.1/c/cnmrstarmodule.c
-drwxrwxr-x   0 jon       (1001) jon       (1001)        0 2022-07-27 18:26:10.874465 pynmrstar-3.3.1/pynmrstar/
--rw-rw-r--   0 jon       (1001) jon       (1001)     1967 2022-07-27 18:05:58.000000 pynmrstar-3.3.1/pynmrstar/__init__.py
--rw-rw-r--   0 jon       (1001) jon       (1001)    11969 2022-07-27 18:05:58.000000 pynmrstar-3.3.1/pynmrstar/_internal.py
--rw-rw-r--   0 jon       (1001) jon       (1001)     1510 2022-07-27 13:35:42.000000 pynmrstar-3.3.1/pynmrstar/definitions.py
--rw-rw-r--   0 jon       (1001) jon       (1001)    45539 2022-07-27 18:05:58.000000 pynmrstar-3.3.1/pynmrstar/entry.py
--rw-rw-r--   0 jon       (1001) jon       (1001)     1449 2021-06-25 23:07:01.000000 pynmrstar-3.3.1/pynmrstar/exceptions.py
--rw-rw-r--   0 jon       (1001) jon       (1001)    50535 2022-07-27 18:05:58.000000 pynmrstar-3.3.1/pynmrstar/loop.py
--rw-rw-r--   0 jon       (1001) jon       (1001)    15152 2022-07-27 18:05:58.000000 pynmrstar-3.3.1/pynmrstar/parser.py
-drwxrwxr-x   0 jon       (1001) jon       (1001)        0 2022-07-27 18:26:10.874465 pynmrstar-3.3.1/pynmrstar/reference_files/
--rw-rw-r--   0 jon       (1001) jon       (1001)     9942 2021-01-27 16:34:26.000000 pynmrstar-3.3.1/pynmrstar/reference_files/comments.str
--rw-rw-r--   0 jon       (1001) jon       (1001)     3432 2021-01-27 16:34:26.000000 pynmrstar-3.3.1/pynmrstar/reference_files/data_types.csv
--rw-rw-r--   0 jon       (1001) jon       (1001)  3694703 2021-01-27 16:34:26.000000 pynmrstar-3.3.1/pynmrstar/reference_files/schema.csv
--rw-rw-r--   0 jon       (1001) jon       (1001)    13371 2022-02-14 21:57:45.000000 pynmrstar-3.3.1/pynmrstar/remove_non_nef_data.py
--rw-rw-r--   0 jon       (1001) jon       (1001)    42974 2022-07-27 18:05:58.000000 pynmrstar-3.3.1/pynmrstar/saveframe.py
--rw-rw-r--   0 jon       (1001) jon       (1001)    15858 2022-07-27 18:05:58.000000 pynmrstar-3.3.1/pynmrstar/schema.py
--rwxrwxr-x   0 jon       (1001) jon       (1001)     4662 2022-07-27 18:05:58.000000 pynmrstar-3.3.1/pynmrstar/utils.py
-drwxrwxr-x   0 jon       (1001) jon       (1001)        0 2022-07-27 18:26:10.874465 pynmrstar-3.3.1/pynmrstar.egg-info/
--rw-rw-r--   0 jon       (1001) jon       (1001)     2750 2022-07-27 18:26:10.000000 pynmrstar-3.3.1/pynmrstar.egg-info/PKG-INFO
--rw-rw-r--   0 jon       (1001) jon       (1001)      577 2022-07-27 18:26:10.000000 pynmrstar-3.3.1/pynmrstar.egg-info/SOURCES.txt
--rw-rw-r--   0 jon       (1001) jon       (1001)        1 2022-07-27 18:26:10.000000 pynmrstar-3.3.1/pynmrstar.egg-info/dependency_links.txt
--rw-rw-r--   0 jon       (1001) jon       (1001)       21 2022-07-27 18:26:10.000000 pynmrstar-3.3.1/pynmrstar.egg-info/requires.txt
--rw-rw-r--   0 jon       (1001) jon       (1001)       19 2022-07-27 18:26:10.000000 pynmrstar-3.3.1/pynmrstar.egg-info/top_level.txt
--rw-rw-r--   0 jon       (1001) jon       (1001)       38 2022-07-27 18:26:10.878465 pynmrstar-3.3.1/setup.cfg
--rw-rw-r--   0 jon       (1001) jon       (1001)     2535 2021-09-30 18:17:18.000000 pynmrstar-3.3.1/setup.py
+drwxrwxr-x   0 jon       (1001) jon       (1001)        0 2023-04-17 19:07:38.206275 pynmrstar-3.3.2/
+-rw-rw-r--   0 jon       (1001) jon       (1001)       41 2021-04-29 22:04:53.000000 pynmrstar-3.3.2/MANIFEST.in
+-rw-rw-r--   0 jon       (1001) jon       (1001)     2757 2023-04-17 19:07:38.206275 pynmrstar-3.3.2/PKG-INFO
+-rw-rw-r--   0 jon       (1001) jon       (1001)     1243 2023-04-16 16:05:46.000000 pynmrstar-3.3.2/README.rst
+drwxrwxr-x   0 jon       (1001) jon       (1001)        0 2023-04-17 19:07:38.198275 pynmrstar-3.3.2/c/
+-rw-rw-r--   0 jon       (1001) jon       (1001)    25233 2021-06-25 23:07:01.000000 pynmrstar-3.3.2/c/cnmrstarmodule.c
+drwxrwxr-x   0 jon       (1001) jon       (1001)        0 2023-04-17 19:07:38.202275 pynmrstar-3.3.2/pynmrstar/
+-rw-rw-r--   0 jon       (1001) jon       (1001)     1967 2022-07-27 18:05:58.000000 pynmrstar-3.3.2/pynmrstar/__init__.py
+-rw-rw-r--   0 jon       (1001) jon       (1001)    11969 2023-04-16 16:05:46.000000 pynmrstar-3.3.2/pynmrstar/_internal.py
+-rw-rw-r--   0 jon       (1001) jon       (1001)     1510 2022-07-27 13:35:42.000000 pynmrstar-3.3.2/pynmrstar/definitions.py
+-rw-rw-r--   0 jon       (1001) jon       (1001)    45486 2023-04-16 16:05:46.000000 pynmrstar-3.3.2/pynmrstar/entry.py
+-rw-rw-r--   0 jon       (1001) jon       (1001)     1449 2021-06-25 23:07:01.000000 pynmrstar-3.3.2/pynmrstar/exceptions.py
+-rw-rw-r--   0 jon       (1001) jon       (1001)    50535 2022-07-27 18:05:58.000000 pynmrstar-3.3.2/pynmrstar/loop.py
+-rw-rw-r--   0 jon       (1001) jon       (1001)    15152 2023-01-26 22:06:41.000000 pynmrstar-3.3.2/pynmrstar/parser.py
+drwxrwxr-x   0 jon       (1001) jon       (1001)        0 2023-04-17 19:07:38.202275 pynmrstar-3.3.2/pynmrstar/reference_files/
+-rw-rw-r--   0 jon       (1001) jon       (1001)     9942 2021-01-27 16:34:26.000000 pynmrstar-3.3.2/pynmrstar/reference_files/comments.str
+-rw-rw-r--   0 jon       (1001) jon       (1001)     3432 2021-01-27 16:34:26.000000 pynmrstar-3.3.2/pynmrstar/reference_files/data_types.csv
+-rw-rw-r--   0 jon       (1001) jon       (1001)  3694703 2021-01-27 16:34:26.000000 pynmrstar-3.3.2/pynmrstar/reference_files/schema.csv
+-rw-rw-r--   0 jon       (1001) jon       (1001)    13371 2022-02-14 21:57:45.000000 pynmrstar-3.3.2/pynmrstar/remove_non_nef_data.py
+-rw-rw-r--   0 jon       (1001) jon       (1001)    43146 2023-04-16 16:05:46.000000 pynmrstar-3.3.2/pynmrstar/saveframe.py
+-rw-rw-r--   0 jon       (1001) jon       (1001)    15858 2022-07-27 18:05:58.000000 pynmrstar-3.3.2/pynmrstar/schema.py
+-rwxrwxr-x   0 jon       (1001) jon       (1001)     4662 2022-07-27 18:05:58.000000 pynmrstar-3.3.2/pynmrstar/utils.py
+drwxrwxr-x   0 jon       (1001) jon       (1001)        0 2023-04-17 19:07:38.202275 pynmrstar-3.3.2/pynmrstar.egg-info/
+-rw-rw-r--   0 jon       (1001) jon       (1001)     2757 2023-04-17 19:07:38.000000 pynmrstar-3.3.2/pynmrstar.egg-info/PKG-INFO
+-rw-rw-r--   0 jon       (1001) jon       (1001)      577 2023-04-17 19:07:38.000000 pynmrstar-3.3.2/pynmrstar.egg-info/SOURCES.txt
+-rw-rw-r--   0 jon       (1001) jon       (1001)        1 2023-04-17 19:07:38.000000 pynmrstar-3.3.2/pynmrstar.egg-info/dependency_links.txt
+-rw-rw-r--   0 jon       (1001) jon       (1001)       21 2023-04-17 19:07:38.000000 pynmrstar-3.3.2/pynmrstar.egg-info/requires.txt
+-rw-rw-r--   0 jon       (1001) jon       (1001)       19 2023-04-17 19:07:38.000000 pynmrstar-3.3.2/pynmrstar.egg-info/top_level.txt
+-rw-rw-r--   0 jon       (1001) jon       (1001)       38 2023-04-17 19:07:38.206275 pynmrstar-3.3.2/setup.cfg
+-rw-rw-r--   0 jon       (1001) jon       (1001)     2535 2021-09-30 18:17:18.000000 pynmrstar-3.3.2/setup.py
```

### Comparing `pynmrstar-3.3.1/PKG-INFO` & `pynmrstar-3.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pynmrstar
-Version: 3.3.1
+Version: 3.3.2
 Summary: PyNMR-STAR provides tools for reading, writing, modifying, and interacting with NMR-STAR files. Maintained by the BMRB.
 Home-page: https://github.com/uwbmrb/PyNMRSTAR
 Author: Jon Wedell
 Author-email: wedell@uchc.edu
 License: MIT
 Description: Welcome to PyNMR-STAR!
         ======================================
         
         A Python module for reading, writing, and manipulating NMR-STAR files.
         
         |BuildStatus| |License| |Wheel| |PythonVersions|
         
-        Python versions supported: 3.6, 3.7, 3.8, and 3.9.
+        Python versions supported: 3.6, 3.7, 3.8, 3.9, 3.10, 3.11
         
         Overview
         --------
         
         This library was developed by the BMRB to give the Python-using NMR
         community tools to work with the NMR-STAR data format. It is used
         internally and is actively maintained. The library is thoroughly
```

### Comparing `pynmrstar-3.3.1/README.rst` & `pynmrstar-3.3.2/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Welcome to PyNMR-STAR!
 ======================================
 
 A Python module for reading, writing, and manipulating NMR-STAR files.
 
 |BuildStatus| |License| |Wheel| |PythonVersions|
 
-Python versions supported: 3.6, 3.7, 3.8, and 3.9.
+Python versions supported: 3.6, 3.7, 3.8, 3.9, 3.10, 3.11
 
 Overview
 --------
 
 This library was developed by the BMRB to give the Python-using NMR
 community tools to work with the NMR-STAR data format. It is used
 internally and is actively maintained. The library is thoroughly
```

### Comparing `pynmrstar-3.3.1/c/cnmrstarmodule.c` & `pynmrstar-3.3.2/c/cnmrstarmodule.c`

 * *Files identical despite different names*

### Comparing `pynmrstar-3.3.1/pynmrstar/__init__.py` & `pynmrstar-3.3.2/pynmrstar/__init__.py`

 * *Files identical despite different names*

### Comparing `pynmrstar-3.3.1/pynmrstar/_internal.py` & `pynmrstar-3.3.2/pynmrstar/_internal.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from io import StringIO, BytesIO
 from typing import Dict, Union, IO, List, Tuple
 from urllib.error import HTTPError, URLError
 from urllib.request import urlopen, Request
 
 import pynmrstar
 
-__version__: str = "3.3.1"
+__version__: str = "3.3.2"
 min_cnmrstar_version: str = "3.2.0"
 
 # If we have requests, open a session to reuse for the duration of the program run
 try:
     from requests import session as _requests_session
     # This replaces the urllib HTTPError if we have requests
     from requests.exceptions import HTTPError, ConnectionError
```

### Comparing `pynmrstar-3.3.1/pynmrstar/definitions.py` & `pynmrstar-3.3.2/pynmrstar/definitions.py`

 * *Files identical despite different names*

### Comparing `pynmrstar-3.3.1/pynmrstar/entry.py` & `pynmrstar-3.3.2/pynmrstar/entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -801,17 +801,15 @@
                 print(f"\t\t[{pos2}] {repr(one_loop)}")
 
     def remove_empty_saveframes(self) -> None:
         """ This method will remove all empty saveframes in an entry
         (the loops in the saveframe must also be empty for the saveframe
         to be deleted). "Empty" means no values in tags, not no tags present."""
 
-        for pos, entry in enumerate(self._frame_list):
-            if entry.empty:
-                del self._frame_list[pos]
+        self._frame_list = [_ for _ in self._frame_list if not _.empty]
 
     def remove_saveframe(self, item: Union[str, List[str], Tuple[str], 'saveframe_mod.Saveframe',
                                            List['saveframe_mod.Saveframe'], Tuple['saveframe_mod.Saveframe']]) -> None:
         """ Removes one or more saveframes from the entry. You can remove saveframes either by passing the saveframe
         object itself, the saveframe name (as a string), or a list or tuple of either."""
 
         parsed_list: list
```

### Comparing `pynmrstar-3.3.1/pynmrstar/exceptions.py` & `pynmrstar-3.3.2/pynmrstar/exceptions.py`

 * *Files identical despite different names*

### Comparing `pynmrstar-3.3.1/pynmrstar/loop.py` & `pynmrstar-3.3.2/pynmrstar/loop.py`

 * *Files identical despite different names*

### Comparing `pynmrstar-3.3.1/pynmrstar/parser.py` & `pynmrstar-3.3.2/pynmrstar/parser.py`

 * *Files identical despite different names*

### Comparing `pynmrstar-3.3.1/pynmrstar/reference_files/comments.str` & `pynmrstar-3.3.2/pynmrstar/reference_files/comments.str`

 * *Files identical despite different names*

### Comparing `pynmrstar-3.3.1/pynmrstar/reference_files/data_types.csv` & `pynmrstar-3.3.2/pynmrstar/reference_files/data_types.csv`

 * *Files identical despite different names*

### Comparing `pynmrstar-3.3.1/pynmrstar/reference_files/schema.csv` & `pynmrstar-3.3.2/pynmrstar/reference_files/schema.csv`

 * *Files identical despite different names*

### Comparing `pynmrstar-3.3.1/pynmrstar/remove_non_nef_data.py` & `pynmrstar-3.3.2/pynmrstar/remove_non_nef_data.py`

 * *Files identical despite different names*

### Comparing `pynmrstar-3.3.1/pynmrstar/saveframe.py` & `pynmrstar-3.3.2/pynmrstar/saveframe.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,23 +250,27 @@
 
     @property
     def category(self) -> str:
         return self._category
 
     @category.setter
     def category(self, category):
-        """ Updates the saveframe category. """
+        """ Updates the saveframe category. Sets the Sf_category tag if not present,
+         updates it if present. """
 
         if category in definitions.NULL_VALUES:
             raise ValueError("Cannot set the saveframe category to a null-equivalent value.")
 
-        # Update the sf_category tag too
-        lc_tags = self._lc_tags
-        if 'sf_category' in lc_tags:
-            self.tags[lc_tags['sf_category']] = category
+        # Update the sf_category tag if present - otherwise add it
+        category_tag = self.get_tag('sf_category', whole_tag=True)
+        if category_tag:
+            category_tag[0][1] = category
+        else:
+            self.add_tag('Sf_category', category)
+
         self._category = category
 
     @property
     def empty(self) -> bool:
         """ Check if the saveframe has no data. Ignore the structural tags."""
 
         for tag in self._tags:
```

### Comparing `pynmrstar-3.3.1/pynmrstar/schema.py` & `pynmrstar-3.3.2/pynmrstar/schema.py`

 * *Files identical despite different names*

### Comparing `pynmrstar-3.3.1/pynmrstar/utils.py` & `pynmrstar-3.3.2/pynmrstar/utils.py`

 * *Files identical despite different names*

### Comparing `pynmrstar-3.3.1/pynmrstar.egg-info/PKG-INFO` & `pynmrstar-3.3.2/pynmrstar.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pynmrstar
-Version: 3.3.1
+Version: 3.3.2
 Summary: PyNMR-STAR provides tools for reading, writing, modifying, and interacting with NMR-STAR files. Maintained by the BMRB.
 Home-page: https://github.com/uwbmrb/PyNMRSTAR
 Author: Jon Wedell
 Author-email: wedell@uchc.edu
 License: MIT
 Description: Welcome to PyNMR-STAR!
         ======================================
         
         A Python module for reading, writing, and manipulating NMR-STAR files.
         
         |BuildStatus| |License| |Wheel| |PythonVersions|
         
-        Python versions supported: 3.6, 3.7, 3.8, and 3.9.
+        Python versions supported: 3.6, 3.7, 3.8, 3.9, 3.10, 3.11
         
         Overview
         --------
         
         This library was developed by the BMRB to give the Python-using NMR
         community tools to work with the NMR-STAR data format. It is used
         internally and is actively maintained. The library is thoroughly
```

### Comparing `pynmrstar-3.3.1/pynmrstar.egg-info/SOURCES.txt` & `pynmrstar-3.3.2/pynmrstar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pynmrstar-3.3.1/setup.py` & `pynmrstar-3.3.2/setup.py`

 * *Files identical despite different names*

