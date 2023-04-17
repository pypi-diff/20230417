# Comparing `tmp/nxtomomill-0.9.0a2.tar.gz` & `tmp/nxtomomill-0.9.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nxtomomill-0.9.0a2.tar", last modified: Thu Jun 16 09:32:20 2022, max compression
+gzip compressed data, was "dist/nxtomomill-0.9.0a3.tar", last modified: Fri Jun 24 07:15:50 2022, max compression
```

## Comparing `nxtomomill-0.9.0a2.tar` & `nxtomomill-0.9.0a3.tar`

### file list

```diff
@@ -1,88 +1,89 @@
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2022-06-16 09:32:20.316707 nxtomomill-0.9.0a2/
--rw-r--r--   0 payno    (81067) soft      (3401)     1257 2022-01-07 07:14:39.000000 nxtomomill-0.9.0a2/LICENSE
--rw-r--r--   0 payno    (81067) soft      (3401)     2083 2022-06-16 09:32:20.316707 nxtomomill-0.9.0a2/PKG-INFO
--rw-r--r--   0 payno    (81067) soft      (3401)     1104 2022-04-13 12:11:35.000000 nxtomomill-0.9.0a2/README.md
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2022-06-16 09:32:20.312707 nxtomomill-0.9.0a2/nxtomomill/
--rw-r--r--   0 payno    (81067) soft      (3401)       67 2022-03-14 15:58:43.000000 nxtomomill-0.9.0a2/nxtomomill/__init__.py
--rw-r--r--   0 payno    (81067) soft      (3401)     8483 2022-04-27 11:12:26.000000 nxtomomill-0.9.0a2/nxtomomill/__main__.py
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2022-06-16 09:32:20.312707 nxtomomill-0.9.0a2/nxtomomill/app/
--rw-r--r--   0 payno    (81067) soft      (3401)        0 2022-01-07 07:14:39.000000 nxtomomill-0.9.0a2/nxtomomill/app/__init__.py
--rw-r--r--   0 payno    (81067) soft      (3401)     8697 2022-04-27 11:12:26.000000 nxtomomill-0.9.0a2/nxtomomill/app/dxfile2nx.py
--rw-r--r--   0 payno    (81067) soft      (3401)     5145 2022-06-07 06:53:13.000000 nxtomomill-0.9.0a2/nxtomomill/app/edf2nx.py
--rw-r--r--   0 payno    (81067) soft      (3401)     2523 2022-04-27 11:12:26.000000 nxtomomill-0.9.0a2/nxtomomill/app/edfquickstart.py
--rw-r--r--   0 payno    (81067) soft      (3401)    15751 2022-04-27 11:12:26.000000 nxtomomill-0.9.0a2/nxtomomill/app/h52nx.py
--rw-r--r--   0 payno    (81067) soft      (3401)    15120 2022-04-27 11:12:26.000000 nxtomomill-0.9.0a2/nxtomomill/app/h5_3dxrd2nx.py
--rw-r--r--   0 payno    (81067) soft      (3401)     4170 2022-04-27 11:12:26.000000 nxtomomill-0.9.0a2/nxtomomill/app/h5quickstart.py
--rw-r--r--   0 payno    (81067) soft      (3401)    15329 2022-03-24 07:58:10.000000 nxtomomill-0.9.0a2/nxtomomill/app/patch_nx.py
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2022-06-16 09:32:20.312707 nxtomomill-0.9.0a2/nxtomomill/converter/
--rw-r--r--   0 payno    (81067) soft      (3401)      410 2022-04-27 11:12:26.000000 nxtomomill-0.9.0a2/nxtomomill/converter/__init__.py
--rw-r--r--   0 payno    (81067) soft      (3401)     1530 2022-01-07 07:14:39.000000 nxtomomill-0.9.0a2/nxtomomill/converter/baseconverter.py
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2022-06-16 09:32:20.312707 nxtomomill-0.9.0a2/nxtomomill/converter/dxfile/
--rw-r--r--   0 payno    (81067) soft      (3401)     1508 2022-03-24 07:58:10.000000 nxtomomill-0.9.0a2/nxtomomill/converter/dxfile/__init__.py
--rw-r--r--   0 payno    (81067) soft      (3401)    26420 2022-03-24 07:58:10.000000 nxtomomill-0.9.0a2/nxtomomill/converter/dxfile/dxfileconverter.py
--rw-r--r--   0 payno    (81067) soft      (3401)     5032 2022-03-24 07:58:10.000000 nxtomomill-0.9.0a2/nxtomomill/converter/dxfile/test_dxfile.py
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2022-06-16 09:32:20.312707 nxtomomill-0.9.0a2/nxtomomill/converter/edf/
--rw-r--r--   0 payno    (81067) soft      (3401)        0 2022-01-07 07:14:39.000000 nxtomomill-0.9.0a2/nxtomomill/converter/edf/__init__.py
--rw-r--r--   0 payno    (81067) soft      (3401)    31376 2022-06-16 09:27:01.000000 nxtomomill-0.9.0a2/nxtomomill/converter/edf/edfconverter.py
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2022-06-16 09:32:20.312707 nxtomomill-0.9.0a2/nxtomomill/converter/hdf5/
--rw-r--r--   0 payno    (81067) soft      (3401)     1470 2022-01-07 07:14:39.000000 nxtomomill-0.9.0a2/nxtomomill/converter/hdf5/__init__.py
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2022-06-16 09:32:20.312707 nxtomomill-0.9.0a2/nxtomomill/converter/hdf5/acquisition/
--rw-r--r--   0 payno    (81067) soft      (3401)        0 2022-01-07 07:14:39.000000 nxtomomill-0.9.0a2/nxtomomill/converter/hdf5/acquisition/__init__.py
--rw-r--r--   0 payno    (81067) soft      (3401)    27859 2022-06-16 09:27:01.000000 nxtomomill-0.9.0a2/nxtomomill/converter/hdf5/acquisition/baseacquisition.py
--rw-r--r--   0 payno    (81067) soft      (3401)     7679 2022-03-24 08:36:12.000000 nxtomomill-0.9.0a2/nxtomomill/converter/hdf5/acquisition/pcotomoacquisition.py
--rw-r--r--   0 payno    (81067) soft      (3401)    40981 2022-06-16 09:27:01.000000 nxtomomill-0.9.0a2/nxtomomill/converter/hdf5/acquisition/standardacquisition.py
--rw-r--r--   0 payno    (81067) soft      (3401)     8249 2022-06-16 09:27:01.000000 nxtomomill-0.9.0a2/nxtomomill/converter/hdf5/acquisition/utils.py
--rw-r--r--   0 payno    (81067) soft      (3401)     4605 2022-03-24 07:58:10.000000 nxtomomill-0.9.0a2/nxtomomill/converter/hdf5/acquisition/xrd3dacquisition.py
--rw-r--r--   0 payno    (81067) soft      (3401)     4712 2022-03-24 07:58:10.000000 nxtomomill-0.9.0a2/nxtomomill/converter/hdf5/acquisition/xrdctacquisition.py
--rw-r--r--   0 payno    (81067) soft      (3401)     5872 2022-06-16 09:26:57.000000 nxtomomill-0.9.0a2/nxtomomill/converter/hdf5/acquisition/zseriesacquisition.py
--rw-r--r--   0 payno    (81067) soft      (3401)    39454 2022-06-16 09:27:01.000000 nxtomomill-0.9.0a2/nxtomomill/converter/hdf5/hdf5converter.py
--rw-r--r--   0 payno    (81067) soft      (3401)     1750 2022-01-07 07:14:39.000000 nxtomomill-0.9.0a2/nxtomomill/converter/hdf5/setup.py
--rw-r--r--   0 payno    (81067) soft      (3401)     1925 2022-06-16 09:26:57.000000 nxtomomill-0.9.0a2/nxtomomill/converter/hdf5/utils.py
--rw-r--r--   0 payno    (81067) soft      (3401)     1783 2022-01-07 07:14:39.000000 nxtomomill-0.9.0a2/nxtomomill/converter/setup.py
--rw-r--r--   0 payno    (81067) soft      (3401)     1522 2022-06-16 09:27:01.000000 nxtomomill-0.9.0a2/nxtomomill/converter/version.py
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2022-06-16 09:32:20.316707 nxtomomill-0.9.0a2/nxtomomill/io/
--rw-r--r--   0 payno    (81067) soft      (3401)       40 2022-03-24 07:58:10.000000 nxtomomill-0.9.0a2/nxtomomill/io/__init__.py
--rw-r--r--   0 payno    (81067) soft      (3401)     3672 2022-05-02 11:24:26.000000 nxtomomill-0.9.0a2/nxtomomill/io/acquisitionstep.py
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2022-06-16 09:32:20.316707 nxtomomill-0.9.0a2/nxtomomill/io/config/
--rw-r--r--   0 payno    (81067) soft      (3401)     1626 2022-04-27 11:12:26.000000 nxtomomill-0.9.0a2/nxtomomill/io/config/__init__.py
--rw-r--r--   0 payno    (81067) soft      (3401)     8417 2022-06-16 09:27:01.000000 nxtomomill-0.9.0a2/nxtomomill/io/config/configbase.py
--rw-r--r--   0 payno    (81067) soft      (3401)    13260 2022-04-27 11:12:26.000000 nxtomomill-0.9.0a2/nxtomomill/io/config/confighandler.py
--rw-r--r--   0 payno    (81067) soft      (3401)    38407 2022-06-16 09:27:01.000000 nxtomomill-0.9.0a2/nxtomomill/io/config/edfconfig.py
--rw-r--r--   0 payno    (81067) soft      (3401)    48461 2022-06-16 09:27:01.000000 nxtomomill-0.9.0a2/nxtomomill/io/config/hdf5config.py
--rw-r--r--   0 payno    (81067) soft      (3401)    13274 2022-04-27 11:12:26.000000 nxtomomill-0.9.0a2/nxtomomill/io/confighandler.py
--rw-r--r--   0 payno    (81067) soft      (3401)    12612 2022-03-24 07:58:10.000000 nxtomomill-0.9.0a2/nxtomomill/io/framegroup.py
--rw-r--r--   0 payno    (81067) soft      (3401)     1706 2022-01-07 07:14:39.000000 nxtomomill-0.9.0a2/nxtomomill/io/setup.py
--rw-r--r--   0 payno    (81067) soft      (3401)     5198 2022-04-27 11:12:26.000000 nxtomomill-0.9.0a2/nxtomomill/io/utils.py
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2022-06-16 09:32:20.316707 nxtomomill-0.9.0a2/nxtomomill/nexus/
--rw-r--r--   0 payno    (81067) soft      (3401)      264 2022-06-07 06:53:13.000000 nxtomomill-0.9.0a2/nxtomomill/nexus/__init__.py
--rw-r--r--   0 payno    (81067) soft      (3401)    29595 2022-06-16 09:27:01.000000 nxtomomill-0.9.0a2/nxtomomill/nexus/nxdetector.py
--rw-r--r--   0 payno    (81067) soft      (3401)     8498 2022-06-07 06:53:13.000000 nxtomomill-0.9.0a2/nxtomomill/nexus/nxinstrument.py
--rw-r--r--   0 payno    (81067) soft      (3401)     4778 2022-06-16 09:27:01.000000 nxtomomill-0.9.0a2/nxtomomill/nexus/nxmonitor.py
--rw-r--r--   0 payno    (81067) soft      (3401)    11001 2022-06-07 06:53:13.000000 nxtomomill-0.9.0a2/nxtomomill/nexus/nxobject.py
--rw-r--r--   0 payno    (81067) soft      (3401)    10158 2022-06-07 06:53:13.000000 nxtomomill-0.9.0a2/nxtomomill/nexus/nxsample.py
--rw-r--r--   0 payno    (81067) soft      (3401)     5996 2022-06-07 06:53:13.000000 nxtomomill-0.9.0a2/nxtomomill/nexus/nxsource.py
--rw-r--r--   0 payno    (81067) soft      (3401)    15656 2022-06-16 09:27:01.000000 nxtomomill-0.9.0a2/nxtomomill/nexus/nxtomo.py
--rw-r--r--   0 payno    (81067) soft      (3401)     5343 2022-06-14 14:51:40.000000 nxtomomill-0.9.0a2/nxtomomill/nexus/utils.py
--rw-r--r--   0 payno    (81067) soft      (3401)     6991 2022-03-24 07:58:10.000000 nxtomomill-0.9.0a2/nxtomomill/plugins.py
--rw-r--r--   0 payno    (81067) soft      (3401)     5587 2022-06-16 09:27:01.000000 nxtomomill-0.9.0a2/nxtomomill/settings.py
--rw-r--r--   0 payno    (81067) soft      (3401)     1785 2022-01-07 07:14:39.000000 nxtomomill-0.9.0a2/nxtomomill/setup.py
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2022-06-16 09:32:20.316707 nxtomomill-0.9.0a2/nxtomomill/utils/
--rw-r--r--   0 payno    (81067) soft      (3401)      721 2022-03-24 07:58:10.000000 nxtomomill-0.9.0a2/nxtomomill/utils/__init__.py
--rw-r--r--   0 payno    (81067) soft      (3401)     1614 2022-03-24 07:58:10.000000 nxtomomill-0.9.0a2/nxtomomill/utils/context.py
--rw-r--r--   0 payno    (81067) soft      (3401)     1799 2022-03-24 07:58:10.000000 nxtomomill-0.9.0a2/nxtomomill/utils/file_path.py
--rw-r--r--   0 payno    (81067) soft      (3401)    16964 2022-04-13 13:58:58.000000 nxtomomill-0.9.0a2/nxtomomill/utils/frameappender.py
--rw-r--r--   0 payno    (81067) soft      (3401)     3245 2022-04-13 13:58:58.000000 nxtomomill-0.9.0a2/nxtomomill/utils/h5pyutils.py
--rw-r--r--   0 payno    (81067) soft      (3401)     3190 2022-03-24 07:58:10.000000 nxtomomill-0.9.0a2/nxtomomill/utils/hdf5.py
--rw-r--r--   0 payno    (81067) soft      (3401)    18170 2022-04-13 13:50:23.000000 nxtomomill-0.9.0a2/nxtomomill/utils/nxsplitter.py
--rw-r--r--   0 payno    (81067) soft      (3401)     3112 2022-05-19 08:39:46.000000 nxtomomill-0.9.0a2/nxtomomill/utils/progress.py
--rw-r--r--   0 payno    (81067) soft      (3401)    19320 2022-06-16 09:27:01.000000 nxtomomill-0.9.0a2/nxtomomill/utils/utils.py
--rw-r--r--   0 payno    (81067) soft      (3401)     4345 2022-06-16 09:30:29.000000 nxtomomill-0.9.0a2/nxtomomill/version.py
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2022-06-16 09:32:20.312707 nxtomomill-0.9.0a2/nxtomomill.egg-info/
--rw-r--r--   0 payno    (81067) soft      (3401)     2083 2022-06-16 09:32:20.000000 nxtomomill-0.9.0a2/nxtomomill.egg-info/PKG-INFO
--rw-r--r--   0 payno    (81067) soft      (3401)     2406 2022-06-16 09:32:20.000000 nxtomomill-0.9.0a2/nxtomomill.egg-info/SOURCES.txt
--rw-r--r--   0 payno    (81067) soft      (3401)        1 2022-06-16 09:32:20.000000 nxtomomill-0.9.0a2/nxtomomill.egg-info/dependency_links.txt
--rw-r--r--   0 payno    (81067) soft      (3401)       57 2022-06-16 09:32:20.000000 nxtomomill-0.9.0a2/nxtomomill.egg-info/entry_points.txt
--rw-r--r--   0 payno    (81067) soft      (3401)      187 2022-06-16 09:32:20.000000 nxtomomill-0.9.0a2/nxtomomill.egg-info/requires.txt
--rw-r--r--   0 payno    (81067) soft      (3401)       11 2022-06-16 09:32:20.000000 nxtomomill-0.9.0a2/nxtomomill.egg-info/top_level.txt
--rw-r--r--   0 payno    (81067) soft      (3401)     1282 2022-06-16 09:32:20.316707 nxtomomill-0.9.0a2/setup.cfg
--rw-r--r--   0 payno    (81067) soft      (3401)     1487 2022-03-14 15:58:43.000000 nxtomomill-0.9.0a2/setup.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2022-06-24 07:15:50.000000 nxtomomill-0.9.0a3/
+-rw-r--r--   0 payno     (1000) payno     (1000)     1257 2022-01-07 07:17:40.000000 nxtomomill-0.9.0a3/LICENSE
+-rw-r--r--   0 payno     (1000) payno     (1000)     2083 2022-06-24 07:15:50.000000 nxtomomill-0.9.0a3/PKG-INFO
+-rw-r--r--   0 payno     (1000) payno     (1000)     1104 2022-04-06 12:57:56.000000 nxtomomill-0.9.0a3/README.md
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2022-06-24 07:15:50.000000 nxtomomill-0.9.0a3/nxtomomill/
+-rw-r--r--   0 payno     (1000) payno     (1000)       67 2022-01-07 07:17:40.000000 nxtomomill-0.9.0a3/nxtomomill/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     8483 2022-06-17 09:56:13.000000 nxtomomill-0.9.0a3/nxtomomill/__main__.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2022-06-24 07:15:50.000000 nxtomomill-0.9.0a3/nxtomomill/app/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2022-01-07 07:17:40.000000 nxtomomill-0.9.0a3/nxtomomill/app/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     8697 2022-06-17 09:56:13.000000 nxtomomill-0.9.0a3/nxtomomill/app/dxfile2nx.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     5145 2022-06-17 09:56:13.000000 nxtomomill-0.9.0a3/nxtomomill/app/edf2nx.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2523 2022-06-17 09:56:13.000000 nxtomomill-0.9.0a3/nxtomomill/app/edfquickstart.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    15751 2022-06-17 09:56:13.000000 nxtomomill-0.9.0a3/nxtomomill/app/h52nx.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    15120 2022-06-17 09:56:13.000000 nxtomomill-0.9.0a3/nxtomomill/app/h5_3dxrd2nx.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     4170 2022-06-17 09:56:13.000000 nxtomomill-0.9.0a3/nxtomomill/app/h5quickstart.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    15329 2022-03-25 07:14:03.000000 nxtomomill-0.9.0a3/nxtomomill/app/patch_nx.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2022-06-24 07:15:50.000000 nxtomomill-0.9.0a3/nxtomomill/converter/
+-rw-r--r--   0 payno     (1000) payno     (1000)      410 2022-06-17 09:56:13.000000 nxtomomill-0.9.0a3/nxtomomill/converter/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1530 2022-01-07 07:17:40.000000 nxtomomill-0.9.0a3/nxtomomill/converter/baseconverter.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2022-06-24 07:15:50.000000 nxtomomill-0.9.0a3/nxtomomill/converter/dxfile/
+-rw-r--r--   0 payno     (1000) payno     (1000)     1508 2022-02-03 09:31:26.000000 nxtomomill-0.9.0a3/nxtomomill/converter/dxfile/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    26420 2022-03-25 07:14:03.000000 nxtomomill-0.9.0a3/nxtomomill/converter/dxfile/dxfileconverter.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     5032 2022-03-25 07:14:03.000000 nxtomomill-0.9.0a3/nxtomomill/converter/dxfile/test_dxfile.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2022-06-24 07:15:50.000000 nxtomomill-0.9.0a3/nxtomomill/converter/edf/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2022-01-07 07:17:40.000000 nxtomomill-0.9.0a3/nxtomomill/converter/edf/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    31376 2022-06-17 09:57:26.000000 nxtomomill-0.9.0a3/nxtomomill/converter/edf/edfconverter.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2022-06-24 07:15:50.000000 nxtomomill-0.9.0a3/nxtomomill/converter/hdf5/
+-rw-r--r--   0 payno     (1000) payno     (1000)     1470 2022-01-07 07:17:40.000000 nxtomomill-0.9.0a3/nxtomomill/converter/hdf5/__init__.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2022-06-24 07:15:50.000000 nxtomomill-0.9.0a3/nxtomomill/converter/hdf5/acquisition/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2022-01-07 07:17:40.000000 nxtomomill-0.9.0a3/nxtomomill/converter/hdf5/acquisition/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    27859 2022-06-20 19:21:23.000000 nxtomomill-0.9.0a3/nxtomomill/converter/hdf5/acquisition/baseacquisition.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     7679 2022-03-25 07:14:03.000000 nxtomomill-0.9.0a3/nxtomomill/converter/hdf5/acquisition/pcotomoacquisition.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    40981 2022-06-20 19:21:23.000000 nxtomomill-0.9.0a3/nxtomomill/converter/hdf5/acquisition/standardacquisition.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     8249 2022-06-17 09:57:26.000000 nxtomomill-0.9.0a3/nxtomomill/converter/hdf5/acquisition/utils.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     4605 2022-03-25 07:14:03.000000 nxtomomill-0.9.0a3/nxtomomill/converter/hdf5/acquisition/xrd3dacquisition.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     4712 2022-03-25 07:14:03.000000 nxtomomill-0.9.0a3/nxtomomill/converter/hdf5/acquisition/xrdctacquisition.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     5872 2022-06-20 19:21:23.000000 nxtomomill-0.9.0a3/nxtomomill/converter/hdf5/acquisition/zseriesacquisition.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    39454 2022-06-20 19:21:23.000000 nxtomomill-0.9.0a3/nxtomomill/converter/hdf5/hdf5converter.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1750 2022-01-07 07:17:40.000000 nxtomomill-0.9.0a3/nxtomomill/converter/hdf5/setup.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1925 2022-06-20 19:21:23.000000 nxtomomill-0.9.0a3/nxtomomill/converter/hdf5/utils.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1783 2022-01-07 07:17:40.000000 nxtomomill-0.9.0a3/nxtomomill/converter/setup.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1522 2022-06-17 09:57:26.000000 nxtomomill-0.9.0a3/nxtomomill/converter/version.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2022-06-24 07:15:50.000000 nxtomomill-0.9.0a3/nxtomomill/io/
+-rw-r--r--   0 payno     (1000) payno     (1000)       40 2022-02-03 09:31:27.000000 nxtomomill-0.9.0a3/nxtomomill/io/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3672 2022-03-25 07:14:03.000000 nxtomomill-0.9.0a3/nxtomomill/io/acquisitionstep.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2022-06-24 07:15:50.000000 nxtomomill-0.9.0a3/nxtomomill/io/config/
+-rw-r--r--   0 payno     (1000) payno     (1000)     1626 2022-06-17 09:56:13.000000 nxtomomill-0.9.0a3/nxtomomill/io/config/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     8417 2022-06-17 09:57:26.000000 nxtomomill-0.9.0a3/nxtomomill/io/config/configbase.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    13260 2022-06-17 09:56:13.000000 nxtomomill-0.9.0a3/nxtomomill/io/config/confighandler.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    38406 2022-06-24 07:14:00.000000 nxtomomill-0.9.0a3/nxtomomill/io/config/edfconfig.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    48461 2022-06-20 19:21:23.000000 nxtomomill-0.9.0a3/nxtomomill/io/config/hdf5config.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    13274 2022-06-17 09:56:13.000000 nxtomomill-0.9.0a3/nxtomomill/io/confighandler.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    12612 2022-02-03 09:31:27.000000 nxtomomill-0.9.0a3/nxtomomill/io/framegroup.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1706 2022-01-07 07:17:40.000000 nxtomomill-0.9.0a3/nxtomomill/io/setup.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     5198 2022-06-17 09:56:13.000000 nxtomomill-0.9.0a3/nxtomomill/io/utils.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2022-06-24 07:15:50.000000 nxtomomill-0.9.0a3/nxtomomill/nexus/
+-rw-r--r--   0 payno     (1000) payno     (1000)      264 2022-06-17 09:56:13.000000 nxtomomill-0.9.0a3/nxtomomill/nexus/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    30309 2022-06-24 07:14:00.000000 nxtomomill-0.9.0a3/nxtomomill/nexus/nxdetector.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     8498 2022-06-17 09:56:13.000000 nxtomomill-0.9.0a3/nxtomomill/nexus/nxinstrument.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     4778 2022-06-17 09:57:26.000000 nxtomomill-0.9.0a3/nxtomomill/nexus/nxmonitor.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    11795 2022-06-24 07:14:00.000000 nxtomomill-0.9.0a3/nxtomomill/nexus/nxobject.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    10158 2022-06-17 09:56:13.000000 nxtomomill-0.9.0a3/nxtomomill/nexus/nxsample.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     5996 2022-06-17 09:56:13.000000 nxtomomill-0.9.0a3/nxtomomill/nexus/nxsource.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    15656 2022-06-20 19:21:23.000000 nxtomomill-0.9.0a3/nxtomomill/nexus/nxtomo.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1646 2022-04-05 15:04:20.000000 nxtomomill-0.9.0a3/nxtomomill/nexus/nxtransformations.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     5343 2022-06-17 09:56:13.000000 nxtomomill-0.9.0a3/nxtomomill/nexus/utils.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     6991 2022-03-25 07:14:03.000000 nxtomomill-0.9.0a3/nxtomomill/plugins.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     5587 2022-06-20 19:21:23.000000 nxtomomill-0.9.0a3/nxtomomill/settings.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1785 2022-01-07 07:17:40.000000 nxtomomill-0.9.0a3/nxtomomill/setup.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2022-06-24 07:15:50.000000 nxtomomill-0.9.0a3/nxtomomill/utils/
+-rw-r--r--   0 payno     (1000) payno     (1000)      721 2022-03-25 07:14:03.000000 nxtomomill-0.9.0a3/nxtomomill/utils/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1614 2022-03-25 07:14:03.000000 nxtomomill-0.9.0a3/nxtomomill/utils/context.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1799 2022-03-25 07:14:03.000000 nxtomomill-0.9.0a3/nxtomomill/utils/file_path.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    16964 2022-06-17 09:56:13.000000 nxtomomill-0.9.0a3/nxtomomill/utils/frameappender.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3245 2022-06-17 09:56:13.000000 nxtomomill-0.9.0a3/nxtomomill/utils/h5pyutils.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3190 2022-03-25 07:14:03.000000 nxtomomill-0.9.0a3/nxtomomill/utils/hdf5.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    18170 2022-03-25 07:14:03.000000 nxtomomill-0.9.0a3/nxtomomill/utils/nxsplitter.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3112 2022-03-25 07:14:03.000000 nxtomomill-0.9.0a3/nxtomomill/utils/progress.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    19320 2022-06-17 09:57:26.000000 nxtomomill-0.9.0a3/nxtomomill/utils/utils.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     4345 2022-06-24 07:15:25.000000 nxtomomill-0.9.0a3/nxtomomill/version.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2022-06-24 07:15:50.000000 nxtomomill-0.9.0a3/nxtomomill.egg-info/
+-rw-r--r--   0 payno     (1000) payno     (1000)     2083 2022-06-24 07:15:50.000000 nxtomomill-0.9.0a3/nxtomomill.egg-info/PKG-INFO
+-rw-r--r--   0 payno     (1000) payno     (1000)     2444 2022-06-24 07:15:50.000000 nxtomomill-0.9.0a3/nxtomomill.egg-info/SOURCES.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)        1 2022-06-24 07:15:50.000000 nxtomomill-0.9.0a3/nxtomomill.egg-info/dependency_links.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)       57 2022-06-24 07:15:50.000000 nxtomomill-0.9.0a3/nxtomomill.egg-info/entry_points.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)      187 2022-06-24 07:15:50.000000 nxtomomill-0.9.0a3/nxtomomill.egg-info/requires.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)       11 2022-06-24 07:15:50.000000 nxtomomill-0.9.0a3/nxtomomill.egg-info/top_level.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)     1282 2022-06-24 07:15:50.000000 nxtomomill-0.9.0a3/setup.cfg
+-rw-r--r--   0 payno     (1000) payno     (1000)     1487 2022-01-07 07:17:40.000000 nxtomomill-0.9.0a3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `nxtomomill-0.9.0a2/LICENSE` & `nxtomomill-0.9.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `nxtomomill-0.9.0a2/PKG-INFO` & `nxtomomill-0.9.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nxtomomill
-Version: 0.9.0a2
+Version: 0.9.0a3
 Summary: "applications and library to convert raw format to NXTomo format"
 Home-page: https://gitlab.esrf.fr/tomotools/nxtomomill
 Author: data analysis unit
 Author-email: henri.payno@esrf.fr
 License: MIT
 Project-URL: Bug Tracker, https://gitlab.esrf.fr/tomotools/nxtomomill/-/issues
 Platform: UNKNOWN
```

### Comparing `nxtomomill-0.9.0a2/README.md` & `nxtomomill-0.9.0a3/README.md`

 * *Files identical despite different names*

### Comparing `nxtomomill-0.9.0a2/nxtomomill/__main__.py` & `nxtomomill-0.9.0a3/nxtomomill/__main__.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-0.9.0a2/nxtomomill/app/dxfile2nx.py` & `nxtomomill-0.9.0a3/nxtomomill/app/dxfile2nx.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-0.9.0a2/nxtomomill/app/edf2nx.py` & `nxtomomill-0.9.0a3/nxtomomill/app/edf2nx.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-0.9.0a2/nxtomomill/app/edfquickstart.py` & `nxtomomill-0.9.0a3/nxtomomill/app/edfquickstart.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-0.9.0a2/nxtomomill/app/h52nx.py` & `nxtomomill-0.9.0a3/nxtomomill/app/h52nx.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-0.9.0a2/nxtomomill/app/h5_3dxrd2nx.py` & `nxtomomill-0.9.0a3/nxtomomill/app/h5_3dxrd2nx.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-0.9.0a2/nxtomomill/app/h5quickstart.py` & `nxtomomill-0.9.0a3/nxtomomill/app/h5quickstart.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-0.9.0a2/nxtomomill/app/patch_nx.py` & `nxtomomill-0.9.0a3/nxtomomill/app/patch_nx.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-0.9.0a2/nxtomomill/converter/baseconverter.py` & `nxtomomill-0.9.0a3/nxtomomill/converter/baseconverter.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-0.9.0a2/nxtomomill/converter/dxfile/__init__.py` & `nxtomomill-0.9.0a3/nxtomomill/converter/dxfile/__init__.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-0.9.0a2/nxtomomill/converter/dxfile/dxfileconverter.py` & `nxtomomill-0.9.0a3/nxtomomill/converter/dxfile/dxfileconverter.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-0.9.0a2/nxtomomill/converter/dxfile/test_dxfile.py` & `nxtomomill-0.9.0a3/nxtomomill/converter/dxfile/test_dxfile.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-0.9.0a2/nxtomomill/converter/edf/edfconverter.py` & `nxtomomill-0.9.0a3/nxtomomill/converter/edf/edfconverter.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-0.9.0a2/nxtomomill/converter/hdf5/__init__.py` & `nxtomomill-0.9.0a3/nxtomomill/converter/hdf5/__init__.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-0.9.0a2/nxtomomill/converter/hdf5/acquisition/baseacquisition.py` & `nxtomomill-0.9.0a3/nxtomomill/converter/hdf5/acquisition/baseacquisition.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-0.9.0a2/nxtomomill/converter/hdf5/acquisition/pcotomoacquisition.py` & `nxtomomill-0.9.0a3/nxtomomill/converter/hdf5/acquisition/pcotomoacquisition.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-0.9.0a2/nxtomomill/converter/hdf5/acquisition/standardacquisition.py` & `nxtomomill-0.9.0a3/nxtomomill/converter/hdf5/acquisition/standardacquisition.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-0.9.0a2/nxtomomill/converter/hdf5/acquisition/utils.py` & `nxtomomill-0.9.0a3/nxtomomill/converter/hdf5/acquisition/utils.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-0.9.0a2/nxtomomill/converter/hdf5/acquisition/xrd3dacquisition.py` & `nxtomomill-0.9.0a3/nxtomomill/converter/hdf5/acquisition/xrd3dacquisition.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-0.9.0a2/nxtomomill/converter/hdf5/acquisition/xrdctacquisition.py` & `nxtomomill-0.9.0a3/nxtomomill/converter/hdf5/acquisition/xrdctacquisition.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-0.9.0a2/nxtomomill/converter/hdf5/acquisition/zseriesacquisition.py` & `nxtomomill-0.9.0a3/nxtomomill/converter/hdf5/acquisition/zseriesacquisition.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-0.9.0a2/nxtomomill/converter/hdf5/hdf5converter.py` & `nxtomomill-0.9.0a3/nxtomomill/converter/hdf5/hdf5converter.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-0.9.0a2/nxtomomill/converter/hdf5/setup.py` & `nxtomomill-0.9.0a3/nxtomomill/converter/hdf5/setup.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-0.9.0a2/nxtomomill/converter/hdf5/utils.py` & `nxtomomill-0.9.0a3/nxtomomill/converter/hdf5/utils.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-0.9.0a2/nxtomomill/converter/setup.py` & `nxtomomill-0.9.0a3/nxtomomill/converter/setup.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-0.9.0a2/nxtomomill/converter/version.py` & `nxtomomill-0.9.0a3/nxtomomill/converter/version.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-0.9.0a2/nxtomomill/io/acquisitionstep.py` & `nxtomomill-0.9.0a3/nxtomomill/io/acquisitionstep.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-0.9.0a2/nxtomomill/io/config/__init__.py` & `nxtomomill-0.9.0a3/nxtomomill/io/config/__init__.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-0.9.0a2/nxtomomill/io/config/configbase.py` & `nxtomomill-0.9.0a3/nxtomomill/io/config/configbase.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-0.9.0a2/nxtomomill/io/config/confighandler.py` & `nxtomomill-0.9.0a3/nxtomomill/io/config/confighandler.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-0.9.0a2/nxtomomill/io/config/edfconfig.py` & `nxtomomill-0.9.0a3/nxtomomill/io/config/edfconfig.py`

 * *Files 0% similar despite different names*

```diff
@@ -320,15 +320,15 @@
         self._energy_unit = EnergySI.KILOELECTRONVOLT
         self._x_trans_unit = MetricSystem.CENTIMETER
         self._y_trans_unit = MetricSystem.CENTIMETER
         self._z_trans_unit = MetricSystem.CENTIMETER
 
         # sample
         self._sample_name = None
-        self._force_angle_calculation = False
+        self._force_angle_calculation = True
         self._force_angle_calculation_endpoint = False
         self._force_angle_calculation_revert_neg_scan_range = True
 
         # source
         self._instrument_name = None
         self._source_name = "ESRF"
         self._source_type = SourceType.SYNCHROTRON_X_RAY_SOURCE
```

### Comparing `nxtomomill-0.9.0a2/nxtomomill/io/config/hdf5config.py` & `nxtomomill-0.9.0a3/nxtomomill/io/config/hdf5config.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-0.9.0a2/nxtomomill/io/confighandler.py` & `nxtomomill-0.9.0a3/nxtomomill/io/confighandler.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-0.9.0a2/nxtomomill/io/framegroup.py` & `nxtomomill-0.9.0a3/nxtomomill/io/framegroup.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-0.9.0a2/nxtomomill/io/setup.py` & `nxtomomill-0.9.0a3/nxtomomill/io/setup.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-0.9.0a2/nxtomomill/io/utils.py` & `nxtomomill-0.9.0a3/nxtomomill/io/utils.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-0.9.0a2/nxtomomill/nexus/nxdetector.py` & `nxtomomill-0.9.0a3/nxtomomill/nexus/nxdetector.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 from operator import is_not
 from silx.utils.proxy import docstring
 from silx.io.url import DataUrl
 from h5py import VirtualSource
 from typing import Iterable, Optional, Union
 import numpy
 import h5py
+from nxtomomill.utils.frameappender import FrameAppender
 from nxtomomill.utils.h5pyutils import from_virtual_source_to_data_url
 
 try:
     from tomoscan.esrf.scan.hdf5scan import ImageKey
 except ImportError:
     from tomoscan.esrf.hdf5scan import ImageKey
 from tomoscan.nexus.paths.nxtomo import get_paths as get_nexus_path
@@ -89,14 +90,16 @@
             default_unit=MetricSystem.METER
         )  # detector / sample distance
         self.field_of_view = field_of_view
         self._count_time = ElementWithUnit(default_unit=TimeSystem.SECOND)
         self.estimated_cor_from_motor = None
         self.tomo_n = None
         self.group_size = None
+        self.__master_vds_file = None
+        # used to record the virtual dataset set file origin in order to solve relative links
         self._set_freeze(True)
 
     @property
     def data(self) -> Optional[Union[numpy.ndarray, tuple]]:
         """data can be None, a numpy array or a list of DataUrl xor h5py Virtual Source"""
         return self._data
 
@@ -112,15 +115,15 @@
                     f"data is expected to be {self._expected_dim}d not {data.ndim}d"
                 )
         elif isinstance(data, (tuple, list)):
             for elmt in data:
                 if has_VDSmap:
                     if not isinstance(elmt, (DataUrl, VirtualSource, VDSmap)):
                         raise TypeError(
-                            f"element of 'data' are expected to be silx DataUrl or h5py virtualSource. Not {type(elmt)}"
+                            f"element of 'data' are expected to be a 3D numpy array, a list of silx DataUrl or a list of h5py virtualSource. Not {type(elmt)}"
                         )
             data = tuple(data)
         elif data is None:
             pass
         else:
             raise TypeError(
                 f"data is expected to be an instance of {numpy.ndarray}, None or a list of silx DataUrl or h5py Virtual Source. Not {type(data)}"
@@ -318,14 +321,15 @@
 
         nx_dict = {}
         if self.data is not None:
             # add data
             path_data = f"{self.path}/{nexus_detector_paths.DATA}"
             nx_dict[path_data] = self.data
             nx_dict["@".join([path_data, "interpretation"])] = "image"
+            nx_dict["__vds_master_file__"] = self.__master_vds_file
             # add attributes to data
             nx_dict[f"{self.path}@NX_class"] = "NXdetector"
             nx_dict[f"{self.path}@signal"] = nexus_detector_paths.DATA
             nx_dict[f"{self.path}@SILX_style/axis_scale_types"] = [
                 "linear",
                 "linear",
             ]
@@ -336,14 +340,17 @@
     ) -> None:
         possible_as_values = ("as_virtual_source", "as_data_url", "as_numpy_array")
         if load_data_as not in possible_as_values:
             raise ValueError(
                 f"load_data_as is expected to be in {possible_as_values} and not {load_data_as}"
             )
 
+        self.__master_vds_file = file_path
+        # record the input file if we need to solve virtual dataset path from it
+
         nexus_paths = get_nexus_path(nexus_version)
         nexus_detector_paths = nexus_paths.nx_detector_paths
 
         data_dataset_path = f"{data_path}/{nexus_detector_paths.DATA}"
         with HDF5File(file_path, mode="r") as h5f:
             if data_dataset_path in h5f:
                 dataset = h5f[data_dataset_path]
@@ -404,15 +411,21 @@
                             data_path=data_dataset_path,
                             scheme="silx",
                         )
                     ]
                 self.data = urls
             elif load_data_as == "as_virtual_source":
                 if dataset.is_virtual:
-                    self.data = dataset.virtual_sources()
+                    virtual_sources = []
+                    for vs_info in dataset.virtual_sources():
+                        _, vs = FrameAppender._recreate_vs(
+                            vs_info=vs_info, vds_file=file_path
+                        )
+                        virtual_sources.append(vs)
+                    self.data = virtual_sources
                 else:
                     raise ValueError(f"{data_dataset_path} is not virtual")
 
         self.x_pixel_size, self.x_pixel_size.unit = get_data_and_unit(
             file_path=file_path,
             data_path="/".join([data_path, nexus_detector_paths.X_PIXEL_SIZE]),
             default_unit=MetricSystem.METER,
```

### Comparing `nxtomomill-0.9.0a2/nxtomomill/nexus/nxinstrument.py` & `nxtomomill-0.9.0a3/nxtomomill/nexus/nxinstrument.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-0.9.0a2/nxtomomill/nexus/nxmonitor.py` & `nxtomomill-0.9.0a3/nxtomomill/nexus/nxmonitor.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-0.9.0a2/nxtomomill/nexus/nxobject.py` & `nxtomomill-0.9.0a3/nxtomomill/nexus/nxobject.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 __authors__ = ["H. Payno"]
 __license__ = "MIT"
 __date__ = "03/02/2022"
 
 
 from typing import Optional
 from silx.io.url import DataUrl
+from nxtomomill.utils.context import cwd_context
 from tomoscan.unitsystem import Unit
 from tomoscan.nexus.paths.nxtomo import LATEST_VERSION as LATEST_NXTOMO_VERSION
 from silx.io.dictdump import dicttonx
 import h5py
 import os
 
 
@@ -167,14 +168,18 @@
                 raise TypeError(
                     f"{key} is expected to be None or an instance of str not {type(value)}"
                 )
         if not isinstance(overwrite, bool):
             raise TypeError
 
         entry_path = "/".join([data_path, self.path])
+        if entry_path in ("/", ""):
+            raise ValueError(
+                "data_path AND nx_object cannot be both empty strings (you must provide a name to nx tomo"
+            )
         # not fully sure about the dicttoh5 "add" behavior
         if os.path.exists(file_path):
             with h5py.File(file_path, mode="a") as h5f:
                 if entry_path in h5f:
                     if overwrite:
                         del h5f[entry_path]
                     else:
@@ -187,14 +192,15 @@
         )
         # retrieve virtual sources and DataUrl
         datasets_to_handle_in_postprocessing = {}
         for key in self._get_virtual_sources(nx_dict):
             datasets_to_handle_in_postprocessing[key] = nx_dict.pop(key)
         for key in self._get_data_urls(nx_dict):
             datasets_to_handle_in_postprocessing[key] = nx_dict.pop(key)
+        master_vds_file = self._get_vds_master_file_folder(nx_dict)
 
         # retrieve attributes
         attributes = {}
 
         dataset_to_postpone = tuple(datasets_to_handle_in_postprocessing.keys())
         for key, value in nx_dict.items():
             if key.startswith(dataset_to_postpone):
@@ -206,43 +212,47 @@
         dicttonx(
             nx_dict,
             h5file=file_path,
             h5path=data_path,
             update_mode="replace",
             mode="a",
         )
+
         assert os.path.exists(file_path)
-        # now handle nx_dict containing h5py.virtualSource or DataUrl
-        # this cannot be handled from the nxdetector class because not aware about
-        # the output file.
-        for (
-            dataset_path,
-            v_sources_or_data_urls,
-        ) in datasets_to_handle_in_postprocessing.items():
-            for v_source_or_data_url in v_sources_or_data_urls:
-                if isinstance(v_source_or_data_url, DataUrl):
-                    data = DataUrl(
-                        file_path=v_source_or_data_url.file_path(),
-                        data_path=v_source_or_data_url.data_path(),
-                        scheme=v_source_or_data_url.scheme(),
-                        data_slice=v_source_or_data_url.data_slice(),
+
+        # in order to solve relative path we need to be on the (source) master file working directory
+        with cwd_context(master_vds_file):
+            # now handle nx_dict containing h5py.virtualSource or DataUrl
+            # this cannot be handled from the nxdetector class because not aware about
+            # the output file.
+            for (
+                dataset_path,
+                v_sources_or_data_urls,
+            ) in datasets_to_handle_in_postprocessing.items():
+                for v_source_or_data_url in v_sources_or_data_urls:
+                    if isinstance(v_source_or_data_url, DataUrl):
+                        data = DataUrl(
+                            file_path=v_source_or_data_url.file_path(),
+                            data_path=v_source_or_data_url.data_path(),
+                            scheme=v_source_or_data_url.scheme(),
+                            data_slice=v_source_or_data_url.data_slice(),
+                        )
+                    else:
+                        data = v_source_or_data_url
+                    from nxtomomill.utils.frameappender import (
+                        FrameAppender,
+                    )  # avoid cyclic import
+
+                    frame_appender = FrameAppender(
+                        data=data,
+                        file_path=file_path,
+                        data_path="/".join([data_path, dataset_path]),
+                        where="end",
                     )
-                else:
-                    data = v_source_or_data_url
-                from nxtomomill.utils.frameappender import (
-                    FrameAppender,
-                )  # avoid cyclic import
-
-                frame_appender = FrameAppender(
-                    data=data,
-                    file_path=file_path,
-                    data_path="/".join([data_path, dataset_path]),
-                    where="end",
-                )
-                frame_appender.process()
+                    frame_appender.process()
 
         # write attributes of dataset defined from a list of DataUrl or VirtualSource
         assert os.path.exists(file_path)
         dicttonx(
             attributes,
             h5file=file_path,
             h5path=data_path,
@@ -282,14 +292,22 @@
         keys = []
         for key, value in ddict.items():
             if has_virtual_sources(value):
                 keys.append(key)
         return tuple(keys)
 
     @staticmethod
+    def _get_vds_master_file_folder(nx_dict: dict):
+        path = nx_dict.pop("__vds_master_file__", None)
+        if path is not None:
+            return os.path.dirname(path)
+        else:
+            return None
+
+    @staticmethod
     def _get_data_urls(ddict) -> tuple:
         """Return key / path containing a list or a tuple of silx.io.url.DataUrl"""
 
         def has_data_url(value):
             if isinstance(value, DataUrl):
                 return True
             elif isinstance(value, (list, tuple)):
```

### Comparing `nxtomomill-0.9.0a2/nxtomomill/nexus/nxsample.py` & `nxtomomill-0.9.0a3/nxtomomill/nexus/nxsample.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-0.9.0a2/nxtomomill/nexus/nxsource.py` & `nxtomomill-0.9.0a3/nxtomomill/nexus/nxsource.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-0.9.0a2/nxtomomill/nexus/nxtomo.py` & `nxtomomill-0.9.0a3/nxtomomill/nexus/nxtomo.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-0.9.0a2/nxtomomill/nexus/utils.py` & `nxtomomill-0.9.0a3/nxtomomill/nexus/utils.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-0.9.0a2/nxtomomill/plugins.py` & `nxtomomill-0.9.0a3/nxtomomill/plugins.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-0.9.0a2/nxtomomill/settings.py` & `nxtomomill-0.9.0a3/nxtomomill/settings.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-0.9.0a2/nxtomomill/setup.py` & `nxtomomill-0.9.0a3/nxtomomill/setup.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-0.9.0a2/nxtomomill/utils/__init__.py` & `nxtomomill-0.9.0a3/nxtomomill/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-0.9.0a2/nxtomomill/utils/context.py` & `nxtomomill-0.9.0a3/nxtomomill/utils/context.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-0.9.0a2/nxtomomill/utils/file_path.py` & `nxtomomill-0.9.0a3/nxtomomill/utils/file_path.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-0.9.0a2/nxtomomill/utils/frameappender.py` & `nxtomomill-0.9.0a3/nxtomomill/utils/frameappender.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-0.9.0a2/nxtomomill/utils/h5pyutils.py` & `nxtomomill-0.9.0a3/nxtomomill/utils/h5pyutils.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-0.9.0a2/nxtomomill/utils/hdf5.py` & `nxtomomill-0.9.0a3/nxtomomill/utils/hdf5.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-0.9.0a2/nxtomomill/utils/nxsplitter.py` & `nxtomomill-0.9.0a3/nxtomomill/utils/nxsplitter.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-0.9.0a2/nxtomomill/utils/progress.py` & `nxtomomill-0.9.0a3/nxtomomill/utils/progress.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-0.9.0a2/nxtomomill/utils/utils.py` & `nxtomomill-0.9.0a3/nxtomomill/utils/utils.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-0.9.0a2/nxtomomill/version.py` & `nxtomomill-0.9.0a3/nxtomomill/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     "final": 15,
 }
 
 MAJOR = 0
 MINOR = 9
 MICRO = 0
 RELEV = "alpha"  # <16
-SERIAL = 2  # <16
+SERIAL = 3  # <16
 
 date = __date__
 
 _version_info = namedtuple(
     "version_info", ["major", "minor", "micro", "releaselevel", "serial"]
 )
```

### Comparing `nxtomomill-0.9.0a2/nxtomomill.egg-info/PKG-INFO` & `nxtomomill-0.9.0a3/nxtomomill.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nxtomomill
-Version: 0.9.0a2
+Version: 0.9.0a3
 Summary: "applications and library to convert raw format to NXTomo format"
 Home-page: https://gitlab.esrf.fr/tomotools/nxtomomill
 Author: data analysis unit
 Author-email: henri.payno@esrf.fr
 License: MIT
 Project-URL: Bug Tracker, https://gitlab.esrf.fr/tomotools/nxtomomill/-/issues
 Platform: UNKNOWN
```

### Comparing `nxtomomill-0.9.0a2/nxtomomill.egg-info/SOURCES.txt` & `nxtomomill-0.9.0a3/nxtomomill.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 nxtomomill/nexus/nxdetector.py
 nxtomomill/nexus/nxinstrument.py
 nxtomomill/nexus/nxmonitor.py
 nxtomomill/nexus/nxobject.py
 nxtomomill/nexus/nxsample.py
 nxtomomill/nexus/nxsource.py
 nxtomomill/nexus/nxtomo.py
+nxtomomill/nexus/nxtransformations.py
 nxtomomill/nexus/utils.py
 nxtomomill/utils/__init__.py
 nxtomomill/utils/context.py
 nxtomomill/utils/file_path.py
 nxtomomill/utils/frameappender.py
 nxtomomill/utils/h5pyutils.py
 nxtomomill/utils/hdf5.py
```

### Comparing `nxtomomill-0.9.0a2/setup.cfg` & `nxtomomill-0.9.0a3/setup.cfg`

 * *Files identical despite different names*

### Comparing `nxtomomill-0.9.0a2/setup.py` & `nxtomomill-0.9.0a3/setup.py`

 * *Files identical despite different names*

