# Comparing `tmp/newsworthycharts-1.9.1.tar.gz` & `tmp/newsworthycharts-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/newsworthycharts-1.9.1.tar", last modified: Mon Feb 10 10:46:28 2020, max compression
+gzip compressed data, was "dist/newsworthycharts-1.9.2.tar", last modified: Mon Feb 10 13:05:10 2020, max compression
```

## Comparing `newsworthycharts-1.9.1.tar` & `newsworthycharts-1.9.2.tar`

### file list

```diff
@@ -1,39 +1,42 @@
-drwxr-xr-x   0 jens      (1000) jens      (1000)        0 2020-02-10 10:46:28.000000 newsworthycharts-1.9.1/
-drwxr-xr-x   0 jens      (1000) jens      (1000)        0 2020-02-10 10:46:28.000000 newsworthycharts-1.9.1/newsworthycharts/
--rw-r--r--   0 jens      (1000) jens      (1000)    16671 2020-01-11 10:07:02.000000 newsworthycharts-1.9.1/newsworthycharts/chart.py
--rw-r--r--   0 jens      (1000) jens      (1000)    16962 2020-01-11 10:07:02.000000 newsworthycharts-1.9.1/newsworthycharts/serialchart.py
--rw-r--r--   0 jens      (1000) jens      (1000)    11106 2020-02-10 10:43:27.000000 newsworthycharts-1.9.1/newsworthycharts/datawrapper.py
--rw-r--r--   0 jens      (1000) jens      (1000)     3869 2020-01-23 20:20:17.000000 newsworthycharts-1.9.1/newsworthycharts/storage.py
--rw-r--r--   0 jens      (1000) jens      (1000)     2740 2019-09-03 09:05:57.000000 newsworthycharts-1.9.1/newsworthycharts/scatterplot.py
--rw-r--r--   0 jens      (1000) jens      (1000)      400 2020-01-23 20:20:17.000000 newsworthycharts-1.9.1/newsworthycharts/__init__.py
--rw-r--r--   0 jens      (1000) jens      (1000)     3599 2019-09-16 18:56:45.000000 newsworthycharts-1.9.1/newsworthycharts/categoricalchart.py
-drwxr-xr-x   0 jens      (1000) jens      (1000)        0 2020-02-10 10:46:28.000000 newsworthycharts-1.9.1/newsworthycharts/lib/
--rw-r--r--   0 jens      (1000) jens      (1000)     3488 2019-09-20 13:57:34.000000 newsworthycharts-1.9.1/newsworthycharts/lib/utils.py
--rw-r--r--   0 jens      (1000) jens      (1000)      388 2019-09-20 14:26:56.000000 newsworthycharts-1.9.1/newsworthycharts/lib/colors.py
--rw-r--r--   0 jens      (1000) jens      (1000)      154 2020-01-23 20:20:17.000000 newsworthycharts-1.9.1/newsworthycharts/lib/mimetypes.py
--rw-r--r--   0 jens      (1000) jens      (1000)     4853 2020-01-23 20:20:17.000000 newsworthycharts-1.9.1/newsworthycharts/lib/datalist.py
--rw-r--r--   0 jens      (1000) jens      (1000)     1248 2019-09-03 09:05:57.000000 newsworthycharts-1.9.1/newsworthycharts/lib/color_fn.py
--rw-r--r--   0 jens      (1000) jens      (1000)        0 2019-08-30 11:08:52.000000 newsworthycharts-1.9.1/newsworthycharts/lib/__init__.py
--rw-r--r--   0 jens      (1000) jens      (1000)     1962 2019-08-30 12:43:32.000000 newsworthycharts-1.9.1/newsworthycharts/lib/locator.py
--rw-r--r--   0 jens      (1000) jens      (1000)     2985 2020-01-11 10:07:02.000000 newsworthycharts-1.9.1/newsworthycharts/lib/formatter.py
-drwxr-xr-x   0 jens      (1000) jens      (1000)        0 2020-02-10 10:46:28.000000 newsworthycharts-1.9.1/newsworthycharts/rc/
--rw-r--r--   0 jens      (1000) jens      (1000)     1260 2019-09-03 13:22:43.000000 newsworthycharts-1.9.1/newsworthycharts/rc/newsworthy
-drwxr-xr-x   0 jens      (1000) jens      (1000)        0 2020-02-10 10:46:28.000000 newsworthycharts-1.9.1/test/
--rw-r--r--   0 jens      (1000) jens      (1000)     1333 2019-09-20 14:26:14.000000 newsworthycharts-1.9.1/test/test_categorical_chart.py
--rw-r--r--   0 jens      (1000) jens      (1000)      801 2020-01-23 20:20:17.000000 newsworthycharts-1.9.1/test/test_data_list.py
--rw-r--r--   0 jens      (1000) jens      (1000)     4861 2020-01-11 10:07:02.000000 newsworthycharts-1.9.1/test/test_serial_chart.py
--rw-r--r--   0 jens      (1000) jens      (1000)     5682 2020-02-10 10:39:19.000000 newsworthycharts-1.9.1/test/test_datawrapper.py
--rw-r--r--   0 jens      (1000) jens      (1000)     8487 2019-09-20 12:02:23.000000 newsworthycharts-1.9.1/test/test_main.py
-drwxr-xr-x   0 jens      (1000) jens      (1000)        0 2020-02-10 10:46:28.000000 newsworthycharts-1.9.1/newsworthycharts.egg-info/
--rw-r--r--   0 jens      (1000) jens      (1000)      131 2020-02-10 10:46:28.000000 newsworthycharts-1.9.1/newsworthycharts.egg-info/requires.txt
--rw-r--r--   0 jens      (1000) jens      (1000)     9268 2020-02-10 10:46:28.000000 newsworthycharts-1.9.1/newsworthycharts.egg-info/PKG-INFO
--rw-r--r--   0 jens      (1000) jens      (1000)      921 2020-02-10 10:46:28.000000 newsworthycharts-1.9.1/newsworthycharts.egg-info/SOURCES.txt
--rw-r--r--   0 jens      (1000) jens      (1000)        1 2019-03-31 20:39:42.000000 newsworthycharts-1.9.1/newsworthycharts.egg-info/not-zip-safe
--rw-r--r--   0 jens      (1000) jens      (1000)       17 2020-02-10 10:46:28.000000 newsworthycharts-1.9.1/newsworthycharts.egg-info/top_level.txt
--rw-r--r--   0 jens      (1000) jens      (1000)        1 2020-02-10 10:46:28.000000 newsworthycharts-1.9.1/newsworthycharts.egg-info/dependency_links.txt
--rw-r--r--   0 jens      (1000) jens      (1000)     9268 2020-02-10 10:46:28.000000 newsworthycharts-1.9.1/PKG-INFO
--rw-r--r--   0 jens      (1000) jens      (1000)      109 2020-02-10 10:46:28.000000 newsworthycharts-1.9.1/setup.cfg
--rw-r--r--   0 jens      (1000) jens      (1000)     6704 2020-02-10 10:46:04.000000 newsworthycharts-1.9.1/README.rst
--rw-r--r--   0 jens      (1000) jens      (1000)      940 2020-01-24 07:02:28.000000 newsworthycharts-1.9.1/setup.py
--rw-r--r--   0 jens      (1000) jens      (1000)     1069 2018-11-02 10:21:19.000000 newsworthycharts-1.9.1/LICENSE.txt
--rw-r--r--   0 jens      (1000) jens      (1000)       61 2019-08-30 11:08:52.000000 newsworthycharts-1.9.1/MANIFEST.in
+drwxr-xr-x   0 jens      (1000) jens      (1000)        0 2020-02-10 13:05:10.000000 newsworthycharts-1.9.2/
+drwxr-xr-x   0 jens      (1000) jens      (1000)        0 2020-02-10 13:05:10.000000 newsworthycharts-1.9.2/newsworthycharts/
+-rw-r--r--   0 jens      (1000) jens      (1000)    16671 2020-01-11 10:07:02.000000 newsworthycharts-1.9.2/newsworthycharts/chart.py
+-rw-r--r--   0 jens      (1000) jens      (1000)    16962 2020-01-11 10:07:02.000000 newsworthycharts-1.9.2/newsworthycharts/serialchart.py
+drwxr-xr-x   0 jens      (1000) jens      (1000)        0 2020-02-10 13:05:10.000000 newsworthycharts-1.9.2/newsworthycharts/translations/
+-rw-rw-r--   0 jens      (1000) jens      (1000)       75 2020-02-10 10:26:05.000000 newsworthycharts-1.9.2/newsworthycharts/translations/.~lock.datawrapper_regions.csv#
+-rw-rw-r--   0 jens      (1000) jens      (1000)     9214 2020-02-10 10:43:17.000000 newsworthycharts-1.9.2/newsworthycharts/translations/datawrapper_regions.csv
+-rw-r--r--   0 jens      (1000) jens      (1000)    11146 2020-02-10 13:02:07.000000 newsworthycharts-1.9.2/newsworthycharts/datawrapper.py
+-rw-r--r--   0 jens      (1000) jens      (1000)     3869 2020-01-23 20:20:17.000000 newsworthycharts-1.9.2/newsworthycharts/storage.py
+-rw-r--r--   0 jens      (1000) jens      (1000)     2740 2019-09-03 09:05:57.000000 newsworthycharts-1.9.2/newsworthycharts/scatterplot.py
+-rw-r--r--   0 jens      (1000) jens      (1000)      400 2020-01-23 20:20:17.000000 newsworthycharts-1.9.2/newsworthycharts/__init__.py
+-rw-r--r--   0 jens      (1000) jens      (1000)     3599 2019-09-16 18:56:45.000000 newsworthycharts-1.9.2/newsworthycharts/categoricalchart.py
+drwxr-xr-x   0 jens      (1000) jens      (1000)        0 2020-02-10 13:05:10.000000 newsworthycharts-1.9.2/newsworthycharts/lib/
+-rw-r--r--   0 jens      (1000) jens      (1000)     3488 2019-09-20 13:57:34.000000 newsworthycharts-1.9.2/newsworthycharts/lib/utils.py
+-rw-r--r--   0 jens      (1000) jens      (1000)      388 2019-09-20 14:26:56.000000 newsworthycharts-1.9.2/newsworthycharts/lib/colors.py
+-rw-r--r--   0 jens      (1000) jens      (1000)      154 2020-01-23 20:20:17.000000 newsworthycharts-1.9.2/newsworthycharts/lib/mimetypes.py
+-rw-r--r--   0 jens      (1000) jens      (1000)     4853 2020-01-23 20:20:17.000000 newsworthycharts-1.9.2/newsworthycharts/lib/datalist.py
+-rw-r--r--   0 jens      (1000) jens      (1000)     1248 2019-09-03 09:05:57.000000 newsworthycharts-1.9.2/newsworthycharts/lib/color_fn.py
+-rw-r--r--   0 jens      (1000) jens      (1000)        0 2019-08-30 11:08:52.000000 newsworthycharts-1.9.2/newsworthycharts/lib/__init__.py
+-rw-r--r--   0 jens      (1000) jens      (1000)     1962 2019-08-30 12:43:32.000000 newsworthycharts-1.9.2/newsworthycharts/lib/locator.py
+-rw-r--r--   0 jens      (1000) jens      (1000)     2985 2020-01-11 10:07:02.000000 newsworthycharts-1.9.2/newsworthycharts/lib/formatter.py
+drwxr-xr-x   0 jens      (1000) jens      (1000)        0 2020-02-10 13:05:10.000000 newsworthycharts-1.9.2/newsworthycharts/rc/
+-rw-r--r--   0 jens      (1000) jens      (1000)     1260 2019-09-03 13:22:43.000000 newsworthycharts-1.9.2/newsworthycharts/rc/newsworthy
+drwxr-xr-x   0 jens      (1000) jens      (1000)        0 2020-02-10 13:05:10.000000 newsworthycharts-1.9.2/test/
+-rw-r--r--   0 jens      (1000) jens      (1000)     1333 2019-09-20 14:26:14.000000 newsworthycharts-1.9.2/test/test_categorical_chart.py
+-rw-r--r--   0 jens      (1000) jens      (1000)      801 2020-01-23 20:20:17.000000 newsworthycharts-1.9.2/test/test_data_list.py
+-rw-r--r--   0 jens      (1000) jens      (1000)     4861 2020-01-11 10:07:02.000000 newsworthycharts-1.9.2/test/test_serial_chart.py
+-rw-r--r--   0 jens      (1000) jens      (1000)     5682 2020-02-10 10:39:19.000000 newsworthycharts-1.9.2/test/test_datawrapper.py
+-rw-r--r--   0 jens      (1000) jens      (1000)     8487 2019-09-20 12:02:23.000000 newsworthycharts-1.9.2/test/test_main.py
+drwxr-xr-x   0 jens      (1000) jens      (1000)        0 2020-02-10 13:05:10.000000 newsworthycharts-1.9.2/newsworthycharts.egg-info/
+-rw-r--r--   0 jens      (1000) jens      (1000)      131 2020-02-10 13:05:10.000000 newsworthycharts-1.9.2/newsworthycharts.egg-info/requires.txt
+-rw-r--r--   0 jens      (1000) jens      (1000)     9344 2020-02-10 13:05:10.000000 newsworthycharts-1.9.2/newsworthycharts.egg-info/PKG-INFO
+-rw-r--r--   0 jens      (1000) jens      (1000)     1037 2020-02-10 13:05:10.000000 newsworthycharts-1.9.2/newsworthycharts.egg-info/SOURCES.txt
+-rw-r--r--   0 jens      (1000) jens      (1000)        1 2019-03-31 20:39:42.000000 newsworthycharts-1.9.2/newsworthycharts.egg-info/not-zip-safe
+-rw-r--r--   0 jens      (1000) jens      (1000)       17 2020-02-10 13:05:10.000000 newsworthycharts-1.9.2/newsworthycharts.egg-info/top_level.txt
+-rw-r--r--   0 jens      (1000) jens      (1000)        1 2020-02-10 13:05:10.000000 newsworthycharts-1.9.2/newsworthycharts.egg-info/dependency_links.txt
+-rw-r--r--   0 jens      (1000) jens      (1000)     9344 2020-02-10 13:05:10.000000 newsworthycharts-1.9.2/PKG-INFO
+-rw-r--r--   0 jens      (1000) jens      (1000)      109 2020-02-10 13:05:10.000000 newsworthycharts-1.9.2/setup.cfg
+-rw-r--r--   0 jens      (1000) jens      (1000)     6748 2020-02-10 13:04:38.000000 newsworthycharts-1.9.2/README.rst
+-rw-r--r--   0 jens      (1000) jens      (1000)      940 2020-01-24 07:02:28.000000 newsworthycharts-1.9.2/setup.py
+-rw-r--r--   0 jens      (1000) jens      (1000)     1069 2018-11-02 10:21:19.000000 newsworthycharts-1.9.2/LICENSE.txt
+-rw-r--r--   0 jens      (1000) jens      (1000)      101 2020-02-10 12:58:39.000000 newsworthycharts-1.9.2/MANIFEST.in
```

### Comparing `newsworthycharts-1.9.1/newsworthycharts/chart.py` & `newsworthycharts-1.9.2/newsworthycharts/chart.py`

 * *Files identical despite different names*

### Comparing `newsworthycharts-1.9.1/newsworthycharts/serialchart.py` & `newsworthycharts-1.9.2/newsworthycharts/serialchart.py`

 * *Files identical despite different names*

### Comparing `newsworthycharts-1.9.1/newsworthycharts/datawrapper.py` & `newsworthycharts-1.9.2/newsworthycharts/datawrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 
 from .storage import Storage, LocalStorage
 from .chart import Chart
 from .lib.utils import loadstyle
 from .lib.formatter import Formatter
 from .lib.datalist import DataList
 
+HERE = os.path.dirname(__file__)
+
 class DatawrapperChart(Chart):
     # TODO: Make file_types dynami. Available file types depend on the
     # account level. png is available at all levels.
     file_types = ["png"]
 
     def __init__(self, width: int, height: int, storage: Storage=LocalStorage(),
                  style: str='newsworthy', language: str='en-GB'):
@@ -289,15 +291,15 @@
     def _translate_region(self, region):
         """Tries to translate a region name to DW convention.
 
         Lookup tables are defined in csv file.
         """
         if self._translations is None:
             _translations = {}
-            file_path = "newsworthycharts/translations/datawrapper_regions.csv"
+            file_path = os.path.join(HERE, 'translations', "datawrapper_regions.csv")
             with open(file_path) as f:
                 for row in csv.DictReader(f, skipinitialspace=True):
                     _translations[row["newsworthy_id"]] = row["datawrapper_id"]
             self._translations = _translations
 
         try:
             return self._translations[region]
```

### Comparing `newsworthycharts-1.9.1/newsworthycharts/storage.py` & `newsworthycharts-1.9.2/newsworthycharts/storage.py`

 * *Files identical despite different names*

### Comparing `newsworthycharts-1.9.1/newsworthycharts/scatterplot.py` & `newsworthycharts-1.9.2/newsworthycharts/scatterplot.py`

 * *Files identical despite different names*

### Comparing `newsworthycharts-1.9.1/newsworthycharts/categoricalchart.py` & `newsworthycharts-1.9.2/newsworthycharts/categoricalchart.py`

 * *Files identical despite different names*

### Comparing `newsworthycharts-1.9.1/newsworthycharts/lib/utils.py` & `newsworthycharts-1.9.2/newsworthycharts/lib/utils.py`

 * *Files identical despite different names*

### Comparing `newsworthycharts-1.9.1/newsworthycharts/lib/datalist.py` & `newsworthycharts-1.9.2/newsworthycharts/lib/datalist.py`

 * *Files identical despite different names*

### Comparing `newsworthycharts-1.9.1/newsworthycharts/lib/color_fn.py` & `newsworthycharts-1.9.2/newsworthycharts/lib/color_fn.py`

 * *Files identical despite different names*

### Comparing `newsworthycharts-1.9.1/newsworthycharts/lib/locator.py` & `newsworthycharts-1.9.2/newsworthycharts/lib/locator.py`

 * *Files identical despite different names*

### Comparing `newsworthycharts-1.9.1/newsworthycharts/lib/formatter.py` & `newsworthycharts-1.9.2/newsworthycharts/lib/formatter.py`

 * *Files identical despite different names*

### Comparing `newsworthycharts-1.9.1/newsworthycharts/rc/newsworthy` & `newsworthycharts-1.9.2/newsworthycharts/rc/newsworthy`

 * *Files identical despite different names*

### Comparing `newsworthycharts-1.9.1/test/test_categorical_chart.py` & `newsworthycharts-1.9.2/test/test_categorical_chart.py`

 * *Files identical despite different names*

### Comparing `newsworthycharts-1.9.1/test/test_data_list.py` & `newsworthycharts-1.9.2/test/test_data_list.py`

 * *Files identical despite different names*

### Comparing `newsworthycharts-1.9.1/test/test_serial_chart.py` & `newsworthycharts-1.9.2/test/test_serial_chart.py`

 * *Files identical despite different names*

### Comparing `newsworthycharts-1.9.1/test/test_datawrapper.py` & `newsworthycharts-1.9.2/test/test_datawrapper.py`

 * *Files identical despite different names*

### Comparing `newsworthycharts-1.9.1/test/test_main.py` & `newsworthycharts-1.9.2/test/test_main.py`

 * *Files identical despite different names*

### Comparing `newsworthycharts-1.9.1/newsworthycharts.egg-info/PKG-INFO` & `newsworthycharts-1.9.2/newsworthycharts.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: newsworthycharts
-Version: 1.9.1
+Version: 1.9.2
 Summary: Create charts and publish on Amazon S3.
 Home-page: https://github.com/jplusplus/newsworthycharts
 Author: Jens Finnäs and Leo Wallentin, J++ Stockholm
 Author-email: stockholm@jplusplus.org
 License: MIT
-Download-URL: https://github.com/jplusplus/newsworthycharts/archive/1.9.1.tar.gz
+Download-URL: https://github.com/jplusplus/newsworthycharts/archive/1.9.2.tar.gz
 Description: This  module contains methods for producing graphs and publishing them on Amazon S3, or in the location of your choice.
         
         It is written and maintained for `Newsworthy <https://www.newsworthy.se/en/>`_, but could possibly come in handy for other people as well.
         
         By `Journalism++ Stockholm <http://jplusplus.org/sv>`_.
         
         Installing
@@ -109,17 +109,21 @@
         ---------
         
         - next
         
           - Fix a crash in some special cases with serial charts shorter than a year.
           - Fix a bug where diff between series was not highlighted if one value was close to zero.
         
+        - 1.9.2
+        
+          - Include translations in build.
+        
         - 1.9.1
         
-            - Translates region to Datawrapper standard when making maps. 
+            - Translates region to Datawrapper standard when making maps.
         
         - 1.9.0
         
             - Allows list of dicts to be passed to DatawrapperChart to be make tables, categorical maps etc.
         
         - 1.8.2
```

### Comparing `newsworthycharts-1.9.1/newsworthycharts.egg-info/SOURCES.txt` & `newsworthycharts-1.9.2/newsworthycharts.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -21,12 +21,14 @@
 newsworthycharts/lib/colors.py
 newsworthycharts/lib/datalist.py
 newsworthycharts/lib/formatter.py
 newsworthycharts/lib/locator.py
 newsworthycharts/lib/mimetypes.py
 newsworthycharts/lib/utils.py
 newsworthycharts/rc/newsworthy
+newsworthycharts/translations/.~lock.datawrapper_regions.csv#
+newsworthycharts/translations/datawrapper_regions.csv
 test/test_categorical_chart.py
 test/test_data_list.py
 test/test_datawrapper.py
 test/test_main.py
 test/test_serial_chart.py
```

### Comparing `newsworthycharts-1.9.1/PKG-INFO` & `newsworthycharts-1.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: newsworthycharts
-Version: 1.9.1
+Version: 1.9.2
 Summary: Create charts and publish on Amazon S3.
 Home-page: https://github.com/jplusplus/newsworthycharts
 Author: Jens Finnäs and Leo Wallentin, J++ Stockholm
 Author-email: stockholm@jplusplus.org
 License: MIT
-Download-URL: https://github.com/jplusplus/newsworthycharts/archive/1.9.1.tar.gz
+Download-URL: https://github.com/jplusplus/newsworthycharts/archive/1.9.2.tar.gz
 Description: This  module contains methods for producing graphs and publishing them on Amazon S3, or in the location of your choice.
         
         It is written and maintained for `Newsworthy <https://www.newsworthy.se/en/>`_, but could possibly come in handy for other people as well.
         
         By `Journalism++ Stockholm <http://jplusplus.org/sv>`_.
         
         Installing
@@ -109,17 +109,21 @@
         ---------
         
         - next
         
           - Fix a crash in some special cases with serial charts shorter than a year.
           - Fix a bug where diff between series was not highlighted if one value was close to zero.
         
+        - 1.9.2
+        
+          - Include translations in build.
+        
         - 1.9.1
         
-            - Translates region to Datawrapper standard when making maps. 
+            - Translates region to Datawrapper standard when making maps.
         
         - 1.9.0
         
             - Allows list of dicts to be passed to DatawrapperChart to be make tables, categorical maps etc.
         
         - 1.8.2
```

### Comparing `newsworthycharts-1.9.1/README.rst` & `newsworthycharts-1.9.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -100,17 +100,21 @@
 ---------
 
 - next
 
   - Fix a crash in some special cases with serial charts shorter than a year.
   - Fix a bug where diff between series was not highlighted if one value was close to zero.
 
+- 1.9.2
+
+  - Include translations in build.
+
 - 1.9.1
 
-    - Translates region to Datawrapper standard when making maps. 
+    - Translates region to Datawrapper standard when making maps.
 
 - 1.9.0
 
     - Allows list of dicts to be passed to DatawrapperChart to be make tables, categorical maps etc.
 
 - 1.8.2
```

### Comparing `newsworthycharts-1.9.1/setup.py` & `newsworthycharts-1.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `newsworthycharts-1.9.1/LICENSE.txt` & `newsworthycharts-1.9.2/LICENSE.txt`

 * *Files identical despite different names*

