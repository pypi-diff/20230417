# Comparing `tmp/eis1600-0.8.0.tar.gz` & `tmp/eis1600-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eis1600-0.8.0.tar", last modified: Fri Mar 31 13:57:23 2023, max compression
+gzip compressed data, was "eis1600-0.8.1.tar", last modified: Mon Apr 17 10:03:40 2023, max compression
```

## Comparing `eis1600-0.8.0.tar` & `eis1600-0.8.1.tar`

### file list

```diff
@@ -1,68 +1,75 @@
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-03-31 13:57:23.427583 eis1600-0.8.0/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1046 2022-09-21 09:22:30.000000 eis1600-0.8.0/LICENSE
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     7817 2023-03-31 13:57:23.427583 eis1600-0.8.0/PKG-INFO
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5820 2023-03-31 11:49:54.000000 eis1600-0.8.0/README.md
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-03-31 13:57:23.419582 eis1600-0.8.0/eis1600/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-09-19 09:55:48.000000 eis1600-0.8.0/eis1600/__init__.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-03-31 13:57:23.419582 eis1600-0.8.0/eis1600/dates/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      918 2022-11-29 10:14:30.000000 eis1600-0.8.0/eis1600/dates/Date.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.8.0/eis1600/dates/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5850 2023-03-03 08:38:58.000000 eis1600-0.8.0/eis1600/dates/date_patterns.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3988 2023-03-31 12:48:59.000000 eis1600-0.8.0/eis1600/dates/methods.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-03-31 13:57:23.419582 eis1600-0.8.0/eis1600/gazetteers/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4228 2023-03-31 08:45:40.000000 eis1600-0.8.0/eis1600/gazetteers/Onomastics.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1959 2023-03-23 13:30:57.000000 eis1600-0.8.0/eis1600/gazetteers/Toponyms.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-03-09 08:52:31.000000 eis1600-0.8.0/eis1600/gazetteers/__init__.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-03-31 13:57:23.419582 eis1600-0.8.0/eis1600/gazetteers/data/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.8.0/eis1600/gazetteers/data/__init__.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-03-31 13:57:23.423583 eis1600-0.8.0/eis1600/helper/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1280 2023-03-06 11:57:01.000000 eis1600-0.8.0/eis1600/helper/Singleton.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-10-20 15:09:05.000000 eis1600-0.8.0/eis1600/helper/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      193 2022-11-14 11:12:12.000000 eis1600-0.8.0/eis1600/helper/ar_normalization.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1189 2023-01-26 12:00:28.000000 eis1600-0.8.0/eis1600/helper/fix_miu_annotation.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      365 2023-03-31 11:03:40.000000 eis1600-0.8.0/eis1600/helper/logging.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     6461 2023-03-09 10:15:31.000000 eis1600-0.8.0/eis1600/helper/miu_random_revisions.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    11013 2023-03-03 08:38:58.000000 eis1600-0.8.0/eis1600/helper/repo.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-03-31 13:57:23.423583 eis1600-0.8.0/eis1600/markdown/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1760 2022-11-08 08:28:10.000000 eis1600-0.8.0/eis1600/markdown/UIDs.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-09-30 09:01:09.000000 eis1600-0.8.0/eis1600/markdown/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4794 2023-02-23 07:56:48.000000 eis1600-0.8.0/eis1600/markdown/convert_mARkdown_to_EIS1600TMP.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4574 2023-02-23 07:56:48.000000 eis1600-0.8.0/eis1600/markdown/insert_uids.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    13118 2023-03-03 08:38:58.000000 eis1600-0.8.0/eis1600/markdown/methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3474 2023-03-27 08:26:41.000000 eis1600-0.8.0/eis1600/markdown/re_pattern.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2856 2023-02-23 07:56:48.000000 eis1600-0.8.0/eis1600/markdown/update_uids.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5279 2023-03-03 08:38:58.000000 eis1600-0.8.0/eis1600/markdown/update_uids_old_process.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-03-31 13:57:23.423583 eis1600-0.8.0/eis1600/miu/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3282 2023-03-31 12:48:59.000000 eis1600-0.8.0/eis1600/miu/HeadingTracker.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5153 2023-03-27 13:45:41.000000 eis1600-0.8.0/eis1600/miu/YAMLHandler.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-08 08:28:10.000000 eis1600-0.8.0/eis1600/miu/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2715 2023-02-23 07:39:16.000000 eis1600-0.8.0/eis1600/miu/disassemble_into_miu_files.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     8748 2023-03-31 12:32:01.000000 eis1600-0.8.0/eis1600/miu/methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2590 2022-11-21 11:57:36.000000 eis1600-0.8.0/eis1600/miu/reassemble_from_miu_files.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2448 2023-03-03 08:38:58.000000 eis1600-0.8.0/eis1600/miu/yml_handling.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-03-31 13:57:23.423583 eis1600-0.8.0/eis1600/nlp/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-17 12:10:00.000000 eis1600-0.8.0/eis1600/nlp/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2017 2023-03-31 12:22:46.000000 eis1600-0.8.0/eis1600/nlp/cameltools.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3672 2023-03-31 11:52:32.000000 eis1600-0.8.0/eis1600/nlp/ner_annotate_mius.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2725 2023-03-31 12:22:06.000000 eis1600-0.8.0/eis1600/nlp/utils.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-03-31 13:57:23.427583 eis1600-0.8.0/eis1600/onomastics/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-03-02 09:23:30.000000 eis1600-0.8.0/eis1600/onomastics/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1647 2023-03-31 11:37:14.000000 eis1600-0.8.0/eis1600/onomastics/annotation.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     7814 2023-03-31 13:43:22.000000 eis1600-0.8.0/eis1600/onomastics/methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1899 2023-03-27 10:49:58.000000 eis1600-0.8.0/eis1600/onomastics/re_pattern.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-03-31 13:57:23.427583 eis1600-0.8.0/eis1600/preprocessing/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.8.0/eis1600/preprocessing/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     7550 2023-03-31 13:11:16.000000 eis1600-0.8.0/eis1600/preprocessing/methods.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-03-31 13:57:23.427583 eis1600-0.8.0/eis1600/stats/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-02-17 08:45:10.000000 eis1600-0.8.0/eis1600/stats/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      842 2023-02-17 15:06:29.000000 eis1600-0.8.0/eis1600/stats/methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1978 2023-02-17 15:05:56.000000 eis1600-0.8.0/eis1600/stats/miu_stats.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-03-31 13:57:23.419582 eis1600-0.8.0/eis1600.egg-info/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     7817 2023-03-31 13:57:23.000000 eis1600-0.8.0/eis1600.egg-info/PKG-INFO
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1547 2023-03-31 13:57:23.000000 eis1600-0.8.0/eis1600.egg-info/SOURCES.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        1 2023-03-31 13:57:23.000000 eis1600-0.8.0/eis1600.egg-info/dependency_links.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      700 2023-03-31 13:57:23.000000 eis1600-0.8.0/eis1600.egg-info/entry_points.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)       46 2023-03-31 13:57:23.000000 eis1600-0.8.0/eis1600.egg-info/requires.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        8 2023-03-31 13:57:23.000000 eis1600-0.8.0/eis1600.egg-info/top_level.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)       38 2023-03-31 13:57:23.427583 eis1600-0.8.0/setup.cfg
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2036 2023-03-31 11:49:54.000000 eis1600-0.8.0/setup.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-17 10:03:40.664719 eis1600-0.8.1/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1046 2022-09-21 09:22:30.000000 eis1600-0.8.1/LICENSE
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     7956 2023-04-17 10:03:40.664719 eis1600-0.8.1/PKG-INFO
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5895 2023-04-13 08:22:59.000000 eis1600-0.8.1/README.md
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-17 10:03:40.652719 eis1600-0.8.1/eis1600/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-09-19 09:55:48.000000 eis1600-0.8.1/eis1600/__init__.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-17 10:03:40.652719 eis1600-0.8.1/eis1600/dates/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      911 2023-04-05 11:10:16.000000 eis1600-0.8.1/eis1600/dates/Date.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.8.1/eis1600/dates/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5856 2023-04-06 11:34:18.000000 eis1600-0.8.1/eis1600/dates/date_patterns.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3924 2023-04-12 06:44:26.000000 eis1600-0.8.1/eis1600/dates/methods.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-17 10:03:40.652719 eis1600-0.8.1/eis1600/gazetteers/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4225 2023-04-14 12:34:00.000000 eis1600-0.8.1/eis1600/gazetteers/Onomastics.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3259 2023-04-12 08:40:27.000000 eis1600-0.8.1/eis1600/gazetteers/Toponyms.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-03-09 08:52:31.000000 eis1600-0.8.1/eis1600/gazetteers/__init__.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-17 10:03:40.652719 eis1600-0.8.1/eis1600/gazetteers/data/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.8.1/eis1600/gazetteers/data/__init__.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-17 10:03:40.656719 eis1600-0.8.1/eis1600/helper/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1280 2023-04-06 10:45:49.000000 eis1600-0.8.1/eis1600/helper/Singleton.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-10-20 15:09:05.000000 eis1600-0.8.1/eis1600/helper/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1030 2023-04-06 13:50:26.000000 eis1600-0.8.1/eis1600/helper/ar_normalization.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-17 10:03:40.656719 eis1600-0.8.1/eis1600/helper/data/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-04-03 10:40:59.000000 eis1600-0.8.1/eis1600/helper/data/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      374 2023-04-05 10:09:07.000000 eis1600-0.8.1/eis1600/helper/entity_tags.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1237 2023-04-12 06:44:26.000000 eis1600-0.8.1/eis1600/helper/fix_miu_annotation.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      365 2023-03-31 11:03:40.000000 eis1600-0.8.1/eis1600/helper/logging.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      637 2023-04-06 09:28:14.000000 eis1600-0.8.1/eis1600/helper/markdown_methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3723 2023-04-14 12:34:00.000000 eis1600-0.8.1/eis1600/helper/markdown_patterns.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     6461 2023-03-09 10:15:31.000000 eis1600-0.8.1/eis1600/helper/miu_random_revisions.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      370 2023-04-13 08:15:00.000000 eis1600-0.8.1/eis1600/helper/my_json_ecoder.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10796 2023-04-05 11:18:46.000000 eis1600-0.8.1/eis1600/helper/repo.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1425 2023-04-13 08:57:43.000000 eis1600-0.8.1/eis1600/helper/yml_to_json.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-17 10:03:40.656719 eis1600-0.8.1/eis1600/markdown/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1822 2023-04-12 07:11:17.000000 eis1600-0.8.1/eis1600/markdown/UIDs.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-09-30 09:01:09.000000 eis1600-0.8.1/eis1600/markdown/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4794 2023-02-23 07:56:48.000000 eis1600-0.8.1/eis1600/markdown/convert_mARkdown_to_EIS1600TMP.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4574 2023-02-23 07:56:48.000000 eis1600-0.8.1/eis1600/markdown/insert_uids.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    13026 2023-04-13 10:26:19.000000 eis1600-0.8.1/eis1600/markdown/methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2856 2023-02-23 07:56:48.000000 eis1600-0.8.1/eis1600/markdown/update_uids.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5284 2023-04-05 08:21:34.000000 eis1600-0.8.1/eis1600/markdown/update_uids_old_process.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-17 10:03:40.660719 eis1600-0.8.1/eis1600/miu/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3484 2023-04-12 15:29:30.000000 eis1600-0.8.1/eis1600/miu/HeadingTracker.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     6622 2023-04-14 12:11:46.000000 eis1600-0.8.1/eis1600/miu/YAMLHandler.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-08 08:28:10.000000 eis1600-0.8.1/eis1600/miu/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2715 2023-02-23 07:39:16.000000 eis1600-0.8.1/eis1600/miu/disassemble_into_miu_files.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     8907 2023-04-12 06:50:23.000000 eis1600-0.8.1/eis1600/miu/methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2590 2022-11-21 11:57:36.000000 eis1600-0.8.1/eis1600/miu/reassemble_from_miu_files.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     6008 2023-04-17 08:45:53.000000 eis1600-0.8.1/eis1600/miu/yml_handling.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-17 10:03:40.660719 eis1600-0.8.1/eis1600/nlp/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-17 12:10:00.000000 eis1600-0.8.1/eis1600/nlp/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2017 2023-03-31 12:22:46.000000 eis1600-0.8.1/eis1600/nlp/cameltools.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3672 2023-03-31 11:52:32.000000 eis1600-0.8.1/eis1600/nlp/ner_annotate_mius.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2726 2023-04-05 11:18:46.000000 eis1600-0.8.1/eis1600/nlp/utils.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-17 10:03:40.660719 eis1600-0.8.1/eis1600/onomastics/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-03-02 09:23:30.000000 eis1600-0.8.1/eis1600/onomastics/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1201 2023-04-17 07:58:03.000000 eis1600-0.8.1/eis1600/onomastics/annotation.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     9095 2023-04-17 09:53:13.000000 eis1600-0.8.1/eis1600/onomastics/methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1966 2023-04-17 09:33:17.000000 eis1600-0.8.1/eis1600/onomastics/re_pattern.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-17 10:03:40.660719 eis1600-0.8.1/eis1600/processing/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.8.1/eis1600/processing/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4660 2023-04-12 08:23:03.000000 eis1600-0.8.1/eis1600/processing/postprocessing.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4604 2023-04-14 13:42:02.000000 eis1600-0.8.1/eis1600/processing/preprocessing.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-17 10:03:40.664719 eis1600-0.8.1/eis1600/stats/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-02-17 08:45:10.000000 eis1600-0.8.1/eis1600/stats/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      842 2023-02-17 15:06:29.000000 eis1600-0.8.1/eis1600/stats/methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1978 2023-02-17 15:05:56.000000 eis1600-0.8.1/eis1600/stats/miu_stats.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-17 10:03:40.652719 eis1600-0.8.1/eis1600.egg-info/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     7956 2023-04-17 10:03:40.000000 eis1600-0.8.1/eis1600.egg-info/PKG-INFO
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1749 2023-04-17 10:03:40.000000 eis1600-0.8.1/eis1600.egg-info/SOURCES.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        1 2023-04-17 10:03:40.000000 eis1600-0.8.1/eis1600.egg-info/dependency_links.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      746 2023-04-17 10:03:40.000000 eis1600-0.8.1/eis1600.egg-info/entry_points.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)       52 2023-04-17 10:03:40.000000 eis1600-0.8.1/eis1600.egg-info/requires.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        8 2023-04-17 10:03:40.000000 eis1600-0.8.1/eis1600.egg-info/top_level.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)       38 2023-04-17 10:03:40.664719 eis1600-0.8.1/setup.cfg
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2138 2023-04-17 10:03:32.000000 eis1600-0.8.1/setup.py
```

### Comparing `eis1600-0.8.0/LICENSE` & `eis1600-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.0/PKG-INFO` & `eis1600-0.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eis1600
-Version: 0.8.0
+Version: 0.8.1
 Summary: EIS1600 project tools and utilities
 Home-page: https://github.com/EIS1600/eis1600-pkg
 Author: Lisa Mischer
 Author-email: mischer.lisa@gmail.com
 License: MIT License
 Description: # EIS1600 Tools
         
@@ -109,15 +109,15 @@
         $ convert_mARkdown_to_EIS1600 <input_dir> <output_dir>
         $ insert_uids <input_dir> <output_dir>
         ```
         
         ### Disassembling
         
         Disassemble files into the MIU repo. MIU repo has to be next to TEXT repo.
-        Must be run from the root of TEXT repo, this will disassemble all files from the AUTOREPORT.
+        Must be run from the root of TEXT repo, this will disassemble all files from the `AUTOREPORT`.
         ```shell
         $ disassemble_into_miu_files
         ```
         Give the relative path to a file to disassemble a singe file.
         ```shell
         $ disassemble_into_miu_files data/<author>/<text>/<edition>.EIS1600
         ```
@@ -179,14 +179,22 @@
         reviewed    : NOT REVIEWED
         ```
         to
         ```yaml
         reviewed    : REVIEWED
         ```
         
+        ## For MC
+        
+        ### Collect YAMLHeader into JSON
+        
+        ```shell
+        $ yml_to_json
+        ```
+        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.7, <3.9
```

### Comparing `eis1600-0.8.0/README.md` & `eis1600-0.8.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -101,15 +101,15 @@
 $ convert_mARkdown_to_EIS1600 <input_dir> <output_dir>
 $ insert_uids <input_dir> <output_dir>
 ```
 
 ### Disassembling
 
 Disassemble files into the MIU repo. MIU repo has to be next to TEXT repo.
-Must be run from the root of TEXT repo, this will disassemble all files from the AUTOREPORT.
+Must be run from the root of TEXT repo, this will disassemble all files from the `AUTOREPORT`.
 ```shell
 $ disassemble_into_miu_files
 ```
 Give the relative path to a file to disassemble a singe file.
 ```shell
 $ disassemble_into_miu_files data/<author>/<text>/<edition>.EIS1600
 ```
@@ -170,7 +170,15 @@
 ```yaml
 reviewed    : NOT REVIEWED
 ```
 to
 ```yaml
 reviewed    : REVIEWED
 ```
+
+## For MC
+
+### Collect YAMLHeader into JSON
+
+```shell
+$ yml_to_json
+```
```

### Comparing `eis1600-0.8.0/eis1600/dates/Date.py` & `eis1600-0.8.1/eis1600/dates/Date.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 class Date:
     """
 
     :param int year: year.
     :param int length: number of tokens which make up the date expression.
     :param Literal['B', 'D', 'K', 'H', 'P', 'L'] category:
     """
-    def __init__(self, year: int, length: int,
-            category: Literal['B', 'D', 'K', 'H', 'P', 'L'] = 'X'):
+    def __init__(self, year: int, length: int, category: Literal['B', 'D', 'K', 'H', 'P', 'L', 'X'] = 'X'):
         self.year = year
         self.length = length
         self.category = category
 
     def __eq__(self, other):
         return self.year == other.year and self.length == other.length and self.category == other.category
```

### Comparing `eis1600-0.8.0/eis1600/dates/date_patterns.py` & `eis1600-0.8.1/eis1600/dates/date_patterns.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import re
 
 from openiti.helper.ara import denormalize
 
-from eis1600.helper.ar_normalization import normalize_set
-from eis1600.markdown.re_pattern import AR_STR, WORD
+from eis1600.helper.ar_normalization import normalize_dict
+from eis1600.helper.markdown_patterns import WORD
 
 ONES = {
         'واحد': 1, 'احدى': 1, 'احد': 1, 'اثنين': 2, 'اثنتين': 2, 'اثنتي': 2, 'ثلاث': 3, 'ثلث': 3, 'اربع': 4, 'خمس': 5,
         'ست': 6, 'سبع': 7, 'ثماني': 8, 'ثمان': 8, 'تسع': 9
 }
-ONES_NOR = normalize_set(ONES)
+ONES_NOR = normalize_dict(ONES)
 TEN = {
         'عشرة': 10, 'عشري': 10, 'عشر': 10, 'عشرين': 20, 'ثلاثين': 30, 'اربعين': 40, 'خمسين': 50, 'ستين': 60,
         'سبعين': 70,
         'ثمانين': 80, 'تسعين': 90
 }
-TEN_NOR = normalize_set(TEN)
+TEN_NOR = normalize_dict(TEN)
 HUNDRED = {
         'مائة': 100, 'ماية': 100, 'مية': 100, 'مئة': 100, 'مائتين': 200, 'مايتين': 200, 'ميتين': 200,
         'ثلاثمائة': 300, 'ثلاث مائة': 300, 'ثلثمائة': 300, 'ثلث مائة': 300, 'اربعمائة': 400, 'اربع مائة': 400,
         'خمسمائة': 500, 'خمس مائة': 500, 'ستمائة': 600, 'ست مائة': 600, 'سبعمائة': 700, 'سبع مائة': 700,
         'ثمانمائة': 800, 'ثمان مائة': 800, 'ثمانيمائة': 800, 'ثماني مائة': 800, 'تسعمائة': 900, 'تسع مائة': 900,
         'ثلاثماية': 300, 'ثلاث ماية': 300, 'ثلثماية': 300, 'ثلث ماية': 300, 'اربعماية': 400, 'اربع ماية': 400,
         'خمسماية': 500, 'خمس ماية': 500, 'ستماية': 600, 'ست ماية': 600, 'سبعماية': 700, 'سبع ماية': 700,
@@ -27,37 +27,37 @@
         'ثلاثمية': 300, 'ثلاث مية': 300, 'ثلثمية': 300, 'ثلث مية': 300, 'اربعمية': 400, 'اربع مية': 400, 'خمسمية': 500,
         'خمس مية': 500, 'ستمية': 600, 'ست مية': 600, 'سبعمية': 700, 'سبع مية': 700, 'ثمانمية': 800, 'ثمان مية': 800,
         'ثمانيمية': 800, 'ثماني مية': 800, 'تسعمية': 900, 'تسع مية': 900, 'ثلاثمئة': 300, 'ثلاث مئة': 300,
         'ثلثمئة': 300, 'ثلث مئة': 300, 'اربعمئة': 400, 'اربع مئة': 400, 'خمسمئة': 500, 'خمس مئة': 500, 'ستمئة': 600,
         'ست مئة': 600, 'سبعمئة': 700, 'سبع مئة': 700, 'ثمانمئة': 800, 'ثمان مئة': 800, 'ثمانيمئة': 800,
         'ثماني مئة': 800, 'تسعمئة': 900, 'تسع مئة': 900
 }
-HUNDRED_NOR = normalize_set(HUNDRED)
+HUNDRED_NOR = normalize_dict(HUNDRED)
 
 DAY_ONES = {
         'واحد': 1, 'حادي': 1, 'ثاني': 2, 'ثالث': 3, 'رابع': 4, 'خامس': 5, 'خميس': 5, 'سادس': 6, 'سابع': 7,
         'ثامن': 8, 'تاسع': 9, 'عاشر': 10
 }
-DAY_ONES_NOR = normalize_set(DAY_ONES)
+DAY_ONES_NOR = normalize_dict(DAY_ONES)
 DAY_TEN = {'عشرة': 10, 'عشري': 10, 'عشر': 10, 'عشرين': 20, 'عشرون': 20, 'ثلاثين': 30, 'ثلاثون': 30}
-DAY_TEN_NOR = normalize_set(DAY_TEN)
+DAY_TEN_NOR = normalize_dict(DAY_TEN)
 WEEKDAYS = {
         'يوم الأحد': 1, 'يوم الاثنين': 2, 'يوم الثلاثاء': 3, 'يوم الأربعاء': 4, 'يمو الخميس': 5, 'يوم الجمعة': 6,
         'يوم السبت': 7
 }
-WEEKDAYS_NOR = normalize_set(WEEKDAYS)
+WEEKDAYS_NOR = normalize_dict(WEEKDAYS)
 
 MONTHS = {
         'محرم': 1, 'شهر الله المحرم': 1, 'صفر': 2, 'صفر الخير': 2, 'ربيع': 3, 'ربيع الاول': 3, 'ربيع الثاني': 4,
         'ربيع الاخر': 4, 'جمادى الاول': 5, 'جمادى الاولى': 5, 'جمادى الاخرة': 6, 'جمادى الاخر': 6, 'جمادى الثانية': 6,
         'رجب': 7, 'رجب الفرد': 7, 'رجب المبارك': 7, 'شعبان': 8, 'شعبان المكرم': 8, 'رمضان': 9,
         'رمضان المعظم': 9, 'شوال': 10, 'ذي القعدة': 11, 'ذي قعدة': 11, 'ذي الحجة': 12, 'ذي حجة': 12, 'ذو القعدة': 11,
         'ذو قعدة': 11, 'ذو الحجة': 12, 'ذو حجة': 12, 'اخر': -1
 }
-MONTHS_NOR = normalize_set(MONTHS)
+MONTHS_NOR = normalize_dict(MONTHS)
 
 AR_MONTHS = '|'.join(['(?:' + r'\s'.join(denormalize(key).split()) + ')' for key in MONTHS.keys()])
 AR_ONES = '|'.join([denormalize(key) for key in ONES.keys()])
 AR_TEN = '|'.join([denormalize(key) for key in TEN.keys()])
 AR_HUNDRED = '|'.join(['(?:' + r'\s'.join(denormalize(key).split()) + ')' for key in HUNDRED.keys()])
 AR_ONES_DAY = '|'.join([denormalize(key) for key in DAY_ONES.keys()])
 AR_TEN_DAY = '|'.join([denormalize(key) for key in DAY_TEN.keys()])
@@ -73,11 +73,11 @@
 DATE_PATTERN = re.compile(DATE)
 MONTH_PATTERN = re.compile(AR_MONTHS)
 
 DATE_CATEGORIES = {
         'ولد': 'B', 'مولد': 'B', 'مات': 'D', 'موت': 'D', 'توفي': 'D', 'وفات': 'D', 'حج': 'P',
         'سمع': 'K', 'قرا': 'K', 'استقر': 'O', 'اجاز': 'K', 'انفصل': 'O', 'لقي': 'M'
 }
-DATE_CATEGORIES_NOR = normalize_set(DATE_CATEGORIES)
+DATE_CATEGORIES_NOR = normalize_dict(DATE_CATEGORIES)
 
 AR_DATE_CATEGORIES = '|'.join([denormalize(key) for key in DATE_CATEGORIES.keys()])
 DATE_CATEGORY_PATTERN = re.compile(r'\s[وف]?(?P<date_category>' + AR_DATE_CATEGORIES + r')')
```

### Comparing `eis1600-0.8.0/eis1600/dates/methods.py` & `eis1600-0.8.1/eis1600/dates/methods.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from openiti.helper.ara import normalize_ara_heavy
 
 from eis1600.dates.Date import Date
 from eis1600.dates.date_patterns import DATE_CATEGORIES_NOR, DATE_CATEGORY_PATTERN, DATE_PATTERN, \
     DAY_ONES_NOR, \
     DAY_TEN_NOR, MONTHS_NOR, \
     WEEKDAYS_NOR, ONES_NOR, TEN_NOR, HUNDRED_NOR
-from eis1600.preprocessing.methods import get_tokens_and_tags
+from eis1600.processing.preprocessing import get_tokens_and_tags
 
 
 def parse_year(m: Match[str]) -> (int, int):
     year = 0
     length = 1  # word sana
     if m.group('ones'):
         year += ONES_NOR.get(normalize_ara_heavy(m.group('ones')))
@@ -35,22 +35,22 @@
     :param YAMLHandler yml_handler: arabic text.
     """
     headings = yml_handler.headings
     for key, val in headings:
         if DATE_PATTERN.search(val):
             m = DATE_PATTERN.search(val)
             year, length = parse_year(m)
-            yml_handler.add_date_headings(Date(year, length, 'H').get_tag()[:-1])   # Cut of trailing whitespace
+            yml_handler.add_date_headings(year)
 
 
 def tag_dates_fulltext(text: str) -> str:
     """Inserts date tags in the arabic text and returns the text with the tags.
 
     :param str text: arabic text.
-    :returns str: arabic text with date tags.
+    :return str: arabic text with date tags.
     """
     text_updated = text
     m = DATE_PATTERN.search(text_updated)
     while m:
         month = None
         day = 0
         weekday = None
@@ -93,15 +93,15 @@
 
 
 def date_annotate_miu_text(ner_df: DataFrame, yml: YAMLHandler) -> Series:
     """Annotate dates in the headings and in the MIU text, returns a list of tag per token.
 
     :param DataFrame ner_df: df containing the 'TOKENS' column.
     :param YAMLHandler yml: yml_header to collect date tags in.
-    :returns Series: List of date tags per token, which can be added as additional column to the df.
+    :return Series: List of date tags per token, which can be added as additional column to the df.
     """
     get_dates_headings(yml)
 
     ner_df.mask(ner_df == '', None, inplace=True)
     tokens = ner_df['TOKENS'].dropna()
     ar_text = ' '.join(tokens)
```

### Comparing `eis1600-0.8.0/eis1600/gazetteers/Onomastics.py` & `eis1600-0.8.1/eis1600/gazetteers/Onomastics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
 
 from importlib_resources import files
-from typing import List, Tuple, Pattern
+from typing import List, Pattern
 import pandas as pd
 from eis1600.helper.Singleton import Singleton
 from openiti.helper.ara import denormalize
 
 path = files('eis1600.gazetteers.data').joinpath('onomastic_gazetteer.csv')
 
 
@@ -87,17 +87,16 @@
         return Onomastics.__tot
 
     @staticmethod
     def get_ngrams_regex() -> Pattern[str]:
         return Onomastics.__ngrams_regex
 
     @staticmethod
-    def get_ngram_tag(ngram) -> str:
+    def get_ngram_tag(ngram: str) -> str:
         lookup = Onomastics.__ngrams.loc[Onomastics.__ngrams['VALUE'].str.fullmatch(denormalize(ngram))]
         if len(lookup) > 1:
             all_pos = ['Ü' + cat + str(n) for cat, n in zip(lookup['CATEGORY'].to_list(), lookup['NGRAM'].to_list())]
             return '___'.join(all_pos) + ' '
         elif len(lookup) == 1:
             return 'Ü' + str(lookup.iloc[0]['CATEGORY']) + str(lookup.iloc[0]['NGRAM']) + ' '
         else:
             return 'ÜNaN' + str(len(ngram)) + ' '
-
```

### Comparing `eis1600-0.8.0/eis1600/gazetteers/Toponyms.py` & `eis1600-0.8.1/eis1600/gazetteers/Toponyms.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,53 @@
+from eis1600.helper.ar_normalization import denormalize_list
 from importlib_resources import files
 from typing import List, Tuple
 import pandas as pd
 from eis1600.helper.Singleton import Singleton
 
 file_path = files('eis1600.gazetteers.data')
 thurayya_path = file_path.joinpath('toponyms.csv')
 regions_path = file_path.joinpath('regions_gazetteer.csv')
 
 
-def split_toponyms(tops: str) -> List[str]:
-    return tops.split('، ')
-
-
 @Singleton
 class Toponyms:
     """
     Gazetteer
 
+    :ivar DataFrame __df: The dataFrame.
     :ivar __places List[str]: List of all place names and their prefixed variants.
     :ivar __regions List[str]: List of all region names and their prefixed variants.
     :ivar __total List[str]: List of all toponyms and their prefixed variants.
     :ivar __rpl List[Tuple[str, str]]: List of tuples: expression and its replacement.
     """
+    __df = None
     __places = None
     __regions = None
     __total = None
     __rpl = None
 
     def __init__(self) -> None:
-        thurayya_df = pd.read_csv(thurayya_path, usecols=['placeLabel', 'toponyms', 'typeLabel', 'geometry'],
+        def split_toponyms(tops: str) -> List[str]:
+            return tops.split('، ')
+
+        thurayya_df = pd.read_csv(thurayya_path, usecols=['uri', 'placeLabel', 'toponyms', 'province', 'typeLabel',
+                                                          'geometry'],
                                   converters={'toponyms': split_toponyms})
         regions_df = pd.read_csv(regions_path)
         prefixes = ['ب', 'و', 'وب']
 
-        places = thurayya_df['toponyms'].explode().to_list()
-        Toponyms.__places = places + [prefix + top for prefix in prefixes for top in places]
+        def get_all_variations(tops: List[str]) -> List[str]:
+            variations = denormalize_list(tops)
+            prefixed_variations = [prefix + top for prefix in prefixes for top in variations]
+            return variations + prefixed_variations
+
+        thurayya_df['toponyms'] = thurayya_df['toponyms'].apply(get_all_variations)
+        Toponyms.__df = thurayya_df.explode('toponyms', ignore_index=True)
+        Toponyms.__places = Toponyms.__df['toponyms'].to_list()
         regions = regions_df['REGION'].to_list()
         Toponyms.__regions = regions + [prefix + reg for prefix in prefixes for reg in regions]
 
         Toponyms.__total = Toponyms.__places + Toponyms.__regions
         Toponyms.__rpl = [(elem, elem.replace(' ', '_')) for elem in Toponyms.__total if ' ' in elem]
 
     @staticmethod
@@ -52,7 +61,22 @@
     @staticmethod
     def total() -> List[str]:
         return Toponyms.__total
 
     @staticmethod
     def replacements() -> List[Tuple[str, str]]:
         return Toponyms.__rpl
+
+    @staticmethod
+    def look_up_entity(entity: str) -> Tuple[str, str, List[str], List[str]]:
+        if entity in Toponyms.__places:
+            matches = Toponyms.__df.loc[Toponyms.__df['toponyms'].str.fullmatch(entity), ['uri', 'placeLabel',
+                                                                                          'province']]
+            uris = matches['uri'].to_list()
+            provinces = matches['province'].to_list()
+            place = matches['placeLabel'].unique()
+            if len(place) == 1:
+                return place[0], '@' + '@'.join(uris) + '@', uris, provinces
+            else:
+                return '::'.join(place), '@' + '@'.join(uris) + '@', uris, provinces
+        else:
+            return entity, '', [], []
```

### Comparing `eis1600-0.8.0/eis1600/helper/Singleton.py` & `eis1600-0.8.1/eis1600/helper/Singleton.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.0/eis1600/helper/fix_miu_annotation.py` & `eis1600-0.8.1/eis1600/helper/fix_miu_annotation.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import re
 from glob import glob
 from p_tqdm import p_uimap
-from eis1600.preprocessing.methods import get_yml_and_MIU_df, write_updated_miu_to_file
+from eis1600.processing.preprocessing import get_yml_and_miu_df
+from eis1600.processing.postprocessing import write_updated_miu_to_file
 
 
 sheikhuna = re.compile('[و]?شيخنا')
 
 
 def untag_sheikhuna(row):
     if row['TOKENS'] and sheikhuna.match(row['TOKENS']) and row['TAGS_LISTS'] and [tag for tag in row['TAGS_LISTS']
@@ -21,15 +22,15 @@
 
 def check_file(file):
     with open(file, 'r+', encoding='utf-8') as fh:
         fh.readline()
         fh.readline()
         if fh.readline() == 'reviewed    : REVIEWED2\n':
             fh.seek(0)
-            yml, df = get_yml_and_MIU_df(fh)
+            yml, df = get_yml_and_miu_df(fh)
             df['TAGS_LISTS'], changed = zip(*df[['TOKENS', 'TAGS_LISTS']].apply(untag_sheikhuna, axis=1))
             if any(changed):
                 write_updated_miu_to_file(fh, yml, df)
 
 
 def main():
     files = glob('*.EIS1600')
```

### Comparing `eis1600-0.8.0/eis1600/helper/miu_random_revisions.py` & `eis1600-0.8.1/eis1600/helper/miu_random_revisions.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.0/eis1600/helper/repo.py` & `eis1600-0.8.1/eis1600/helper/repo.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 :function travers_eis1600_dir(path, file_ext_from, file_ext_to): Discontinued
 """
 import re
 from glob import glob
 from os.path import split, splitext
 from typing import List, Literal, Optional
 
-from eis1600.markdown.re_pattern import FIXED_POETRY_OLD_PATH_PATTERN
+from eis1600.helper.markdown_patterns import FIXED_POETRY_OLD_PATH_PATTERN
 
 
 def get_entry(file_name: str, checked_entry: bool) -> str:
     """Formats README entry for that file_name.
 
     Only used internally.
     :param str file_name: The name of the file whose entry is added to the README
@@ -151,20 +151,18 @@
 
 
 def read_files_from_autoreport(path: str) -> List[str]:
     """Get the list of files from the README to process further.
 
     Get the list of files from the README which are to be processed in further steps.
     :param str path: The root of the text repo, path to the README
-    :param str which: The section heading from the README indicating the section from which to read the file list from.
-    :param bool only_checked: If True, only read those lines with a ticked checkbox, defaults to True.
     :return list[str]: List of URIs from files to process further
     """
 
-    which_pattern = re.compile('## DOUBLE-CHECKED Files \(\d+\) - ready for MIU\n')
+    which_pattern = re.compile(r'## DOUBLE-CHECKED Files \(\d+\) - ready for MIU\n')
     file_list = []
 
     try:
         with open(path + 'AUTOREPORT.md', 'r', encoding='utf8') as autoreport_h:
             line = next(autoreport_h)
             # Find section in the AUTOREPORT to read from
             while not which_pattern.match(line):
```

### Comparing `eis1600-0.8.0/eis1600/markdown/UIDs.py` & `eis1600-0.8.1/eis1600/markdown/UIDs.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,25 +23,28 @@
         """
 
         ids = []
         for i in range(0, 5000000):
             ids.append(randint(400000000000, 999999999999))
         return set(ids)
 
-    IDS = _generate_ids.__func__()
-    """Set of 5000000 random UIDs generated once and shared by all instances of this class."""
+    IDS = None
 
     def __init__(self, existing_uids: Optional[List[int]] = None) -> None:
         """Constructor method, creates an individual set uids per instance.
 
         Adaptes the pre-generated set of UIDs to the current instance by subtracting already existing UIDs,
         if this list was given to the constructor. Otherwise it uses a copy of the static IDS set.
         :param List[int] existing_uids: List of already used UIDs in the current text.
         """
 
+        if UIDs.IDS is None:
+            """Set of 5000000 random UIDs generated once and shared by all instances of this class."""
+            UIDs.IDS = UIDs._generate_ids()
+
         if existing_uids:
             self.ids = UIDs.IDS.difference(existing_uids)
         else:
             self.ids = copy(UIDs.IDS)
 
         self.iter = self.ids.__iter__()
```

### Comparing `eis1600-0.8.0/eis1600/markdown/convert_mARkdown_to_EIS1600TMP.py` & `eis1600-0.8.1/eis1600/markdown/convert_mARkdown_to_EIS1600TMP.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.0/eis1600/markdown/insert_uids.py` & `eis1600-0.8.1/eis1600/markdown/insert_uids.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.0/eis1600/markdown/methods.py` & `eis1600-0.8.1/eis1600/markdown/methods.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from typing import Optional
 
 from os.path import split, splitext
 
 from eis1600.markdown.UIDs import UIDs
-from eis1600.markdown.re_pattern import EMPTY_FIRST_PARAGRAPH_PATTERN, EMPTY_PARAGRAPH_PATTERN, HEADER_END_PATTERN, \
-    MIU_LIGHT_OR_EIS1600_PATTERN, MIU_TAG_AND_TEXT_PATTERN, NORMALIZE_BIO_CHR_MD_PATTERN, ONLY_PAGE_TAG_PATTERN, \
+from eis1600.helper.markdown_patterns import EMPTY_FIRST_PARAGRAPH_PATTERN, EMPTY_PARAGRAPH_PATTERN, \
+    HEADER_END_PATTERN, \
+    MIU_TAG_AND_TEXT_PATTERN, NORMALIZE_BIO_CHR_MD_PATTERN, ONLY_PAGE_TAG_PATTERN, \
     PAGE_TAG_IN_BETWEEN_PATTERN, \
     PAGE_TAG_PATTERN, \
     PAGE_TAG_SPLITTING_PARAGRAPH_PATTERN, SPACES_CROWD_PATTERN, NEWLINES_CROWD_PATTERN, \
-    POETRY_PATTERN, SPACES_AFTER_NEWLINES_PATTERN, PAGE_TAG_ON_NEWLINE_PATTERN, TAG_AND_TEXT_SAME_LINE_PATTERN, \
+    POETRY_PATTERN, SPACES_AFTER_NEWLINES_PATTERN, PAGE_TAG_ON_NEWLINE_PATTERN, UID_TAG_AND_TEXT_SAME_LINE_PATTERN, \
     UID_PATTERN, \
     HEADING_OR_BIO_PATTERN, \
     BIO_CHR_TO_NEWLINE_PATTERN
 
 
 def normalize_bio_chr_md(paragraph: str) -> str:
     md = NORMALIZE_BIO_CHR_MD_PATTERN.match(paragraph).group(0)
@@ -57,15 +58,15 @@
         print(f'Convert {uri} from mARkdown to EIS1600 file')
 
     with open(infile, 'r', encoding='utf8') as infile_h:
         text = infile_h.read()
 
     header_and_text = HEADER_END_PATTERN.split(text)
     header = header_and_text[0] + header_and_text[1]
-    text = header_and_text[2][1:]   # Ignore second new line after #META#Header#End#
+    text = header_and_text[2][1:]  # Ignore second new line after #META#Header#End#
 
     if text[0:2] == '#\n':
         # Some texts start with a plain #, remove these
         text = text[2:]
 
     # fix
     text = text.replace('~\n', '\n')
@@ -135,15 +136,15 @@
 
     with open(infile, 'r', encoding='utf8') as infile_h:
         text = infile_h.read()
 
     # disassemble text into paragraphs
     header_and_text = HEADER_END_PATTERN.split(text)
     header = header_and_text[0] + header_and_text[1]
-    text = header_and_text[2][1:]   # Ignore second new line after #META#Header#End#
+    text = header_and_text[2][1:]  # Ignore second new line after #META#Header#End#
     text = NEWLINES_CROWD_PATTERN.sub('\n\n', text)
     text = text.split('\n\n')
     text_updated = []
 
     uids = UIDs()
 
     text_iter = text.__iter__()
@@ -179,17 +180,17 @@
                             text_updated[-1] += ' ' + page_tag + ' ' + next_p
                         prev_p = paragraph
                         paragraph = next_p
                         next_p = next(text_iter, None)
                 elif text_updated:
                     text_updated[-1] += ' ' + page_tag
                 # else:
-                    # Remove PageV00P000 at the beginning in an individual paragraph
-                    # text_updated.append(paragraph)
-                    # pass
+                # Remove PageV00P000 at the beginning in an individual paragraph
+                # text_updated.append(paragraph)
+                # pass
             else:
                 paragraph = f'_ء_={uids.get_uid()}= ::UNDEFINED:: ~\n' + paragraph
                 text_updated.append(paragraph)
 
         prev_p = paragraph
         paragraph = next_p
 
@@ -220,15 +221,15 @@
 
     with open(infile, 'r', encoding='utf8') as infile_h:
         text = infile_h.read()
 
     # disassemble text into paragraphs
     header_and_text = HEADER_END_PATTERN.split(text)
     header = header_and_text[0] + header_and_text[1]
-    text = header_and_text[2][1:]   # Ignore second new line after #META#Header#End#
+    text = header_and_text[2][1:]  # Ignore second new line after #META#Header#End#
     text = NEWLINES_CROWD_PATTERN.sub('\n\n', text)
     text = text.split('\n\n')
     text_updated = []
 
     used_ids = []
 
     # Collect existing UIDs
@@ -270,25 +271,23 @@
                 heading_and_text = paragraph.splitlines()
                 if len(heading_and_text) > 1:
                     paragraph = heading_and_text[0] + f'\n\n_ء_={uids.get_uid()}= ::UNDEFINED:: ~\n' + \
                                 heading_and_text[1]
             elif not UID_PATTERN.match(paragraph):
                 section_header = '' if paragraph.startswith('::') else '::UNDEFINED:: ~\n'
                 paragraph = f'_ء_={uids.get_uid()}= {section_header}' + paragraph
-            elif TAG_AND_TEXT_SAME_LINE_PATTERN.match(paragraph):
-                paragraph = TAG_AND_TEXT_SAME_LINE_PATTERN.sub(r'\1\n\2', paragraph)
+            elif UID_TAG_AND_TEXT_SAME_LINE_PATTERN.match(paragraph):
+                paragraph = UID_TAG_AND_TEXT_SAME_LINE_PATTERN.sub(r'\1\2\n\3', paragraph)
                 # Insert a paragraph tag
                 heading_and_text = paragraph.splitlines()
-                paragraph = heading_and_text[0] + f'\n\n_ء_={uids.get_uid()}= ::UNDEFINED:: ~\n' + \
-                            heading_and_text[1]
+                paragraph = heading_and_text[0] + f'\n\n_ء_={uids.get_uid()}= ::UNDEFINED:: ~\n' + heading_and_text[1]
             elif MIU_TAG_AND_TEXT_PATTERN.match(paragraph):
                 # Insert a paragraph tag
                 heading_and_text = paragraph.splitlines()
-                paragraph = heading_and_text[0] + f'\n\n_ء_={uids.get_uid()}= ::UNDEFINED:: ~\n' + \
-                            heading_and_text[1]
+                paragraph = heading_and_text[0] + f'\n\n_ء_={uids.get_uid()}= ::UNDEFINED:: ~\n' + heading_and_text[1]
 
             if ONLY_PAGE_TAG_PATTERN.fullmatch(paragraph):
                 # Add page tags to previous paragraph if there is no other information contained in the current
                 # paragraph
                 page_tag = ONLY_PAGE_TAG_PATTERN.match(paragraph).group('page_tag')
                 if PAGE_TAG_IN_BETWEEN_PATTERN.search('\n\n'.join([prev_p, paragraph, next_p])):
                     if text_updated:
@@ -299,17 +298,17 @@
                             text_updated[-1] += ' ' + page_tag + ' ' + next_p_text
                         prev_p = paragraph
                         paragraph = next_p
                         next_p = next(text_iter, None)
                 elif text_updated:
                     text_updated[-1] += ' ' + page_tag
                 # else:
-                    # Remove PageV00P000 at the beginning in an individual paragraph
-                    # text_updated.append(paragraph)
-                    # pass
+                # Remove PageV00P000 at the beginning in an individual paragraph
+                # text_updated.append(paragraph)
+                # pass
             elif not EMPTY_PARAGRAPH_PATTERN.fullmatch(paragraph):
                 # Do not add empty paragraphs to the updated text
                 text_updated.append(paragraph)
         prev_p = paragraph
         paragraph = next_p
 
     # reassemble text
```

### Comparing `eis1600-0.8.0/eis1600/markdown/re_pattern.py` & `eis1600-0.8.1/eis1600/helper/markdown_patterns.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import re
 
+from eis1600.helper.entity_tags import get_entity_tags
+
 AR_LETTERS_CHARSET = frozenset(
         u'\u0621\u0622\u0623\u0624\u0625\u0626\u0627'
         u'\u0628\u0629\u062a\u062b\u062c\u062d\u062e'
         u'\u062f\u0630\u0631\u0632\u0633\u0634\u0635'
         u'\u0636\u0637\u0638\u0639\u063a\u0640\u0641'
         u'\u0642\u0643\u0644\u0645\u0646\u0647\u0648'
         u'\u0649\u064a\u0671\u067e\u0686\u06a4\u06af'
 )
-AR_STR = r'[' + u''.join(AR_LETTERS_CHARSET) + ']+'
+AR_CHR = r'[' + u''.join(AR_LETTERS_CHARSET) + ']'
+AR_STR = AR_CHR + '+'
 AR_STR_AND_TAGS = r'[' + u''.join(AR_LETTERS_CHARSET) + 'a-zA-ZÜ0-9]+'
 WORD = r'(?:\s' + AR_STR + ')'
 
 # EIS1600 mARkdown
 UID = r'_ء_(#)?=(?P<UID>\d{12})= '
 UID_PATTERN = re.compile(UID)
 MIU_UID = r'_ء_#=(?P<UID>\d{12})= '
@@ -36,21 +39,25 @@
 MIU_TAG_PATTERN = re.compile(r'(' + MIU_UID + r'(?P<category>[^\n]+))')
 CATEGORY_PATTERN = re.compile(r'[$|@]+(?:[A-Z]+[|])?')
 SECTION_TAG = r'_ء_=\d{12}= ::[A-Z]+:: ~'
 SECTION_PATTERN = re.compile(SECTION_TAG)
 SECTION_SPLITTER_PATTERN = re.compile(r'\n\n(' + SECTION_TAG + ')\n(?:_ء_)?')
 TAG_PATTERN = re.compile(r'Ü?(?:[a-zA-Z0-9_%~]+(?:\.[a-zA-Z0-9_%~]+)?)|' + PAGE_TAG + '|(?:::)')
 NOR_DIGIT_NOR_AR_STR = r'[^\d\n' + u''.join(AR_LETTERS_CHARSET) + ']+?'
-TAG_AND_TEXT_SAME_LINE_PATTERN = re.compile(
-        r'(_ء_#=\d{12}= [$@]+(?:' + NOR_DIGIT_NOR_AR_STR + r')?(?:\d+)?(?:' + NOR_DIGIT_NOR_AR_STR + r')?) ('
-                                                                                                               r'(?:\( ?)?' +
-        AR_STR + r')'
-)
+TAG_AND_TEXT_SAME_LINE = r'([$@]+' + NOR_DIGIT_NOR_AR_STR + r'\d*' + NOR_DIGIT_NOR_AR_STR + r') ?((?:[(\[] ?)?' + AR_STR + r')'
+UID_TAG_AND_TEXT_SAME_LINE_PATTERN = re.compile(
+        r'(_ء_#=\d{12}= )' + TAG_AND_TEXT_SAME_LINE)
 MIU_TAG_AND_TEXT_PATTERN = re.compile(r'(' + MIU_UID + r'[$@]+?(?: \d+)?)\n((?:\( ?)?' + AR_STR + r')')
 
+# MIU entity tags
+entity_tags = '|'.join(get_entity_tags())
+ENTITY_TAGS_PATTERN = re.compile(r'Ü?(?P<entity>' + entity_tags + r')(?P<length>\d{1,2})(?:[A-Z0-9]+)?')
+YEAR_PATTERN = re.compile(r'Ü?Y\d{1,2}(?P<cat>[A-Z])(?P<written>\d{4})(?P<i>I)?Y(?P<real>\d{4})?')
+AGE_PATTERN = re.compile(r'Ü?A\d(?P<cat>[A-Z])(?P<written>\d{2,3})(?P<i>I)?A(?P<real>\d{2,3})?')
+
 # EIS1600 light mARkdown
 HEADING_OR_BIO_PATTERN = re.compile(r'# [|$]+')
 MIU_LIGHT_OR_EIS1600_PATTERN = re.compile(r'#|_ء_#')
 
 # Fix mARkdown files
 SPACES_CROWD_PATTERN = re.compile(r' +')
 NEWLINES_CROWD_PATTERN = re.compile(r'\n{3,}')
@@ -63,14 +70,11 @@
 BELONGS_TO_PREV_PARAGRAPH_PATTERN = re.compile(r'\n(.{1,10})\n')
 PAGE_TAG_ON_NEWLINE_PATTERN = re.compile(r'\n' + PAGE_TAG)
 PAGE_TAG_SPLITTING_PARAGRAPH_PATTERN = re.compile(
         '(' + AR_STR + ' ?)' + r'\n\n' + PAGE_TAG + r'\n\n' + '(' + AR_STR +
         ')'
 )
 NORMALIZE_BIO_CHR_MD_PATTERN = re.compile('# ([$@]((BIO|CHR)_[A-Z]+[$@])| RAW)')
-BIO_CHR_TO_NEWLINE_PATTERN = re.compile(
-        r'(# [$@]+(?:' + NOR_DIGIT_NOR_AR_STR + r')?(?:\d+)?(?:' + NOR_DIGIT_NOR_AR_STR + r')?) ((?:(?:\(|\[) ?)?'
-        + AR_STR + r')'
-)
+BIO_CHR_TO_NEWLINE_PATTERN = re.compile(TAG_AND_TEXT_SAME_LINE)
 
 # Fixed poetry old file path pattern
 FIXED_POETRY_OLD_PATH_PATTERN = re.compile(r'/Users/romanov/_OpenITI/_main_corpus/\w+/data/')
```

### Comparing `eis1600-0.8.0/eis1600/markdown/update_uids.py` & `eis1600-0.8.1/eis1600/markdown/update_uids.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.0/eis1600/markdown/update_uids_old_process.py` & `eis1600-0.8.1/eis1600/markdown/update_uids_old_process.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import sys
 import os
 from argparse import ArgumentParser, Action, RawDescriptionHelpFormatter
 from multiprocessing import Pool
 
 from eis1600.helper.repo import get_files_from_eis1600_dir, write_to_readme, read_files_from_readme
-from eis1600.markdown.re_pattern import BIO_CHR_TO_NEWLINE_PATTERN, HEADER_END_PATTERN, HEADING_OR_BIO_PATTERN, \
+from eis1600.helper.markdown_patterns import BIO_CHR_TO_NEWLINE_PATTERN, HEADER_END_PATTERN, HEADING_OR_BIO_PATTERN, \
     MIU_LIGHT_OR_EIS1600_PATTERN, NEWLINES_CROWD_PATTERN, UID_PATTERN
 
 
 class CheckFileEndingAction(Action):
     def __call__(self, parser, namespace, input_arg, option_string=None):
         if input_arg and os.path.isfile(input_arg):
             filepath, fileext = os.path.splitext(input_arg)
```

### Comparing `eis1600-0.8.0/eis1600/miu/HeadingTracker.py` & `eis1600-0.8.1/eis1600/miu/HeadingTracker.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 import copy
+import json
 
-from typing import Dict, Optional, Type
+from typing import Dict, Optional
 
 
 class HeadingTracker:
     """A class to keep track of the super elements of a MIU.
 
     This class keeps track of the headings on different levels to keep this information in the MIU YAML header. Some
     headings are empty stings
@@ -30,48 +31,55 @@
 
     def __iter__(self):
         """Iterate over headings which are not None. Omits page_tag."""
         for key, val in self.__dict__.items():
             if key.startswith('h') and val is not None:
                 yield key, val
 
-    def get_curr_state(self) -> Type[HeadingTracker]:
+    def get_curr_state(self) -> HeadingTracker:
         """Get current state of the tacker as deepcopy.
 
         Returns a deepcopy of the current state.
-        :returns HeadingTracker: Deepcopy of the current state of the tracker.
+        :return HeadingTracker: Deepcopy of the current state of the tracker.
         """
 
         return copy.deepcopy(self)
 
     def get_yamlfied(self) -> str:
         """Stringifies HeadingTracker in YAML format, only includes levels which are set.
 
         :return str: returns the HeadingTracker in YAML format as a string.
         """
 
         if self.h1 is None:
             return '[]'
 
         heading_tracker_str = '\n'
-        heading_tracker_str += '    - h1    : "' + self.h1 + '"\n'
+        heading_tracker_str += '    - h1    : \'' + self.h1 + '\'\n'
         if self.h2 is not None:
-            heading_tracker_str += '    - h2    : "' + self.h2 + '"\n'
+            heading_tracker_str += '    - h2    : \'' + self.h2 + '\'\n'
             if self.h3 is not None:
-                heading_tracker_str += '    - h3    : "' + self.h3 + '"\n'
+                heading_tracker_str += '    - h3    : \'' + self.h3 + '\'\n'
                 if self.h4 is not None:
-                    heading_tracker_str += '    - h4    : "' + self.h4 + '"\n'
+                    heading_tracker_str += '    - h4    : \'' + self.h4 + '\'\n'
 
         if self.page_tag:
-            heading_tracker_str += '    - page_tag    : "' + self.page_tag + '"'
+            heading_tracker_str += '    - page_tag    : \'' + self.page_tag + '\''
         else:
             heading_tracker_str = heading_tracker_str[:-1]
 
         return heading_tracker_str
 
+    def to_json(self) -> Dict:
+        json_dict = {}
+        for key, val in vars(self).items():
+            if val is not None:
+                json_dict[key] = val
+        return json_dict
+
     def track_headings(self, level: int, heading: str) -> None:
         """Checks which of the levels changed and sets all sub levels to None (some headings are just an empty string).
 
         :param int level: The level of the heading indicated by the number of leading `|`.
         :param str heading: The new heading text for the given level.
         """
```

### Comparing `eis1600-0.8.0/eis1600/miu/YAMLHandler.py` & `eis1600-0.8.1/eis1600/miu/YAMLHandler.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,56 @@
 from __future__ import annotations
 
-from typing import Any, Dict, Optional, Type
+from typing import Any, Dict, List, Optional, Tuple
 
-from eis1600.markdown.re_pattern import MIU_HEADER
+from eis1600.helper.markdown_patterns import MIU_HEADER
 from eis1600.miu.HeadingTracker import HeadingTracker
 
 
 class YAMLHandler:
     """A class to take care of the MIU YAML Headers
 
     :param Dict yml: the YAML header as a dict, optional.
     :ivar Literal['NOT REVIEWED', 'REVIEWED'] reviewed: Indicates if the file has manually been reviewed, defaults to
     'NOT REVIEWED'.
     :ivar str reviewer: Initials of the reviewer if the file was already manually reviewed, defaults to None.
     :ivar HeadingTracker headings: HeadingTracker returned by the get_curr_state method of the HeaderTracker.
-    :ivar List[str] dates_headings: List of dates contained in headings
-    :ivar List[str] dates: List of dates contained in text
-    :ivar str nasab_filtered: unanalysed nasab str, parts are connected by '_'.
+    :ivar List[str] dates_headings: List of dates tags contained in headings.
+    :ivar List[int] dates: List of dates contained in the text.
+    :ivar Dict onomstics: contains onomastic elements by category.
     :ivar str category: String categorising the type of the entry, bio, chr, dict, etc.
     """
 
     @staticmethod
     def __parse_yml_val(val: str) -> Any:
-        if val.startswith('"'):
-            return val.strip('"')
-        elif val.isdigit():
+        if val.isdigit():
             return int(val)
         elif val == 'True':
             return True
         elif val == 'False':
             return False
-        elif val == 'None':
+        elif val == 'None' or val == '':
             return None
-        elif val.startswith('["'):
-            val_list = val.strip('[]')
-            val_list = val_list.replace('"', '')
-            return val_list.split(',')
+        elif val.startswith(('\'', '"')):
+            return val.strip('\'"')
+        elif val.startswith('['):
+            # List - no comma allowed in strings, it is used as the separator!
+            raw_val_list = val.strip('[]')
+            if raw_val_list.startswith('(') and raw_val_list.endswith(')'):
+                # List of tuples
+                val_list = raw_val_list.strip('()').split('), (')
+                values = []
+                for v in val_list:
+                    t = v.split(', ')
+                    values.append((YAMLHandler.__parse_yml_val(t[0]), YAMLHandler.__parse_yml_val(t[1])))
+            else:
+                # List of other values
+                val_list = raw_val_list.split(', ')
+                values = [YAMLHandler.__parse_yml_val(v) for v in val_list]
+            return values
         else:
             return val
 
     @staticmethod
     def __parse_yml(yml_str: str) -> Dict:
         yml = {}
         level = []
@@ -72,78 +83,102 @@
 
     def __init__(self, yml: Optional[Dict] = None) -> None:
         self.reviewed = 'NOT REVIEWED'
         self.reviewer = None
         self.headings = None
         self.dates_headings = None
         self.dates = None
+        self.onomastics = {}
         self.nasab_filtered = None
         self.category = None
+        self.ambigious_toponyms = False
 
         if yml:
             for key, val in yml.items():
                 if key == 'headings':
                     val = HeadingTracker(val)
                 self.__setattr__(key, val)
 
     @classmethod
-    def from_yml_str(cls, yml_str: str) -> Type[YAMLHandler]:
+    def from_yml_str(cls, yml_str: str) -> YAMLHandler:
         """Return instance with attr set from the yml_str."""
         return cls(YAMLHandler.__parse_yml(yml_str))
 
     def set_category(self, category: str) -> None:
         self.category = category
 
-    def set_headings(self, headings: Type[HeadingTracker]) -> None:
+    def set_ambigious_toponyms(self) -> None:
+        self.ambigious_toponyms = True
+
+    def set_headings(self, headings: HeadingTracker) -> None:
         self.headings = headings
 
     def unset_reviewed(self) -> None:
         self.reviewed = 'NOT REVIEWED'
         self.reviewer = None
 
     def get_yamlfied(self) -> str:
         yaml_str = MIU_HEADER + 'Begin#\n\n'
         for key, val in vars(self).items():
-            if key.startswith('dates') and val is not None:
-                yaml_str += key + '    : ['
-                for date in val:
-                    yaml_str += '"' + date + '",'
-                yaml_str = yaml_str[:-1]
-                yaml_str += ']\n'
-            elif key == 'category' and val is not None:
-                yaml_str += key + '    : "' + val + '"\n'
-            else:
+            if key == 'category' and val is not None:
+                yaml_str += key + '    : \'' + val + '\'\n'
+            elif isinstance(val, dict):
+                yaml_str += key + '    :\n'
+                for key2, val2 in val.items():
+                    yaml_str += '   - ' + key2 + '  : ' + str(val2) + '\n'
+            elif val is not None:
                 yaml_str += key + '    : ' + str(val) + '\n'
         yaml_str += '\n' + MIU_HEADER + 'End#\n\n'
 
         return yaml_str
 
+    def to_json(self) -> Dict:
+        json_dict = {}
+        for key, val in vars(self).items():
+            if val is not None:
+                json_dict[key] = val
+        return json_dict
+
     def is_bio(self) -> bool:
         return self.category == '$' or self.category == '$$'
 
     def is_reviewed(self) -> bool:
-        return self.reviewed == 'REVIEWED'
+        return self.reviewed.startswith('REVIEWED')
 
-    def add_date(self, date_tag: str) -> None:
+    def add_date(self, date: int) -> None:
         if self.dates:
-            if date_tag not in self.dates:
-                self.dates.append(date_tag)
+            if date not in self.dates:
+                self.dates.append(date)
         else:
-            self.dates = [date_tag]
+            self.dates = [date]
 
-    def add_date_headings(self, date_tag: str) -> None:
+    def add_date_headings(self, date: int) -> None:
         if self.dates_headings:
-            if date_tag not in self.dates_headings:
-                self.dates_headings.append(date_tag)
+            if date not in self.dates_headings:
+                self.dates_headings.append(date)
         else:
-            self.dates_headings = [date_tag]
+            self.dates_headings = [date]
+
+    def add_nas(self, nas: List[Tuple[int, str]]) -> None:
+        if hasattr(self, 'onomastics') and self.onomastics:
+            self.onomanstics['nas'] = nas
+        else:
+            self.onomastics = {'nas': nas}
 
     def add_nasab_filtered(self, nasab_filtered: str) -> None:
         self.nasab_filtered = nasab_filtered
 
+    def add_tagged_entities(self, entities_dict: dict) -> None:
+        for key, val in entities_dict.items():
+            if key == 'onomastics' and hasattr(self, 'onomastics') and self.onomastics:
+                for key2, val2 in val.items():
+                    self.onomastics[key2] = val2
+            else:
+                self.__setattr__(key, val)
+
     def __setitem__(self, key: str, value: Any) -> None:
         super().__setattr__(key, value)
 
     def __repr__(self) -> str:
         return str(self.__dict__)
 
     def __str__(self) -> str:
```

### Comparing `eis1600-0.8.0/eis1600/miu/disassemble_into_miu_files.py` & `eis1600-0.8.1/eis1600/miu/disassemble_into_miu_files.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.0/eis1600/miu/methods.py` & `eis1600-0.8.1/eis1600/miu/methods.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from glob import glob
 from logging import Logger
 from os.path import splitext, split, exists
-from typing import List, Optional, Type
+from typing import List, Optional
 from pathlib import Path
 
 from eis1600.onomastics.methods import nasab_annotate_miu
 
 from eis1600.dates.methods import date_annotate_miu_text
 from eis1600.miu.HeadingTracker import HeadingTracker
-from eis1600.preprocessing.methods import get_yml_and_MIU_df, write_updated_miu_to_file
+from eis1600.processing.preprocessing import get_yml_and_miu_df
+from eis1600.processing.postprocessing import write_updated_miu_to_file
 from eis1600.nlp.utils import camel2md_as_list, annotate_miu_text
 from eis1600.miu.yml_handling import create_yml_header, extract_yml_header_and_text
-from eis1600.markdown.re_pattern import CATEGORY_PATTERN, HEADER_END_PATTERN, HEADING_PATTERN, MIU_TAG_PATTERN, \
+from eis1600.helper.markdown_patterns import CATEGORY_PATTERN, HEADER_END_PATTERN, HEADING_PATTERN, MIU_TAG_PATTERN, \
     MIU_UID_PATTERN, PAGE_TAG_PATTERN
 
 
 def disassemble_text(infile: str, out_path: str, verbose: Optional[bool] = None) -> None:
     """Disassemble text into MIU files.
 
     Retrieve MIU files by disassembling the text based on the EIS1600 mARkdown.
@@ -162,32 +163,33 @@
 
     # if the file is already annotated, do nothing
     if exists(tsv_path) and not force_annotation:
         return
 
     with open(path, 'r+', encoding='utf-8') as miu_file_object:
         # 1. open miu file and disassemble the file to its parts
-        yml_handler, df = get_yml_and_MIU_df(miu_file_object)
+        yml_handler, df = get_yml_and_miu_df(miu_file_object)
 
         # 2. annotate NEs and lemmatize
         df['NER_LABELS'], df['LEMMAS'], df['POS_TAGS'] = annotate_miu_text(df)
 
         # 3. convert cameltools labels format to markdown format
         df['NER_TAGS'] = camel2md_as_list(df['NER_LABELS'].tolist())
 
         # 4. annotate dates
         df['DATE_TAGS'] = date_annotate_miu_text(df[['TOKENS']], yml_handler)
 
         # 5. annotate onomastic information
-        df['NASAB_TAGS'] = nasab_annotate_miu(df, yml_handler, logger)
+        # TODO Needs to be run after the NASAB END tag was inserted
+        df['NASAB_TAGS'] = nasab_annotate_miu(df, yml_handler, path, logger)
 
-        # 5. save csv file
+        # 6. save csv file
         df.to_csv(tsv_path, index=False, sep='\t')
 
-        # 6. reconstruct the text and save it to the output file
+        # 7. reconstruct the text, populate yml with annotated entities and save it to the output file
         if output_path == path:
             write_updated_miu_to_file(
                 miu_file_object, yml_handler, df[['SECTIONS', 'TOKENS', 'TAGS_LISTS', 'NER_TAGS',
                                                  'DATE_TAGS', 'NASAB_TAGS']]
                 )
         else:
             with open(output_path, 'w', encoding='utf-8') as out_file_object:
```

### Comparing `eis1600-0.8.0/eis1600/miu/reassemble_from_miu_files.py` & `eis1600-0.8.1/eis1600/miu/reassemble_from_miu_files.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.0/eis1600/nlp/cameltools.py` & `eis1600-0.8.1/eis1600/nlp/cameltools.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.0/eis1600/nlp/ner_annotate_mius.py` & `eis1600-0.8.1/eis1600/nlp/ner_annotate_mius.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.0/eis1600/nlp/utils.py` & `eis1600-0.8.1/eis1600/nlp/utils.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -62,8 +62,8 @@
                 if temp_class is not None:
                     temp_tokens.append(_label)
                 else:
                     converted_tokens.append(default_str)
     if len(temp_tokens) > 0 and temp_class is not None:
         converted_tokens.append(f"{types_mapping.get(temp_class, 'ÜM')}{len(temp_tokens)}")
         converted_tokens.extend([default_str] * (len(temp_tokens) - 1))
-    return converted_tokens
+    return converted_tokens
```

### Comparing `eis1600-0.8.0/eis1600/onomastics/methods.py` & `eis1600-0.8.1/eis1600/onomastics/methods.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,151 +3,181 @@
 from typing import Optional
 
 import pandas as pd
 from numpy import nan
 from pandas import Series
 
 from eis1600.miu.YAMLHandler import YAMLHandler
-
 from eis1600.gazetteers.Onomastics import Onomastics
 from eis1600.gazetteers.Toponyms import Toponyms
-from eis1600.onomastics.re_pattern import ABU_ABI, BANU_BANI, IBN_IBNA, BN_BNT, DIN_DAULA, DATES, PARENTHESIS, \
-    QUOTES, PUNCTUATION, SPACES, SPELLING, UMM, YURIFA_K_BI
-from eis1600.preprocessing.methods import get_tokens_and_tags, get_yml_and_MIU_df, reconstruct_miu_text_with_tags, \
-    write_updated_miu_to_file
+from eis1600.onomastics.re_pattern import ABU, ABI, BANU_BANI, CRF_PATTERN, IBN_IBNA, BN_BNT, SHR_PATTERN, SPELLING, UMM
+from eis1600.processing.preprocessing import get_tokens_and_tags, get_yml_and_miu_df
+from eis1600.processing.postprocessing import reconstruct_miu_text_with_tags, write_updated_miu_to_file
 
 
-def nasab_filtering(nasab_text: str, yml_handler: YAMLHandler, logger_nasab: Logger) -> None:
-    """Filters elements from the nasab which were not recognized by the current onomastic gazetteer.
-
-    Filters elements from the nasab which were not recognized by the current onomastic gazetteer. Unrecognized uni-
-    and bi-grams are logged and the manipulated nasab string is added to the YAMLHandler.
-    :param str nasab_text: nasab text as one single string which was cleaned from spelling information.
-    :param YAMLHandler yml_handler: YAMLHandler of the MIU to which the manipulated nasab string is added.
-    :param Logger logger_nasab: logger for unrecognized uni- and bi-grams.
-    """
+def get_nas(text: str, yml_handler: YAMLHandler) -> str:
     og = Onomastics.instance()
-    tg = Toponyms.instance()
-    text_mnpld = nasab_text
-    text_mnpld = PARENTHESIS.sub(r'\g<1>', text_mnpld)
-    text_mnpld = QUOTES.sub('', text_mnpld)
-    text_mnpld = DATES.sub('', text_mnpld)
-    text_mnpld = PUNCTUATION.sub('', text_mnpld)
-    text_mnpld = SPACES.sub(' ', text_mnpld)
-    m = SPELLING.search(text_mnpld)
-    while m:
-        text_mnpld = text_mnpld[:m.start()] + m.group(0).replace(' ', '_') + text_mnpld[m.end():]
-        m = SPELLING.search(text_mnpld, m.end())
+
+    text_mnpld = ABU.sub(' ابو_', text)
+    text_mnpld = UMM.sub(' ام_', text_mnpld)
+    text_mnpld = ABI.sub(' ابي_', text_mnpld)
+    text_mnpld = IBN_IBNA.sub(r' \g<1>', text_mnpld)
 
     m = og.get_ngrams_regex().search(text_mnpld)
     while m:
         text_mnpld = text_mnpld[:m.start()] + m.group(1) + m.group(2).replace(' ', '_') + text_mnpld[m.end():]
         m = og.get_ngrams_regex().search(text_mnpld, m.end())
 
-    # They should be catched by regex - no manual manipulation
-    # text_mnpld = ABU_ABI.sub(' ابو_', text_mnpld)
-    # text_mnpld = UMM.sub(' ام_', text_mnpld)
-    # text_mnpld = IBN_IBNA.sub(r'\g<1>', text_mnpld)
-    # text_mnpld = BN_BNT.sub(r'_\g<1>_', text_mnpld)
-    # text_mnpld = DIN_DAULA.sub(r'_\g<1>', text_mnpld)
-    # text_mnpld = YURIFA_K_BI.sub('\g<1>_\g<2>_\g<3>', text_mnpld)
-    text_mnpld = BANU_BANI.sub('<بنو_', text_mnpld)
-    for elem in tg.total():
-        text_mnpld = text_mnpld.replace('نائب ' + elem, 'نائب_' + elem)
-    for elem, repl in tg.replacements():
-        text_mnpld = text_mnpld.replace(elem, repl)
+    m_bn = list(BN_BNT.finditer(text_mnpld))
+    if m_bn:
+        start = m_bn[0].start()
+        end = m_bn[-1].end()
+        pos_abu = text_mnpld[start:end].find(' ابو_')
+        pos_umm = text_mnpld[start:end].find(' ام_')
+        pos = max(pos_abu, pos_umm)
+        if pos > 1:
+            end = min(end, start+pos-1)
+        last_ancestor = text_mnpld[end+1:].find(' ')
+        ancestors = BN_BNT.split(text_mnpld[start:end+1+last_ancestor])
+        if ancestors[0] == '':
+            ancestors = ancestors[1:]
+        nas = [(i, txt) for i, txt in enumerate([a for a in ancestors if not a.startswith('بن')])]
+        yml_handler.add_nas(nas)
+        nas_w_tags = ''
+        for elem in ancestors:
+            if not elem.startswith('بن'):
+                num_tokens = len(elem.replace('_', ' ').split())
+                nas_w_tags += ' ÜNAS' + str(num_tokens)
+            nas_w_tags += ' ' + elem
+        text_w_tags = text_mnpld[:start+1].replace('_', ' ') +\
+                      nas_w_tags[1:].replace(' ', '_') + \
+                      text_mnpld[end+1+last_ancestor:].replace('_', ' ')
 
-    yml_handler.add_nasab_filtered(text_mnpld)
+        return text_w_tags
 
-    if logger_nasab:
-        # Log unidentified tokens as uni- and bi-grams
-        tokens = text_mnpld.split()
-        unknown_uni = [t for t in tokens if '_' not in t and t not in og.total() + tg.total()]
-        prev = None
-        unknown_bi = []
-        for t in tokens:
-            if not prev and '_' not in t and t not in og.total() + tg.total() + ['بن', 'بنت']:
-                prev = t
-            else:
-                if '_' not in t and t not in og.total() + tg.total() + ['بن', 'بنت']:
-                    unknown_bi.append(prev + ' ' + t)
-                    prev = t
-                else:
-                    prev = None
-        logger_nasab.info('\n'.join(unknown_uni + unknown_bi))
+    return text_mnpld
 
 
-def tag_nasab(text: str) -> str:
+def tag_nasab(text: str, logger_nasab: Logger) -> str:
     """Annotate the nasab part of the MIU.
 
     :param str text: nasab part of the MIU as one single string.
-    :returns str: the nasab part pf the MIU which contains also the tags in front of the recognized elements.
+    :return str: the nasab part pf the MIU which contains also the tags in front of the recognized elements.
     """
     og = Onomastics.instance()
-    text_updated = text
-    m = og.get_ngrams_regex().search(text_updated)
+    tg = Toponyms.instance()
+    text_mnpld = text.replace(' بن ', ' بن_')
+    # for m in BANU_BANI.finditer(text_mnpld):
+    #     print(f'{m.group(0)} last: {text_mnpld[m.end()]}')
+    text_mnpld = text_mnpld.replace('من ولد ', 'من_ولد_')
+    m = og.get_ngrams_regex().search(text_mnpld)
     while m:
         tag = og.get_ngram_tag(m.group(2))
         pos = m.start()
+        end = m.end()
         if m.group(1) == ' ':
             pos += 1
-        text_updated = text_updated[:pos] + tag + text_updated[pos:]
+        if tag.startswith('ÜEXP'):
+            if CRF_PATTERN.search(m.group(2)) or SHR_PATTERN.search(m.group(2)):
+                tag = 'ÜSHR'
+                if text_mnpld[end:].startswith('ابن '):
+                    tag += '2 '
+                    text_mnpld = text_mnpld[:end] + text_mnpld[end+1:].replace(' ', '_', 1)
+                else:
+                    tag += '1 '
+                if m.group(2).endswith(' ب'):
+                    end -= 1
+
+                text_mnpld = text_mnpld[:end] + tag + text_mnpld[end:]
+                text_mnpld = text_mnpld[:pos] + \
+                             text_mnpld[pos+1:end+len(tag)+1].replace(' ', '_') + \
+                             text_mnpld[end+len(tag)+1:]
+            # else:
+            #     tag = ''
+            #     print(f'start: {text_mnpld[pos:end]} end: {text_mnpld[end:]}')
+        else:
+            text_mnpld = text_mnpld[:pos] + tag + text_mnpld[pos:]
 
-        m = og.get_ngrams_regex().search(text_updated, m.end() + len(tag))
+        end += len(tag)
 
-    return text_updated
+        m = og.get_ngrams_regex().search(text_mnpld, end)
+
+    if logger_nasab:
+        # Log unidentified tokens as uni- and bi-grams
+        filtered = text_mnpld
+        m = og.get_ngrams_regex().search(filtered)
+        while m:
+            filtered = filtered[:m.start()] + m.group(1) + m.group(2).replace(' ', '_') + filtered[m.end():]
+            m = og.get_ngrams_regex().search(filtered, m.end())
+        tokens = [token for token in filtered.split() if not token.startswith('Ü')]
+        unknown_uni = [t for t in tokens if not ('_' in t or t in og.total() + tg.total())]
+        prev = None
+        unknown_bi = []
+        for t in tokens:
+            if not prev and not ('_' in t or t in og.total() + tg.total() + ['بن', 'بنت']):
+                prev = t
+            else:
+                if not ('_' in t or t in og.total() + tg.total() + ['بن', 'بنت']):
+                    unknown_bi.append(prev + ' ' + t)
+                    prev = t
+                else:
+                    prev = None
+        logger_nasab.info('\n'.join(unknown_uni + unknown_bi))
+
+    return text_mnpld.replace('_', ' ')
 
 
 def tag_spelling(text: str) -> str:
     """Tags spelling information which is stated in the nasab part of the MIU text.
 
     Spelling is detected when two elements of the spelling gazetteer are found successively.
     :param str text: the nasab part as one string.
-    :returns str: nasab part as one string including tags for found spelling.
+    :return str: nasab part as one string including tags for found spelling.
     """
     text_updated = text
     m = SPELLING.search(text_updated)
     while m:
         tag = 'ÜSPL' + str(len(m.group(0).split())) + ' '
         pos = m.start()
         text_updated = text_updated[:pos] + tag + text_updated[pos:]
 
         m = SPELLING.search(text_updated, m.end() + len(tag))
 
     return text_updated
 
 
-def nasab_annotate_miu(df: pd.DataFrame, yml_handler: YAMLHandler, logger_nasab: Optional[Logger]) -> Series:
+def nasab_annotate_miu(df: pd.DataFrame, yml_handler: YAMLHandler, file: str, logger_nasab: Optional[Logger]) -> \
+        Series:
     """Onomastic analysis of the nasab part of the MIU.
 
     :param DataFrame df: DataFrame of the MIU.
     :param YAMLHandler yml_handler: YAMLHandler of the MIU.
+    :param Path file: the MIU which was opened.
     :param Logger logger_nasab: logs unrecognized uni- and bi-grams to a log file, optional.
-    :returns Series: a series of the same length as the df containing the nasab tags corresponding to the tokens.
+    :return Series: a series of the same length as the df containing the nasab tags corresponding to the tokens.
     """
-    # TODO this here
-    # if not yml_header.is_bio():
-    #     return [nan] * len(df), yml_handler
-    if '$' not in df.iloc[0]['SECTIONS'] or '$$$' in df.iloc[0]['SECTIONS'] or not yml_handler.is_reviewed():
+    if not yml_handler.is_bio():
         return Series([nan] * len(df))
 
-    # TODO remove, as we have a NLP model which sets the NASAB tag (what about the '::'?)
-    # For not annotated MIUs
-    # idcs = df[df['TOKENS'].notna() & df['TOKENS'].isin(og.end())].index
-    # idx = idcs[0] if idcs.any() else min(49, len(df))
-
     s_notna = df['TAGS_LISTS'].loc[df['TAGS_LISTS'].notna()].apply(lambda tag_list: ','.join(tag_list))
-    idx = s_notna.loc[s_notna.str.contains('NASAB')].index[0]
+    try:
+        idx = s_notna.loc[s_notna.str.contains('NASAB')].index[0]
+    except IndexError:
+        print(
+                f'MIU does not have a NASAB tag, most likely the MIU is not a biography but a cross reference. '
+                f'Check:\n{file}'
+        )
+        return Series([nan] * len(df))
 
-    nasab_idx = df['TOKENS'].loc[df['TOKENS'].notna()].iloc[:idx - 2].index
+    # The following blacklisted elements are considered noise in the text data and are therefore ignored but kept
+    blacklist = ['(', ')', '[', ']', '"', "'", '.', '،', '؟', '!', ':', '؛', ',', ';', '?', '|']
+    nasab_idx = df.loc[df['TOKENS'].notna() & ~df['TOKENS'].isin(blacklist) & df.index.isin(df.iloc[:idx].index)].index
 
     text = ' '.join(df['TOKENS'].loc[nasab_idx])
 
-    nasab_filtering(text, yml_handler, logger_nasab)
-
     tagged_spelling = tag_spelling(text)
     ar_tokens, tags = get_tokens_and_tags(tagged_spelling)
     df.loc[nasab_idx, 'NASAB_TAGS'] = tags
 
     count = 0
     spl_idcs = []
     for row in df.loc[nasab_idx].itertuples():
@@ -156,37 +186,40 @@
         if count > 0:
             count -= 1
             spl_idcs.append(row[0])
 
     nasab_idx = df.loc[nasab_idx.difference(spl_idcs)].index
     text = ' '.join(df['TOKENS'].loc[nasab_idx])
 
-    tagged_onomastics = tag_nasab(text)
+    text_w_mnpld_nas = get_nas(text, yml_handler)
+    tagged_onomastics = tag_nasab(text_w_mnpld_nas, logger_nasab)
     ar_tokens, tags = get_tokens_and_tags(tagged_onomastics)
     df.loc[nasab_idx, 'NASAB_TAGS'] = tags
 
     if idx != len(df):
         # TODO make NASAB stay on same line
         df.loc[idx - 1, 'NASAB_END'] = 'NASAB'
 
     return df['NASAB_TAGS'].to_list()
 
 
-def nasab_annotation(file: Path, logger_nasab: Logger) -> str:
-    """Only used for onomastic_annotation cmdline script"""
+def nasab_annotation(file: str, logger_nasab: Logger) -> str:
+    """Only used for onomastic_annotation cmdline script."""
     with open(file, 'r', encoding='utf-8') as miu_file_object:
-        yml_handler, df = get_yml_and_MIU_df(miu_file_object)
+        yml_handler, df = get_yml_and_miu_df(miu_file_object)
+    if '$' not in df.iloc[0]['SECTIONS'] or '$$$' in df.iloc[0]['SECTIONS'] or not yml_handler.is_reviewed():
+        df['NASAB_TAGS'] = Series([nan] * len(df))
+    else:
+        yml_handler.set_category('$')
+        df['NASAB_TAGS'] = nasab_annotate_miu(df, yml_handler, file, logger_nasab)
 
-    df['NASAB_TAGS'] = nasab_annotate_miu(df, yml_handler, logger_nasab)
     yml_handler.unset_reviewed()
 
     reconstructed_miu = reconstruct_miu_text_with_tags(df[['SECTIONS', 'TOKENS', 'NASAB_TAGS']])
 
     output_path = str(file).replace('training_data', 'training_nasab')
     with open(output_path, 'w', encoding='utf-8') as out_file_object:
         write_updated_miu_to_file(
-            out_file_object, yml_handler, df[['SECTIONS', 'TOKENS', 'TAGS_LISTS', 'NASAB_TAGS']], True
+            out_file_object, yml_handler, df[['SECTIONS', 'TOKENS', 'TAGS_LISTS', 'NASAB_TAGS']]
         )
 
-    # return df['NASAB_TAGS'].fillna('').tolist(), yml_handler, text_w_cutoff
-
     return f'{file}\n' + reconstructed_miu
```

### Comparing `eis1600-0.8.0/eis1600/onomastics/re_pattern.py` & `eis1600-0.8.1/eis1600/onomastics/re_pattern.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 import re
 
-from eis1600.markdown.re_pattern import AR_STR
+from eis1600.helper.markdown_patterns import AR_CHR, AR_STR
 
-ABU_ABI = re.compile(' [و]?[اأ]ب[ويى] ')
-UMM = re.compile(' [و]?[اأ]م ')
-IBN_IBNA = re.compile('[اإ](بن[ةه]?)(?= )')
-BN_BNT = re.compile(' (بن[ت]?) ')
-DIN_DAULA = re.compile(' (الدين|الدول[ةه])')
-BANU_BANI = re.compile('بن[ويى] ')
-YURIFA_K_BI = re.compile('([تي]عرف) (ك' + AR_STR + ') (ب)')
+ABU = re.compile(r' [اأ]بو ')
+ABI = re.compile(r' [اأ]ب[يى] ')
+UMM = re.compile(r' [اأ]م ')
+IBN_IBNA = re.compile(r' [اإ](بن[ةه]?)(?= )')
+BN_BNT = re.compile(r' (بن[ت]?) ')
+DIN_DAULA = re.compile(r' (الدين|الدول[ةه])')
+BANU_BANI = re.compile(r'بن[ويى] ')
+YURIFA_K_BI = re.compile(r'([تي]عرف) (ك' + AR_STR + r') (ب)')
+
+CRF_PATTERN = re.compile(AR_CHR + r'*?عر' + AR_CHR + r'*?ف')
+SHR_PATTERN = re.compile(AR_CHR + r'*?شت?ه' + AR_CHR + r'*?ر')
+LQB_PATTERN = re.compile(AR_CHR + r'*?لق' + AR_CHR + r'*?ب')
+
+LETTERS = r'(?:[أا]لف)|(?:باء)|(?:تاء)|(?:ثاء)|(?:جيم)|(?:حاء)|(?:خاء)|(?:داء)|(?:دال)|(?:ذاء)|(?:ذال)|(?:راء)|(' \
+          r'?:زاء)|(?:زاي)|(?:زين)|(?:سين)|(?:شين)|(?:صاد)|(?:ضاد)|(?:طاء)|(?:ظاء)|(?:عين)|(?:غين)|(?:فاء)|(?:قاف)|(' \
+          r'?:كاف)|(?:كاء)|(?:لام)|(?:ميم)|(?:نون)|(?:هاء)|(?:واو)|(?:ياء)|(?:همزة)|(?:تاء مربوطة)|(?:تاء ت[أا]نيث)|(' \
+          r'?:[أا]لف مقصورة)|(?:تاء ثالثة)|(?:فتحة)|(?:فتح)|(?:مفتوحة)|(?:فتحتين)|(?:مفتوحتين)|(?:ضمة)|(?:ضم)|(' \
+          r'?:مضمومة)|(?:ضمتين)|(?:مضمومتين)|(?:كسرة)|(?:كسر)|(?:مكسورة، كسرتين)|(?:مكسورتين)|(?:مدة)|(?:شدة)|(' \
+          r'?:مشددة)|(?:تشديد)|(?:سكون)|(?:ساكنة)|(?:دون)|(?:ثم)|(?:بعدها)|(?:بينهما)|(?:أو)|(?:معجمة)|(?:حروف)|(' \
+          r'?:آخر الحروف)|(?:مهملة)|(?:مهملتين)|(?:موحدة)|(?:موحدتين)|(?:مثناة)|(?:مثناتين)|(?:[أا]ولى)|(?:ثانية)|(' \
+          r'?:ثالثة)|(?:في آخره)|(?:آخره)|(?:[أا]وله)|(?:تحتانية)|(?:تصريف)'
 
-DATES = re.compile('\[[^\]]+\]')
-PARENTHESIS = re.compile('\(([^)]+)\)')
-QUOTES = re.compile('"[^"]+"')
-PUNCTUATION = re.compile('[.،؟!:؛,;?|]')
-
-SPACES = re.compile(' {2,}')
-
-LETTERS = '(?:[أا]لف)|(?:باء)|(?:تاء)|(?:ثاء)|(?:جيم)|(?:حاء)|(?:خاء)|(?:داء)|(?:دال)|(?:ذاء)|(?:ذال)|(?:راء)|(' \
-          '?:زاء)|(?:زاي)|(?:زين)|(?:سين)|(?:شين)|(?:صاد)|(?:ضاد)|(?:طاء)|(?:ظاء)|(?:عين)|(?:غين)|(?:فاء)|(?:قاف)|(' \
-          '?:كاف)|(?:كاء)|(?:لام)|(?:ميم)|(?:نون)|(?:هاء)|(?:واو)|(?:ياء)|(?:همزة)|(?:تاء مربوطة)|(?:تاء ت[أا]نيث)|(' \
-          '?:[أا]لف مقصورة)|(?:تاء ثالثة)|(?:فتحة)|(?:فتح)|(?:مفتوحة)|(?:فتحتين)|(?:مفتوحتين)|(?:ضمة)|(?:ضم)|(' \
-          '?:مضمومة)|(?:ضمتين)|(?:مضمومتين)|(?:كسرة)|(?:كسر)|(?:مكسورة، كسرتين)|(?:مكسورتين)|(?:مدة)|(?:شدة)|(' \
-          '?:مشددة)|(?:تشديد)|(?:سكون)|(?:ساكنة)|(?:دون)|(?:ثم)|(?:بعدها)|(?:بينهما)|(?:أو)|(?:معجمة)|(?:حروف)|(?:آخر ' \
-          'الحروف)|(?:مهملة)|(?:مهملتين)|(?:موحدة)|(?:موحدتين)|(?:مثناة)|(?:مثناتين)|(?:[أا]ولى)|(?:ثانية)|(' \
-          '?:ثالثة)|(?:في آخره)|(?:آخره)|(?:[أا]وله)|(?:تحتانية)|(?:تصريف)'
-
-SPELLING = re.compile('(?<= )([بو]?(?:ال)?(?:' + LETTERS + ') ){2,}')
+SPELLING = re.compile(r'(?<= )([بو]?(?:ال)?(?:' + LETTERS + r') ){2,}')
```

### Comparing `eis1600-0.8.0/eis1600/stats/methods.py` & `eis1600-0.8.1/eis1600/stats/methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.0/eis1600/stats/miu_stats.py` & `eis1600-0.8.1/eis1600/stats/miu_stats.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.0/eis1600.egg-info/PKG-INFO` & `eis1600-0.8.1/eis1600.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eis1600
-Version: 0.8.0
+Version: 0.8.1
 Summary: EIS1600 project tools and utilities
 Home-page: https://github.com/EIS1600/eis1600-pkg
 Author: Lisa Mischer
 Author-email: mischer.lisa@gmail.com
 License: MIT License
 Description: # EIS1600 Tools
         
@@ -109,15 +109,15 @@
         $ convert_mARkdown_to_EIS1600 <input_dir> <output_dir>
         $ insert_uids <input_dir> <output_dir>
         ```
         
         ### Disassembling
         
         Disassemble files into the MIU repo. MIU repo has to be next to TEXT repo.
-        Must be run from the root of TEXT repo, this will disassemble all files from the AUTOREPORT.
+        Must be run from the root of TEXT repo, this will disassemble all files from the `AUTOREPORT`.
         ```shell
         $ disassemble_into_miu_files
         ```
         Give the relative path to a file to disassemble a singe file.
         ```shell
         $ disassemble_into_miu_files data/<author>/<text>/<edition>.EIS1600
         ```
@@ -179,14 +179,22 @@
         reviewed    : NOT REVIEWED
         ```
         to
         ```yaml
         reviewed    : REVIEWED
         ```
         
+        ## For MC
+        
+        ### Collect YAMLHeader into JSON
+        
+        ```shell
+        $ yml_to_json
+        ```
+        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.7, <3.9
```

### Comparing `eis1600-0.8.0/eis1600.egg-info/SOURCES.txt` & `eis1600-0.8.1/eis1600.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -15,24 +15,29 @@
 eis1600/gazetteers/Onomastics.py
 eis1600/gazetteers/Toponyms.py
 eis1600/gazetteers/__init__.py
 eis1600/gazetteers/data/__init__.py
 eis1600/helper/Singleton.py
 eis1600/helper/__init__.py
 eis1600/helper/ar_normalization.py
+eis1600/helper/entity_tags.py
 eis1600/helper/fix_miu_annotation.py
 eis1600/helper/logging.py
+eis1600/helper/markdown_methods.py
+eis1600/helper/markdown_patterns.py
 eis1600/helper/miu_random_revisions.py
+eis1600/helper/my_json_ecoder.py
 eis1600/helper/repo.py
+eis1600/helper/yml_to_json.py
+eis1600/helper/data/__init__.py
 eis1600/markdown/UIDs.py
 eis1600/markdown/__init__.py
 eis1600/markdown/convert_mARkdown_to_EIS1600TMP.py
 eis1600/markdown/insert_uids.py
 eis1600/markdown/methods.py
-eis1600/markdown/re_pattern.py
 eis1600/markdown/update_uids.py
 eis1600/markdown/update_uids_old_process.py
 eis1600/miu/HeadingTracker.py
 eis1600/miu/YAMLHandler.py
 eis1600/miu/__init__.py
 eis1600/miu/disassemble_into_miu_files.py
 eis1600/miu/methods.py
@@ -42,12 +47,13 @@
 eis1600/nlp/cameltools.py
 eis1600/nlp/ner_annotate_mius.py
 eis1600/nlp/utils.py
 eis1600/onomastics/__init__.py
 eis1600/onomastics/annotation.py
 eis1600/onomastics/methods.py
 eis1600/onomastics/re_pattern.py
-eis1600/preprocessing/__init__.py
-eis1600/preprocessing/methods.py
+eis1600/processing/__init__.py
+eis1600/processing/postprocessing.py
+eis1600/processing/preprocessing.py
 eis1600/stats/__init__.py
 eis1600/stats/methods.py
 eis1600/stats/miu_stats.py
```

### Comparing `eis1600-0.8.0/eis1600.egg-info/entry_points.txt` & `eis1600-0.8.1/eis1600.egg-info/entry_points.txt`

 * *Files 18% similar despite different names*

```diff
@@ -6,8 +6,9 @@
 insert_uids = eis1600.markdown.insert_uids:main
 miu_random_revisions = eis1600.helper.miu_random_revisions:main
 miu_stats = eis1600.stats.miu_stats:main
 onomastic_annotation = eis1600.onomastics.annotation:main
 reassemble_from_miu_files = eis1600.miu.reassemble_from_miu_files:main
 update_uids = eis1600.markdown.update_uids:main
 xx_update_uids_old_process = eis1600.markdown.update_uids_old_process:main
+yml_to_json = eis1600.helper.yml_to_json:main
```

### Comparing `eis1600-0.8.0/setup.py` & `eis1600-0.8.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='eis1600',
-      version='0.8.0',
+      version='0.8.1',
       description='EIS1600 project tools and utilities',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/EIS1600/eis1600-pkg',
       author='Lisa Mischer',
       author_email='mischer.lisa@gmail.com',
       license='MIT License',
       packages=find_packages(include=['eis1600', 'eis1600.*'], exclude=['excluded']),
-      package_data={'gazetteers.data': ['*.csv']},
+      package_data={'gazetteers.data': ['*.csv'], 'helper.data': ['*.csv']},
       entry_points={
           'console_scripts': [
                   'annotate_mius = eis1600.nlp.ner_annotate_mius:main [NER]',
                   'convert_mARkdown_to_EIS1600TMP = eis1600.markdown.convert_mARkdown_to_EIS1600TMP:main',
                   'disassemble_into_miu_files = eis1600.miu.disassemble_into_miu_files:main',
                   'fix_miu_annotation = eis1600.helper.fix_miu_annotation:main',
                   'insert_uids = eis1600.markdown.insert_uids:main',
                   'miu_random_revisions = eis1600.helper.miu_random_revisions:main',
                   'miu_stats = eis1600.stats.miu_stats:main',
                   'onomastic_annotation = eis1600.onomastics.annotation:main',
                   'reassemble_from_miu_files = eis1600.miu.reassemble_from_miu_files:main',
                   'update_uids = eis1600.markdown.update_uids:main',
-                  'xx_update_uids_old_process = eis1600.markdown.update_uids_old_process:main'
+                  'xx_update_uids_old_process = eis1600.markdown.update_uids_old_process:main',
+                  'yml_to_json = eis1600.helper.yml_to_json:main'
           ],
       },
       python_requires='>=3.7, <3.9',
-      install_requires=['openiti', 'pandas', 'tqdm', 'p_tqdm'],
+      install_requires=['openiti', 'pandas', 'numpy', 'tqdm', 'p_tqdm'],
       extras_require={'NER': ['camel-tools']},
       classifiers=['Programming Language :: Python :: 3',
                    'License :: OSI Approved :: MIT License',
                    'Operating System :: OS Independent',
                    'Development Status :: 1 - Planning',
                    'Intended Audience :: Science/Research']
       )
```

