# Comparing `tmp/clarifai-9.3.2.tar.gz` & `tmp/clarifai-9.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clarifai-9.3.2.tar", last modified: Wed Apr 12 18:10:29 2023, max compression
+gzip compressed data, was "clarifai-9.3.3.tar", last modified: Mon Apr 17 20:36:41 2023, max compression
```

## Comparing `clarifai-9.3.2.tar` & `clarifai-9.3.3.tar`

### file list

```diff
@@ -1,97 +1,126 @@
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-12 18:10:29.564670 clarifai-9.3.2/
--rw-r--r--   0 zeiler     (503) staff       (20)      555 2021-12-09 18:28:59.000000 clarifai-9.3.2/LICENSE
--rw-r--r--   0 zeiler     (503) staff       (20)       21 2022-07-01 04:22:44.000000 clarifai-9.3.2/MANIFEST.in
--rw-r--r--   0 zeiler     (503) staff       (20)     2882 2023-04-12 18:10:29.564470 clarifai-9.3.2/PKG-INFO
--rw-r--r--   0 zeiler     (503) staff       (20)     2347 2023-01-03 21:48:03.000000 clarifai-9.3.2/README.md
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-12 18:10:29.552491 clarifai-9.3.2/clarifai/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai/__init__.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-12 18:10:29.553402 clarifai-9.3.2/clarifai/auth/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai/auth/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)    12387 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai/auth/helper.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-12 18:10:29.554028 clarifai-9.3.2/clarifai/client/
--rw-r--r--   0 zeiler     (503) staff       (20)      121 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai/client/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)      536 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai/client/abc.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3606 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai/client/stub.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-12 18:10:29.554527 clarifai-9.3.2/clarifai/data_upload/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai/data_upload/__init__.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-12 18:10:29.555547 clarifai-9.3.2/clarifai/data_upload/datasets/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.3.2/clarifai/data_upload/datasets/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1693 2023-03-23 03:08:12.000000 clarifai-9.3.2/clarifai/data_upload/datasets/base.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1089 2023-03-23 03:08:12.000000 clarifai-9.3.2/clarifai/data_upload/datasets/features.py
--rw-r--r--   0 zeiler     (503) staff       (20)     9235 2023-03-23 03:08:12.000000 clarifai-9.3.2/clarifai/data_upload/datasets/image.py
--rw-r--r--   0 zeiler     (503) staff       (20)     2110 2023-03-23 03:08:12.000000 clarifai-9.3.2/clarifai/data_upload/datasets/text.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-12 18:10:29.556330 clarifai-9.3.2/clarifai/data_upload/datasets/zoo/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.3.2/clarifai/data_upload/datasets/zoo/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3651 2023-03-23 03:08:12.000000 clarifai-9.3.2/clarifai/data_upload/datasets/zoo/coco_captions.py
--rw-r--r--   0 zeiler     (503) staff       (20)     4856 2023-03-23 03:08:12.000000 clarifai-9.3.2/clarifai/data_upload/datasets/zoo/coco_detection.py
--rw-r--r--   0 zeiler     (503) staff       (20)     6196 2023-03-23 03:08:12.000000 clarifai-9.3.2/clarifai/data_upload/datasets/zoo/coco_segmentation.py
--rw-r--r--   0 zeiler     (503) staff       (20)      540 2023-03-23 03:08:12.000000 clarifai-9.3.2/clarifai/data_upload/examples.py
--rw-r--r--   0 zeiler     (503) staff       (20)    10917 2023-03-23 03:08:12.000000 clarifai-9.3.2/clarifai/data_upload/upload.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-12 18:10:29.558333 clarifai-9.3.2/clarifai/listing/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai/listing/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1169 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai/listing/concepts.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1184 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai/listing/datasets.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3632 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai/listing/inputs.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1466 2023-04-11 15:50:37.000000 clarifai-9.3.2/clarifai/listing/installed_module_versions.py
--rw-r--r--   0 zeiler     (503) staff       (20)     7764 2023-04-12 16:48:35.000000 clarifai-9.3.2/clarifai/listing/lister.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1506 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai/listing/models.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1480 2023-04-11 15:50:37.000000 clarifai-9.3.2/clarifai/listing/module_versions.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1170 2023-04-11 15:50:37.000000 clarifai-9.3.2/clarifai/listing/modules.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-12 18:10:29.558991 clarifai-9.3.2/clarifai/modules/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai/modules/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     2020 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai/modules/css.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1383 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai/modules/pages.py
--rw-r--r--   0 zeiler     (503) staff       (20)     4131 2023-03-23 03:08:12.000000 clarifai-9.3.2/clarifai/modules/style.css
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-12 18:10:29.559375 clarifai-9.3.2/clarifai/urls/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2022-07-20 04:15:05.000000 clarifai-9.3.2/clarifai/urls/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3172 2023-01-07 05:29:12.000000 clarifai-9.3.2/clarifai/urls/helper.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-12 18:10:29.553162 clarifai-9.3.2/clarifai.egg-info/
--rw-r--r--   0 zeiler     (503) staff       (20)     2882 2023-04-12 18:10:29.000000 clarifai-9.3.2/clarifai.egg-info/PKG-INFO
--rw-r--r--   0 zeiler     (503) staff       (20)     2555 2023-04-12 18:10:29.000000 clarifai-9.3.2/clarifai.egg-info/SOURCES.txt
--rw-r--r--   0 zeiler     (503) staff       (20)        1 2023-04-12 18:10:29.000000 clarifai-9.3.2/clarifai.egg-info/dependency_links.txt
--rw-r--r--   0 zeiler     (503) staff       (20)       21 2023-04-12 18:10:29.000000 clarifai-9.3.2/clarifai.egg-info/requires.txt
--rw-r--r--   0 zeiler     (503) staff       (20)       24 2023-04-12 18:10:29.000000 clarifai-9.3.2/clarifai.egg-info/top_level.txt
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-12 18:10:29.559715 clarifai-9.3.2/clarifai_utils/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai_utils/__init__.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-12 18:10:29.560001 clarifai-9.3.2/clarifai_utils/auth/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai_utils/auth/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)    12387 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai_utils/auth/helper.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-12 18:10:29.560467 clarifai-9.3.2/clarifai_utils/client/
--rw-r--r--   0 zeiler     (503) staff       (20)      121 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai_utils/client/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)      536 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai_utils/client/abc.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3606 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai_utils/client/stub.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-12 18:10:29.560878 clarifai-9.3.2/clarifai_utils/data_upload/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai_utils/data_upload/__init__.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-12 18:10:29.561575 clarifai-9.3.2/clarifai_utils/data_upload/datasets/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.3.2/clarifai_utils/data_upload/datasets/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1693 2023-03-23 03:08:12.000000 clarifai-9.3.2/clarifai_utils/data_upload/datasets/base.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1089 2023-03-23 03:08:12.000000 clarifai-9.3.2/clarifai_utils/data_upload/datasets/features.py
--rw-r--r--   0 zeiler     (503) staff       (20)     9235 2023-03-23 03:08:12.000000 clarifai-9.3.2/clarifai_utils/data_upload/datasets/image.py
--rw-r--r--   0 zeiler     (503) staff       (20)     2110 2023-03-23 03:08:12.000000 clarifai-9.3.2/clarifai_utils/data_upload/datasets/text.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-12 18:10:29.562129 clarifai-9.3.2/clarifai_utils/data_upload/datasets/zoo/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.3.2/clarifai_utils/data_upload/datasets/zoo/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3651 2023-03-23 03:08:12.000000 clarifai-9.3.2/clarifai_utils/data_upload/datasets/zoo/coco_captions.py
--rw-r--r--   0 zeiler     (503) staff       (20)     4856 2023-03-23 03:08:12.000000 clarifai-9.3.2/clarifai_utils/data_upload/datasets/zoo/coco_detection.py
--rw-r--r--   0 zeiler     (503) staff       (20)     6196 2023-03-23 03:08:12.000000 clarifai-9.3.2/clarifai_utils/data_upload/datasets/zoo/coco_segmentation.py
--rw-r--r--   0 zeiler     (503) staff       (20)      540 2023-03-23 03:08:12.000000 clarifai-9.3.2/clarifai_utils/data_upload/examples.py
--rw-r--r--   0 zeiler     (503) staff       (20)    10917 2023-03-23 03:08:12.000000 clarifai-9.3.2/clarifai_utils/data_upload/upload.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-12 18:10:29.563430 clarifai-9.3.2/clarifai_utils/listing/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai_utils/listing/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1169 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai_utils/listing/concepts.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1184 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai_utils/listing/datasets.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3632 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai_utils/listing/inputs.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1466 2023-04-11 15:50:37.000000 clarifai-9.3.2/clarifai_utils/listing/installed_module_versions.py
--rw-r--r--   0 zeiler     (503) staff       (20)     7764 2023-04-12 16:48:35.000000 clarifai-9.3.2/clarifai_utils/listing/lister.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1506 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai_utils/listing/models.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1480 2023-04-11 15:50:37.000000 clarifai-9.3.2/clarifai_utils/listing/module_versions.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1170 2023-04-11 15:50:37.000000 clarifai-9.3.2/clarifai_utils/listing/modules.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-12 18:10:29.563970 clarifai-9.3.2/clarifai_utils/modules/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai_utils/modules/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     2020 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai_utils/modules/css.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1383 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai_utils/modules/pages.py
--rw-r--r--   0 zeiler     (503) staff       (20)     4131 2023-03-23 03:08:12.000000 clarifai-9.3.2/clarifai_utils/modules/style.css
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-12 18:10:29.564228 clarifai-9.3.2/clarifai_utils/urls/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2022-07-20 04:15:05.000000 clarifai-9.3.2/clarifai_utils/urls/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3172 2023-01-07 05:29:12.000000 clarifai-9.3.2/clarifai_utils/urls/helper.py
--rw-r--r--   0 zeiler     (503) staff       (20)       38 2023-04-12 18:10:29.564720 clarifai-9.3.2/setup.cfg
--rw-r--r--   0 zeiler     (503) staff       (20)      887 2023-04-12 18:10:12.000000 clarifai-9.3.2/setup.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-04-17 20:36:41.585719 clarifai-9.3.3/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      555 2023-01-17 09:53:52.000000 clarifai-9.3.3/LICENSE
+-rw-r--r--   0 yvettezhang   (501) staff       (20)       21 2023-01-17 09:53:52.000000 clarifai-9.3.3/MANIFEST.in
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     2882 2023-04-17 20:36:41.585202 clarifai-9.3.3/PKG-INFO
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     2347 2023-01-17 09:53:52.000000 clarifai-9.3.3/README.md
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-04-17 20:36:41.521605 clarifai-9.3.3/clarifai/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-01-17 09:53:52.000000 clarifai-9.3.3/clarifai/__init__.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-04-17 20:36:41.525388 clarifai-9.3.3/clarifai/auth/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-01-17 09:53:52.000000 clarifai-9.3.3/clarifai/auth/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    12387 2023-01-17 09:53:52.000000 clarifai-9.3.3/clarifai/auth/helper.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-04-17 20:36:41.528551 clarifai-9.3.3/clarifai/client/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      121 2023-01-17 09:53:52.000000 clarifai-9.3.3/clarifai/client/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      536 2023-01-17 09:53:52.000000 clarifai-9.3.3/clarifai/client/abc.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     3606 2023-01-17 09:53:52.000000 clarifai-9.3.3/clarifai/client/stub.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-04-17 20:36:41.531233 clarifai-9.3.3/clarifai/data_upload/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-01-17 09:53:52.000000 clarifai-9.3.3/clarifai/data_upload/__init__.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-04-17 20:36:41.535470 clarifai-9.3.3/clarifai/data_upload/datasets/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-04-03 17:20:53.000000 clarifai-9.3.3/clarifai/data_upload/datasets/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1693 2023-04-03 17:20:53.000000 clarifai-9.3.3/clarifai/data_upload/datasets/base.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1089 2023-04-03 17:20:53.000000 clarifai-9.3.3/clarifai/data_upload/datasets/features.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     9235 2023-04-03 17:20:53.000000 clarifai-9.3.3/clarifai/data_upload/datasets/image.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     2110 2023-04-03 17:20:53.000000 clarifai-9.3.3/clarifai/data_upload/datasets/text.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-04-17 20:36:41.538680 clarifai-9.3.3/clarifai/data_upload/datasets/zoo/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-04-03 17:20:53.000000 clarifai-9.3.3/clarifai/data_upload/datasets/zoo/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     3651 2023-04-03 17:20:53.000000 clarifai-9.3.3/clarifai/data_upload/datasets/zoo/coco_captions.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     4856 2023-04-03 17:20:53.000000 clarifai-9.3.3/clarifai/data_upload/datasets/zoo/coco_detection.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     6196 2023-04-03 17:20:53.000000 clarifai-9.3.3/clarifai/data_upload/datasets/zoo/coco_segmentation.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-04-17 20:36:41.514934 clarifai-9.3.3/clarifai/data_upload/examples/
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-04-17 20:36:41.540037 clarifai-9.3.3/clarifai/data_upload/examples/image_classification/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-04-03 17:20:53.000000 clarifai-9.3.3/clarifai/data_upload/examples/image_classification/__init__.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-04-17 20:36:41.541226 clarifai-9.3.3/clarifai/data_upload/examples/image_classification/cifar10/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-04-03 17:20:53.000000 clarifai-9.3.3/clarifai/data_upload/examples/image_classification/cifar10/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1091 2023-04-03 17:20:53.000000 clarifai-9.3.3/clarifai/data_upload/examples/image_classification/cifar10/dataset.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-04-17 20:36:41.542955 clarifai-9.3.3/clarifai/data_upload/examples/image_classification/food-101/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-04-03 17:20:53.000000 clarifai-9.3.3/clarifai/data_upload/examples/image_classification/food-101/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1195 2023-04-03 17:20:53.000000 clarifai-9.3.3/clarifai/data_upload/examples/image_classification/food-101/dataset.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-04-17 20:36:41.544143 clarifai-9.3.3/clarifai/data_upload/examples/text_classification/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-04-03 17:20:53.000000 clarifai-9.3.3/clarifai/data_upload/examples/text_classification/__init__.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-04-17 20:36:41.544948 clarifai-9.3.3/clarifai/data_upload/examples/text_classification/imdb_dataset/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-04-03 17:20:53.000000 clarifai-9.3.3/clarifai/data_upload/examples/text_classification/imdb_dataset/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1049 2023-04-03 17:20:53.000000 clarifai-9.3.3/clarifai/data_upload/examples/text_classification/imdb_dataset/dataset.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      540 2023-04-03 17:20:53.000000 clarifai-9.3.3/clarifai/data_upload/examples.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    10917 2023-04-03 17:20:53.000000 clarifai-9.3.3/clarifai/data_upload/upload.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-04-17 20:36:41.546068 clarifai-9.3.3/clarifai/dataset_export/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     5130 2023-04-17 18:32:17.000000 clarifai-9.3.3/clarifai/dataset_export/dataset_export_inputs.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-04-17 20:36:41.553478 clarifai-9.3.3/clarifai/listing/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-01-17 09:53:52.000000 clarifai-9.3.3/clarifai/listing/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1169 2023-01-17 09:53:52.000000 clarifai-9.3.3/clarifai/listing/concepts.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1184 2023-01-17 09:53:52.000000 clarifai-9.3.3/clarifai/listing/datasets.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     3632 2023-01-17 09:53:52.000000 clarifai-9.3.3/clarifai/listing/inputs.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1466 2023-04-03 17:20:53.000000 clarifai-9.3.3/clarifai/listing/installed_module_versions.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     7764 2023-04-17 18:32:17.000000 clarifai-9.3.3/clarifai/listing/lister.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1506 2023-01-17 09:53:52.000000 clarifai-9.3.3/clarifai/listing/models.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1480 2023-04-03 17:20:53.000000 clarifai-9.3.3/clarifai/listing/module_versions.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1170 2023-04-03 17:20:53.000000 clarifai-9.3.3/clarifai/listing/modules.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-04-17 20:36:41.555921 clarifai-9.3.3/clarifai/modules/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-01-17 09:53:52.000000 clarifai-9.3.3/clarifai/modules/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     2020 2023-01-17 09:53:52.000000 clarifai-9.3.3/clarifai/modules/css.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1383 2023-01-17 09:53:52.000000 clarifai-9.3.3/clarifai/modules/pages.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-04-17 20:36:41.557093 clarifai-9.3.3/clarifai/urls/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     3172 2023-01-17 09:53:52.000000 clarifai-9.3.3/clarifai/urls/helper.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-04-17 20:36:41.524376 clarifai-9.3.3/clarifai.egg-info/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     2882 2023-04-17 20:36:41.000000 clarifai-9.3.3/clarifai.egg-info/PKG-INFO
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     3738 2023-04-17 20:36:41.000000 clarifai-9.3.3/clarifai.egg-info/SOURCES.txt
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        1 2023-04-17 20:36:41.000000 clarifai-9.3.3/clarifai.egg-info/dependency_links.txt
+-rw-r--r--   0 yvettezhang   (501) staff       (20)       21 2023-04-17 20:36:41.000000 clarifai-9.3.3/clarifai.egg-info/requires.txt
+-rw-r--r--   0 yvettezhang   (501) staff       (20)       24 2023-04-17 20:36:41.000000 clarifai-9.3.3/clarifai.egg-info/top_level.txt
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-04-17 20:36:41.557991 clarifai-9.3.3/clarifai_utils/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-01-17 09:53:52.000000 clarifai-9.3.3/clarifai_utils/__init__.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-04-17 20:36:41.558901 clarifai-9.3.3/clarifai_utils/auth/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-01-17 09:53:52.000000 clarifai-9.3.3/clarifai_utils/auth/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    12387 2023-01-17 09:53:52.000000 clarifai-9.3.3/clarifai_utils/auth/helper.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-04-17 20:36:41.560878 clarifai-9.3.3/clarifai_utils/client/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      121 2023-01-17 09:53:52.000000 clarifai-9.3.3/clarifai_utils/client/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      536 2023-01-17 09:53:52.000000 clarifai-9.3.3/clarifai_utils/client/abc.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     3606 2023-01-17 09:53:52.000000 clarifai-9.3.3/clarifai_utils/client/stub.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-04-17 20:36:41.562737 clarifai-9.3.3/clarifai_utils/data_upload/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-01-17 09:53:52.000000 clarifai-9.3.3/clarifai_utils/data_upload/__init__.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-04-17 20:36:41.566840 clarifai-9.3.3/clarifai_utils/data_upload/datasets/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-04-03 17:20:53.000000 clarifai-9.3.3/clarifai_utils/data_upload/datasets/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1693 2023-04-03 17:20:53.000000 clarifai-9.3.3/clarifai_utils/data_upload/datasets/base.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1089 2023-04-03 17:20:53.000000 clarifai-9.3.3/clarifai_utils/data_upload/datasets/features.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     9235 2023-04-03 17:20:53.000000 clarifai-9.3.3/clarifai_utils/data_upload/datasets/image.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     2110 2023-04-03 17:20:53.000000 clarifai-9.3.3/clarifai_utils/data_upload/datasets/text.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-04-17 20:36:41.569447 clarifai-9.3.3/clarifai_utils/data_upload/datasets/zoo/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-04-03 17:20:53.000000 clarifai-9.3.3/clarifai_utils/data_upload/datasets/zoo/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     3651 2023-04-03 17:20:53.000000 clarifai-9.3.3/clarifai_utils/data_upload/datasets/zoo/coco_captions.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     4856 2023-04-03 17:20:53.000000 clarifai-9.3.3/clarifai_utils/data_upload/datasets/zoo/coco_detection.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     6196 2023-04-03 17:20:53.000000 clarifai-9.3.3/clarifai_utils/data_upload/datasets/zoo/coco_segmentation.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-04-17 20:36:41.517492 clarifai-9.3.3/clarifai_utils/data_upload/examples/
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-04-17 20:36:41.569958 clarifai-9.3.3/clarifai_utils/data_upload/examples/image_classification/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-04-03 17:20:53.000000 clarifai-9.3.3/clarifai_utils/data_upload/examples/image_classification/__init__.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-04-17 20:36:41.570913 clarifai-9.3.3/clarifai_utils/data_upload/examples/image_classification/cifar10/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-04-03 17:20:53.000000 clarifai-9.3.3/clarifai_utils/data_upload/examples/image_classification/cifar10/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1091 2023-04-03 17:20:53.000000 clarifai-9.3.3/clarifai_utils/data_upload/examples/image_classification/cifar10/dataset.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-04-17 20:36:41.572921 clarifai-9.3.3/clarifai_utils/data_upload/examples/image_classification/food-101/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-04-03 17:20:53.000000 clarifai-9.3.3/clarifai_utils/data_upload/examples/image_classification/food-101/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1195 2023-04-03 17:20:53.000000 clarifai-9.3.3/clarifai_utils/data_upload/examples/image_classification/food-101/dataset.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-04-17 20:36:41.573938 clarifai-9.3.3/clarifai_utils/data_upload/examples/text_classification/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-04-03 17:20:53.000000 clarifai-9.3.3/clarifai_utils/data_upload/examples/text_classification/__init__.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-04-17 20:36:41.575393 clarifai-9.3.3/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-04-03 17:20:53.000000 clarifai-9.3.3/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1049 2023-04-03 17:20:53.000000 clarifai-9.3.3/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/dataset.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      540 2023-04-03 17:20:53.000000 clarifai-9.3.3/clarifai_utils/data_upload/examples.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    10917 2023-04-03 17:20:53.000000 clarifai-9.3.3/clarifai_utils/data_upload/upload.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-04-17 20:36:41.575972 clarifai-9.3.3/clarifai_utils/dataset_export/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     5130 2023-04-17 18:32:17.000000 clarifai-9.3.3/clarifai_utils/dataset_export/dataset_export_inputs.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-04-17 20:36:41.580842 clarifai-9.3.3/clarifai_utils/listing/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-01-17 09:53:52.000000 clarifai-9.3.3/clarifai_utils/listing/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1169 2023-01-17 09:53:52.000000 clarifai-9.3.3/clarifai_utils/listing/concepts.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1184 2023-01-17 09:53:52.000000 clarifai-9.3.3/clarifai_utils/listing/datasets.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     3632 2023-01-17 09:53:52.000000 clarifai-9.3.3/clarifai_utils/listing/inputs.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1466 2023-04-03 17:20:53.000000 clarifai-9.3.3/clarifai_utils/listing/installed_module_versions.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     7764 2023-04-17 18:32:17.000000 clarifai-9.3.3/clarifai_utils/listing/lister.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1506 2023-01-17 09:53:52.000000 clarifai-9.3.3/clarifai_utils/listing/models.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1480 2023-04-03 17:20:53.000000 clarifai-9.3.3/clarifai_utils/listing/module_versions.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1170 2023-04-03 17:20:53.000000 clarifai-9.3.3/clarifai_utils/listing/modules.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-04-17 20:36:41.582969 clarifai-9.3.3/clarifai_utils/modules/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-01-17 09:53:52.000000 clarifai-9.3.3/clarifai_utils/modules/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     2020 2023-01-17 09:53:52.000000 clarifai-9.3.3/clarifai_utils/modules/css.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1383 2023-01-17 09:53:52.000000 clarifai-9.3.3/clarifai_utils/modules/pages.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     4131 2023-03-01 14:52:28.000000 clarifai-9.3.3/clarifai_utils/modules/style.css
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-04-17 20:36:41.584173 clarifai-9.3.3/clarifai_utils/urls/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     3172 2023-01-17 09:53:52.000000 clarifai-9.3.3/clarifai_utils/urls/helper.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)       38 2023-04-17 20:36:41.585906 clarifai-9.3.3/setup.cfg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      897 2023-04-17 20:36:10.000000 clarifai-9.3.3/setup.py
```

### Comparing `clarifai-9.3.2/LICENSE` & `clarifai-9.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.2/PKG-INFO` & `clarifai-9.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clarifai
-Version: 9.3.2
+Version: 9.3.3
 Summary: Clarifai Python Utilities
 Home-page: https://github.com/Clarifai/clarifai-python-utils
 Author: Clarifai
 Author-email: support@clarifai.com
 License: Apache 2.0
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3
```

### Comparing `clarifai-9.3.2/README.md` & `clarifai-9.3.3/README.md`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.2/clarifai/auth/helper.py` & `clarifai-9.3.3/clarifai/auth/helper.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.2/clarifai/client/abc.py` & `clarifai-9.3.3/clarifai/client/abc.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.2/clarifai/client/stub.py` & `clarifai-9.3.3/clarifai/client/stub.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.2/clarifai/data_upload/datasets/base.py` & `clarifai-9.3.3/clarifai/data_upload/datasets/base.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.2/clarifai/data_upload/datasets/features.py` & `clarifai-9.3.3/clarifai/data_upload/datasets/features.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.2/clarifai/data_upload/datasets/image.py` & `clarifai-9.3.3/clarifai/data_upload/datasets/image.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.2/clarifai/data_upload/datasets/text.py` & `clarifai-9.3.3/clarifai/data_upload/datasets/text.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.2/clarifai/data_upload/datasets/zoo/coco_captions.py` & `clarifai-9.3.3/clarifai/data_upload/datasets/zoo/coco_captions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.2/clarifai/data_upload/datasets/zoo/coco_detection.py` & `clarifai-9.3.3/clarifai/data_upload/datasets/zoo/coco_detection.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.2/clarifai/data_upload/datasets/zoo/coco_segmentation.py` & `clarifai-9.3.3/clarifai/data_upload/datasets/zoo/coco_segmentation.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.2/clarifai/data_upload/examples.py` & `clarifai-9.3.3/clarifai/data_upload/examples.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.2/clarifai/data_upload/upload.py` & `clarifai-9.3.3/clarifai/data_upload/upload.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.2/clarifai/listing/concepts.py` & `clarifai-9.3.3/clarifai/listing/concepts.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.2/clarifai/listing/datasets.py` & `clarifai-9.3.3/clarifai/listing/datasets.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.2/clarifai/listing/inputs.py` & `clarifai-9.3.3/clarifai/listing/inputs.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.2/clarifai/listing/installed_module_versions.py` & `clarifai-9.3.3/clarifai/listing/installed_module_versions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.2/clarifai/listing/lister.py` & `clarifai-9.3.3/clarifai/listing/lister.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.2/clarifai/listing/models.py` & `clarifai-9.3.3/clarifai/listing/models.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.2/clarifai/listing/module_versions.py` & `clarifai-9.3.3/clarifai/listing/module_versions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.2/clarifai/listing/modules.py` & `clarifai-9.3.3/clarifai/listing/modules.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.2/clarifai/modules/css.py` & `clarifai-9.3.3/clarifai/modules/css.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.2/clarifai/modules/pages.py` & `clarifai-9.3.3/clarifai/modules/pages.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.2/clarifai/modules/style.css` & `clarifai-9.3.3/clarifai_utils/modules/style.css`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.2/clarifai/urls/helper.py` & `clarifai-9.3.3/clarifai/urls/helper.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.2/clarifai.egg-info/PKG-INFO` & `clarifai-9.3.3/clarifai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clarifai
-Version: 9.3.2
+Version: 9.3.3
 Summary: Clarifai Python Utilities
 Home-page: https://github.com/Clarifai/clarifai-python-utils
 Author: Clarifai
 Author-email: support@clarifai.com
 License: Apache 2.0
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3
```

### Comparing `clarifai-9.3.2/clarifai_utils/auth/helper.py` & `clarifai-9.3.3/clarifai_utils/auth/helper.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.2/clarifai_utils/client/abc.py` & `clarifai-9.3.3/clarifai_utils/client/abc.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.2/clarifai_utils/client/stub.py` & `clarifai-9.3.3/clarifai_utils/client/stub.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.2/clarifai_utils/data_upload/datasets/base.py` & `clarifai-9.3.3/clarifai_utils/data_upload/datasets/base.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.2/clarifai_utils/data_upload/datasets/features.py` & `clarifai-9.3.3/clarifai_utils/data_upload/datasets/features.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.2/clarifai_utils/data_upload/datasets/image.py` & `clarifai-9.3.3/clarifai_utils/data_upload/datasets/image.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.2/clarifai_utils/data_upload/datasets/text.py` & `clarifai-9.3.3/clarifai_utils/data_upload/datasets/text.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.2/clarifai_utils/data_upload/datasets/zoo/coco_captions.py` & `clarifai-9.3.3/clarifai_utils/data_upload/datasets/zoo/coco_captions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.2/clarifai_utils/data_upload/datasets/zoo/coco_detection.py` & `clarifai-9.3.3/clarifai_utils/data_upload/datasets/zoo/coco_detection.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.2/clarifai_utils/data_upload/datasets/zoo/coco_segmentation.py` & `clarifai-9.3.3/clarifai_utils/data_upload/datasets/zoo/coco_segmentation.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.2/clarifai_utils/data_upload/examples.py` & `clarifai-9.3.3/clarifai_utils/data_upload/examples.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.2/clarifai_utils/data_upload/upload.py` & `clarifai-9.3.3/clarifai_utils/data_upload/upload.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.2/clarifai_utils/listing/concepts.py` & `clarifai-9.3.3/clarifai_utils/listing/concepts.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.2/clarifai_utils/listing/datasets.py` & `clarifai-9.3.3/clarifai_utils/listing/datasets.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.2/clarifai_utils/listing/inputs.py` & `clarifai-9.3.3/clarifai_utils/listing/inputs.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.2/clarifai_utils/listing/installed_module_versions.py` & `clarifai-9.3.3/clarifai_utils/listing/installed_module_versions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.2/clarifai_utils/listing/lister.py` & `clarifai-9.3.3/clarifai_utils/listing/lister.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.2/clarifai_utils/listing/models.py` & `clarifai-9.3.3/clarifai_utils/listing/models.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.2/clarifai_utils/listing/module_versions.py` & `clarifai-9.3.3/clarifai_utils/listing/module_versions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.2/clarifai_utils/listing/modules.py` & `clarifai-9.3.3/clarifai_utils/listing/modules.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.2/clarifai_utils/modules/css.py` & `clarifai-9.3.3/clarifai_utils/modules/css.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.2/clarifai_utils/modules/pages.py` & `clarifai-9.3.3/clarifai_utils/modules/pages.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.2/clarifai_utils/urls/helper.py` & `clarifai-9.3.3/clarifai_utils/urls/helper.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.2/setup.py` & `clarifai-9.3.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
-packages = setuptools.find_packages(include=["clarifai*"])
+packages = setuptools.find_namespace_packages(include=["clarifai*"])
 
 setuptools.setup(
     name="clarifai",
-    version="9.3.2",
+    version="9.3.3",
     author="Clarifai",
     author_email="support@clarifai.com",
     description="Clarifai Python Utilities",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Clarifai/clarifai-python-utils",
     packages=packages,
```

