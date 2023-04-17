# Comparing `tmp/kmerator-0.7.3b0.tar.gz` & `tmp/kmerator-0.7.4b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kmerator-0.7.3b0.tar", last modified: Wed Apr 12 13:40:52 2023, max compression
+gzip compressed data, was "kmerator-0.7.4b0.tar", last modified: Mon Apr 17 07:39:42 2023, max compression
```

## Comparing `kmerator-0.7.3b0.tar` & `kmerator-0.7.4b0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2023-04-12 13:40:52.350484 kmerator-0.7.3b0/
--rw-r--r--   0 benoit    (1017) bio2m     (1010)      180 2023-04-12 13:16:53.000000 kmerator-0.7.3b0/MANIFEST.in
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)    13140 2023-04-12 13:40:52.347167 kmerator-0.7.3b0/PKG-INFO
--rw-r--r--   0 benoit    (1017) bio2m     (1010)    11313 2023-03-07 12:59:57.000000 kmerator-0.7.3b0/README.md
-drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2023-04-12 13:40:52.245235 kmerator-0.7.3b0/img/
--rw-r--r--   0 benoit    (1017) bio2m     (1010)    19242 2022-07-21 09:53:27.000000 kmerator-0.7.3b0/img/specific-contigs.png
--rw-r--r--   0 benoit    (1017) bio2m     (1010)    65389 2022-07-21 09:52:52.000000 kmerator-0.7.3b0/img/specific-kmers.png
-drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2023-04-12 13:40:52.330993 kmerator-0.7.3b0/kmerator.egg-info/
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)    13140 2023-04-12 13:40:52.000000 kmerator-0.7.3b0/kmerator.egg-info/PKG-INFO
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)      272 2023-04-12 13:40:52.000000 kmerator-0.7.3b0/kmerator.egg-info/SOURCES.txt
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)        1 2023-04-12 13:40:52.000000 kmerator-0.7.3b0/kmerator.egg-info/dependency_links.txt
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)       53 2023-04-12 13:40:52.000000 kmerator-0.7.3b0/kmerator.egg-info/entry_points.txt
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)       18 2023-04-12 13:40:52.000000 kmerator-0.7.3b0/kmerator.egg-info/requires.txt
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)        1 2023-04-12 13:40:52.000000 kmerator-0.7.3b0/kmerator.egg-info/top_level.txt
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)       38 2023-04-12 13:40:52.353102 kmerator-0.7.3b0/setup.cfg
--rw-r--r--   0 benoit    (1017) bio2m     (1010)     1008 2023-02-28 16:14:06.000000 kmerator-0.7.3b0/setup.py
+drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2023-04-17 07:39:42.686406 kmerator-0.7.4b0/
+-rw-r--r--   0 benoit    (1017) bio2m     (1010)      182 2023-04-17 07:20:43.000000 kmerator-0.7.4b0/MANIFEST.in
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)    13140 2023-04-17 07:39:42.682873 kmerator-0.7.4b0/PKG-INFO
+-rw-r--r--   0 benoit    (1017) bio2m     (1010)    11313 2023-03-07 12:59:57.000000 kmerator-0.7.4b0/README.md
+drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2023-04-17 07:39:42.588153 kmerator-0.7.4b0/img/
+-rw-r--r--   0 benoit    (1017) bio2m     (1010)    19242 2022-07-21 09:53:27.000000 kmerator-0.7.4b0/img/specific-contigs.png
+-rw-r--r--   0 benoit    (1017) bio2m     (1010)    65389 2022-07-21 09:52:52.000000 kmerator-0.7.4b0/img/specific-kmers.png
+drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2023-04-17 07:39:42.668444 kmerator-0.7.4b0/kmerator.egg-info/
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)    13140 2023-04-17 07:39:42.000000 kmerator-0.7.4b0/kmerator.egg-info/PKG-INFO
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)      272 2023-04-17 07:39:42.000000 kmerator-0.7.4b0/kmerator.egg-info/SOURCES.txt
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)        1 2023-04-17 07:39:42.000000 kmerator-0.7.4b0/kmerator.egg-info/dependency_links.txt
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)       53 2023-04-17 07:39:42.000000 kmerator-0.7.4b0/kmerator.egg-info/entry_points.txt
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)       18 2023-04-17 07:39:42.000000 kmerator-0.7.4b0/kmerator.egg-info/requires.txt
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)        1 2023-04-17 07:39:42.000000 kmerator-0.7.4b0/kmerator.egg-info/top_level.txt
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)       38 2023-04-17 07:39:42.688722 kmerator-0.7.4b0/setup.cfg
+-rw-r--r--   0 benoit    (1017) bio2m     (1010)     1008 2023-02-28 16:14:06.000000 kmerator-0.7.4b0/setup.py
```

### Comparing `kmerator-0.7.3b0/PKG-INFO` & `kmerator-0.7.4b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kmerator
-Version: 0.7.3b0
+Version: 0.7.4b0
 Summary: Find specific gene or transcript kmers. And more.
 Home-page: https://github.com/Transipedia/kmerator
 Author: Sébastien RIQUIER, IRMB, Montpellier
 Author-email: sebastien.riquier@ucd.ie
 License: GPLv3
 Description: # Kmerator
```

### Comparing `kmerator-0.7.3b0/README.md` & `kmerator-0.7.4b0/README.md`

 * *Files identical despite different names*

### Comparing `kmerator-0.7.3b0/img/specific-contigs.png` & `kmerator-0.7.4b0/img/specific-contigs.png`

 * *Files identical despite different names*

### Comparing `kmerator-0.7.3b0/img/specific-kmers.png` & `kmerator-0.7.4b0/img/specific-kmers.png`

 * *Files identical despite different names*

### Comparing `kmerator-0.7.3b0/kmerator.egg-info/PKG-INFO` & `kmerator-0.7.4b0/kmerator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kmerator
-Version: 0.7.3b0
+Version: 0.7.4b0
 Summary: Find specific gene or transcript kmers. And more.
 Home-page: https://github.com/Transipedia/kmerator
 Author: Sébastien RIQUIER, IRMB, Montpellier
 Author-email: sebastien.riquier@ucd.ie
 License: GPLv3
 Description: # Kmerator
```

### Comparing `kmerator-0.7.3b0/setup.py` & `kmerator-0.7.4b0/setup.py`

 * *Files identical despite different names*

