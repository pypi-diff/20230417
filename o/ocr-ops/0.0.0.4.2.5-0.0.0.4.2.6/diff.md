# Comparing `tmp/ocr-ops-0.0.0.4.2.5.tar.gz` & `tmp/ocr-ops-0.0.0.4.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocr-ops-0.0.0.4.2.5.tar", last modified: Sun Apr 16 21:02:53 2023, max compression
+gzip compressed data, was "ocr-ops-0.0.0.4.2.6.tar", last modified: Sun Apr 16 22:17:04 2023, max compression
```

## Comparing `ocr-ops-0.0.0.4.2.5.tar` & `ocr-ops-0.0.0.4.2.6.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-16 21:02:53.668344 ocr-ops-0.0.0.4.2.5/
--rw-r--r--   0 tandonp    (501) staff       (20)     1071 2022-03-27 19:39:41.000000 ocr-ops-0.0.0.4.2.5/LICENSE
--rw-r--r--   0 tandonp    (501) staff       (20)       24 2022-03-21 02:23:19.000000 ocr-ops-0.0.0.4.2.5/MANIFEST.in
--rw-r--r--   0 tandonp    (501) staff       (20)     1254 2023-04-16 21:02:53.668165 ocr-ops-0.0.0.4.2.5/PKG-INFO
--rw-r--r--   0 tandonp    (501) staff       (20)      835 2023-03-19 20:02:57.000000 ocr-ops-0.0.0.4.2.5/README.md
-drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-16 21:02:53.661762 ocr-ops-0.0.0.4.2.5/ocr_ops/
--rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-03-27 22:16:22.000000 ocr-ops-0.0.0.4.2.5/ocr_ops/__init__.py
-drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-16 21:02:53.662703 ocr-ops-0.0.0.4.2.5/ocr_ops/dependency/
--rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-03-27 17:57:54.000000 ocr-ops-0.0.0.4.2.5/ocr_ops/dependency/__init__.py
--rw-r--r--   0 tandonp    (501) staff       (20)     1322 2022-06-03 07:01:48.000000 ocr-ops-0.0.0.4.2.5/ocr_ops/dependency/ffmpeg.py
-drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-16 21:02:53.663215 ocr-ops-0.0.0.4.2.5/ocr_ops/experimental/
--rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-03-27 20:44:00.000000 ocr-ops-0.0.0.4.2.5/ocr_ops/experimental/__init__.py
--rw-r--r--   0 tandonp    (501) staff       (20)     4773 2022-05-30 22:56:14.000000 ocr-ops-0.0.0.4.2.5/ocr_ops/experimental/ocr_fusion.py
-drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-16 21:02:53.663580 ocr-ops-0.0.0.4.2.5/ocr_ops/framework/
--rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-03-09 07:46:32.000000 ocr-ops-0.0.0.4.2.5/ocr_ops/framework/__init__.py
-drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-16 21:02:53.664373 ocr-ops-0.0.0.4.2.5/ocr_ops/framework/op/
--rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-03-27 18:12:24.000000 ocr-ops-0.0.0.4.2.5/ocr_ops/framework/op/__init__.py
--rw-r--r--   0 tandonp    (501) staff       (20)     8670 2023-04-16 20:58:32.000000 ocr-ops-0.0.0.4.2.5/ocr_ops/framework/op/abstract_ocr_op.py
--rw-r--r--   0 tandonp    (501) staff       (20)      718 2023-04-16 20:58:32.000000 ocr-ops-0.0.0.4.2.5/ocr_ops/framework/op/drop_op.py
--rw-r--r--   0 tandonp    (501) staff       (20)     2385 2022-06-09 02:59:29.000000 ocr-ops-0.0.0.4.2.5/ocr_ops/framework/op/ffmpeg_op.py
--rw-r--r--   0 tandonp    (501) staff       (20)     5559 2023-04-16 02:58:51.000000 ocr-ops-0.0.0.4.2.5/ocr_ops/framework/op/ocr_op.py
-drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-16 21:02:53.665010 ocr-ops-0.0.0.4.2.5/ocr_ops/framework/op/result/
--rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-05-30 17:21:51.000000 ocr-ops-0.0.0.4.2.5/ocr_ops/framework/op/result/__init__.py
--rw-r--r--   0 tandonp    (501) staff       (20)      764 2022-06-09 03:07:59.000000 ocr-ops-0.0.0.4.2.5/ocr_ops/framework/op/result/ffmeg_result.py
--rw-r--r--   0 tandonp    (501) staff       (20)     6878 2023-04-16 20:58:32.000000 ocr-ops-0.0.0.4.2.5/ocr_ops/framework/op/result/ocr_result.py
-drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-16 21:02:53.665337 ocr-ops-0.0.0.4.2.5/ocr_ops/framework/pipeline/
--rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-03-27 18:13:01.000000 ocr-ops-0.0.0.4.2.5/ocr_ops/framework/pipeline/__init__.py
--rw-r--r--   0 tandonp    (501) staff       (20)     8262 2023-04-16 20:58:32.000000 ocr-ops-0.0.0.4.2.5/ocr_ops/framework/pipeline/ocr_pipeline.py
-drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-16 21:02:53.666146 ocr-ops-0.0.0.4.2.5/ocr_ops/instances/
--rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-03-09 07:46:32.000000 ocr-ops-0.0.0.4.2.5/ocr_ops/instances/__init__.py
--rw-r--r--   0 tandonp    (501) staff       (20)     1656 2023-03-19 20:05:54.000000 ocr-ops-0.0.0.4.2.5/ocr_ops/instances/cv.py
--rw-r--r--   0 tandonp    (501) staff       (20)     3155 2022-06-08 03:45:51.000000 ocr-ops-0.0.0.4.2.5/ocr_ops/instances/ocr.py
--rw-r--r--   0 tandonp    (501) staff       (20)     5505 2023-03-19 20:05:54.000000 ocr-ops-0.0.0.4.2.5/ocr_ops/instances/text.py
-drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-16 21:02:53.666742 ocr-ops-0.0.0.4.2.5/ocr_ops/run_finding/
--rw-r--r--   0 tandonp    (501) staff       (20)        0 2023-04-01 22:33:11.000000 ocr-ops-0.0.0.4.2.5/ocr_ops/run_finding/__init__.py
--rw-r--r--   0 tandonp    (501) staff       (20)     2432 2023-04-02 20:05:16.000000 ocr-ops-0.0.0.4.2.5/ocr_ops/run_finding/interval.py
--rw-r--r--   0 tandonp    (501) staff       (20)     2928 2023-04-01 22:33:11.000000 ocr-ops-0.0.0.4.2.5/ocr_ops/run_finding/run_finding.py
-drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-16 21:02:53.667909 ocr-ops-0.0.0.4.2.5/ocr_ops/test/
--rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-03-27 17:58:47.000000 ocr-ops-0.0.0.4.2.5/ocr_ops/test/__init__.py
--rw-r--r--   0 tandonp    (501) staff       (20)     3354 2022-06-09 03:02:43.000000 ocr-ops-0.0.0.4.2.5/ocr_ops/test/test_ffmpeg_op.py
--rw-r--r--   0 tandonp    (501) staff       (20)     1897 2022-06-03 07:03:09.000000 ocr-ops-0.0.0.4.2.5/ocr_ops/test/test_installs.py
--rw-r--r--   0 tandonp    (501) staff       (20)     9090 2023-04-02 00:02:40.000000 ocr-ops-0.0.0.4.2.5/ocr_ops/test/test_ocr_ops.py
--rw-r--r--   0 tandonp    (501) staff       (20)    17189 2023-04-16 20:58:32.000000 ocr-ops-0.0.0.4.2.5/ocr_ops/test/test_ocr_pipeline.py
--rw-r--r--   0 tandonp    (501) staff       (20)     7079 2023-04-16 20:58:32.000000 ocr-ops-0.0.0.4.2.5/ocr_ops/test/test_run_finding.py
-drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-16 21:02:53.662448 ocr-ops-0.0.0.4.2.5/ocr_ops.egg-info/
--rw-r--r--   0 tandonp    (501) staff       (20)     1254 2023-04-16 21:02:53.000000 ocr-ops-0.0.0.4.2.5/ocr_ops.egg-info/PKG-INFO
--rw-r--r--   0 tandonp    (501) staff       (20)     1166 2023-04-16 21:02:53.000000 ocr-ops-0.0.0.4.2.5/ocr_ops.egg-info/SOURCES.txt
--rw-r--r--   0 tandonp    (501) staff       (20)        1 2023-04-16 21:02:53.000000 ocr-ops-0.0.0.4.2.5/ocr_ops.egg-info/dependency_links.txt
--rw-r--r--   0 tandonp    (501) staff       (20)      127 2023-04-16 21:02:53.000000 ocr-ops-0.0.0.4.2.5/ocr_ops.egg-info/requires.txt
--rw-r--r--   0 tandonp    (501) staff       (20)        8 2023-04-16 21:02:53.000000 ocr-ops-0.0.0.4.2.5/ocr_ops.egg-info/top_level.txt
--rw-r--r--   0 tandonp    (501) staff       (20)      258 2023-03-18 07:55:39.000000 ocr-ops-0.0.0.4.2.5/pyproject.toml
--rw-r--r--   0 tandonp    (501) staff       (20)      126 2023-03-18 09:31:17.000000 ocr-ops-0.0.0.4.2.5/requirements.txt
--rw-r--r--   0 tandonp    (501) staff       (20)       38 2023-04-16 21:02:53.668408 ocr-ops-0.0.0.4.2.5/setup.cfg
--rw-r--r--   0 tandonp    (501) staff       (20)      756 2023-04-16 21:02:45.000000 ocr-ops-0.0.0.4.2.5/setup.py
+drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-16 22:17:04.708256 ocr-ops-0.0.0.4.2.6/
+-rw-r--r--   0 tandonp    (501) staff       (20)     1071 2022-03-27 19:39:41.000000 ocr-ops-0.0.0.4.2.6/LICENSE
+-rw-r--r--   0 tandonp    (501) staff       (20)       24 2022-03-21 02:23:19.000000 ocr-ops-0.0.0.4.2.6/MANIFEST.in
+-rw-r--r--   0 tandonp    (501) staff       (20)     1254 2023-04-16 22:17:04.708093 ocr-ops-0.0.0.4.2.6/PKG-INFO
+-rw-r--r--   0 tandonp    (501) staff       (20)      835 2023-03-19 20:02:57.000000 ocr-ops-0.0.0.4.2.6/README.md
+drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-16 22:17:04.703115 ocr-ops-0.0.0.4.2.6/ocr_ops/
+-rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-03-27 22:16:22.000000 ocr-ops-0.0.0.4.2.6/ocr_ops/__init__.py
+drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-16 22:17:04.704277 ocr-ops-0.0.0.4.2.6/ocr_ops/dependency/
+-rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-03-27 17:57:54.000000 ocr-ops-0.0.0.4.2.6/ocr_ops/dependency/__init__.py
+-rw-r--r--   0 tandonp    (501) staff       (20)     1322 2022-06-03 07:01:48.000000 ocr-ops-0.0.0.4.2.6/ocr_ops/dependency/ffmpeg.py
+drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-16 22:17:04.704572 ocr-ops-0.0.0.4.2.6/ocr_ops/experimental/
+-rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-03-27 20:44:00.000000 ocr-ops-0.0.0.4.2.6/ocr_ops/experimental/__init__.py
+-rw-r--r--   0 tandonp    (501) staff       (20)     4773 2022-05-30 22:56:14.000000 ocr-ops-0.0.0.4.2.6/ocr_ops/experimental/ocr_fusion.py
+drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-16 22:17:04.704719 ocr-ops-0.0.0.4.2.6/ocr_ops/framework/
+-rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-03-09 07:46:32.000000 ocr-ops-0.0.0.4.2.6/ocr_ops/framework/__init__.py
+drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-16 22:17:04.705399 ocr-ops-0.0.0.4.2.6/ocr_ops/framework/op/
+-rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-03-27 18:12:24.000000 ocr-ops-0.0.0.4.2.6/ocr_ops/framework/op/__init__.py
+-rw-r--r--   0 tandonp    (501) staff       (20)     8670 2023-04-16 20:58:32.000000 ocr-ops-0.0.0.4.2.6/ocr_ops/framework/op/abstract_ocr_op.py
+-rw-r--r--   0 tandonp    (501) staff       (20)      718 2023-04-16 20:58:32.000000 ocr-ops-0.0.0.4.2.6/ocr_ops/framework/op/drop_op.py
+-rw-r--r--   0 tandonp    (501) staff       (20)     2385 2022-06-09 02:59:29.000000 ocr-ops-0.0.0.4.2.6/ocr_ops/framework/op/ffmpeg_op.py
+-rw-r--r--   0 tandonp    (501) staff       (20)     5559 2023-04-16 02:58:51.000000 ocr-ops-0.0.0.4.2.6/ocr_ops/framework/op/ocr_op.py
+drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-16 22:17:04.705816 ocr-ops-0.0.0.4.2.6/ocr_ops/framework/op/result/
+-rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-05-30 17:21:51.000000 ocr-ops-0.0.0.4.2.6/ocr_ops/framework/op/result/__init__.py
+-rw-r--r--   0 tandonp    (501) staff       (20)      764 2022-06-09 03:07:59.000000 ocr-ops-0.0.0.4.2.6/ocr_ops/framework/op/result/ffmeg_result.py
+-rw-r--r--   0 tandonp    (501) staff       (20)     6878 2023-04-16 20:58:32.000000 ocr-ops-0.0.0.4.2.6/ocr_ops/framework/op/result/ocr_result.py
+drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-16 22:17:04.706098 ocr-ops-0.0.0.4.2.6/ocr_ops/framework/pipeline/
+-rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-03-27 18:13:01.000000 ocr-ops-0.0.0.4.2.6/ocr_ops/framework/pipeline/__init__.py
+-rw-r--r--   0 tandonp    (501) staff       (20)     8225 2023-04-16 22:12:55.000000 ocr-ops-0.0.0.4.2.6/ocr_ops/framework/pipeline/ocr_pipeline.py
+drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-16 22:17:04.706631 ocr-ops-0.0.0.4.2.6/ocr_ops/instances/
+-rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-03-09 07:46:32.000000 ocr-ops-0.0.0.4.2.6/ocr_ops/instances/__init__.py
+-rw-r--r--   0 tandonp    (501) staff       (20)     1642 2023-04-16 22:12:55.000000 ocr-ops-0.0.0.4.2.6/ocr_ops/instances/cv.py
+-rw-r--r--   0 tandonp    (501) staff       (20)     4011 2023-04-16 22:12:55.000000 ocr-ops-0.0.0.4.2.6/ocr_ops/instances/ocr.py
+-rw-r--r--   0 tandonp    (501) staff       (20)     5505 2023-03-19 20:05:54.000000 ocr-ops-0.0.0.4.2.6/ocr_ops/instances/text.py
+drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-16 22:17:04.707032 ocr-ops-0.0.0.4.2.6/ocr_ops/run_finding/
+-rw-r--r--   0 tandonp    (501) staff       (20)        0 2023-04-01 22:33:11.000000 ocr-ops-0.0.0.4.2.6/ocr_ops/run_finding/__init__.py
+-rw-r--r--   0 tandonp    (501) staff       (20)     2432 2023-04-02 20:05:16.000000 ocr-ops-0.0.0.4.2.6/ocr_ops/run_finding/interval.py
+-rw-r--r--   0 tandonp    (501) staff       (20)     2928 2023-04-01 22:33:11.000000 ocr-ops-0.0.0.4.2.6/ocr_ops/run_finding/run_finding.py
+drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-16 22:17:04.707868 ocr-ops-0.0.0.4.2.6/ocr_ops/test/
+-rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-03-27 17:58:47.000000 ocr-ops-0.0.0.4.2.6/ocr_ops/test/__init__.py
+-rw-r--r--   0 tandonp    (501) staff       (20)     3354 2022-06-09 03:02:43.000000 ocr-ops-0.0.0.4.2.6/ocr_ops/test/test_ffmpeg_op.py
+-rw-r--r--   0 tandonp    (501) staff       (20)     1897 2022-06-03 07:03:09.000000 ocr-ops-0.0.0.4.2.6/ocr_ops/test/test_installs.py
+-rw-r--r--   0 tandonp    (501) staff       (20)     9090 2023-04-02 00:02:40.000000 ocr-ops-0.0.0.4.2.6/ocr_ops/test/test_ocr_ops.py
+-rw-r--r--   0 tandonp    (501) staff       (20)    17173 2023-04-16 22:12:55.000000 ocr-ops-0.0.0.4.2.6/ocr_ops/test/test_ocr_pipeline.py
+-rw-r--r--   0 tandonp    (501) staff       (20)     7043 2023-04-16 22:12:55.000000 ocr-ops-0.0.0.4.2.6/ocr_ops/test/test_run_finding.py
+drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-16 22:17:04.704012 ocr-ops-0.0.0.4.2.6/ocr_ops.egg-info/
+-rw-r--r--   0 tandonp    (501) staff       (20)     1254 2023-04-16 22:17:04.000000 ocr-ops-0.0.0.4.2.6/ocr_ops.egg-info/PKG-INFO
+-rw-r--r--   0 tandonp    (501) staff       (20)     1166 2023-04-16 22:17:04.000000 ocr-ops-0.0.0.4.2.6/ocr_ops.egg-info/SOURCES.txt
+-rw-r--r--   0 tandonp    (501) staff       (20)        1 2023-04-16 22:17:04.000000 ocr-ops-0.0.0.4.2.6/ocr_ops.egg-info/dependency_links.txt
+-rw-r--r--   0 tandonp    (501) staff       (20)      127 2023-04-16 22:17:04.000000 ocr-ops-0.0.0.4.2.6/ocr_ops.egg-info/requires.txt
+-rw-r--r--   0 tandonp    (501) staff       (20)        8 2023-04-16 22:17:04.000000 ocr-ops-0.0.0.4.2.6/ocr_ops.egg-info/top_level.txt
+-rw-r--r--   0 tandonp    (501) staff       (20)      258 2023-03-18 07:55:39.000000 ocr-ops-0.0.0.4.2.6/pyproject.toml
+-rw-r--r--   0 tandonp    (501) staff       (20)      126 2023-03-18 09:31:17.000000 ocr-ops-0.0.0.4.2.6/requirements.txt
+-rw-r--r--   0 tandonp    (501) staff       (20)       38 2023-04-16 22:17:04.708310 ocr-ops-0.0.0.4.2.6/setup.cfg
+-rw-r--r--   0 tandonp    (501) staff       (20)      756 2023-04-16 22:17:00.000000 ocr-ops-0.0.0.4.2.6/setup.py
```

### Comparing `ocr-ops-0.0.0.4.2.5/LICENSE` & `ocr-ops-0.0.0.4.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ocr-ops-0.0.0.4.2.5/PKG-INFO` & `ocr-ops-0.0.0.4.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocr-ops
-Version: 0.0.0.4.2.5
+Version: 0.0.0.4.2.6
 Summary: OCR-Ops
 Home-page: https://github.com/prateekt/ocr-ops
 Author: Prateek Tandon
 Author-email: prateek1.tandon@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ocr-ops-0.0.0.4.2.5/README.md` & `ocr-ops-0.0.0.4.2.6/README.md`

 * *Files identical despite different names*

### Comparing `ocr-ops-0.0.0.4.2.5/ocr_ops/dependency/ffmpeg.py` & `ocr-ops-0.0.0.4.2.6/ocr_ops/dependency/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `ocr-ops-0.0.0.4.2.5/ocr_ops/experimental/ocr_fusion.py` & `ocr-ops-0.0.0.4.2.6/ocr_ops/experimental/ocr_fusion.py`

 * *Files identical despite different names*

### Comparing `ocr-ops-0.0.0.4.2.5/ocr_ops/framework/op/abstract_ocr_op.py` & `ocr-ops-0.0.0.4.2.6/ocr_ops/framework/op/abstract_ocr_op.py`

 * *Files identical despite different names*

### Comparing `ocr-ops-0.0.0.4.2.5/ocr_ops/framework/op/drop_op.py` & `ocr-ops-0.0.0.4.2.6/ocr_ops/framework/op/drop_op.py`

 * *Files identical despite different names*

### Comparing `ocr-ops-0.0.0.4.2.5/ocr_ops/framework/op/ffmpeg_op.py` & `ocr-ops-0.0.0.4.2.6/ocr_ops/framework/op/ffmpeg_op.py`

 * *Files identical despite different names*

### Comparing `ocr-ops-0.0.0.4.2.5/ocr_ops/framework/op/ocr_op.py` & `ocr-ops-0.0.0.4.2.6/ocr_ops/framework/op/ocr_op.py`

 * *Files identical despite different names*

### Comparing `ocr-ops-0.0.0.4.2.5/ocr_ops/framework/op/result/ffmeg_result.py` & `ocr-ops-0.0.0.4.2.6/ocr_ops/framework/op/result/ffmeg_result.py`

 * *Files identical despite different names*

### Comparing `ocr-ops-0.0.0.4.2.5/ocr_ops/framework/op/result/ocr_result.py` & `ocr-ops-0.0.0.4.2.6/ocr_ops/framework/op/result/ocr_result.py`

 * *Files identical despite different names*

### Comparing `ocr-ops-0.0.0.4.2.5/ocr_ops/framework/pipeline/ocr_pipeline.py` & `ocr-ops-0.0.0.4.2.6/ocr_ops/framework/pipeline/ocr_pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import os.path
 from enum import Enum
 from typing import Optional, Dict, Any, List, Union
 
 from algo_ops.dependency.sys_util import get_image_files, is_image_file
 from algo_ops.ops.op import Op
-from algo_ops.ops.text import TextOp
 from algo_ops.paraloop import paraloop
 from algo_ops.pipeline.cv_pipeline import CVPipeline
 from algo_ops.pipeline.pipeline import Pipeline
 
 from ocr_ops.framework.op.abstract_ocr_op import AbstractOCROp, EasyOCROp
 from ocr_ops.framework.op.drop_op import DropOp
 from ocr_ops.framework.op.ocr_op import (
```

### Comparing `ocr-ops-0.0.0.4.2.5/ocr_ops/instances/cv.py` & `ocr-ops-0.0.0.4.2.6/ocr_ops/instances/cv.py`

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

### Comparing `ocr-ops-0.0.0.4.2.5/ocr_ops/instances/text.py` & `ocr-ops-0.0.0.4.2.6/ocr_ops/instances/text.py`

 * *Files identical despite different names*

### Comparing `ocr-ops-0.0.0.4.2.5/ocr_ops/run_finding/interval.py` & `ocr-ops-0.0.0.4.2.6/ocr_ops/run_finding/interval.py`

 * *Files identical despite different names*

### Comparing `ocr-ops-0.0.0.4.2.5/ocr_ops/run_finding/run_finding.py` & `ocr-ops-0.0.0.4.2.6/ocr_ops/run_finding/run_finding.py`

 * *Files identical despite different names*

### Comparing `ocr-ops-0.0.0.4.2.5/ocr_ops/test/test_ffmpeg_op.py` & `ocr-ops-0.0.0.4.2.6/ocr_ops/test/test_ffmpeg_op.py`

 * *Files identical despite different names*

### Comparing `ocr-ops-0.0.0.4.2.5/ocr_ops/test/test_installs.py` & `ocr-ops-0.0.0.4.2.6/ocr_ops/test/test_installs.py`

 * *Files identical despite different names*

### Comparing `ocr-ops-0.0.0.4.2.5/ocr_ops/test/test_ocr_ops.py` & `ocr-ops-0.0.0.4.2.6/ocr_ops/test/test_ocr_ops.py`

 * *Files identical despite different names*

### Comparing `ocr-ops-0.0.0.4.2.5/ocr_ops/test/test_ocr_pipeline.py` & `ocr-ops-0.0.0.4.2.6/ocr_ops/test/test_ocr_pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,17 +49,15 @@
                 "test_autosave3",
                 "test_autosave4",
             ),
             files=("test.pkl",),
         )
 
     def _assert_pass_vis_tests(
-        self,
-        ocr_pipeline: OCRPipeline,
-        file_list=None,
+        self, ocr_pipeline: OCRPipeline, file_list=None,
     ) -> None:
         # test vis input / output
         if file_list is None:
             file_list = ["['run_ocr']", "['run_ocr']_violin", "run_ocr"]
         with self.assertRaises(ValueError):
             ocr_pipeline.vis_input()
         ocr_pipeline.vis()
```

### Comparing `ocr-ops-0.0.0.4.2.5/ocr_ops/test/test_run_finding.py` & `ocr-ops-0.0.0.4.2.6/ocr_ops/test/test_run_finding.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,21 +172,18 @@
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

### Comparing `ocr-ops-0.0.0.4.2.5/ocr_ops.egg-info/PKG-INFO` & `ocr-ops-0.0.0.4.2.6/ocr_ops.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocr-ops
-Version: 0.0.0.4.2.5
+Version: 0.0.0.4.2.6
 Summary: OCR-Ops
 Home-page: https://github.com/prateekt/ocr-ops
 Author: Prateek Tandon
 Author-email: prateek1.tandon@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ocr-ops-0.0.0.4.2.5/ocr_ops.egg-info/SOURCES.txt` & `ocr-ops-0.0.0.4.2.6/ocr_ops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ocr-ops-0.0.0.4.2.5/setup.py` & `ocr-ops-0.0.0.4.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 with open("requirements.txt") as f:
     required = f.read().splitlines()
 
 setuptools.setup(
     name="ocr-ops",
-    version="0.0.0.4.2.5",
+    version="0.0.0.4.2.6",
     author="Prateek Tandon",
     author_email="prateek1.tandon@gmail.com",
     description="OCR-Ops",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/prateekt/ocr-ops",
     packages=setuptools.find_packages(),
```

