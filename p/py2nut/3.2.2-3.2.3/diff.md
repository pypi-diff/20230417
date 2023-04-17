# Comparing `tmp/py2nut-3.2.2.tar.gz` & `tmp/py2nut-3.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py2nut-3.2.2.tar", last modified: Fri Apr 14 05:36:28 2023, max compression
+gzip compressed data, was "py2nut-3.2.3.tar", last modified: Mon Apr 17 03:25:34 2023, max compression
```

## Comparing `py2nut-3.2.2.tar` & `py2nut-3.2.3.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 05:36:28.970569 py2nut-3.2.2/
--rw-rw-rw-   0        0        0    35803 2022-07-21 09:01:30.000000 py2nut-3.2.2/LICENSE
--rw-rw-rw-   0        0        0       22 2022-12-05 05:43:45.000000 py2nut-3.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0    21795 2023-04-14 05:36:28.969574 py2nut-3.2.2/PKG-INFO
--rw-rw-rw-   0        0        0    21290 2022-12-05 05:43:25.000000 py2nut-3.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 05:36:28.827928 py2nut-3.2.2/py2Nut/
--rw-rw-rw-   0        0        0       23 2023-03-30 09:09:08.000000 py2nut-3.2.2/py2Nut/__init__.py
--rw-rw-rw-   0        0        0        3 2022-12-05 07:43:05.000000 py2nut-3.2.2/py2Nut/_lib.py
--rw-rw-rw-   0        0        0       42 2022-12-05 07:42:35.000000 py2nut-3.2.2/py2Nut/nutApi.py
--rw-rw-rw-   0        0        0       52 2022-12-05 05:21:51.000000 py2nut-3.2.2/py2Nut/nutDataframe.py
--rw-rw-rw-   0        0        0       45 2022-12-05 07:42:04.000000 py2nut-3.2.2/py2Nut/nutDate.py
--rw-rw-rw-   0        0        0       37 2022-12-05 09:05:13.000000 py2nut-3.2.2/py2Nut/nutDb.py
--rw-rw-rw-   0        0        0       46 2022-12-05 09:05:55.000000 py2nut-3.2.2/py2Nut/nutEmail.py
--rw-rw-rw-   0        0        0       48 2022-12-05 09:04:21.000000 py2nut-3.2.2/py2Nut/nutFiles.py
--rw-rw-rw-   0        0        0       40 2022-12-05 09:20:39.000000 py2nut-3.2.2/py2Nut/nutFtp.py
--rw-rw-rw-   0        0        0       48 2022-12-05 07:42:53.000000 py2nut-3.2.2/py2Nut/nutOther.py
-drwxrwxrwx   0        0        0        0 2023-04-14 05:36:28.831060 py2nut-3.2.2/py2Nut/xlrd/
--rw-rw-rw-   0        0        0    34373 2022-07-21 09:01:30.000000 py2nut-3.2.2/py2Nut/xlrd/xlsx.py
-drwxrwxrwx   0        0        0        0 2023-04-14 05:36:28.852879 py2nut-3.2.2/py2nut.egg-info/
--rw-rw-rw-   0        0        0    21795 2023-04-14 05:36:28.000000 py2nut-3.2.2/py2nut.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1164 2023-04-14 05:36:28.000000 py2nut-3.2.2/py2nut.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 05:36:28.000000 py2nut-3.2.2/py2nut.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-04-14 05:36:28.000000 py2nut-3.2.2/py2nut.egg-info/requires.txt
--rw-rw-rw-   0        0        0       78 2023-04-14 05:36:28.000000 py2nut-3.2.2/py2nut.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-14 05:36:28.856851 py2nut-3.2.2/pynut_1tools/
-drwxrwxrwx   0        0        0        0 2023-04-14 05:36:28.881936 py2nut-3.2.2/pynut_1tools/pyNutTools/
--rw-rw-rw-   0        0        0       25 2023-04-04 08:29:08.000000 py2nut-3.2.2/pynut_1tools/pyNutTools/__init__.py
--rw-rw-rw-   0        0        0     2054 2022-12-07 03:56:44.000000 py2nut-3.2.2/pynut_1tools/pyNutTools/_lib.py
--rw-rw-rw-   0        0        0    32349 2023-04-04 08:31:33.000000 py2nut-3.2.2/pynut_1tools/pyNutTools/nutDataframe.py
--rw-rw-rw-   0        0        0    18046 2022-12-07 03:57:19.000000 py2nut-3.2.2/pynut_1tools/pyNutTools/nutDate.py
--rw-rw-rw-   0        0        0     8711 2023-03-07 04:16:53.000000 py2nut-3.2.2/pynut_1tools/pyNutTools/nutOther.py
--rw-rw-rw-   0        0        0     1029 2023-03-07 04:16:55.000000 py2nut-3.2.2/pynut_1tools/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 05:36:28.885775 py2nut-3.2.2/pynut_2api/
-drwxrwxrwx   0        0        0        0 2023-04-14 05:36:28.896767 py2nut-3.2.2/pynut_2api/pyNutApi/
--rw-rw-rw-   0        0        0       23 2023-03-07 04:16:57.000000 py2nut-3.2.2/pynut_2api/pyNutApi/__init__.py
--rw-rw-rw-   0        0        0     3607 2023-04-14 05:30:35.000000 py2nut-3.2.2/pynut_2api/pyNutApi/_lib.py
--rw-rw-rw-   0        0        0    28921 2023-04-14 05:32:54.000000 py2nut-3.2.2/pynut_2api/pyNutApi/nutApi.py
--rw-rw-rw-   0        0        0     1079 2023-04-14 05:27:51.000000 py2nut-3.2.2/pynut_2api/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 05:36:28.901114 py2nut-3.2.2/pynut_2files/
-drwxrwxrwx   0        0        0        0 2023-04-14 05:36:28.913720 py2nut-3.2.2/pynut_2files/pyNutFiles/
--rw-rw-rw-   0        0        0       23 2023-03-30 09:07:33.000000 py2nut-3.2.2/pynut_2files/pyNutFiles/__init__.py
--rw-rw-rw-   0        0        0     6710 2022-12-07 04:06:54.000000 py2nut-3.2.2/pynut_2files/pyNutFiles/_lib.py
--rw-rw-rw-   0        0        0   128574 2023-04-14 05:25:41.000000 py2nut-3.2.2/pynut_2files/pyNutFiles/nutFiles.py
--rw-rw-rw-   0        0        0     1170 2023-04-14 05:28:03.000000 py2nut-3.2.2/pynut_2files/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 05:36:28.920208 py2nut-3.2.2/pynut_3db/
-drwxrwxrwx   0        0        0        0 2023-04-14 05:36:28.931917 py2nut-3.2.2/pynut_3db/pyNutDB/
--rw-rw-rw-   0        0        0       23 2023-03-07 04:17:04.000000 py2nut-3.2.2/pynut_3db/pyNutDB/__init__.py
--rw-rw-rw-   0        0        0     2591 2022-12-05 13:21:28.000000 py2nut-3.2.2/pynut_3db/pyNutDB/_lib.py
--rw-rw-rw-   0        0        0    21550 2023-03-07 04:17:05.000000 py2nut-3.2.2/pynut_3db/pyNutDB/nutDb.py
--rw-rw-rw-   0        0        0     1051 2023-04-14 05:28:19.000000 py2nut-3.2.2/pynut_3db/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 05:36:28.936317 py2nut-3.2.2/pynut_3email/
-drwxrwxrwx   0        0        0        0 2023-04-14 05:36:28.947539 py2nut-3.2.2/pynut_3email/pyNutEmail/
--rw-rw-rw-   0        0        0       21 2023-04-14 05:29:30.000000 py2nut-3.2.2/pynut_3email/pyNutEmail/__init__.py
--rw-rw-rw-   0        0        0     4303 2022-12-05 13:20:03.000000 py2nut-3.2.2/pynut_3email/pyNutEmail/_lib.py
--rw-rw-rw-   0        0        0    35893 2023-01-04 05:22:20.000000 py2nut-3.2.2/pynut_3email/pyNutEmail/nutEmail.py
--rw-rw-rw-   0        0        0     1064 2023-04-14 05:28:29.000000 py2nut-3.2.2/pynut_3email/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 05:36:28.951619 py2nut-3.2.2/pynut_3ftp/
-drwxrwxrwx   0        0        0        0 2023-04-14 05:36:28.964039 py2nut-3.2.2/pynut_3ftp/pyNutFtp/
--rw-rw-rw-   0        0        0       23 2023-04-14 05:29:30.000000 py2nut-3.2.2/pynut_3ftp/pyNutFtp/__init__.py
--rw-rw-rw-   0        0        0     3476 2023-01-04 05:34:31.000000 py2nut-3.2.2/pynut_3ftp/pyNutFtp/_lib.py
--rw-rw-rw-   0        0        0    29570 2023-01-04 05:57:55.000000 py2nut-3.2.2/pynut_3ftp/pyNutFtp/nutFtp.py
--rw-rw-rw-   0        0        0     1072 2023-04-14 05:28:37.000000 py2nut-3.2.2/pynut_3ftp/setup.py
--rw-rw-rw-   0        0        0       42 2023-04-14 05:36:28.971630 py2nut-3.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1565 2023-02-08 10:26:55.000000 py2nut-3.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 03:25:34.564768 py2nut-3.2.3/
+-rw-rw-rw-   0        0        0    35803 2022-07-21 09:01:30.000000 py2nut-3.2.3/LICENSE
+-rw-rw-rw-   0        0        0       22 2022-12-05 05:43:45.000000 py2nut-3.2.3/MANIFEST.in
+-rw-rw-rw-   0        0        0    21795 2023-04-17 03:25:34.560779 py2nut-3.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0    21290 2022-12-05 05:43:25.000000 py2nut-3.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 03:25:34.124852 py2nut-3.2.3/py2Nut/
+-rw-rw-rw-   0        0        0       23 2023-04-14 05:42:20.000000 py2nut-3.2.3/py2Nut/__init__.py
+-rw-rw-rw-   0        0        0        3 2022-12-05 07:43:05.000000 py2nut-3.2.3/py2Nut/_lib.py
+-rw-rw-rw-   0        0        0       42 2022-12-05 07:42:35.000000 py2nut-3.2.3/py2Nut/nutApi.py
+-rw-rw-rw-   0        0        0       52 2022-12-05 05:21:51.000000 py2nut-3.2.3/py2Nut/nutDataframe.py
+-rw-rw-rw-   0        0        0       45 2022-12-05 07:42:04.000000 py2nut-3.2.3/py2Nut/nutDate.py
+-rw-rw-rw-   0        0        0       37 2022-12-05 09:05:13.000000 py2nut-3.2.3/py2Nut/nutDb.py
+-rw-rw-rw-   0        0        0       46 2022-12-05 09:05:55.000000 py2nut-3.2.3/py2Nut/nutEmail.py
+-rw-rw-rw-   0        0        0       48 2022-12-05 09:04:21.000000 py2nut-3.2.3/py2Nut/nutFiles.py
+-rw-rw-rw-   0        0        0       40 2022-12-05 09:20:39.000000 py2nut-3.2.3/py2Nut/nutFtp.py
+-rw-rw-rw-   0        0        0       48 2022-12-05 07:42:53.000000 py2nut-3.2.3/py2Nut/nutOther.py
+drwxrwxrwx   0        0        0        0 2023-04-17 03:25:34.134854 py2nut-3.2.3/py2Nut/xlrd/
+-rw-rw-rw-   0        0        0    34373 2022-07-21 09:01:30.000000 py2nut-3.2.3/py2Nut/xlrd/xlsx.py
+drwxrwxrwx   0        0        0        0 2023-04-17 03:25:34.264864 py2nut-3.2.3/py2nut.egg-info/
+-rw-rw-rw-   0        0        0    21795 2023-04-17 03:25:33.000000 py2nut-3.2.3/py2nut.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1164 2023-04-17 03:25:33.000000 py2nut-3.2.3/py2nut.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 03:25:33.000000 py2nut-3.2.3/py2nut.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-04-17 03:25:33.000000 py2nut-3.2.3/py2nut.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       78 2023-04-17 03:25:33.000000 py2nut-3.2.3/py2nut.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 03:25:34.271846 py2nut-3.2.3/pynut_1tools/
+drwxrwxrwx   0        0        0        0 2023-04-17 03:25:34.380864 py2nut-3.2.3/pynut_1tools/pyNutTools/
+-rw-rw-rw-   0        0        0       25 2023-04-04 08:29:08.000000 py2nut-3.2.3/pynut_1tools/pyNutTools/__init__.py
+-rw-rw-rw-   0        0        0     2054 2022-12-07 03:56:44.000000 py2nut-3.2.3/pynut_1tools/pyNutTools/_lib.py
+-rw-rw-rw-   0        0        0    32349 2023-04-04 08:31:33.000000 py2nut-3.2.3/pynut_1tools/pyNutTools/nutDataframe.py
+-rw-rw-rw-   0        0        0    18046 2022-12-07 03:57:19.000000 py2nut-3.2.3/pynut_1tools/pyNutTools/nutDate.py
+-rw-rw-rw-   0        0        0     8711 2023-03-07 04:16:53.000000 py2nut-3.2.3/pynut_1tools/pyNutTools/nutOther.py
+-rw-rw-rw-   0        0        0     1029 2023-03-07 04:16:55.000000 py2nut-3.2.3/pynut_1tools/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 03:25:34.386540 py2nut-3.2.3/pynut_2api/
+drwxrwxrwx   0        0        0        0 2023-04-17 03:25:34.431927 py2nut-3.2.3/pynut_2api/pyNutApi/
+-rw-rw-rw-   0        0        0       23 2023-03-07 04:16:57.000000 py2nut-3.2.3/pynut_2api/pyNutApi/__init__.py
+-rw-rw-rw-   0        0        0     3607 2023-04-14 05:30:35.000000 py2nut-3.2.3/pynut_2api/pyNutApi/_lib.py
+-rw-rw-rw-   0        0        0    29117 2023-04-17 03:23:52.000000 py2nut-3.2.3/pynut_2api/pyNutApi/nutApi.py
+-rw-rw-rw-   0        0        0     1079 2023-04-14 05:27:51.000000 py2nut-3.2.3/pynut_2api/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 03:25:34.464837 py2nut-3.2.3/pynut_2files/
+drwxrwxrwx   0        0        0        0 2023-04-17 03:25:34.481792 py2nut-3.2.3/pynut_2files/pyNutFiles/
+-rw-rw-rw-   0        0        0       23 2023-03-30 09:07:33.000000 py2nut-3.2.3/pynut_2files/pyNutFiles/__init__.py
+-rw-rw-rw-   0        0        0     6710 2022-12-07 04:06:54.000000 py2nut-3.2.3/pynut_2files/pyNutFiles/_lib.py
+-rw-rw-rw-   0        0        0   128574 2023-04-14 05:25:41.000000 py2nut-3.2.3/pynut_2files/pyNutFiles/nutFiles.py
+-rw-rw-rw-   0        0        0     1170 2023-04-14 05:28:03.000000 py2nut-3.2.3/pynut_2files/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 03:25:34.490965 py2nut-3.2.3/pynut_3db/
+drwxrwxrwx   0        0        0        0 2023-04-17 03:25:34.504927 py2nut-3.2.3/pynut_3db/pyNutDB/
+-rw-rw-rw-   0        0        0       23 2023-03-07 04:17:04.000000 py2nut-3.2.3/pynut_3db/pyNutDB/__init__.py
+-rw-rw-rw-   0        0        0     2591 2022-12-05 13:21:28.000000 py2nut-3.2.3/pynut_3db/pyNutDB/_lib.py
+-rw-rw-rw-   0        0        0    21550 2023-03-07 04:17:05.000000 py2nut-3.2.3/pynut_3db/pyNutDB/nutDb.py
+-rw-rw-rw-   0        0        0     1051 2023-04-14 05:28:19.000000 py2nut-3.2.3/pynut_3db/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 03:25:34.509990 py2nut-3.2.3/pynut_3email/
+drwxrwxrwx   0        0        0        0 2023-04-17 03:25:34.525872 py2nut-3.2.3/pynut_3email/pyNutEmail/
+-rw-rw-rw-   0        0        0       21 2023-04-14 05:29:30.000000 py2nut-3.2.3/pynut_3email/pyNutEmail/__init__.py
+-rw-rw-rw-   0        0        0     4303 2022-12-05 13:20:03.000000 py2nut-3.2.3/pynut_3email/pyNutEmail/_lib.py
+-rw-rw-rw-   0        0        0    35893 2023-01-04 05:22:20.000000 py2nut-3.2.3/pynut_3email/pyNutEmail/nutEmail.py
+-rw-rw-rw-   0        0        0     1064 2023-04-14 05:28:29.000000 py2nut-3.2.3/pynut_3email/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 03:25:34.536843 py2nut-3.2.3/pynut_3ftp/
+drwxrwxrwx   0        0        0        0 2023-04-17 03:25:34.552852 py2nut-3.2.3/pynut_3ftp/pyNutFtp/
+-rw-rw-rw-   0        0        0       23 2023-04-14 05:29:30.000000 py2nut-3.2.3/pynut_3ftp/pyNutFtp/__init__.py
+-rw-rw-rw-   0        0        0     3476 2023-01-04 05:34:31.000000 py2nut-3.2.3/pynut_3ftp/pyNutFtp/_lib.py
+-rw-rw-rw-   0        0        0    29570 2023-01-04 05:57:55.000000 py2nut-3.2.3/pynut_3ftp/pyNutFtp/nutFtp.py
+-rw-rw-rw-   0        0        0     1072 2023-04-14 05:28:37.000000 py2nut-3.2.3/pynut_3ftp/setup.py
+-rw-rw-rw-   0        0        0       42 2023-04-17 03:25:34.566763 py2nut-3.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1565 2023-02-08 10:26:55.000000 py2nut-3.2.3/setup.py
```

### Comparing `py2nut-3.2.2/LICENSE` & `py2nut-3.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.2/PKG-INFO` & `py2nut-3.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py2nut
-Version: 3.2.2
+Version: 3.2.3
 Summary: This Library allows you to make Misc operations in various domain
 Home-page: https://github.com/Laurent-Tupin/py2nut
 Author: Laurent Tupin
 Author-email: laurent.tupinn@gmail.com
 License: Copyright 2022-2035
 Platform: UNKNOWN
 Classifier: License :: Free For Home Use
```

### Comparing `py2nut-3.2.2/README.md` & `py2nut-3.2.3/README.md`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.2/py2Nut/xlrd/xlsx.py` & `py2nut-3.2.3/py2Nut/xlrd/xlsx.py`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.2/py2nut.egg-info/PKG-INFO` & `py2nut-3.2.3/py2nut.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py2nut
-Version: 3.2.2
+Version: 3.2.3
 Summary: This Library allows you to make Misc operations in various domain
 Home-page: https://github.com/Laurent-Tupin/py2nut
 Author: Laurent Tupin
 Author-email: laurent.tupinn@gmail.com
 License: Copyright 2022-2035
 Platform: UNKNOWN
 Classifier: License :: Free For Home Use
```

### Comparing `py2nut-3.2.2/py2nut.egg-info/SOURCES.txt` & `py2nut-3.2.3/py2nut.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.2/pynut_1tools/pyNutTools/_lib.py` & `py2nut-3.2.3/pynut_1tools/pyNutTools/_lib.py`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.2/pynut_1tools/pyNutTools/nutDataframe.py` & `py2nut-3.2.3/pynut_1tools/pyNutTools/nutDataframe.py`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.2/pynut_1tools/pyNutTools/nutDate.py` & `py2nut-3.2.3/pynut_1tools/pyNutTools/nutDate.py`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.2/pynut_1tools/pyNutTools/nutOther.py` & `py2nut-3.2.3/pynut_1tools/pyNutTools/nutOther.py`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.2/pynut_1tools/setup.py` & `py2nut-3.2.3/pynut_1tools/setup.py`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.2/pynut_2api/pyNutApi/_lib.py` & `py2nut-3.2.3/pynut_2api/pyNutApi/_lib.py`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.2/pynut_2api/pyNutApi/nutApi.py` & `py2nut-3.2.3/pynut_2api/pyNutApi/nutApi.py`

 * *Files 1% similar despite different names*

```diff
@@ -403,31 +403,36 @@
         logger.error('  - URL : |{}|'.format( str_url ))
         raise
     if not fBL_checkConnexion(o_page):
         logger.error(' ERROR in fDf_bSoup_GetArray: fBL_checkConnexion(o_page): ')
         logger.error('  - URL : |{}|'.format(str_url))
         return False
     try:
-        bs_soup = BeautifulSoup(o_page.content, "html.parser")      # lxml   # html5lib
+        bs_soup =   BeautifulSoup(o_page.content, "html.parser")
     except Exception as err:
         logger.error(' ERROR in fDf_bSoup_GetArray: BeautifulSoup(o_page.content, "html.parser") : |{}|'.format(err))
         logger.error('  - URL : |{}|'.format( str_url ))
         raise
     try:
-        arr_result_tr = fArr_webScrapTableTr(bs_soup, bl_th = bl_th, bl_cleanXA0 = bl_cleanXA0)
-        arr_result_li = fArr_webScrapUlLi(bs_soup, bl_cleanXA0 = bl_cleanXA0)
+        arr_result_li =     fArr_webScrapUlLi(bs_soup, bl_cleanXA0 = bl_cleanXA0)
+        arr_result_tr =     fArr_webScrapTableTr(bs_soup, bl_th = bl_th, bl_cleanXA0 = bl_cleanXA0)
     except Exception as err:
         logger.error('  ERROR in fDf_bSoup_GetArray: LOOP on tables / rows / cells: |{}|'.format(err))
         logger.error('  - URL : |{}|'.format(str_url))
         raise
     # END
     try:
-        df1 =   pd.DataFrame(arr_result_tr)
-        df2 =   pd.DataFrame(arr_result_li)
-        df =    dframe.fDf_Concat_wColOfDf1(df1, df2)
+        if arr_result_li == []:
+            df =    pd.DataFrame(arr_result_tr)
+        elif arr_result_tr == []:
+            df =    pd.DataFrame(arr_result_li)
+        else:
+            df1 =   pd.DataFrame(arr_result_li)
+            df2 =   pd.DataFrame(arr_result_tr)
+            df =    dframe.fDf_Concat_wColOfDf1(df1, df2, int_emptyRow = 1)
     except Exception as err:
         logger.error('  ERROR in fDf_bSoup_GetArray: Pandas Dataframe: |{}|'.format(err))
         logger.error('  - URL : |{}|'.format(str_url))
         raise
     return df
```

### Comparing `py2nut-3.2.2/pynut_2api/setup.py` & `py2nut-3.2.3/pynut_2api/setup.py`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.2/pynut_2files/pyNutFiles/_lib.py` & `py2nut-3.2.3/pynut_2files/pyNutFiles/_lib.py`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.2/pynut_2files/pyNutFiles/nutFiles.py` & `py2nut-3.2.3/pynut_2files/pyNutFiles/nutFiles.py`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.2/pynut_2files/setup.py` & `py2nut-3.2.3/pynut_2files/setup.py`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.2/pynut_3db/pyNutDB/_lib.py` & `py2nut-3.2.3/pynut_3db/pyNutDB/_lib.py`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.2/pynut_3db/pyNutDB/nutDb.py` & `py2nut-3.2.3/pynut_3db/pyNutDB/nutDb.py`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.2/pynut_3db/setup.py` & `py2nut-3.2.3/pynut_3db/setup.py`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.2/pynut_3email/pyNutEmail/_lib.py` & `py2nut-3.2.3/pynut_3email/pyNutEmail/_lib.py`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.2/pynut_3email/pyNutEmail/nutEmail.py` & `py2nut-3.2.3/pynut_3email/pyNutEmail/nutEmail.py`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.2/pynut_3email/setup.py` & `py2nut-3.2.3/pynut_3email/setup.py`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.2/pynut_3ftp/pyNutFtp/_lib.py` & `py2nut-3.2.3/pynut_3ftp/pyNutFtp/_lib.py`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.2/pynut_3ftp/pyNutFtp/nutFtp.py` & `py2nut-3.2.3/pynut_3ftp/pyNutFtp/nutFtp.py`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.2/pynut_3ftp/setup.py` & `py2nut-3.2.3/pynut_3ftp/setup.py`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.2/setup.py` & `py2nut-3.2.3/setup.py`

 * *Files identical despite different names*

