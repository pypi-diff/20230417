# Comparing `tmp/pcleaner-1.5.2.tar.gz` & `tmp/pcleaner-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcleaner-1.5.2.tar", last modified: Fri Apr 14 12:56:51 2023, max compression
+gzip compressed data, was "pcleaner-1.5.4.tar", last modified: Mon Apr 17 19:15:57 2023, max compression
```

## Comparing `pcleaner-1.5.2.tar` & `pcleaner-1.5.4.tar`

### file list

```diff
@@ -1,53 +1,67 @@
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-14 12:56:51.407667 pcleaner-1.5.2/
--rw-r--r--   0 corbin    (1000) corbin    (1001)    35129 2023-01-07 18:56:55.000000 pcleaner-1.5.2/LICENSE
--rw-r--r--   0 corbin    (1000) corbin    (1001)    11664 2023-04-14 12:56:51.407667 pcleaner-1.5.2/PKG-INFO
--rw-r--r--   0 corbin    (1000) corbin    (1001)    11039 2023-04-12 00:54:25.000000 pcleaner-1.5.2/README.md
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-14 12:56:51.407667 pcleaner-1.5.2/pcleaner/
--rw-r--r--   0 corbin    (1000) corbin    (1001)       47 2023-04-14 12:56:46.000000 pcleaner-1.5.2/pcleaner/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    17222 2023-04-11 21:05:32.000000 pcleaner-1.5.2/pcleaner/analytics.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     8765 2023-04-14 12:31:00.000000 pcleaner-1.5.2/pcleaner/cleaner.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     5672 2023-01-23 03:12:00.000000 pcleaner-1.5.2/pcleaner/cli_utils.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-14 12:56:51.407667 pcleaner-1.5.2/pcleaner/comic_text_detector/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-01-07 23:23:00.000000 pcleaner-1.5.2/pcleaner/comic_text_detector/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    10114 2023-01-07 23:20:26.000000 pcleaner-1.5.2/pcleaner/comic_text_detector/basemodel.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     8492 2023-01-07 23:33:40.000000 pcleaner-1.5.2/pcleaner/comic_text_detector/inference.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-14 12:56:51.407667 pcleaner-1.5.2/pcleaner/comic_text_detector/models/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-12-24 01:25:46.000000 pcleaner-1.5.2/pcleaner/comic_text_detector/models/__init__.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-14 12:56:51.407667 pcleaner-1.5.2/pcleaner/comic_text_detector/models/yolov5/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-12-24 01:25:46.000000 pcleaner-1.5.2/pcleaner/comic_text_detector/models/yolov5/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    10685 2023-01-07 23:24:30.000000 pcleaner-1.5.2/pcleaner/comic_text_detector/models/yolov5/common.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    14770 2023-01-07 23:38:16.000000 pcleaner-1.5.2/pcleaner/comic_text_detector/models/yolov5/yolo.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-14 12:56:51.407667 pcleaner-1.5.2/pcleaner/comic_text_detector/utils/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-01-07 23:23:32.000000 pcleaner-1.5.2/pcleaner/comic_text_detector/utils/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    27905 2023-01-07 23:20:26.000000 pcleaner-1.5.2/pcleaner/comic_text_detector/utils/db_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2136 2023-01-07 23:25:33.000000 pcleaner-1.5.2/pcleaner/comic_text_detector/utils/export.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2582 2023-01-07 23:25:33.000000 pcleaner-1.5.2/pcleaner/comic_text_detector/utils/general.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     7012 2023-01-07 23:20:26.000000 pcleaner-1.5.2/pcleaner/comic_text_detector/utils/imgproc_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1919 2023-04-13 13:46:43.000000 pcleaner-1.5.2/pcleaner/comic_text_detector/utils/io_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     7283 2023-01-07 23:26:33.000000 pcleaner-1.5.2/pcleaner/comic_text_detector/utils/loss.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    20873 2023-01-07 23:27:00.000000 pcleaner-1.5.2/pcleaner/comic_text_detector/utils/textblock.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    13486 2023-01-07 23:27:26.000000 pcleaner-1.5.2/pcleaner/comic_text_detector/utils/textmask.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3181 2023-01-07 23:28:17.000000 pcleaner-1.5.2/pcleaner/comic_text_detector/utils/weight_init.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    10727 2023-01-07 23:28:28.000000 pcleaner-1.5.2/pcleaner/comic_text_detector/utils/yolov5_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    35861 2023-04-13 14:02:44.000000 pcleaner-1.5.2/pcleaner/config.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     6082 2023-04-13 17:19:01.000000 pcleaner-1.5.2/pcleaner/ctd_interface.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     5573 2023-04-14 12:31:20.000000 pcleaner-1.5.2/pcleaner/denoiser.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-14 12:56:51.407667 pcleaner-1.5.2/pcleaner/gui/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-14 12:39:20.000000 pcleaner-1.5.2/pcleaner/gui/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)      767 2023-04-13 18:30:59.000000 pcleaner-1.5.2/pcleaner/helpers.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    23338 2023-04-13 18:46:48.000000 pcleaner-1.5.2/pcleaner/image_ops.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    24649 2023-04-14 12:54:02.000000 pcleaner-1.5.2/pcleaner/main.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     4845 2023-04-14 12:51:27.000000 pcleaner-1.5.2/pcleaner/model_downloader.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     8183 2023-04-13 18:07:02.000000 pcleaner-1.5.2/pcleaner/pre_processor.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     7546 2023-01-23 03:12:00.000000 pcleaner-1.5.2/pcleaner/profile_cli.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    13299 2023-04-13 19:11:27.000000 pcleaner-1.5.2/pcleaner/structures.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-14 12:56:51.407667 pcleaner-1.5.2/pcleaner.egg-info/
--rw-r--r--   0 corbin    (1000) corbin    (1001)    11664 2023-04-14 12:56:51.000000 pcleaner-1.5.2/pcleaner.egg-info/PKG-INFO
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1437 2023-04-14 12:56:51.000000 pcleaner-1.5.2/pcleaner.egg-info/SOURCES.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)        1 2023-04-14 12:56:51.000000 pcleaner-1.5.2/pcleaner.egg-info/dependency_links.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)       48 2023-04-14 12:56:51.000000 pcleaner-1.5.2/pcleaner.egg-info/entry_points.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)      171 2023-04-14 12:56:51.000000 pcleaner-1.5.2/pcleaner.egg-info/requires.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)        9 2023-04-14 12:56:51.000000 pcleaner-1.5.2/pcleaner.egg-info/top_level.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)      122 2023-01-23 03:12:00.000000 pcleaner-1.5.2/pyproject.toml
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1039 2023-04-14 12:56:51.407667 pcleaner-1.5.2/setup.cfg
--rw-r--r--   0 corbin    (1000) corbin    (1001)       38 2023-01-07 18:56:55.000000 pcleaner-1.5.2/setup.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-17 19:15:57.554623 pcleaner-1.5.4/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    35129 2023-01-07 18:56:55.000000 pcleaner-1.5.4/LICENSE
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    11664 2023-04-17 19:15:57.554623 pcleaner-1.5.4/PKG-INFO
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    11039 2023-04-12 00:54:25.000000 pcleaner-1.5.4/README.md
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-17 19:15:57.547957 pcleaner-1.5.4/pcleaner/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)       82 2023-04-17 18:13:47.000000 pcleaner-1.5.4/pcleaner/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    17232 2023-04-17 18:10:07.000000 pcleaner-1.5.4/pcleaner/analytics.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     8765 2023-04-14 12:31:00.000000 pcleaner-1.5.4/pcleaner/cleaner.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     5841 2023-04-14 16:52:21.000000 pcleaner-1.5.4/pcleaner/cli_utils.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-17 19:15:57.551290 pcleaner-1.5.4/pcleaner/comic_text_detector/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-01-07 23:23:00.000000 pcleaner-1.5.4/pcleaner/comic_text_detector/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    10114 2023-01-07 23:20:26.000000 pcleaner-1.5.4/pcleaner/comic_text_detector/basemodel.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     8492 2023-01-07 23:33:40.000000 pcleaner-1.5.4/pcleaner/comic_text_detector/inference.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-17 19:15:57.551290 pcleaner-1.5.4/pcleaner/comic_text_detector/models/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-12-24 01:25:46.000000 pcleaner-1.5.4/pcleaner/comic_text_detector/models/__init__.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-17 19:15:57.551290 pcleaner-1.5.4/pcleaner/comic_text_detector/models/yolov5/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-12-24 01:25:46.000000 pcleaner-1.5.4/pcleaner/comic_text_detector/models/yolov5/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    10685 2023-01-07 23:24:30.000000 pcleaner-1.5.4/pcleaner/comic_text_detector/models/yolov5/common.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    14770 2023-01-07 23:38:16.000000 pcleaner-1.5.4/pcleaner/comic_text_detector/models/yolov5/yolo.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-17 19:15:57.551290 pcleaner-1.5.4/pcleaner/comic_text_detector/utils/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-01-07 23:23:32.000000 pcleaner-1.5.4/pcleaner/comic_text_detector/utils/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    27905 2023-01-07 23:20:26.000000 pcleaner-1.5.4/pcleaner/comic_text_detector/utils/db_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2136 2023-01-07 23:25:33.000000 pcleaner-1.5.4/pcleaner/comic_text_detector/utils/export.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2582 2023-01-07 23:25:33.000000 pcleaner-1.5.4/pcleaner/comic_text_detector/utils/general.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     7012 2023-01-07 23:20:26.000000 pcleaner-1.5.4/pcleaner/comic_text_detector/utils/imgproc_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1919 2023-04-13 13:46:43.000000 pcleaner-1.5.4/pcleaner/comic_text_detector/utils/io_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     7283 2023-01-07 23:26:33.000000 pcleaner-1.5.4/pcleaner/comic_text_detector/utils/loss.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    20873 2023-01-07 23:27:00.000000 pcleaner-1.5.4/pcleaner/comic_text_detector/utils/textblock.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    13486 2023-01-07 23:27:26.000000 pcleaner-1.5.4/pcleaner/comic_text_detector/utils/textmask.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3181 2023-01-07 23:28:17.000000 pcleaner-1.5.4/pcleaner/comic_text_detector/utils/weight_init.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    10727 2023-01-07 23:28:28.000000 pcleaner-1.5.4/pcleaner/comic_text_detector/utils/yolov5_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    35861 2023-04-13 14:02:44.000000 pcleaner-1.5.4/pcleaner/config.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     6056 2023-04-17 18:08:37.000000 pcleaner-1.5.4/pcleaner/ctd_interface.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     5573 2023-04-14 12:31:20.000000 pcleaner-1.5.4/pcleaner/denoiser.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-17 19:15:57.554623 pcleaner-1.5.4/pcleaner/gui/
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-17 19:15:57.554623 pcleaner-1.5.4/pcleaner/gui/CustomQ/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3206 2022-08-27 14:37:25.000000 pcleaner-1.5.4/pcleaner/gui/CustomQ/CTableWidget.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-17 01:59:57.000000 pcleaner-1.5.4/pcleaner/gui/CustomQ/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-14 12:39:20.000000 pcleaner-1.5.4/pcleaner/gui/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    21094 2023-04-17 02:04:01.000000 pcleaner-1.5.4/pcleaner/gui/file_table.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1904 2023-04-17 01:26:57.000000 pcleaner-1.5.4/pcleaner/gui/launcher.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    34194 2023-04-17 02:09:36.000000 pcleaner-1.5.4/pcleaner/gui/mainwindow_driver.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-17 19:15:57.554623 pcleaner-1.5.4/pcleaner/gui/rc_generated_files/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-17 01:25:41.000000 pcleaner-1.5.4/pcleaner/gui/rc_generated_files/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    81975 2023-04-17 01:43:12.000000 pcleaner-1.5.4/pcleaner/gui/rc_generated_files/icons_rc.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-17 19:15:57.554623 pcleaner-1.5.4/pcleaner/gui/ui_generated_files/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-17 00:09:43.000000 pcleaner-1.5.4/pcleaner/gui/ui_generated_files/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     6310 2023-04-17 00:10:07.000000 pcleaner-1.5.4/pcleaner/gui/ui_generated_files/ui_ImageDetails.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    29139 2023-04-17 02:04:43.000000 pcleaner-1.5.4/pcleaner/gui/ui_generated_files/ui_Mainwindow.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3233 2023-04-17 16:45:08.000000 pcleaner-1.5.4/pcleaner/gui/worker_thread.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1321 2023-04-17 02:10:39.000000 pcleaner-1.5.4/pcleaner/helpers.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    23338 2023-04-13 18:46:48.000000 pcleaner-1.5.4/pcleaner/image_ops.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    26041 2023-04-17 18:36:40.000000 pcleaner-1.5.4/pcleaner/main.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     4845 2023-04-14 12:51:27.000000 pcleaner-1.5.4/pcleaner/model_downloader.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     8183 2023-04-13 18:07:02.000000 pcleaner-1.5.4/pcleaner/pre_processor.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     7546 2023-01-23 03:12:00.000000 pcleaner-1.5.4/pcleaner/profile_cli.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    13299 2023-04-13 19:11:27.000000 pcleaner-1.5.4/pcleaner/structures.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-17 19:15:57.551290 pcleaner-1.5.4/pcleaner.egg-info/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    11664 2023-04-17 19:15:57.000000 pcleaner-1.5.4/pcleaner.egg-info/PKG-INFO
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1855 2023-04-17 19:15:57.000000 pcleaner-1.5.4/pcleaner.egg-info/SOURCES.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        1 2023-04-17 19:15:57.000000 pcleaner-1.5.4/pcleaner.egg-info/dependency_links.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)       48 2023-04-17 19:15:57.000000 pcleaner-1.5.4/pcleaner.egg-info/entry_points.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      188 2023-04-17 19:15:57.000000 pcleaner-1.5.4/pcleaner.egg-info/requires.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        9 2023-04-17 19:15:57.000000 pcleaner-1.5.4/pcleaner.egg-info/top_level.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      122 2023-01-23 03:12:00.000000 pcleaner-1.5.4/pyproject.toml
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1058 2023-04-17 19:15:57.554623 pcleaner-1.5.4/setup.cfg
+-rw-r--r--   0 corbin    (1000) corbin    (1001)       38 2023-01-07 18:56:55.000000 pcleaner-1.5.4/setup.py
```

### Comparing `pcleaner-1.5.2/LICENSE` & `pcleaner-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.2/PKG-INFO` & `pcleaner-1.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcleaner
-Version: 1.5.2
+Version: 1.5.4
 Summary: An AI-powered tool to clean manga panels.
 Home-page: https://github.com/VoxelCubes/PanelCleaner
 Keywords: image processing,cleaning,text removal,manga,ai,machine learning
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `pcleaner-1.5.2/README.md` & `pcleaner-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.2/pcleaner/analytics.py` & `pcleaner-1.5.4/pcleaner/analytics.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,15 +211,15 @@
         if masks_succeeded
         else "N/A"
     )
     success_rate = f"{masks_succeeded / total_boxes:.0%}" if total_boxes else "N/A"
     perfect_mask_rate = f"{perfect_masks / masks_succeeded:.0%}" if masks_succeeded else "N/A"
     masks_failed = total_boxes - masks_succeeded
 
-    highest_mask_index = max(analytics[2] for analytics in analytics if analytics[1])
+    highest_mask_index = max((analytic[2] for analytic in analytics if analytic[1]), default=0)
     # Count the number of times each mask index was used.
     mask_usages_by_index = [0] * (highest_mask_index + 1)
     # Count the number of times each mask was perfect.
     perfect_mask_usages_by_index = [0] * (highest_mask_index + 1)
     for analytic in analytics:
         if analytic[1]:
             mask_usages_by_index[analytic[2]] += 1
```

### Comparing `pcleaner-1.5.2/pcleaner/cleaner.py` & `pcleaner-1.5.4/pcleaner/cleaner.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.2/pcleaner/cli_utils.py` & `pcleaner-1.5.4/pcleaner/cli_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,22 @@
     else:  # ???
         raise NotImplementedError("Your OS is currently not supported.")
 
     path.mkdir(parents=True, exist_ok=True)
     return path
 
 
+def get_log_path() -> Path:
+    """
+    Get the path to the log file.
+    Use the cache directory for this.
+    """
+    return get_cache_path() / f"{__program__}.log"
+
+
 def open_file_with_editor(path: Path, configured_opener: str | None) -> None:
     """
     Open the given file with the given editor.
     If no editor is given, use the default editor for the current OS.
 
     :param path: The path to the file to open.
     :param configured_opener: The configured editor to use.
```

### Comparing `pcleaner-1.5.2/pcleaner/comic_text_detector/basemodel.py` & `pcleaner-1.5.4/pcleaner/comic_text_detector/basemodel.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.2/pcleaner/comic_text_detector/inference.py` & `pcleaner-1.5.4/pcleaner/comic_text_detector/inference.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.2/pcleaner/comic_text_detector/models/yolov5/common.py` & `pcleaner-1.5.4/pcleaner/comic_text_detector/models/yolov5/common.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.2/pcleaner/comic_text_detector/models/yolov5/yolo.py` & `pcleaner-1.5.4/pcleaner/comic_text_detector/models/yolov5/yolo.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.2/pcleaner/comic_text_detector/utils/db_utils.py` & `pcleaner-1.5.4/pcleaner/comic_text_detector/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.2/pcleaner/comic_text_detector/utils/export.py` & `pcleaner-1.5.4/pcleaner/comic_text_detector/utils/export.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.2/pcleaner/comic_text_detector/utils/general.py` & `pcleaner-1.5.4/pcleaner/comic_text_detector/utils/general.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.2/pcleaner/comic_text_detector/utils/imgproc_utils.py` & `pcleaner-1.5.4/pcleaner/comic_text_detector/utils/imgproc_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.2/pcleaner/comic_text_detector/utils/io_utils.py` & `pcleaner-1.5.4/pcleaner/comic_text_detector/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.2/pcleaner/comic_text_detector/utils/loss.py` & `pcleaner-1.5.4/pcleaner/comic_text_detector/utils/loss.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.2/pcleaner/comic_text_detector/utils/textblock.py` & `pcleaner-1.5.4/pcleaner/comic_text_detector/utils/textblock.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.2/pcleaner/comic_text_detector/utils/textmask.py` & `pcleaner-1.5.4/pcleaner/comic_text_detector/utils/textmask.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.2/pcleaner/comic_text_detector/utils/weight_init.py` & `pcleaner-1.5.4/pcleaner/comic_text_detector/utils/weight_init.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.2/pcleaner/comic_text_detector/utils/yolov5_utils.py` & `pcleaner-1.5.4/pcleaner/comic_text_detector/utils/yolov5_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.2/pcleaner/config.py` & `pcleaner-1.5.4/pcleaner/config.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.2/pcleaner/ctd_interface.py` & `pcleaner-1.5.4/pcleaner/ctd_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,16 +158,15 @@
     Then return an array of the image.
 
     :param path: Image path
     :param scale: Scale factor
     :return: Image array
     """
 
-    read_type = cv2.IMREAD_COLOR
-    img = cv2.imdecode(np.fromfile(str(path), dtype=np.uint8), read_type)
+    img = cv2.imdecode(np.fromfile(str(path), dtype=np.uint8), cv2.IMREAD_COLOR)
 
     if scale != 1.0:
         height, width, channels = img.shape
         new_width = int(width * scale)
         new_height = int(height * scale)
         img = cv2.resize(img, (new_width, new_height))
```

### Comparing `pcleaner-1.5.2/pcleaner/denoiser.py` & `pcleaner-1.5.4/pcleaner/denoiser.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.2/pcleaner/image_ops.py` & `pcleaner-1.5.4/pcleaner/image_ops.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.2/pcleaner/main.py` & `pcleaner-1.5.4/pcleaner/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
         [--save-only-mask | --save-only-cleaned | --save-only-text]
         [--separate-noise-mask] [--hide-analytics] [--extract-text]
         [--skip-text-detection] [--skip-pre-processing] [--skip-cleaning] [--skip-denoising]
         [--keep-cache] [--cache-masks] [--debug]
     pcleaner profile (list | new <profile_name> [<profile_path>] | add <profile_name> <profile_path> |
         open <profile_name> | delete <profile_name> | set-default <profile_name> | repair <profile_name> |
         purge-missing) [--debug]
+    pcleaner gui [<image_path> ...] [--debug]
     pcleaner ocr [<image_path> ...] [--output-path=<output_path>] [--debug]
     pcleaner config (show | open)
     pcleaner cache clear (all | models | cleaner)
     pcleaner load models [--cuda | --cpu | --both] [--force]
     pcleaner --help
     pcleaner --version
 
@@ -26,14 +27,15 @@
                      Provide the name to save it under and the path the file is located at.
         open         Open a saved profile in the default editor (unless specified in the config).
         delete       Delete a saved profile.
         set-default  Set a profile as the default profile. This way it will be loaded automatically.
         repair       Repair a profile. This will remove any invalid entries and save the profile.
                      Warning: Changes to the comments won't be preserved, only settings.
         purge-missing  Remove all profiles that link to a file that doesn't exist.
+    gui              Open the GUI. Any number of images and directories can be given to be loaded on startup.
     ocr              Run only the OCR on the given image(s). Any number of images and directories can be given.
                      The output will be saved in a single text file for the whole batch.
     config           View or edit the config file. This stores setting independent of profiles.
         show         Show the current configuration. This doesn't show the current profile.
         open         Open the config file in the default editor (unless specified in the config).
     cache clear      Clear the cache. This is where the program stores downloaded models and other files.
         all          Clear all cache files.
@@ -77,28 +79,28 @@
     --both                          Load both the torch and open cv2 models.
     --force                         Force the models to be downloaded, even if they already exist.
     -d --debug                      Show debug information.
     -v --version                    Show the version and exit.
     -h --help                       Show this screen.
 
 Examples:
-    pcleaner myfolder               This will clean all images in the folder, saving the output to
+    pcleaner clean myfolder               This will clean all images in the folder, saving the output to
                                     a folder inside myfolder called cleaned.
 
-    pcleaner myfolder -o myoutput   This will clean all images in the folder, saving the output to
+    pcleaner clean myfolder -o myoutput   This will clean all images in the folder, saving the output to
                                     a folder called myoutput, placed inside myfolder.
 
-    pcleaner myfolder myfolder2 mypng myjpg  This will clean all images in the folders and all given files,
+    pcleaner clean myfolder myfolder2 mypng myjpg  This will clean all images in the folders and all given files,
                                     saving the outputs to folders called cleaned, placed inside of these folders
                                     or in the parent directory of the input files, respectively.
 
-    pcleaner myfolder -p myprofile  This will clean all the images, but use the settings from the profile
+    pcleaner clean myfolder -p myprofile  This will clean all the images, but use the settings from the profile
                                     called myprofile.
 
-    pcleaner myfolder -p myprofile2 -TP  This will skip the text detection and pre-processing steps,
+    pcleaner clean myfolder -p myprofile2 -TP  This will skip the text detection and pre-processing steps,
                                     but still run the cleaning process using the settings from the profile
                                     called myprofile2. This can be useful when you tweaked settings only
                                     related to the cleaning process. You can save time skipping the first one
                                     or two steps, since the results are saved in the cache directory (unless
                                     you choose to delete them).
 
 """
@@ -112,26 +114,28 @@
 
 from manga_ocr import MangaOcr
 from docopt import magic_docopt
 from logzero import logger, loglevel, DEBUG, INFO
 from tqdm import tqdm
 from natsort import natsorted
 import torch
+import tifffile
 
 from pcleaner import __version__
 import pcleaner.cleaner as cl
 import pcleaner.config as cfg
 import pcleaner.cli_utils as cli
 import pcleaner.pre_processor as pp
 import pcleaner.analytics as an
 import pcleaner.structures as st
 import pcleaner.profile_cli as pc
 import pcleaner.denoiser as dn
 import pcleaner.model_downloader as md
 import pcleaner.helpers as hp
+import pcleaner.gui.launcher as gui
 
 # Supported image suffixes.
 IMG_EXT = [".jpeg", ".jpg", ".png", ".bmp", ".tiff", ".tif", ".jp2", ".dib", ".webp", ".ppm"]
 
 # Allow loading of large images.
 Image.MAX_IMAGE_PIXELS = 2**32
 
@@ -173,18 +177,21 @@
             pc.set_default_profile(config, args.profile_name)
         elif args.repair:
             pc.repair_profile(config, args.profile_name)
         elif args.purge_missing:
             pc.purge_missing_profiles(config)
         else:
             raise ValueError("Invalid profile subcommand.")
+    elif args.gui:
+        gui.launch(args.image_path)
 
     elif args.ocr:
         config = cfg.load_config()
-        run_ocr(config, args.image_path, args.output_path)
+        image_paths = discover_all_images(args.image_path)
+        run_ocr(config, image_paths, args.output_path)
 
     elif args.cache and args.clear:
         config = cfg.load_config()
         clear_cache(config, args.all, args.models, args.cleaner)
 
     elif args.load and args.models:
         config = cfg.load_config()
@@ -430,41 +437,48 @@
     expanded to all bubbles.
 
     :param config: The config to use.
     :param image_paths: The images to run OCR on.
     :param output_path: The path to output the results to.
     """
     cache_dir = config.get_cleaner_cache_dir()
+    profile = config.current_profile
     logger.debug(f"Cache directory: {cache_dir}")
 
     # Delete the cache directory if not explicitly keeping it.
     if len(list(cache_dir.glob("*"))) > 0:
         cli.empty_cache_dir(cache_dir)
     # Get the model file, downloading it if necessary.
     cuda = torch.cuda.is_available()
     model_path = config.get_model_path(cuda)
 
     print("Running text detection AI model...")
-    pp.generate_mask_data(image_paths, model_path=model_path, output_dir=cache_dir)
+    pp.generate_mask_data(
+        image_paths,
+        config_general=profile.general,
+        config_detector=profile.text_detector,
+        model_path=model_path,
+        output_dir=cache_dir,
+    )
 
     print("\n")
 
     # Flush it so it shows up before the progress bar.
     print("Running box data Pre-Processor...", flush=True)
     # Make sure it actually flushes at all costs = wait 100 ms.
     # (It takes several seconds to load the ocr model, so this is fine.)
     time.sleep(0.1)
 
     # Modify the profile to OCR all boxes.
     # Make sure OCR is enabled.
     config.current_profile.pre_processor.ocr_enabled = True
     # Make sure the max size is infinite, so no boxes are skipped in the OCR process.
-    config.current_profile.pre_processor.ocr_max_size = float("inf")
+    config.current_profile.pre_processor.ocr_max_size = 10**10
     # Make sure the sus box min size is infinite, so all boxes with "unknown" language are skipped.
-    config.current_profile.pre_processor.suspicious_box_min_size = float("inf")
+    config.current_profile.pre_processor.suspicious_box_min_size = 10**10
     # Set the OCR blacklist pattern to match everything, so all text gets reported in the analytics.
     config.current_profile.pre_processor.ocr_blacklist_pattern = ".*"
 
     mocr = MangaOcr()
     ocr_analytics = []
     for json_file_path in tqdm(list(cache_dir.glob("*.json"))):
         ocr_analytic = pp.prep_json_file(
@@ -566,23 +580,49 @@
             img_list.append(img_path)
         else:
             raise FileNotFoundError(f"Image path {img_path} does not exist.")
 
     # Ensure all paths are absolute.
     img_list = [path.resolve() for path in img_list]
 
+    # Filter out 5 channel TIFFs, as they are not supported.
+    img_list = [path for path in img_list if not is_5_channel_tiff(path)]
+
     return img_list
 
 
 def find_all_images_shallow(img_dir: Path) -> list[Path]:
     image_list: list[Path] = []
     for file_path in img_dir.glob("*"):
         file_suffix = file_path.suffix
         if file_suffix.lower() not in IMG_EXT:
             continue
         else:
             image_list.append(file_path)
     return image_list
 
 
+def is_5_channel_tiff(path: Path) -> bool:
+    """
+    Returns True if the given file is a TIFF image with a 5.1 channel, False otherwise.
+    """
+    # Check suffix first.
+    if path.suffix not in [".tif", ".tiff"]:
+        return False
+    # Try opening the file as a TIFF image
+    with tifffile.TiffFile(path) as tif:
+        logger.debug("Tiff data:\n" + str(tif.pages[0].tags))
+        # Check if the TIFF image has 5 channels.
+        try:
+            if tif.pages[0].tags["SamplesPerPixel"].value == 5:
+                logger.warning(
+                    f"Found a 5 channel TIFF image: {path}. These are not supported, the image will be skipped."
+                )
+                return True
+        except KeyError:
+            pass
+
+    return False
+
+
 if __name__ == "__main__":
     main()
```

### Comparing `pcleaner-1.5.2/pcleaner/model_downloader.py` & `pcleaner-1.5.4/pcleaner/model_downloader.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.2/pcleaner/pre_processor.py` & `pcleaner-1.5.4/pcleaner/pre_processor.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.2/pcleaner/profile_cli.py` & `pcleaner-1.5.4/pcleaner/profile_cli.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.2/pcleaner/structures.py` & `pcleaner-1.5.4/pcleaner/structures.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.2/pcleaner.egg-info/PKG-INFO` & `pcleaner-1.5.4/pcleaner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcleaner
-Version: 1.5.2
+Version: 1.5.4
 Summary: An AI-powered tool to clean manga panels.
 Home-page: https://github.com/VoxelCubes/PanelCleaner
 Keywords: image processing,cleaning,text removal,manga,ai,machine learning
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `pcleaner-1.5.2/setup.cfg` & `pcleaner-1.5.4/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -31,14 +31,16 @@
 	docopt-ng
 	ConfigUpdater
 	logzero
 	prettytable
 	colorama
 	requests
 	xdg
+	tifffile
+	PySide6
 python_requires = >=3.10
 packages = find:
 
 [options.packages.find]
 exclude = tests*
 
 [options.entry_points]
```

