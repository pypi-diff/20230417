# Comparing `tmp/RobertCommonBasic-0.1.34.tar.gz` & `tmp/RobertCommonBasic-0.1.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RobertCommonBasic-0.1.34.tar", last modified: Thu Mar 16 09:03:35 2023, max compression
+gzip compressed data, was "RobertCommonBasic-0.1.35.tar", last modified: Mon Apr 17 08:26:15 2023, max compression
```

## Comparing `RobertCommonBasic-0.1.34.tar` & `RobertCommonBasic-0.1.35.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxrwxrwx   0        0        0        0 2023-03-16 09:03:35.907838 RobertCommonBasic-0.1.34/
--rw-rw-rw-   0        0        0     1067 2021-08-09 02:56:17.000000 RobertCommonBasic-0.1.34/LICENSE
--rw-rw-rw-   0        0        0       44 2021-08-09 07:19:42.000000 RobertCommonBasic-0.1.34/MANIFEST.in
--rw-rw-rw-   0        0        0     1739 2023-03-16 09:03:35.906839 RobertCommonBasic-0.1.34/PKG-INFO
--rw-rw-rw-   0        0        0     1057 2022-01-13 05:29:18.000000 RobertCommonBasic-0.1.34/README.md
-drwxrwxrwx   0        0        0        0 2023-03-16 09:03:35.828393 RobertCommonBasic-0.1.34/RobertCommonBasic.egg-info/
--rw-rw-rw-   0        0        0     1739 2023-03-16 09:03:35.000000 RobertCommonBasic-0.1.34/RobertCommonBasic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4427 2023-03-16 09:03:35.000000 RobertCommonBasic-0.1.34/RobertCommonBasic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-16 09:03:35.000000 RobertCommonBasic-0.1.34/RobertCommonBasic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      169 2023-03-16 09:03:35.000000 RobertCommonBasic-0.1.34/RobertCommonBasic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-03-16 09:03:35.000000 RobertCommonBasic-0.1.34/RobertCommonBasic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      187 2023-02-09 03:19:57.000000 RobertCommonBasic-0.1.34/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-03-16 09:03:35.829392 RobertCommonBasic-0.1.34/robertcommonbasic/
--rw-rw-rw-   0        0        0        2 2021-08-09 03:27:49.000000 RobertCommonBasic-0.1.34/robertcommonbasic/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-16 09:03:35.829392 RobertCommonBasic-0.1.34/robertcommonbasic/basic/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-16 09:03:35.830388 RobertCommonBasic-0.1.34/robertcommonbasic/basic/base/
--rw-rw-rw-   0        0        0        0 2023-01-04 02:39:20.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/base/__init__.py
--rw-rw-rw-   0        0        0      471 2023-01-04 02:45:25.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/base/constant.py
-drwxrwxrwx   0        0        0        0 2023-03-16 09:03:35.831385 RobertCommonBasic-0.1.34/robertcommonbasic/basic/cache/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/cache/__init__.py
--rw-rw-rw-   0        0        0      667 2022-11-14 07:41:26.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/cache/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-16 09:03:35.832382 RobertCommonBasic-0.1.34/robertcommonbasic/basic/cls/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/cls/__init__.py
--rw-rw-rw-   0        0        0    11450 2022-12-28 03:39:32.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/cls/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-16 09:03:35.840021 RobertCommonBasic-0.1.34/robertcommonbasic/basic/data/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/data/__init__.py
--rw-rw-rw-   0        0        0    13611 2023-01-31 14:01:59.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/data/conversion.py
--rw-rw-rw-   0        0        0     4537 2022-11-14 07:54:50.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/data/crc16.py
--rw-rw-rw-   0        0        0     2229 2022-11-14 03:21:43.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/data/csv.py
--rw-rw-rw-   0        0        0    39297 2022-11-14 09:43:00.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/data/datatuple.py
--rw-rw-rw-   0        0        0     8304 2022-11-14 09:43:00.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/data/frame.py
--rw-rw-rw-   0        0        0     1097 2022-11-14 09:48:07.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/data/nametuple.py
--rw-rw-rw-   0        0        0       62 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/data/type.py
--rw-rw-rw-   0        0        0     5064 2022-11-14 09:43:00.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/data/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-16 09:03:35.843013 RobertCommonBasic-0.1.34/robertcommonbasic/basic/decorator/
--rw-rw-rw-   0        0        0        0 2021-12-08 01:56:09.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/decorator/__init__.py
--rw-rw-rw-   0        0        0     1250 2022-12-05 08:07:43.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/decorator/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-16 09:03:35.844010 RobertCommonBasic-0.1.34/robertcommonbasic/basic/dt/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/dt/__init__.py
--rw-rw-rw-   0        0        0     4474 2022-12-28 02:51:52.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/dt/schedule.py
--rw-rw-rw-   0        0        0     9775 2023-03-09 06:28:35.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/dt/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-16 09:03:35.848882 RobertCommonBasic-0.1.34/robertcommonbasic/basic/encrypt/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/encrypt/__init__.py
--rw-rw-rw-   0        0        0      583 2022-11-14 07:14:55.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/encrypt/aes.py
--rw-rw-rw-   0        0        0     3856 2022-11-14 07:41:26.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/encrypt/dsa.py
--rw-rw-rw-   0        0        0      716 2023-03-09 07:09:06.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/encrypt/hash.py
--rw-rw-rw-   0        0        0      338 2022-11-14 07:14:55.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/encrypt/md5.py
--rw-rw-rw-   0        0        0     2661 2022-11-14 07:25:08.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/encrypt/rsa.py
-drwxrwxrwx   0        0        0        0 2023-03-16 09:03:35.850253 RobertCommonBasic-0.1.34/robertcommonbasic/basic/error/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/error/__init__.py
--rw-rw-rw-   0        0        0     2354 2022-11-14 09:50:44.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/error/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-16 09:03:35.852252 RobertCommonBasic-0.1.34/robertcommonbasic/basic/exector/
--rw-rw-rw-   0        0        0        0 2022-08-31 08:25:14.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/exector/__init__.py
--rw-rw-rw-   0        0        0     3641 2022-11-14 09:50:44.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/exector/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-16 09:03:35.856275 RobertCommonBasic-0.1.34/robertcommonbasic/basic/file/
--rw-rw-rw-   0        0        0        0 2022-11-18 02:39:00.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/file/__init__.py
--rw-rw-rw-   0        0        0     3113 2023-02-21 06:19:45.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/file/csv.py
--rw-rw-rw-   0        0        0     1328 2022-11-18 03:22:13.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/file/ini.py
--rw-rw-rw-   0        0        0     1035 2022-11-18 06:23:07.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/file/log.py
--rw-rw-rw-   0        0        0     3157 2022-11-24 03:18:18.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/file/xml.py
--rw-rw-rw-   0        0        0      339 2022-11-18 06:47:46.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/file/yaml.py
--rw-rw-rw-   0        0        0     3039 2023-03-08 07:31:52.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/file/zip.py
-drwxrwxrwx   0        0        0        0 2023-03-16 09:03:35.858351 RobertCommonBasic-0.1.34/robertcommonbasic/basic/log/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/log/__init__.py
--rw-rw-rw-   0        0        0     4874 2023-03-09 06:33:05.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/log/utils.py
--rw-rw-rw-   0        0        0     1366 2022-12-05 08:20:54.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/log/watch.py
-drwxrwxrwx   0        0        0        0 2023-03-16 09:03:35.859347 RobertCommonBasic-0.1.34/robertcommonbasic/basic/net/
--rw-rw-rw-   0        0        0        0 2022-06-29 12:44:36.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/net/__init__.py
--rw-rw-rw-   0        0        0     5370 2022-11-14 09:59:29.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/net/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-16 09:03:35.862338 RobertCommonBasic-0.1.34/robertcommonbasic/basic/os/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/os/__init__.py
--rw-rw-rw-   0        0        0      228 2022-12-14 09:03:01.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/os/cmd.py
--rw-rw-rw-   0        0        0      400 2022-06-29 09:34:23.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/os/env.py
--rw-rw-rw-   0        0        0     3446 2023-03-16 09:00:41.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/os/file.py
--rw-rw-rw-   0        0        0      533 2023-02-06 07:51:13.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/os/path.py
-drwxrwxrwx   0        0        0        0 2023-03-16 09:03:35.863336 RobertCommonBasic-0.1.34/robertcommonbasic/basic/process/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/process/__init__.py
--rw-rw-rw-   0        0        0     8845 2022-12-14 08:53:18.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/process/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-16 09:03:35.866468 RobertCommonBasic-0.1.34/robertcommonbasic/basic/profile/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/profile/__init__.py
--rw-rw-rw-   0        0        0     1264 2022-11-18 02:27:39.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/profile/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-16 09:03:35.869892 RobertCommonBasic-0.1.34/robertcommonbasic/basic/re/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/re/__init__.py
--rw-rw-rw-   0        0        0     1868 2023-02-09 02:47:33.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/re/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-16 09:03:35.872886 RobertCommonBasic-0.1.34/robertcommonbasic/basic/safetext/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/safetext/__init__.py
--rw-rw-rw-   0        0        0       91 2023-02-03 07:26:22.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/safetext/converter.py
--rw-rw-rw-   0        0        0      377 2022-11-18 02:33:07.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/safetext/funcs.py
-drwxrwxrwx   0        0        0        0 2023-03-16 09:03:35.873883 RobertCommonBasic-0.1.34/robertcommonbasic/basic/sugar/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/sugar/__init__.py
--rw-rw-rw-   0        0        0      377 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/sugar/funcs.py
-drwxrwxrwx   0        0        0        0 2023-03-16 09:03:35.875779 RobertCommonBasic-0.1.34/robertcommonbasic/basic/validation/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/validation/__init__.py
--rw-rw-rw-   0        0        0    36389 2023-02-21 08:51:30.000000 RobertCommonBasic-0.1.34/robertcommonbasic/basic/validation/input.py
-drwxrwxrwx   0        0        0        0 2023-03-16 09:03:35.877120 RobertCommonBasic-0.1.34/robertcommonbasic/tests/
--rw-rw-rw-   0        0        0        0 2021-07-27 06:06:01.000000 RobertCommonBasic-0.1.34/robertcommonbasic/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-16 09:03:35.877120 RobertCommonBasic-0.1.34/robertcommonbasic/tests/test_basic/
--rw-rw-rw-   0        0        0        0 2021-07-27 06:49:18.000000 RobertCommonBasic-0.1.34/robertcommonbasic/tests/test_basic/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-16 09:03:35.878222 RobertCommonBasic-0.1.34/robertcommonbasic/tests/test_basic/test_cls/
--rw-rw-rw-   0        0        0        0 2022-04-22 02:07:10.000000 RobertCommonBasic-0.1.34/robertcommonbasic/tests/test_basic/test_cls/__init__.py
--rw-rw-rw-   0        0        0     1291 2023-03-02 14:03:08.000000 RobertCommonBasic-0.1.34/robertcommonbasic/tests/test_basic/test_cls/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-03-16 09:03:35.882672 RobertCommonBasic-0.1.34/robertcommonbasic/tests/test_basic/test_data/
--rw-rw-rw-   0        0        0        0 2022-01-19 07:38:20.000000 RobertCommonBasic-0.1.34/robertcommonbasic/tests/test_basic/test_data/__init__.py
--rw-rw-rw-   0        0        0      729 2022-06-23 09:21:24.000000 RobertCommonBasic-0.1.34/robertcommonbasic/tests/test_basic/test_data/test_conversion.py
--rw-rw-rw-   0        0        0     5920 2022-04-21 06:58:53.000000 RobertCommonBasic-0.1.34/robertcommonbasic/tests/test_basic/test_data/test_datatupple.py
--rw-rw-rw-   0        0        0     2456 2022-01-27 05:56:15.000000 RobertCommonBasic-0.1.34/robertcommonbasic/tests/test_basic/test_data/test_frame.py
--rw-rw-rw-   0        0        0     3273 2023-01-31 14:11:07.000000 RobertCommonBasic-0.1.34/robertcommonbasic/tests/test_basic/test_data/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-03-16 09:03:35.884052 RobertCommonBasic-0.1.34/robertcommonbasic/tests/test_basic/test_dt/
--rw-rw-rw-   0        0        0        0 2022-03-08 05:59:28.000000 RobertCommonBasic-0.1.34/robertcommonbasic/tests/test_basic/test_dt/__init__.py
--rw-rw-rw-   0        0        0     2169 2023-02-20 02:34:17.000000 RobertCommonBasic-0.1.34/robertcommonbasic/tests/test_basic/test_dt/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-03-16 09:03:35.889633 RobertCommonBasic-0.1.34/robertcommonbasic/tests/test_basic/test_encrypt/
--rw-rw-rw-   0        0        0        0 2021-07-30 08:42:35.000000 RobertCommonBasic-0.1.34/robertcommonbasic/tests/test_basic/test_encrypt/__init__.py
--rw-rw-rw-   0        0        0    32599 2022-07-03 01:41:08.000000 RobertCommonBasic-0.1.34/robertcommonbasic/tests/test_basic/test_encrypt/test_dsa.py
--rw-rw-rw-   0        0        0      270 2022-07-03 01:04:51.000000 RobertCommonBasic-0.1.34/robertcommonbasic/tests/test_basic/test_encrypt/test_md5.py
--rw-rw-rw-   0        0        0     3004 2022-11-22 07:10:43.000000 RobertCommonBasic-0.1.34/robertcommonbasic/tests/test_basic/test_encrypt/test_rsa.py
-drwxrwxrwx   0        0        0        0 2023-03-16 09:03:35.891042 RobertCommonBasic-0.1.34/robertcommonbasic/tests/test_basic/test_exector/
--rw-rw-rw-   0        0        0        0 2022-08-31 08:24:08.000000 RobertCommonBasic-0.1.34/robertcommonbasic/tests/test_basic/test_exector/__init__.py
--rw-rw-rw-   0        0        0     1234 2022-12-05 09:33:27.000000 RobertCommonBasic-0.1.34/robertcommonbasic/tests/test_basic/test_exector/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-03-16 09:03:35.895431 RobertCommonBasic-0.1.34/robertcommonbasic/tests/test_basic/test_file/
--rw-rw-rw-   0        0        0        0 2022-11-18 06:48:14.000000 RobertCommonBasic-0.1.34/robertcommonbasic/tests/test_basic/test_file/__init__.py
--rw-rw-rw-   0        0        0     1090 2023-02-03 06:30:00.000000 RobertCommonBasic-0.1.34/robertcommonbasic/tests/test_basic/test_file/test_csv.py
--rw-rw-rw-   0        0        0     4285 2023-02-02 03:00:01.000000 RobertCommonBasic-0.1.34/robertcommonbasic/tests/test_basic/test_file/test_xml.py
--rw-rw-rw-   0        0        0      705 2023-03-08 07:17:17.000000 RobertCommonBasic-0.1.34/robertcommonbasic/tests/test_basic/test_file/test_zip.py
-drwxrwxrwx   0        0        0        0 2023-03-16 09:03:35.899053 RobertCommonBasic-0.1.34/robertcommonbasic/tests/test_basic/test_net/
--rw-rw-rw-   0        0        0        0 2022-06-29 13:56:13.000000 RobertCommonBasic-0.1.34/robertcommonbasic/tests/test_basic/test_net/__init__.py
--rw-rw-rw-   0        0        0      471 2022-08-09 07:22:09.000000 RobertCommonBasic-0.1.34/robertcommonbasic/tests/test_basic/test_net/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-03-16 09:03:35.901353 RobertCommonBasic-0.1.34/robertcommonbasic/tests/test_basic/test_os/
--rw-rw-rw-   0        0        0        0 2022-03-25 04:05:00.000000 RobertCommonBasic-0.1.34/robertcommonbasic/tests/test_basic/test_os/__init__.py
--rw-rw-rw-   0        0        0      258 2022-06-29 09:29:01.000000 RobertCommonBasic-0.1.34/robertcommonbasic/tests/test_basic/test_os/test_env.py
--rw-rw-rw-   0        0        0      449 2022-11-14 02:56:25.000000 RobertCommonBasic-0.1.34/robertcommonbasic/tests/test_basic/test_os/test_file.py
-drwxrwxrwx   0        0        0        0 2023-03-16 09:03:35.902822 RobertCommonBasic-0.1.34/robertcommonbasic/tests/test_basic/test_re/
--rw-rw-rw-   0        0        0        0 2022-05-18 02:57:45.000000 RobertCommonBasic-0.1.34/robertcommonbasic/tests/test_basic/test_re/__init__.py
--rw-rw-rw-   0        0        0      301 2022-05-18 03:03:38.000000 RobertCommonBasic-0.1.34/robertcommonbasic/tests/test_basic/test_re/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-03-16 09:03:35.905548 RobertCommonBasic-0.1.34/robertcommonbasic/tests/test_basic/test_validation/
--rw-rw-rw-   0        0        0        0 2021-11-19 07:34:54.000000 RobertCommonBasic-0.1.34/robertcommonbasic/tests/test_basic/test_validation/__init__.py
--rw-rw-rw-   0        0        0      218 2022-05-10 03:46:33.000000 RobertCommonBasic-0.1.34/robertcommonbasic/tests/test_basic/test_validation/test_input.py
--rw-rw-rw-   0        0        0       42 2023-03-16 09:03:35.908835 RobertCommonBasic-0.1.34/setup.cfg
--rw-rw-rw-   0        0        0     3876 2023-03-16 09:02:31.000000 RobertCommonBasic-0.1.34/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:26:15.033093 RobertCommonBasic-0.1.35/
+-rw-rw-rw-   0        0        0     1067 2021-08-09 02:56:17.000000 RobertCommonBasic-0.1.35/LICENSE
+-rw-rw-rw-   0        0        0       44 2021-08-09 07:19:42.000000 RobertCommonBasic-0.1.35/MANIFEST.in
+-rw-rw-rw-   0        0        0     1739 2023-04-17 08:26:15.033093 RobertCommonBasic-0.1.35/PKG-INFO
+-rw-rw-rw-   0        0        0     1057 2022-01-13 05:29:18.000000 RobertCommonBasic-0.1.35/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 08:26:14.901099 RobertCommonBasic-0.1.35/RobertCommonBasic.egg-info/
+-rw-rw-rw-   0        0        0     1739 2023-04-17 08:26:14.000000 RobertCommonBasic-0.1.35/RobertCommonBasic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4427 2023-04-17 08:26:14.000000 RobertCommonBasic-0.1.35/RobertCommonBasic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 08:26:14.000000 RobertCommonBasic-0.1.35/RobertCommonBasic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      176 2023-04-17 08:26:14.000000 RobertCommonBasic-0.1.35/RobertCommonBasic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-04-17 08:26:14.000000 RobertCommonBasic-0.1.35/RobertCommonBasic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      194 2023-03-29 09:51:16.000000 RobertCommonBasic-0.1.35/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 08:26:14.903098 RobertCommonBasic-0.1.35/robertcommonbasic/
+-rw-rw-rw-   0        0        0        2 2021-08-09 03:27:49.000000 RobertCommonBasic-0.1.35/robertcommonbasic/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:26:14.904098 RobertCommonBasic-0.1.35/robertcommonbasic/basic/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:26:14.905101 RobertCommonBasic-0.1.35/robertcommonbasic/basic/base/
+-rw-rw-rw-   0        0        0        0 2023-01-04 02:39:20.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/base/__init__.py
+-rw-rw-rw-   0        0        0      471 2023-01-04 02:45:25.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/base/constant.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:26:14.909098 RobertCommonBasic-0.1.35/robertcommonbasic/basic/cache/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/cache/__init__.py
+-rw-rw-rw-   0        0        0      667 2022-11-14 07:41:26.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/cache/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:26:14.911102 RobertCommonBasic-0.1.35/robertcommonbasic/basic/cls/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/cls/__init__.py
+-rw-rw-rw-   0        0        0    12322 2023-04-03 03:01:59.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/cls/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:26:14.924625 RobertCommonBasic-0.1.35/robertcommonbasic/basic/data/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/data/__init__.py
+-rw-rw-rw-   0        0        0    13611 2023-01-31 14:01:59.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/data/conversion.py
+-rw-rw-rw-   0        0        0     4537 2022-11-14 07:54:50.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/data/crc16.py
+-rw-rw-rw-   0        0        0     2229 2022-11-14 03:21:43.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/data/csv.py
+-rw-rw-rw-   0        0        0    39297 2022-11-14 09:43:00.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/data/datatuple.py
+-rw-rw-rw-   0        0        0     8304 2022-11-14 09:43:00.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/data/frame.py
+-rw-rw-rw-   0        0        0     1097 2022-11-14 09:48:07.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/data/nametuple.py
+-rw-rw-rw-   0        0        0       62 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/data/type.py
+-rw-rw-rw-   0        0        0     5064 2022-11-14 09:43:00.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/data/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:26:14.926624 RobertCommonBasic-0.1.35/robertcommonbasic/basic/decorator/
+-rw-rw-rw-   0        0        0        0 2021-12-08 01:56:09.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/decorator/__init__.py
+-rw-rw-rw-   0        0        0     1250 2022-12-05 08:07:43.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/decorator/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:26:14.931661 RobertCommonBasic-0.1.35/robertcommonbasic/basic/dt/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/dt/__init__.py
+-rw-rw-rw-   0        0        0     4474 2022-12-28 02:51:52.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/dt/schedule.py
+-rw-rw-rw-   0        0        0    10445 2023-04-10 06:28:17.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/dt/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:26:14.938849 RobertCommonBasic-0.1.35/robertcommonbasic/basic/encrypt/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/encrypt/__init__.py
+-rw-rw-rw-   0        0        0      583 2022-11-14 07:14:55.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/encrypt/aes.py
+-rw-rw-rw-   0        0        0     3856 2022-11-14 07:41:26.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/encrypt/dsa.py
+-rw-rw-rw-   0        0        0      716 2023-03-09 07:09:06.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/encrypt/hash.py
+-rw-rw-rw-   0        0        0      338 2022-11-14 07:14:55.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/encrypt/md5.py
+-rw-rw-rw-   0        0        0     2661 2022-11-14 07:25:08.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/encrypt/rsa.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:26:14.941815 RobertCommonBasic-0.1.35/robertcommonbasic/basic/error/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/error/__init__.py
+-rw-rw-rw-   0        0        0     2354 2022-11-14 09:50:44.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/error/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:26:14.943816 RobertCommonBasic-0.1.35/robertcommonbasic/basic/exector/
+-rw-rw-rw-   0        0        0        0 2022-08-31 08:25:14.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/exector/__init__.py
+-rw-rw-rw-   0        0        0     3641 2022-11-14 09:50:44.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/exector/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:26:14.952815 RobertCommonBasic-0.1.35/robertcommonbasic/basic/file/
+-rw-rw-rw-   0        0        0        0 2022-11-18 02:39:00.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/file/__init__.py
+-rw-rw-rw-   0        0        0     3113 2023-02-21 06:19:45.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/file/csv.py
+-rw-rw-rw-   0        0        0     1328 2022-11-18 03:22:13.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/file/ini.py
+-rw-rw-rw-   0        0        0     1035 2022-11-18 06:23:07.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/file/log.py
+-rw-rw-rw-   0        0        0     3157 2022-11-24 03:18:18.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/file/xml.py
+-rw-rw-rw-   0        0        0      339 2022-11-18 06:47:46.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/file/yaml.py
+-rw-rw-rw-   0        0        0     3039 2023-03-08 07:31:52.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/file/zip.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:26:14.958676 RobertCommonBasic-0.1.35/robertcommonbasic/basic/log/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/log/__init__.py
+-rw-rw-rw-   0        0        0     6070 2023-04-10 02:23:47.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/log/utils.py
+-rw-rw-rw-   0        0        0     1366 2022-12-05 08:20:54.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/log/watch.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:26:14.960677 RobertCommonBasic-0.1.35/robertcommonbasic/basic/net/
+-rw-rw-rw-   0        0        0        0 2022-06-29 12:44:36.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/net/__init__.py
+-rw-rw-rw-   0        0        0     5874 2023-04-11 03:18:26.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/net/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:26:14.970684 RobertCommonBasic-0.1.35/robertcommonbasic/basic/os/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/os/__init__.py
+-rw-rw-rw-   0        0        0      228 2022-12-14 09:03:01.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/os/cmd.py
+-rw-rw-rw-   0        0        0      400 2022-06-29 09:34:23.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/os/env.py
+-rw-rw-rw-   0        0        0     3446 2023-03-16 09:00:41.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/os/file.py
+-rw-rw-rw-   0        0        0      533 2023-02-06 07:51:13.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/os/path.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:26:14.974027 RobertCommonBasic-0.1.35/robertcommonbasic/basic/process/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/process/__init__.py
+-rw-rw-rw-   0        0        0     8845 2022-12-14 08:53:18.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/process/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:26:14.979023 RobertCommonBasic-0.1.35/robertcommonbasic/basic/profile/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/profile/__init__.py
+-rw-rw-rw-   0        0        0     1264 2022-11-18 02:27:39.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/profile/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:26:14.983538 RobertCommonBasic-0.1.35/robertcommonbasic/basic/re/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/re/__init__.py
+-rw-rw-rw-   0        0        0     1868 2023-02-09 02:47:33.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/re/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:26:14.986573 RobertCommonBasic-0.1.35/robertcommonbasic/basic/safetext/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/safetext/__init__.py
+-rw-rw-rw-   0        0        0       91 2023-02-03 07:26:22.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/safetext/converter.py
+-rw-rw-rw-   0        0        0      377 2022-11-18 02:33:07.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/safetext/funcs.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:26:14.989573 RobertCommonBasic-0.1.35/robertcommonbasic/basic/sugar/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/sugar/__init__.py
+-rw-rw-rw-   0        0        0      377 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/sugar/funcs.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:26:14.991573 RobertCommonBasic-0.1.35/robertcommonbasic/basic/validation/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/validation/__init__.py
+-rw-rw-rw-   0        0        0    36389 2023-02-21 08:51:30.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/validation/input.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:26:14.992572 RobertCommonBasic-0.1.35/robertcommonbasic/tests/
+-rw-rw-rw-   0        0        0        0 2021-07-27 06:06:01.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:26:14.994858 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/
+-rw-rw-rw-   0        0        0        0 2021-07-27 06:49:18.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:26:14.997335 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_cls/
+-rw-rw-rw-   0        0        0        0 2022-04-22 02:07:10.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_cls/__init__.py
+-rw-rw-rw-   0        0        0     1291 2023-03-02 14:03:08.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_cls/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:26:15.006595 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_data/
+-rw-rw-rw-   0        0        0        0 2022-01-19 07:38:20.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_data/__init__.py
+-rw-rw-rw-   0        0        0      729 2022-06-23 09:21:24.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_data/test_conversion.py
+-rw-rw-rw-   0        0        0     5920 2022-04-21 06:58:53.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_data/test_datatupple.py
+-rw-rw-rw-   0        0        0     2456 2022-01-27 05:56:15.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_data/test_frame.py
+-rw-rw-rw-   0        0        0     3568 2023-04-11 13:11:50.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_data/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:26:15.008595 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_dt/
+-rw-rw-rw-   0        0        0        0 2022-03-08 05:59:28.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_dt/__init__.py
+-rw-rw-rw-   0        0        0     2169 2023-02-20 02:34:17.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_dt/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:26:15.013873 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_encrypt/
+-rw-rw-rw-   0        0        0        0 2021-07-30 08:42:35.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_encrypt/__init__.py
+-rw-rw-rw-   0        0        0    32599 2022-07-03 01:41:08.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_encrypt/test_dsa.py
+-rw-rw-rw-   0        0        0      270 2022-07-03 01:04:51.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_encrypt/test_md5.py
+-rw-rw-rw-   0        0        0     3004 2022-11-22 07:10:43.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_encrypt/test_rsa.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:26:15.016095 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_exector/
+-rw-rw-rw-   0        0        0        0 2022-08-31 08:24:08.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_exector/__init__.py
+-rw-rw-rw-   0        0        0     1234 2022-12-05 09:33:27.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_exector/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:26:15.023096 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_file/
+-rw-rw-rw-   0        0        0        0 2022-11-18 06:48:14.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_file/__init__.py
+-rw-rw-rw-   0        0        0     1090 2023-02-03 06:30:00.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_file/test_csv.py
+-rw-rw-rw-   0        0        0     4285 2023-02-02 03:00:01.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_file/test_xml.py
+-rw-rw-rw-   0        0        0      705 2023-03-08 07:17:17.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_file/test_zip.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:26:15.025100 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_net/
+-rw-rw-rw-   0        0        0        0 2022-06-29 13:56:13.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_net/__init__.py
+-rw-rw-rw-   0        0        0      558 2023-04-11 03:14:26.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_net/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:26:15.027094 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_os/
+-rw-rw-rw-   0        0        0        0 2022-03-25 04:05:00.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_os/__init__.py
+-rw-rw-rw-   0        0        0      258 2022-06-29 09:29:01.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_os/test_env.py
+-rw-rw-rw-   0        0        0      449 2022-11-14 02:56:25.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_os/test_file.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:26:15.030093 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_re/
+-rw-rw-rw-   0        0        0        0 2022-05-18 02:57:45.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_re/__init__.py
+-rw-rw-rw-   0        0        0      605 2023-04-11 09:07:57.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_re/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:26:15.032094 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_validation/
+-rw-rw-rw-   0        0        0        0 2021-11-19 07:34:54.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_validation/__init__.py
+-rw-rw-rw-   0        0        0      218 2022-05-10 03:46:33.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_validation/test_input.py
+-rw-rw-rw-   0        0        0       42 2023-04-17 08:26:15.033093 RobertCommonBasic-0.1.35/setup.cfg
+-rw-rw-rw-   0        0        0     3876 2023-04-17 08:23:01.000000 RobertCommonBasic-0.1.35/setup.py
```

### Comparing `RobertCommonBasic-0.1.34/LICENSE` & `RobertCommonBasic-0.1.35/LICENSE`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.34/PKG-INFO` & `RobertCommonBasic-0.1.35/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RobertCommonBasic
-Version: 0.1.34
+Version: 0.1.35
 Summary: Robert Common Basic Library
 Home-page: https://github.com/hun0423/RobertCommonBasic
 Author: Robert0423
 Author-email: 851010070@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `RobertCommonBasic-0.1.34/README.md` & `RobertCommonBasic-0.1.35/README.md`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.34/RobertCommonBasic.egg-info/PKG-INFO` & `RobertCommonBasic-0.1.35/RobertCommonBasic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RobertCommonBasic
-Version: 0.1.34
+Version: 0.1.35
 Summary: Robert Common Basic Library
 Home-page: https://github.com/hun0423/RobertCommonBasic
 Author: Robert0423
 Author-email: 851010070@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `RobertCommonBasic-0.1.34/RobertCommonBasic.egg-info/SOURCES.txt` & `RobertCommonBasic-0.1.35/RobertCommonBasic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.34/robertcommonbasic/basic/cache/utils.py` & `RobertCommonBasic-0.1.35/robertcommonbasic/basic/cache/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.34/robertcommonbasic/basic/cls/utils.py` & `RobertCommonBasic-0.1.35/robertcommonbasic/basic/cls/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,27 +81,48 @@
                 raise Exception(f'func({func.__name__}) time out')
             except Exception as e:
                 raise e
         return wrapper
     return inner_set_timeout_wrapper
 
 
-class RepeatingTimer(Timer):
+class RepeatingTimer():
 
-    """
-     @daemon_thread
-        def thread_func():
-            pass
-    """
-
-    def run(self):
-        self.finished.wait(self.interval)
-        while not self.finished.is_set():
-            self.function(*self.args, **self.kwargs)
-            self.finished.wait(self.interval)
+    def __init__(self, interval, function, args=None, kwargs=None):
+        self.interval = interval
+        self.function = function
+        self.args = args if args is not None else []
+        self.kwargs = kwargs if kwargs is not None else {}
+        self._should_continue = False
+        self.is_running = False
+        self.thread = None
+
+    def is_alive(self):
+        return self._should_continue
+
+    def _handle_function(self):
+        self.is_running = True
+        self.function(self.args, self.kwargs)
+        self.is_running = False
+        self._start_timer()
+
+    def _start_timer(self):
+        if self._should_continue:  # Code could have been running when cancel was called.
+            self.thread = Timer(self.interval, self._handle_function)
+            self.thread.start()
+
+    def start(self):
+        if not self._should_continue and not self.is_running:
+            self._should_continue = True
+            self._start_timer()
+
+    def cancel(self):
+        if self.thread is not None:
+            self._should_continue = False  # Just in case thread is running and cancel fails.
+            self.thread.cancel()
 
 
 class SimpleTimer:
 
     def __init__(self):
         self.timer = None
```

### Comparing `RobertCommonBasic-0.1.34/robertcommonbasic/basic/data/conversion.py` & `RobertCommonBasic-0.1.35/robertcommonbasic/basic/data/conversion.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.34/robertcommonbasic/basic/data/crc16.py` & `RobertCommonBasic-0.1.35/robertcommonbasic/basic/data/crc16.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.34/robertcommonbasic/basic/data/csv.py` & `RobertCommonBasic-0.1.35/robertcommonbasic/basic/data/csv.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.34/robertcommonbasic/basic/data/datatuple.py` & `RobertCommonBasic-0.1.35/robertcommonbasic/basic/data/datatuple.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.34/robertcommonbasic/basic/data/frame.py` & `RobertCommonBasic-0.1.35/robertcommonbasic/basic/data/frame.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.34/robertcommonbasic/basic/data/nametuple.py` & `RobertCommonBasic-0.1.35/robertcommonbasic/basic/data/nametuple.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.34/robertcommonbasic/basic/data/utils.py` & `RobertCommonBasic-0.1.35/robertcommonbasic/basic/data/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.34/robertcommonbasic/basic/decorator/utils.py` & `RobertCommonBasic-0.1.35/robertcommonbasic/basic/decorator/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.34/robertcommonbasic/basic/dt/schedule.py` & `RobertCommonBasic-0.1.35/robertcommonbasic/basic/dt/schedule.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.34/robertcommonbasic/basic/dt/utils.py` & `RobertCommonBasic-0.1.35/robertcommonbasic/basic/dt/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -268,7 +268,24 @@
     if target_tz and not isinstance(target_tz, tzinfo):
         target_tz = get_timezone(str(target_tz))[0]
     if not tm.tzinfo and isinstance(original_tz, tzinfo):
         tm = original_tz.localize(tm)
     if isinstance(target_tz, tzinfo):
         tm = tm.astimezone(target_tz)
     return tm if with_zone else tm.replace(tzinfo=None)
+
+
+def convert_values_property_time(values: Union[dict, list, datetime], original_tz: Union[str, None], target_tz: Union[str, None]):
+    """替换数据里的datetime"""
+    if isinstance(values, list):
+        vs = []
+        for i, v in enumerate(values):
+            vs.append(convert_values_property_time(v, original_tz, target_tz))
+        return vs
+    elif isinstance(values, dict):
+        vs = {}
+        for k, v in values.items():
+            vs[k] = convert_values_property_time(v, original_tz, target_tz)
+        return vs
+    elif isinstance(values, datetime):
+        return convert_time(values, original_tz, target_tz)
+    return values
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `RobertCommonBasic-0.1.34/robertcommonbasic/basic/encrypt/aes.py` & `RobertCommonBasic-0.1.35/robertcommonbasic/basic/encrypt/aes.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.34/robertcommonbasic/basic/encrypt/dsa.py` & `RobertCommonBasic-0.1.35/robertcommonbasic/basic/encrypt/dsa.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.34/robertcommonbasic/basic/encrypt/hash.py` & `RobertCommonBasic-0.1.35/robertcommonbasic/basic/encrypt/hash.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.34/robertcommonbasic/basic/encrypt/rsa.py` & `RobertCommonBasic-0.1.35/robertcommonbasic/basic/encrypt/rsa.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.34/robertcommonbasic/basic/error/utils.py` & `RobertCommonBasic-0.1.35/robertcommonbasic/basic/error/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.34/robertcommonbasic/basic/exector/utils.py` & `RobertCommonBasic-0.1.35/robertcommonbasic/basic/exector/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.34/robertcommonbasic/basic/file/csv.py` & `RobertCommonBasic-0.1.35/robertcommonbasic/basic/file/csv.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.34/robertcommonbasic/basic/file/ini.py` & `RobertCommonBasic-0.1.35/robertcommonbasic/basic/file/ini.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.34/robertcommonbasic/basic/file/log.py` & `RobertCommonBasic-0.1.35/robertcommonbasic/basic/file/log.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.34/robertcommonbasic/basic/file/xml.py` & `RobertCommonBasic-0.1.35/robertcommonbasic/basic/file/xml.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.34/robertcommonbasic/basic/file/zip.py` & `RobertCommonBasic-0.1.35/robertcommonbasic/basic/file/zip.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.34/robertcommonbasic/basic/log/utils.py` & `RobertCommonBasic-0.1.35/robertcommonbasic/basic/log/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 import sys
 import time
+from datetime import datetime
 from colorama import init
 from inspect import stack
 from re import search
 from typing import Any, Optional
 from traceback import StackSummary, walk_stack
 from logging.handlers import TimedRotatingFileHandler
 
@@ -41,32 +42,44 @@
 
 
 class MyLogRecord(object):
   
     def __init__(self, msg, log_level: int = MyLogLevel.INFO, fmt: str = LOG_FORMAT, log_time_fmt: str = LOG_TIME_FORMAT, **kwargs):
         self.fmt = fmt
         self.tm = time.time()
+        self.utc = time.strftime("%Y-%m-%d %H:%M:%S", time.gmtime(int(self.tm)))
         _stack = stack()[1]
-        self.record = {'level': log_level, 'levelname': '{0:<5s}'.format(logging.getLevelName(log_level))[:5], 'utc': get_datetime_from_stamp(self.tm), 'asctime': time.strftime(log_time_fmt, time.localtime(self.tm)), 'message': msg, 'filename': get_file_name(_stack[1]), 'funcName': _stack[3], 'lineno': _stack[2]}
+        self.record = {'level': log_level, 'levelname': '{0:<5s}'.format(logging.getLevelName(log_level))[:5], 'utc': self.utc, 'asctime': time.strftime(log_time_fmt, time.localtime(self.tm)) if kwargs.get('is_utc', False) is False else self.utc, 'message': msg, 'filename': get_file_name(_stack[1]), 'funcName': _stack[3], 'lineno': _stack[2], **kwargs}
 
     def format_msg(self) -> str:
         return f"{self.fmt % self.record}"
 
+    def format_source_msg(self) -> str:
+        fmt = '[%(asctime)s] level: [%(levelname)s] module: [%(filename)s] source: [%(source)s] msg: [%(message)s]'
+        return f"{fmt % self.record}"
+
     def get_msg(self):
         return str(self.record.get('message'))
 
     def get_record(self, columns: Optional[dict] = None) -> dict:
         record = {}
         if isinstance(columns, dict) and len(columns) > 0:
             for k, v in columns.items():
                 record[v] = self.record.get(k)
         else:
             record = self.record
         return record
 
+    def print(self):
+        source = self.record.get('source')
+        if source is None:      # 通讯日志
+            print(self.format_msg())
+        else:       # 点位日志
+            print(self.format_source_msg())
+
 
 class MyStdout:
 
     def __init__(self, autoreset: bool = True):
         init(autoreset=autoreset)
         self.stdout_bak = sys.stdout
         self.stderr_bak = sys.stderr
@@ -86,28 +99,40 @@
             info = f"\033[1;30m{info}\033[0m"
         self.stdout_bak.write(info)
 
     def flush(self):
         pass
 
 
-def init_log(file_path: str, log_level: int, log_interval: int = 1, log_backup: int = 30, log_time_fmt: str = LOG_TIME_FORMAT, attach_handles: list = [], log_format: str = LOG_FORMAT):
+def utc(sec, what):
+    return datetime.utcnow().timetuple()
+
+
+def init_log(file_path: str, log_level: int, log_interval: int = 1, log_backup: int = 30, log_time_fmt: str = LOG_TIME_FORMAT, attach_handles: list = [], log_format: str = LOG_FORMAT, **kwargs):
     file_folder = get_file_folder(file_path)
     if create_dir_if_not_exist(file_folder) is True:
-        handler_file = TimedRotatingFileHandler(filename=file_path, when="D", interval=log_interval, backupCount=log_backup)
+        handler_file = TimedRotatingFileHandler(filename=file_path, when="D", interval=log_interval, backupCount=log_backup, utc=kwargs.get('is_utc', False))
         handler_file.suffix = "%Y-%m-%d_%H-%M.log"
         handler_file.setLevel(log_level)
         attach_handles.append(handler_file)
-
+        if kwargs.get('is_utc', False) is True:
+            logging.Formatter.converter = utc
         return logging.basicConfig(level=log_level, format=log_format, datefmt=log_time_fmt, handlers=attach_handles)
 
 
 def convert_msg(log_content: str):
     if len(log_content) > 0:
-        return search(r'\[(?P<asctime>.*?)] level: \[(?P<level>.*?)] module: \[(?P<module>.*?)] func: \[(?P<func>.*?)] lineno: \[(?P<lineno>.*?)] msg: \[(?P<msg>.*)]', log_content).groupdict()
+        if log_content.find('] level: [') > 0:
+            if log_content.find('] source: [') > 0:     #点错误
+                result = search(r'\[(?P<asctime>.*?)] level: \[(?P<level>.*?)] module: \[(?P<module>.*?)] source: \[(?P<source>.*?)] msg: \[(?P<msg>.*)]', log_content)
+            else:
+                result = search(r'\[(?P<asctime>.*?)] level: \[(?P<level>.*?)] module: \[(?P<module>.*?)] func: \[(?P<func>.*?)] lineno: \[(?P<lineno>.*?)] msg: \[(?P<msg>.*)]', log_content)
+            if result is not None:
+                return result.groupdict()
+    return log_content
 
 
 def format_log(log_content: Any):
     func = stack()[1]
     return {'file': get_file_name(func[1]), 'func': func[3], 'lineno': func[2], 'msg': log_content}
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `RobertCommonBasic-0.1.34/robertcommonbasic/basic/log/watch.py` & `RobertCommonBasic-0.1.35/robertcommonbasic/basic/log/watch.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.34/robertcommonbasic/basic/net/utils.py` & `RobertCommonBasic-0.1.35/robertcommonbasic/basic/net/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 import platform
 import psutil
 import re
 import socket
 import subprocess
 import uuid
 
-from ipaddress import ip_network, ip_address
+from ipaddress import ip_network, ip_address, IPv4Network
 
 
-# 查看当前主机名
 def get_host_name():
+    """查看当前主机名"""
     return socket.gethostname()
 
 
-# 根据主机名称获取当前IP
 def get_host_ip():
+    """根据主机名称获取当前IP"""
     return socket.gethostbyname(socket.gethostname())
 
 
-# 获取当前主机IPV4 和IPV6的所有IP地址(所有系统均通用)
 def get_host_ips(only_ipv4: bool = True):
+    """获取当前主机IPV4 和IPV6的所有IP地址(所有系统均通用)"""
     addrs = socket.getaddrinfo(get_host_name(), None)
     return [item[4][0] for item in addrs if ':' not in item[4][0]] if only_ipv4 is True else [item[4][0] for item in addrs]
 
 
 def get_ip_by_net(ip: str):
     m = re.compile(r"(\d+\.\d+\.\d+\.\d+)(?:/(\d+))?(?::(\d+))?").match(ip)
     if m:
@@ -40,43 +40,55 @@
                         if ':' not in item_ip:
                             item_ip = ip_address(item_ip)
                             if ip_start <= item_ip < ip_end:
                                 return f"{item_ip}" if port is None else f"{item_ip}:{port}"
     return ip
 
 
-def check_ip(ip: str):
+def check_ip(ip: str) -> bool:
+    """检测是否IP"""
     p = re.compile(r'^((25[0-5]|2[0-4]\d|[01]?\d\d?)\.){3}(25[0-5]|2[0-4]\d|[01]?\d\d?)$')
     if p.match(ip):
         return True
     return False
 
 
-# 获取MAC地址
-def get_mac_address():
+def get_mac_address() -> str:
+    """获取MAC地址"""
     mac = uuid.UUID(int=uuid.getnode()).hex[-12:]
     return ":".join([mac[e:e + 2] for e in range(0, 11, 2)]).upper()
 
 
-# 获取网段ip
-def get_networks(ip: str):
+def get_broadcast_by_ip(ip: str):
+    """获取广播地址"""
+    broadcast = "255.255.255.255"
+    for interface, data in psutil.net_if_addrs().items():
+        for addr in data:
+            if addr.family == 2:
+                if addr.address == ip:
+                    return IPv4Network(addr.address + '/' + addr.netmask, False).broadcast_address
+    return broadcast
+
+
+def get_networks(ip: str) -> list:
+    """获取网段ip"""
     ips = []
     m = re.compile(r"(\d+\.\d+\.\d+\.\d+)(?:/(\d+))?(?::(\d+))?").match(ip)
     if m:
         (_ip, net, port) = m.groups()
         __ip = f"{_ip}/{net}" if net is not None else f"{_ip}/24"
         ip_start = ip_address(str(ip_network(__ip, False)).split('/')[0])
         num_addresses = ip_network(__ip, False).num_addresses
         for i in range(num_addresses):
             ips.append(str(ip_address(ip_start) + i))
     return ips
 
 
-# 更改本机地址
 def change_local_ip(ip: str) -> str:
+    """更改本机地址"""
     m = re.compile(r"(\d+\.\d+\.\d+\.\d+)(?:/(\d+))?(?::(\d+))?").match(ip)
     if m:
         (_ip, net, port) = m.groups()
         if _ip is not None and net is not None:
             ips = get_networks(ip)
 
             __ip = f"{_ip}/{net}"
@@ -113,16 +125,16 @@
         return is_inuse_windows(ip, port, protocol)
     elif 'linux-' in machine:
         return is_inuse_linux(ip, port, protocol)
     else:
         raise Exception('Error, sorry, platform is unknown')
 
 
-# 检测端口是否占用
 def check_ip_in_use(ip: str, protocol: str = 'tcp') -> bool:
+    """检测端口是否占用"""
     m = re.compile(r"(\d+\.\d+\.\d+\.\d+)(?:/(\d+))?(?::(\d+))?").match(ip)
     if m:
         (_ip, net, port) = m.groups()
         if _ip is not None and port is not None:
             return get_inuse_fun(_ip, int(str(port)), protocol)
     return False
```

### Comparing `RobertCommonBasic-0.1.34/robertcommonbasic/basic/os/file.py` & `RobertCommonBasic-0.1.35/robertcommonbasic/basic/os/file.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.34/robertcommonbasic/basic/os/path.py` & `RobertCommonBasic-0.1.35/robertcommonbasic/basic/os/path.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.34/robertcommonbasic/basic/process/utils.py` & `RobertCommonBasic-0.1.35/robertcommonbasic/basic/process/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.34/robertcommonbasic/basic/profile/utils.py` & `RobertCommonBasic-0.1.35/robertcommonbasic/basic/profile/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.34/robertcommonbasic/basic/re/utils.py` & `RobertCommonBasic-0.1.35/robertcommonbasic/basic/re/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.34/robertcommonbasic/basic/validation/input.py` & `RobertCommonBasic-0.1.35/robertcommonbasic/basic/validation/input.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.34/robertcommonbasic/tests/test_basic/test_cls/test_utils.py` & `RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_cls/test_utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.34/robertcommonbasic/tests/test_basic/test_data/test_conversion.py` & `RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_data/test_conversion.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.34/robertcommonbasic/tests/test_basic/test_data/test_datatupple.py` & `RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_data/test_datatupple.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.34/robertcommonbasic/tests/test_basic/test_data/test_frame.py` & `RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_data/test_frame.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.34/robertcommonbasic/tests/test_basic/test_data/test_utils.py` & `RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_data/test_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
 import sys
-from robertcommonbasic.basic.data.utils import format_value, revert_exp, chunk_list
+from robertcommonbasic.basic.data.utils import format_value, revert_exp, chunk_list, SimpleEval, DEFAULT_FUNCTIONS
 
 def test_format_value():
 
     print(f"format_value('1.234', '1') = {format_value('1.234', '1')}")
     print(f"format_value('1.234', '-2.0') = {format_value('1.234', '-2.0')}")
     print(f"format_value('-1.234', '2.0') = {format_value('-1.234', '2.0')}")
     print(f"format_value('-1.234', 'v*3') = {format_value('-1.234', 'v*3')}")
@@ -73,8 +73,17 @@
 
 def test_large():
     result = format_value('0.1', '0.15 if v>5 else v', 2)
     print(result)
     print(format_value('2', '(max(4, v*3.3*1000/(4095*150))-4)/16*100', 3))
 
 
-test_large()
+def test_express():
+    try:
+        expression = 'Bucket Brigade Real4 > 0'
+        vs = {'Bucket Brigade Real4': 2}
+        return SimpleEval(None, DEFAULT_FUNCTIONS.copy(), vs).eval(expression)
+    except Exception as e:
+        return None
+
+
+print(test_express())
```

### Comparing `RobertCommonBasic-0.1.34/robertcommonbasic/tests/test_basic/test_dt/test_utils.py` & `RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_dt/test_utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.34/robertcommonbasic/tests/test_basic/test_encrypt/test_dsa.py` & `RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_encrypt/test_dsa.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.34/robertcommonbasic/tests/test_basic/test_encrypt/test_rsa.py` & `RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_encrypt/test_rsa.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.34/robertcommonbasic/tests/test_basic/test_exector/test_utils.py` & `RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_exector/test_utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.34/robertcommonbasic/tests/test_basic/test_file/test_csv.py` & `RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_file/test_csv.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.34/robertcommonbasic/tests/test_basic/test_file/test_xml.py` & `RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_file/test_xml.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.34/robertcommonbasic/tests/test_basic/test_file/test_zip.py` & `RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_file/test_zip.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.34/setup.py` & `RobertCommonBasic-0.1.35/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 # Package meta-data.
 NAME = 'RobertCommonBasic'
 DESCRIPTION = 'Robert Common Basic Library'
 URL = 'https://github.com/hun0423/RobertCommonBasic'
 EMAIL = '851010070@qq.com'
 AUTHOR = 'Robert0423'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.34'
-DATE = '2023-03-16'
+VERSION = '0.1.35'
+DATE = '2023-04-17'
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
 
 # The rest you shouldn't have to touch too much :)
```

