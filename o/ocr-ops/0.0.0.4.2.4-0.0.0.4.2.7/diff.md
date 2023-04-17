# Comparing `tmp/ocr-ops-0.0.0.4.2.4.tar.gz` & `tmp/ocr-ops-0.0.0.4.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocr-ops-0.0.0.4.2.4.tar", last modified: Sun Apr  2 20:10:18 2023, max compression
+gzip compressed data, was "ocr-ops-0.0.0.4.2.7.tar", last modified: Mon Apr 17 04:44:16 2023, max compression
```

## Comparing `ocr-ops-0.0.0.4.2.4.tar` & `ocr-ops-0.0.0.4.2.7.tar`

### file list

```diff
@@ -1,53 +1,54 @@
-drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-02 20:10:18.784522 ocr-ops-0.0.0.4.2.4/
--rw-r--r--   0 tandonp    (501) staff       (20)     1071 2022-03-27 19:39:41.000000 ocr-ops-0.0.0.4.2.4/LICENSE
--rw-r--r--   0 tandonp    (501) staff       (20)       24 2022-03-21 02:23:19.000000 ocr-ops-0.0.0.4.2.4/MANIFEST.in
--rw-r--r--   0 tandonp    (501) staff       (20)     1254 2023-04-02 20:10:18.784371 ocr-ops-0.0.0.4.2.4/PKG-INFO
--rw-r--r--   0 tandonp    (501) staff       (20)      835 2023-03-19 20:02:57.000000 ocr-ops-0.0.0.4.2.4/README.md
-drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-02 20:10:18.778506 ocr-ops-0.0.0.4.2.4/ocr_ops/
--rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-03-27 22:16:22.000000 ocr-ops-0.0.0.4.2.4/ocr_ops/__init__.py
-drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-02 20:10:18.779470 ocr-ops-0.0.0.4.2.4/ocr_ops/dependency/
--rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-03-27 17:57:54.000000 ocr-ops-0.0.0.4.2.4/ocr_ops/dependency/__init__.py
--rw-r--r--   0 tandonp    (501) staff       (20)     1322 2022-06-03 07:01:48.000000 ocr-ops-0.0.0.4.2.4/ocr_ops/dependency/ffmpeg.py
-drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-02 20:10:18.779996 ocr-ops-0.0.0.4.2.4/ocr_ops/experimental/
--rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-03-27 20:44:00.000000 ocr-ops-0.0.0.4.2.4/ocr_ops/experimental/__init__.py
--rw-r--r--   0 tandonp    (501) staff       (20)     4773 2022-05-30 22:56:14.000000 ocr-ops-0.0.0.4.2.4/ocr_ops/experimental/ocr_fusion.py
-drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-02 20:10:18.780139 ocr-ops-0.0.0.4.2.4/ocr_ops/framework/
--rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-03-09 07:46:32.000000 ocr-ops-0.0.0.4.2.4/ocr_ops/framework/__init__.py
-drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-02 20:10:18.781074 ocr-ops-0.0.0.4.2.4/ocr_ops/framework/op/
--rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-03-27 18:12:24.000000 ocr-ops-0.0.0.4.2.4/ocr_ops/framework/op/__init__.py
--rw-r--r--   0 tandonp    (501) staff       (20)     8566 2023-04-01 22:33:11.000000 ocr-ops-0.0.0.4.2.4/ocr_ops/framework/op/abstract_ocr_op.py
--rw-r--r--   0 tandonp    (501) staff       (20)     2385 2022-06-09 02:59:29.000000 ocr-ops-0.0.0.4.2.4/ocr_ops/framework/op/ffmpeg_op.py
--rw-r--r--   0 tandonp    (501) staff       (20)     5559 2023-03-19 20:04:12.000000 ocr-ops-0.0.0.4.2.4/ocr_ops/framework/op/ocr_op.py
-drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-02 20:10:18.781494 ocr-ops-0.0.0.4.2.4/ocr_ops/framework/op/result/
--rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-05-30 17:21:51.000000 ocr-ops-0.0.0.4.2.4/ocr_ops/framework/op/result/__init__.py
--rw-r--r--   0 tandonp    (501) staff       (20)      764 2022-06-09 03:07:59.000000 ocr-ops-0.0.0.4.2.4/ocr_ops/framework/op/result/ffmeg_result.py
--rw-r--r--   0 tandonp    (501) staff       (20)     6737 2023-04-02 00:02:40.000000 ocr-ops-0.0.0.4.2.4/ocr_ops/framework/op/result/ocr_result.py
-drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-02 20:10:18.781870 ocr-ops-0.0.0.4.2.4/ocr_ops/framework/pipeline/
--rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-03-27 18:13:01.000000 ocr-ops-0.0.0.4.2.4/ocr_ops/framework/pipeline/__init__.py
--rw-r--r--   0 tandonp    (501) staff       (20)     8054 2023-04-01 22:33:11.000000 ocr-ops-0.0.0.4.2.4/ocr_ops/framework/pipeline/ocr_pipeline.py
-drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-02 20:10:18.782637 ocr-ops-0.0.0.4.2.4/ocr_ops/instances/
--rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-03-09 07:46:32.000000 ocr-ops-0.0.0.4.2.4/ocr_ops/instances/__init__.py
--rw-r--r--   0 tandonp    (501) staff       (20)     1656 2023-03-19 20:05:54.000000 ocr-ops-0.0.0.4.2.4/ocr_ops/instances/cv.py
--rw-r--r--   0 tandonp    (501) staff       (20)     3155 2022-06-08 03:45:51.000000 ocr-ops-0.0.0.4.2.4/ocr_ops/instances/ocr.py
--rw-r--r--   0 tandonp    (501) staff       (20)     5505 2023-03-19 20:05:54.000000 ocr-ops-0.0.0.4.2.4/ocr_ops/instances/text.py
-drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-02 20:10:18.783034 ocr-ops-0.0.0.4.2.4/ocr_ops/run_finding/
--rw-r--r--   0 tandonp    (501) staff       (20)        0 2023-04-01 22:33:11.000000 ocr-ops-0.0.0.4.2.4/ocr_ops/run_finding/__init__.py
--rw-r--r--   0 tandonp    (501) staff       (20)     2432 2023-04-02 20:05:16.000000 ocr-ops-0.0.0.4.2.4/ocr_ops/run_finding/interval.py
--rw-r--r--   0 tandonp    (501) staff       (20)     2928 2023-04-01 22:33:11.000000 ocr-ops-0.0.0.4.2.4/ocr_ops/run_finding/run_finding.py
-drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-02 20:10:18.784184 ocr-ops-0.0.0.4.2.4/ocr_ops/test/
--rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-03-27 17:58:47.000000 ocr-ops-0.0.0.4.2.4/ocr_ops/test/__init__.py
--rw-r--r--   0 tandonp    (501) staff       (20)     3354 2022-06-09 03:02:43.000000 ocr-ops-0.0.0.4.2.4/ocr_ops/test/test_ffmpeg_op.py
--rw-r--r--   0 tandonp    (501) staff       (20)     1897 2022-06-03 07:03:09.000000 ocr-ops-0.0.0.4.2.4/ocr_ops/test/test_installs.py
--rw-r--r--   0 tandonp    (501) staff       (20)     9090 2023-04-02 00:02:40.000000 ocr-ops-0.0.0.4.2.4/ocr_ops/test/test_ocr_ops.py
--rw-r--r--   0 tandonp    (501) staff       (20)    16051 2023-04-02 00:02:40.000000 ocr-ops-0.0.0.4.2.4/ocr_ops/test/test_ocr_pipeline.py
--rw-r--r--   0 tandonp    (501) staff       (20)     7080 2023-04-02 20:01:34.000000 ocr-ops-0.0.0.4.2.4/ocr_ops/test/test_run_finding.py
-drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-02 20:10:18.779211 ocr-ops-0.0.0.4.2.4/ocr_ops.egg-info/
--rw-r--r--   0 tandonp    (501) staff       (20)     1254 2023-04-02 20:10:18.000000 ocr-ops-0.0.0.4.2.4/ocr_ops.egg-info/PKG-INFO
--rw-r--r--   0 tandonp    (501) staff       (20)     1134 2023-04-02 20:10:18.000000 ocr-ops-0.0.0.4.2.4/ocr_ops.egg-info/SOURCES.txt
--rw-r--r--   0 tandonp    (501) staff       (20)        1 2023-04-02 20:10:18.000000 ocr-ops-0.0.0.4.2.4/ocr_ops.egg-info/dependency_links.txt
--rw-r--r--   0 tandonp    (501) staff       (20)      127 2023-04-02 20:10:18.000000 ocr-ops-0.0.0.4.2.4/ocr_ops.egg-info/requires.txt
--rw-r--r--   0 tandonp    (501) staff       (20)        8 2023-04-02 20:10:18.000000 ocr-ops-0.0.0.4.2.4/ocr_ops.egg-info/top_level.txt
--rw-r--r--   0 tandonp    (501) staff       (20)      258 2023-03-18 07:55:39.000000 ocr-ops-0.0.0.4.2.4/pyproject.toml
--rw-r--r--   0 tandonp    (501) staff       (20)      126 2023-03-18 09:31:17.000000 ocr-ops-0.0.0.4.2.4/requirements.txt
--rw-r--r--   0 tandonp    (501) staff       (20)       38 2023-04-02 20:10:18.784571 ocr-ops-0.0.0.4.2.4/setup.cfg
--rw-r--r--   0 tandonp    (501) staff       (20)      756 2023-04-02 20:10:07.000000 ocr-ops-0.0.0.4.2.4/setup.py
+drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-17 04:44:16.349922 ocr-ops-0.0.0.4.2.7/
+-rw-r--r--   0 tandonp    (501) staff       (20)     1071 2022-03-27 19:39:41.000000 ocr-ops-0.0.0.4.2.7/LICENSE
+-rw-r--r--   0 tandonp    (501) staff       (20)       24 2022-03-21 02:23:19.000000 ocr-ops-0.0.0.4.2.7/MANIFEST.in
+-rw-r--r--   0 tandonp    (501) staff       (20)     1254 2023-04-17 04:44:16.349757 ocr-ops-0.0.0.4.2.7/PKG-INFO
+-rw-r--r--   0 tandonp    (501) staff       (20)      835 2023-03-19 20:02:57.000000 ocr-ops-0.0.0.4.2.7/README.md
+drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-17 04:44:16.343535 ocr-ops-0.0.0.4.2.7/ocr_ops/
+-rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-03-27 22:16:22.000000 ocr-ops-0.0.0.4.2.7/ocr_ops/__init__.py
+drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-17 04:44:16.344554 ocr-ops-0.0.0.4.2.7/ocr_ops/dependency/
+-rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-03-27 17:57:54.000000 ocr-ops-0.0.0.4.2.7/ocr_ops/dependency/__init__.py
+-rw-r--r--   0 tandonp    (501) staff       (20)     1322 2022-06-03 07:01:48.000000 ocr-ops-0.0.0.4.2.7/ocr_ops/dependency/ffmpeg.py
+drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-17 04:44:16.345118 ocr-ops-0.0.0.4.2.7/ocr_ops/experimental/
+-rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-03-27 20:44:00.000000 ocr-ops-0.0.0.4.2.7/ocr_ops/experimental/__init__.py
+-rw-r--r--   0 tandonp    (501) staff       (20)     4773 2022-05-30 22:56:14.000000 ocr-ops-0.0.0.4.2.7/ocr_ops/experimental/ocr_fusion.py
+drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-17 04:44:16.345412 ocr-ops-0.0.0.4.2.7/ocr_ops/framework/
+-rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-03-09 07:46:32.000000 ocr-ops-0.0.0.4.2.7/ocr_ops/framework/__init__.py
+drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-17 04:44:16.346212 ocr-ops-0.0.0.4.2.7/ocr_ops/framework/op/
+-rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-03-27 18:12:24.000000 ocr-ops-0.0.0.4.2.7/ocr_ops/framework/op/__init__.py
+-rw-r--r--   0 tandonp    (501) staff       (20)     8670 2023-04-16 20:58:32.000000 ocr-ops-0.0.0.4.2.7/ocr_ops/framework/op/abstract_ocr_op.py
+-rw-r--r--   0 tandonp    (501) staff       (20)      722 2023-04-17 04:26:49.000000 ocr-ops-0.0.0.4.2.7/ocr_ops/framework/op/drop_op.py
+-rw-r--r--   0 tandonp    (501) staff       (20)     2385 2022-06-09 02:59:29.000000 ocr-ops-0.0.0.4.2.7/ocr_ops/framework/op/ffmpeg_op.py
+-rw-r--r--   0 tandonp    (501) staff       (20)     5559 2023-04-16 02:58:51.000000 ocr-ops-0.0.0.4.2.7/ocr_ops/framework/op/ocr_op.py
+drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-17 04:44:16.346835 ocr-ops-0.0.0.4.2.7/ocr_ops/framework/op/result/
+-rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-05-30 17:21:51.000000 ocr-ops-0.0.0.4.2.7/ocr_ops/framework/op/result/__init__.py
+-rw-r--r--   0 tandonp    (501) staff       (20)      764 2022-06-09 03:07:59.000000 ocr-ops-0.0.0.4.2.7/ocr_ops/framework/op/result/ffmeg_result.py
+-rw-r--r--   0 tandonp    (501) staff       (20)     6878 2023-04-16 20:58:32.000000 ocr-ops-0.0.0.4.2.7/ocr_ops/framework/op/result/ocr_result.py
+drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-17 04:44:16.347095 ocr-ops-0.0.0.4.2.7/ocr_ops/framework/pipeline/
+-rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-03-27 18:13:01.000000 ocr-ops-0.0.0.4.2.7/ocr_ops/framework/pipeline/__init__.py
+-rw-r--r--   0 tandonp    (501) staff       (20)     8225 2023-04-16 22:12:55.000000 ocr-ops-0.0.0.4.2.7/ocr_ops/framework/pipeline/ocr_pipeline.py
+drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-17 04:44:16.347614 ocr-ops-0.0.0.4.2.7/ocr_ops/instances/
+-rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-03-09 07:46:32.000000 ocr-ops-0.0.0.4.2.7/ocr_ops/instances/__init__.py
+-rw-r--r--   0 tandonp    (501) staff       (20)     1642 2023-04-16 22:12:55.000000 ocr-ops-0.0.0.4.2.7/ocr_ops/instances/cv.py
+-rw-r--r--   0 tandonp    (501) staff       (20)     4011 2023-04-16 22:12:55.000000 ocr-ops-0.0.0.4.2.7/ocr_ops/instances/ocr.py
+-rw-r--r--   0 tandonp    (501) staff       (20)     5505 2023-03-19 20:05:54.000000 ocr-ops-0.0.0.4.2.7/ocr_ops/instances/text.py
+drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-17 04:44:16.348145 ocr-ops-0.0.0.4.2.7/ocr_ops/run_finding/
+-rw-r--r--   0 tandonp    (501) staff       (20)        0 2023-04-01 22:33:11.000000 ocr-ops-0.0.0.4.2.7/ocr_ops/run_finding/__init__.py
+-rw-r--r--   0 tandonp    (501) staff       (20)     2432 2023-04-02 20:05:16.000000 ocr-ops-0.0.0.4.2.7/ocr_ops/run_finding/interval.py
+-rw-r--r--   0 tandonp    (501) staff       (20)     2928 2023-04-01 22:33:11.000000 ocr-ops-0.0.0.4.2.7/ocr_ops/run_finding/run_finding.py
+drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-17 04:44:16.349568 ocr-ops-0.0.0.4.2.7/ocr_ops/test/
+-rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-03-27 17:58:47.000000 ocr-ops-0.0.0.4.2.7/ocr_ops/test/__init__.py
+-rw-r--r--   0 tandonp    (501) staff       (20)     3354 2022-06-09 03:02:43.000000 ocr-ops-0.0.0.4.2.7/ocr_ops/test/test_ffmpeg_op.py
+-rw-r--r--   0 tandonp    (501) staff       (20)     1897 2022-06-03 07:03:09.000000 ocr-ops-0.0.0.4.2.7/ocr_ops/test/test_installs.py
+-rw-r--r--   0 tandonp    (501) staff       (20)     9090 2023-04-02 00:02:40.000000 ocr-ops-0.0.0.4.2.7/ocr_ops/test/test_ocr_ops.py
+-rw-r--r--   0 tandonp    (501) staff       (20)    17334 2023-04-17 04:42:58.000000 ocr-ops-0.0.0.4.2.7/ocr_ops/test/test_ocr_pipeline.py
+-rw-r--r--   0 tandonp    (501) staff       (20)     7043 2023-04-16 22:12:55.000000 ocr-ops-0.0.0.4.2.7/ocr_ops/test/test_run_finding.py
+drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-17 04:44:16.344285 ocr-ops-0.0.0.4.2.7/ocr_ops.egg-info/
+-rw-r--r--   0 tandonp    (501) staff       (20)     1254 2023-04-17 04:44:16.000000 ocr-ops-0.0.0.4.2.7/ocr_ops.egg-info/PKG-INFO
+-rw-r--r--   0 tandonp    (501) staff       (20)     1166 2023-04-17 04:44:16.000000 ocr-ops-0.0.0.4.2.7/ocr_ops.egg-info/SOURCES.txt
+-rw-r--r--   0 tandonp    (501) staff       (20)        1 2023-04-17 04:44:16.000000 ocr-ops-0.0.0.4.2.7/ocr_ops.egg-info/dependency_links.txt
+-rw-r--r--   0 tandonp    (501) staff       (20)      127 2023-04-17 04:44:16.000000 ocr-ops-0.0.0.4.2.7/ocr_ops.egg-info/requires.txt
+-rw-r--r--   0 tandonp    (501) staff       (20)        8 2023-04-17 04:44:16.000000 ocr-ops-0.0.0.4.2.7/ocr_ops.egg-info/top_level.txt
+-rw-r--r--   0 tandonp    (501) staff       (20)      258 2023-03-18 07:55:39.000000 ocr-ops-0.0.0.4.2.7/pyproject.toml
+-rw-r--r--   0 tandonp    (501) staff       (20)      126 2023-03-18 09:31:17.000000 ocr-ops-0.0.0.4.2.7/requirements.txt
+-rw-r--r--   0 tandonp    (501) staff       (20)       38 2023-04-17 04:44:16.349973 ocr-ops-0.0.0.4.2.7/setup.cfg
+-rw-r--r--   0 tandonp    (501) staff       (20)      756 2023-04-17 04:44:00.000000 ocr-ops-0.0.0.4.2.7/setup.py
```

### Comparing `ocr-ops-0.0.0.4.2.4/LICENSE` & `ocr-ops-0.0.0.4.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ocr-ops-0.0.0.4.2.4/PKG-INFO` & `ocr-ops-0.0.0.4.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocr-ops
-Version: 0.0.0.4.2.4
+Version: 0.0.0.4.2.7
 Summary: OCR-Ops
 Home-page: https://github.com/prateekt/ocr-ops
 Author: Prateek Tandon
 Author-email: prateek1.tandon@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ocr-ops-0.0.0.4.2.4/README.md` & `ocr-ops-0.0.0.4.2.7/README.md`

 * *Files identical despite different names*

### Comparing `ocr-ops-0.0.0.4.2.4/ocr_ops/dependency/ffmpeg.py` & `ocr-ops-0.0.0.4.2.7/ocr_ops/dependency/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `ocr-ops-0.0.0.4.2.4/ocr_ops/experimental/ocr_fusion.py` & `ocr-ops-0.0.0.4.2.7/ocr_ops/experimental/ocr_fusion.py`

 * *Files identical despite different names*

### Comparing `ocr-ops-0.0.0.4.2.4/ocr_ops/framework/op/abstract_ocr_op.py` & `ocr-ops-0.0.0.4.2.7/ocr_ops/framework/op/abstract_ocr_op.py`

 * *Files 4% similar despite different names*

```diff
@@ -164,14 +164,16 @@
         """
         Save output to file.
 
         param out_path: Path to where file should go
         param basename: File basename
         """
         if self.output is not None:
+            if self.output.output_img is None:
+                raise ValueError("Input image is None.")
             if out_path.endswith(".png"):
                 outfile = out_path
             else:
                 os.makedirs(out_path, exist_ok=True)
                 if basename is not None:
                     outfile = os.path.join(out_path, basename + ".png")
                 else:
```

### Comparing `ocr-ops-0.0.0.4.2.4/ocr_ops/framework/op/ffmpeg_op.py` & `ocr-ops-0.0.0.4.2.7/ocr_ops/framework/op/ffmpeg_op.py`

 * *Files identical despite different names*

### Comparing `ocr-ops-0.0.0.4.2.4/ocr_ops/framework/op/ocr_op.py` & `ocr-ops-0.0.0.4.2.7/ocr_ops/framework/op/ocr_op.py`

 * *Files identical despite different names*

### Comparing `ocr-ops-0.0.0.4.2.4/ocr_ops/framework/op/result/ffmeg_result.py` & `ocr-ops-0.0.0.4.2.7/ocr_ops/framework/op/result/ffmeg_result.py`

 * *Files identical despite different names*

### Comparing `ocr-ops-0.0.0.4.2.4/ocr_ops/framework/op/result/ocr_result.py` & `ocr-ops-0.0.0.4.2.7/ocr_ops/framework/op/result/ocr_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,17 +84,17 @@
     ):
         """
         param text_boxes: Detected text boxes in image
         param input_img: Pointer to raw input image
         param use_bounding_box: Whether bounding box annotations are used
         """
         self.text_boxes: List[TextBox] = text_boxes
-        self.input_img: ImageResult = input_img
+        self.input_img: Optional[ImageResult] = input_img
         self.use_bounding_box = use_bounding_box
-        self.output_img: np.array = self._prepare_output_image()
+        self.output_img: Optional[np.array] = self._prepare_output_image()
         self.words: List[str] = list()
         self.update_words()
 
     def __str__(self):
         return str([str(text_box) for text_box in self.text_boxes])
 
     def _prepare_output_image(self) -> np.array:
@@ -189,15 +189,18 @@
         # prepare dataframe of bounding box results
         input_paths = list()
         texts = list()
         bounding_boxes = list()
         confidences = list()
         for ocr_result in self.ocr_image_results:
             for bounding_box in ocr_result.text_boxes:
-                input_paths.append(ocr_result.input_img.file_path)
+                if ocr_result.input_img is None:
+                    input_paths.append("N/A")
+                else:
+                    input_paths.append(ocr_result.input_img.file_path)
                 texts.append(bounding_box.text)
                 bounding_boxes.append(bounding_box.bounding_box)
                 confidences.append(bounding_box.conf)
         df = pd.DataFrame(
             {
                 "input_path": input_paths,
                 "text": texts,
```

### Comparing `ocr-ops-0.0.0.4.2.4/ocr_ops/framework/pipeline/ocr_pipeline.py` & `ocr-ops-0.0.0.4.2.7/ocr_ops/framework/pipeline/ocr_pipeline.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from algo_ops.dependency.sys_util import get_image_files, is_image_file
 from algo_ops.ops.op import Op
 from algo_ops.paraloop import paraloop
 from algo_ops.pipeline.cv_pipeline import CVPipeline
 from algo_ops.pipeline.pipeline import Pipeline
 
 from ocr_ops.framework.op.abstract_ocr_op import AbstractOCROp, EasyOCROp
+from ocr_ops.framework.op.drop_op import DropOp
 from ocr_ops.framework.op.ocr_op import (
     PyTesseractTextOCROp,
     PyTesseractTextBoxOCROp,
     EasyOCRTextBoxOp,
     EasyOCRTextOp,
 )
 from ocr_ops.framework.op.result.ffmeg_result import FFMPEGResult
@@ -84,14 +85,15 @@
     def __init__(
         self,
         img_pipeline: Optional[CVPipeline],
         ocr_method: OCRMethod,
         output_type: OutputType,
         text_pipeline: Optional[Pipeline],
         autosave_output_img_path: Optional[str] = None,
+        store_intermediate_images: bool = True,
     ):
         """
         param img_pipeline: An optional CVOps pre-processing pipeline to run on image before OCR
         param ocr_method: The ocr method to use
         param output_type: The type (verbosity) of information output from OCR
         param text_pipeline: An optional TextOps pipeline to post-process OCR text
         param autosave_output_img_path: If specified, the place where OCR output images will be auto-saved.
@@ -113,14 +115,16 @@
         if self.img_pipeline is not None:
             ops.append(self.img_pipeline)
         # actual OCR on image
         ops.append(self.ocr_op)
         # text cleaning post-processing
         if self.text_pipeline is not None:
             ops.append(self.text_pipeline)
+        if not store_intermediate_images:
+            ops.append(DropOp())
         super().__init__(ops=ops)
 
     def set_img_pipeline_params(self, func_name: str, params: Dict[str, Any]) -> None:
         """
         Fixes parameters of CVOPs processing pipeline.
 
         param func_name: The function name in CVOPs pipeline
```

### Comparing `ocr-ops-0.0.0.4.2.4/ocr_ops/instances/cv.py` & `ocr-ops-0.0.0.4.2.7/ocr_ops/instances/cv.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,17 +31,15 @@
 
 
 def basic_cv_pipeline() -> CVPipeline:
     """
     Just gray scale image.
     """
 
-    img_pipeline = CVPipeline.init_from_funcs(
-        funcs=[_gray_scale],
-    )
+    img_pipeline = CVPipeline.init_from_funcs(funcs=[_gray_scale],)
     return img_pipeline
 
 
 def black_text_cv_pipeline() -> CVPipeline:
     """
     Initializes computer vision pipeline to isolate black text in an image.
     """
```

### Comparing `ocr-ops-0.0.0.4.2.4/ocr_ops/instances/text.py` & `ocr-ops-0.0.0.4.2.7/ocr_ops/instances/text.py`

 * *Files identical despite different names*

### Comparing `ocr-ops-0.0.0.4.2.4/ocr_ops/run_finding/interval.py` & `ocr-ops-0.0.0.4.2.7/ocr_ops/run_finding/interval.py`

 * *Files identical despite different names*

### Comparing `ocr-ops-0.0.0.4.2.4/ocr_ops/run_finding/run_finding.py` & `ocr-ops-0.0.0.4.2.7/ocr_ops/run_finding/run_finding.py`

 * *Files identical despite different names*

### Comparing `ocr-ops-0.0.0.4.2.4/ocr_ops/test/test_ffmpeg_op.py` & `ocr-ops-0.0.0.4.2.7/ocr_ops/test/test_ffmpeg_op.py`

 * *Files identical despite different names*

### Comparing `ocr-ops-0.0.0.4.2.4/ocr_ops/test/test_installs.py` & `ocr-ops-0.0.0.4.2.7/ocr_ops/test/test_installs.py`

 * *Files identical despite different names*

### Comparing `ocr-ops-0.0.0.4.2.4/ocr_ops/test/test_ocr_ops.py` & `ocr-ops-0.0.0.4.2.7/ocr_ops/test/test_ocr_ops.py`

 * *Files identical despite different names*

### Comparing `ocr-ops-0.0.0.4.2.4/ocr_ops/test/test_ocr_pipeline.py` & `ocr-ops-0.0.0.4.2.7/ocr_ops/test/test_ocr_pipeline.py`

 * *Files 10% similar despite different names*

```diff
@@ -48,23 +48,27 @@
                 "test_autosave2",
                 "test_autosave3",
                 "test_autosave4",
             ),
             files=("test.pkl",),
         )
 
-    def _assert_pass_vis_tests(self, ocr_pipeline: OCRPipeline) -> None:
+    def _assert_pass_vis_tests(
+        self, ocr_pipeline: OCRPipeline, file_list=None,
+    ) -> None:
         # test vis input / output
+        if file_list is None:
+            file_list = ["['run_ocr']", "['run_ocr']_violin", "run_ocr"]
         with self.assertRaises(ValueError):
             ocr_pipeline.vis_input()
         ocr_pipeline.vis()
 
         # test vis profile
         ocr_pipeline.vis_profile()
-        for file in ["['run_ocr']", "['run_ocr']_violin", "run_ocr"]:
+        for file in file_list:
             self.assertTrue(
                 os.path.exists(os.path.join("algo_ops_profile", file + ".png"))
             )
 
     def _assert_pass_save_tests(
         self, ocr_pipeline: OCRPipeline, expected_num_txt: int, expected_num_png: int
     ) -> None:
@@ -117,14 +121,15 @@
                 method()
 
         # test execution on sample image
         output = ocr_pipeline.exec(self.joy_of_data_img)
         self.assertTrue(isinstance(output, OCRPipelineResult))
         output = output[0]
         self.assertTrue(isinstance(output, OCRImageResult))
+        self.assertTrue(isinstance(output.input_img, ImageResult))
         self.assertFalse(output.use_bounding_box)
         self.assertTrue(np.array_equal(output.input_img.img, output.output_img))
         self.assertEqual(len(output), 1)
         self.assertTrue(isinstance(output[0], TextBox))
         self.assertEqual(output[0].text.strip(), "joy of data")
         self.assertEqual(output[0].bounding_box, None)
         self.assertEqual(output[0].conf, None)
@@ -226,15 +231,14 @@
         # test execution on sample image
         output = ocr_pipeline.exec(self.joy_of_data_img)
         self.assertTrue(isinstance(output, OCRPipelineResult))
         self.assertEqual(len(output), 1)
         self.assertTrue(isinstance(output[0], OCRImageResult))
         output = output[0]
         self.assertFalse(output.use_bounding_box)
-        self.assertTrue(np.array_equal(output.input_img.img, output.output_img))
         self.assertEqual(len(output), 3)
         for i, word in enumerate(["joy", "of", "data"]):
             self.assertTrue(isinstance(output[i], TextBox))
             self.assertEqual(output[i].text, word)
             self.assertEqual(output[i].bounding_box, None)
             self.assertEqual(output[i].conf, None)
 
@@ -248,26 +252,28 @@
         self.assertTrue(
             os.path.exists(os.path.join("easyocr_autosave", "joy_of_data.txt"))
         )
 
         # test pickle
         ocr_pipeline.to_pickle(out_pkl_path="test.pkl")
 
-    def test_easyocr_textbox_pipeline(self) -> None:
+    @iter_params(store_intermediate_images=[True, False])
+    def test_easyocr_textbox_pipeline(self, store_intermediate_images: bool) -> None:
         """
         Test EasyOCR TextBox pipeline.
         """
 
         # init and check state
         ocr_pipeline = OCRPipeline(
             img_pipeline=None,
             ocr_method=OCRMethod.EASYOCR,
             output_type=OutputType.TEXTBOX,
             text_pipeline=None,
             autosave_output_img_path="easyocr_autosave",
+            store_intermediate_images=store_intermediate_images,
         )
         self.assertTrue(isinstance(ocr_pipeline.ocr_op, EasyOCRTextBoxOp))
         self.assertEqual(ocr_pipeline.input, None)
         self.assertEqual(ocr_pipeline.output, None)
         for method in [
             ocr_pipeline.vis,
             ocr_pipeline.vis_profile,
@@ -278,30 +284,51 @@
                 method()
 
         # test execution on sample image
         output = ocr_pipeline.exec(self.joy_of_data_img)
         self.assertTrue(isinstance(output, OCRPipelineResult))
         image_result = output[0]
         self.assertTrue(isinstance(image_result, OCRImageResult))
+        if store_intermediate_images:
+            self.assertTrue(isinstance(image_result.input_img, ImageResult))
+            self.assertTrue(isinstance(image_result.input_img.img, np.ndarray))
+            self.assertTrue(isinstance(image_result.output_img, np.ndarray))
+            self.assertFalse(
+                np.array_equal(image_result.input_img.img, image_result.output_img)
+            )
+        else:
+            self.assertTrue(isinstance(image_result.input_img, ImageResult))
+            self.assertEqual(image_result.input_img.img, None)
+            self.assertEqual(image_result.output_img, None)
         self.assertTrue(image_result.use_bounding_box)
-        self.assertFalse(
-            np.array_equal(image_result.input_img.img, image_result.output_img)
-        )
         self.assertEqual(len(image_result), 3)
         for i, word in enumerate(["joy", "of", "data"]):
             self.assertTrue(isinstance(image_result[i], TextBox))
             self.assertEqual(image_result[i].text, word)
             self.assertTrue(isinstance(image_result[i].bounding_box, Polygon))
             self.assertTrue(isinstance(image_result[i].conf, float))
 
         # test save and vis
-        self._assert_pass_save_tests(
-            ocr_pipeline=ocr_pipeline, expected_num_txt=0, expected_num_png=2
-        )
-        self._assert_pass_vis_tests(ocr_pipeline=ocr_pipeline)
+        if store_intermediate_images:
+            self._assert_pass_save_tests(
+                ocr_pipeline=ocr_pipeline, expected_num_txt=0, expected_num_png=2
+            )
+            file_list = None
+        else:
+            with self.assertRaises(ValueError):
+                self._assert_pass_save_tests(
+                    ocr_pipeline=ocr_pipeline, expected_num_txt=0, expected_num_png=2
+                )
+            file_list = [
+                "drop_intermediate_images",
+                "['run_ocr', 'drop_intermediate_images']",
+                "['run_ocr', 'drop_intermediate_images']_violin",
+                "run_ocr",
+            ]
+        self._assert_pass_vis_tests(ocr_pipeline=ocr_pipeline, file_list=file_list)
 
         # test autosave
         self.assertTrue(
             os.path.exists(os.path.join("easyocr_autosave", "joy_of_data.png"))
         )
 
         # test pickle
```

### Comparing `ocr-ops-0.0.0.4.2.4/ocr_ops/test/test_run_finding.py` & `ocr-ops-0.0.0.4.2.7/ocr_ops/test/test_run_finding.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
     find_uninterrupted_runs,
     stitch_with_tol,
     find_runs_with_tol,
 )
 
 
 class TestRunFinding(unittest.TestCase):
-
     def test_interval(self) -> None:
         """
         Test interval class.
         """
 
         # test interval properties
         interval = Interval(0, 1)
@@ -173,21 +172,18 @@
             find_runs_with_tol(series=series, query_elem=3, tol=4), [Interval(10, 11)]
         )
         self.assertListEqual(find_runs_with_tol(series=series, query_elem=4, tol=4), [])
 
         # test 1 elem
         series = [1]
         self.assertListEqual(
-            find_runs_with_tol(series=series, query_elem=1, tol=1),
-            [Interval(0, 1)],
+            find_runs_with_tol(series=series, query_elem=1, tol=1), [Interval(0, 1)],
         )
         self.assertListEqual(
-            find_runs_with_tol(series=series, query_elem=2, tol=1),
-            [],
+            find_runs_with_tol(series=series, query_elem=2, tol=1), [],
         )
 
         # test empty
         series = []
         self.assertListEqual(
-            find_runs_with_tol(series=series, query_elem=1, tol=1),
-            [],
+            find_runs_with_tol(series=series, query_elem=1, tol=1), [],
         )
```

### Comparing `ocr-ops-0.0.0.4.2.4/ocr_ops.egg-info/PKG-INFO` & `ocr-ops-0.0.0.4.2.7/ocr_ops.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocr-ops
-Version: 0.0.0.4.2.4
+Version: 0.0.0.4.2.7
 Summary: OCR-Ops
 Home-page: https://github.com/prateekt/ocr-ops
 Author: Prateek Tandon
 Author-email: prateek1.tandon@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ocr-ops-0.0.0.4.2.4/ocr_ops.egg-info/SOURCES.txt` & `ocr-ops-0.0.0.4.2.7/ocr_ops.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 ocr_ops/dependency/__init__.py
 ocr_ops/dependency/ffmpeg.py
 ocr_ops/experimental/__init__.py
 ocr_ops/experimental/ocr_fusion.py
 ocr_ops/framework/__init__.py
 ocr_ops/framework/op/__init__.py
 ocr_ops/framework/op/abstract_ocr_op.py
+ocr_ops/framework/op/drop_op.py
 ocr_ops/framework/op/ffmpeg_op.py
 ocr_ops/framework/op/ocr_op.py
 ocr_ops/framework/op/result/__init__.py
 ocr_ops/framework/op/result/ffmeg_result.py
 ocr_ops/framework/op/result/ocr_result.py
 ocr_ops/framework/pipeline/__init__.py
 ocr_ops/framework/pipeline/ocr_pipeline.py
```

### Comparing `ocr-ops-0.0.0.4.2.4/setup.py` & `ocr-ops-0.0.0.4.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 with open("requirements.txt") as f:
     required = f.read().splitlines()
 
 setuptools.setup(
     name="ocr-ops",
-    version="0.0.0.4.2.4",
+    version="0.0.0.4.2.7",
     author="Prateek Tandon",
     author_email="prateek1.tandon@gmail.com",
     description="OCR-Ops",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/prateekt/ocr-ops",
     packages=setuptools.find_packages(),
```

