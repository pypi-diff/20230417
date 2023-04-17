# Comparing `tmp/mirrorbot-1.0.tar.gz` & `tmp/mirrorbot-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mirrorbot-1.0.tar", last modified: Mon Apr 17 15:26:11 2023, max compression
+gzip compressed data, was "mirrorbot-1.1.tar", last modified: Mon Apr 17 15:46:04 2023, max compression
```

## Comparing `mirrorbot-1.0.tar` & `mirrorbot-1.1.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:26:11.405460 mirrorbot-1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-17 15:26:11.405460 mirrorbot-1.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:26:11.397460 mirrorbot-1.0/bot/
--rw-r--r--   0 runner    (1001) docker     (123)    60945 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26856 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:26:11.397460 mirrorbot-1.0/bot/helper/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/helper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:26:11.397460 mirrorbot-1.0/bot/helper/ext_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/helper/ext_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30469 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/helper/ext_utils/bot_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/helper/ext_utils/db_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/helper/ext_utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/helper/ext_utils/fs_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/helper/ext_utils/html_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/helper/ext_utils/queued_starter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/helper/ext_utils/shortenurl.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/helper/ext_utils/telegraph_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/helper/ext_utils/timegap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:26:11.397460 mirrorbot-1.0/bot/helper/mirror_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/helper/mirror_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:26:11.401460 mirrorbot-1.0/bot/helper/mirror_utils/download_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/helper/mirror_utils/download_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14104 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/helper/mirror_utils/download_utils/aria2_download.py
--rw-r--r--   0 runner    (1001) docker     (123)    30926 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/helper/mirror_utils/download_utils/direct_link_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/helper/mirror_utils/download_utils/gd_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    13229 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/helper/mirror_utils/download_utils/mega_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/helper/mirror_utils/download_utils/qbit_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7384 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/helper/mirror_utils/download_utils/telegram_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    16258 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/helper/mirror_utils/download_utils/yt_dlp_download_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:26:11.401460 mirrorbot-1.0/bot/helper/mirror_utils/status_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/helper/mirror_utils/status_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/helper/mirror_utils/status_utils/aria_download_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/helper/mirror_utils/status_utils/clone_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/helper/mirror_utils/status_utils/convert_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/helper/mirror_utils/status_utils/extract_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/helper/mirror_utils/status_utils/gd_download_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/helper/mirror_utils/status_utils/mega_download_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/helper/mirror_utils/status_utils/qbit_download_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/helper/mirror_utils/status_utils/queue_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/helper/mirror_utils/status_utils/split_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/helper/mirror_utils/status_utils/telegram_download_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/helper/mirror_utils/status_utils/tg_upload_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/helper/mirror_utils/status_utils/upload_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/helper/mirror_utils/status_utils/yt_dlp_download_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/helper/mirror_utils/status_utils/zip_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:26:11.401460 mirrorbot-1.0/bot/helper/mirror_utils/upload_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/helper/mirror_utils/upload_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45943 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/helper/mirror_utils/upload_utils/gdriveTools.py
--rw-r--r--   0 runner    (1001) docker     (123)    22211 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/helper/mirror_utils/upload_utils/pyrogramEngine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:26:11.401460 mirrorbot-1.0/bot/helper/telegram_helper/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/helper/telegram_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/helper/telegram_helper/bot_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/helper/telegram_helper/button_build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/helper/telegram_helper/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     9145 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/helper/telegram_helper/message_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:26:11.405460 mirrorbot-1.0/bot/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17216 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/modules/anilist.py
--rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/modules/authorize.py
--rw-r--r--   0 runner    (1001) docker     (123)    57929 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/modules/bot_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/modules/broadcast.py
--rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/modules/bt_select.py
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/modules/cancel_mirror.py
--rw-r--r--   0 runner    (1001) docker     (123)    23774 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/modules/clone.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/modules/count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/modules/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/modules/drive_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/modules/eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/modules/gmail.py
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/modules/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)    10523 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/modules/imdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/modules/list.py
--rw-r--r--   0 runner    (1001) docker     (123)    35580 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/modules/listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/modules/mediainfo.py
--rw-r--r--   0 runner    (1001) docker     (123)    24324 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/modules/mirror_leech.py
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/modules/mirror_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/modules/pictures.py
--rw-r--r--   0 runner    (1001) docker     (123)    12419 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/modules/rss.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/modules/save_msg.py
--rw-r--r--   0 runner    (1001) docker     (123)    18977 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/modules/scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)    12477 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/modules/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     6625 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/modules/sel_cat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/modules/shell.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/modules/speedtest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/modules/users.py
--rw-r--r--   0 runner    (1001) docker     (123)    34924 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/modules/users_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4929 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/modules/wayback.py
--rw-r--r--   0 runner    (1001) docker     (123)    21193 2023-04-17 15:26:00.000000 mirrorbot-1.0/bot/modules/ytdlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:26:11.405460 mirrorbot-1.0/mirrorbot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-17 15:26:11.000000 mirrorbot-1.0/mirrorbot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-04-17 15:26:11.000000 mirrorbot-1.0/mirrorbot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 15:26:11.000000 mirrorbot-1.0/mirrorbot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-17 15:26:11.000000 mirrorbot-1.0/mirrorbot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-17 15:26:11.000000 mirrorbot-1.0/mirrorbot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-17 15:26:11.000000 mirrorbot-1.0/mirrorbot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 15:26:11.405460 mirrorbot-1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-17 15:26:00.000000 mirrorbot-1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:46:04.459794 mirrorbot-1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-17 15:46:04.459794 mirrorbot-1.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:46:04.451794 mirrorbot-1.1/bot/
+-rw-r--r--   0 runner    (1001) docker     (123)    60945 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26869 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:46:04.451794 mirrorbot-1.1/bot/helper/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/helper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:46:04.451794 mirrorbot-1.1/bot/helper/ext_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/helper/ext_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30469 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/helper/ext_utils/bot_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/helper/ext_utils/db_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/helper/ext_utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/helper/ext_utils/fs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/helper/ext_utils/html_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/helper/ext_utils/queued_starter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/helper/ext_utils/shortenurl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/helper/ext_utils/telegraph_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/helper/ext_utils/timegap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:46:04.451794 mirrorbot-1.1/bot/helper/mirror_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/helper/mirror_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:46:04.451794 mirrorbot-1.1/bot/helper/mirror_utils/download_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/helper/mirror_utils/download_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14104 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/helper/mirror_utils/download_utils/aria2_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30926 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/helper/mirror_utils/download_utils/direct_link_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/helper/mirror_utils/download_utils/gd_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13229 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/helper/mirror_utils/download_utils/mega_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/helper/mirror_utils/download_utils/qbit_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7384 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/helper/mirror_utils/download_utils/telegram_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16258 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/helper/mirror_utils/download_utils/yt_dlp_download_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:46:04.451794 mirrorbot-1.1/bot/helper/mirror_utils/status_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/helper/mirror_utils/status_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/helper/mirror_utils/status_utils/aria_download_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/helper/mirror_utils/status_utils/clone_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/helper/mirror_utils/status_utils/convert_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/helper/mirror_utils/status_utils/extract_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/helper/mirror_utils/status_utils/gd_download_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/helper/mirror_utils/status_utils/mega_download_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/helper/mirror_utils/status_utils/qbit_download_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/helper/mirror_utils/status_utils/queue_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/helper/mirror_utils/status_utils/split_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/helper/mirror_utils/status_utils/telegram_download_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/helper/mirror_utils/status_utils/tg_upload_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/helper/mirror_utils/status_utils/upload_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/helper/mirror_utils/status_utils/yt_dlp_download_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/helper/mirror_utils/status_utils/zip_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:46:04.455794 mirrorbot-1.1/bot/helper/mirror_utils/upload_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/helper/mirror_utils/upload_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45943 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/helper/mirror_utils/upload_utils/gdriveTools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22211 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/helper/mirror_utils/upload_utils/pyrogramEngine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:46:04.455794 mirrorbot-1.1/bot/helper/telegram_helper/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/helper/telegram_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/helper/telegram_helper/bot_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/helper/telegram_helper/button_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/helper/telegram_helper/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9145 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/helper/telegram_helper/message_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:46:04.455794 mirrorbot-1.1/bot/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17216 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/modules/anilist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/modules/authorize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57929 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/modules/bot_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/modules/broadcast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/modules/bt_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/modules/cancel_mirror.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23774 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/modules/clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/modules/count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/modules/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/modules/drive_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/modules/eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/modules/gmail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/modules/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10523 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/modules/imdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/modules/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35580 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/modules/listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/modules/mediainfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24324 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/modules/mirror_leech.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/modules/mirror_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/modules/pictures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12419 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/modules/rss.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/modules/save_msg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18977 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/modules/scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12477 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/modules/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6625 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/modules/sel_cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/modules/shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/modules/speedtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/modules/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34924 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/modules/users_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4929 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/modules/wayback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21193 2023-04-17 15:45:54.000000 mirrorbot-1.1/bot/modules/ytdlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:46:04.459794 mirrorbot-1.1/mirrorbot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-17 15:46:04.000000 mirrorbot-1.1/mirrorbot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-04-17 15:46:04.000000 mirrorbot-1.1/mirrorbot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 15:46:04.000000 mirrorbot-1.1/mirrorbot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-17 15:46:04.000000 mirrorbot-1.1/mirrorbot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-17 15:46:04.000000 mirrorbot-1.1/mirrorbot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-17 15:46:04.000000 mirrorbot-1.1/mirrorbot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 15:46:04.459794 mirrorbot-1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-17 15:45:54.000000 mirrorbot-1.1/setup.py
```

### Comparing `mirrorbot-1.0/bot/__init__.py` & `mirrorbot-1.1/bot/__init__.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/__main__.py` & `mirrorbot-1.1/bot/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,28 +85,28 @@
     mem_t = get_readable_file_size(memory.total)
     mem_a = get_readable_file_size(memory.available)
     mem_u = get_readable_file_size(memory.used)
     if config_dict['EMOJI_THEME']:
             stats = f'<b>       📊 Bot Statistics </b>\n' \
                     f'🛠 Updated On: {last_commit}\n'\
                     f'⏰️ Uptime: {currentTime}\n'\
-                    f'🤖 Version: {version}\n'\
+                    f'🤖 Pypi Version: {version}\n'\
                     f'🟢 OS Uptime: {osUptime}\n'\
                     f'🖥︄ CPU: [{progress_bar(cpuUsage)}] {cpuUsage}%\n'\
                     f'🎮 RAM: [{progress_bar(mem_p)}] {mem_p}%\n'\
                     f'💾 Disk: [{progress_bar(disk)}] {disk}%\n'\
                     f'💿 Disk Free: {free}\n'\
                     f'🔺 Upload Data: {sent}\n'\
                     f'🔻 Download Data: {recv}\n\n'
 
     else:
             stats = f'<b>    📊 Bot Statistics </b>\n' \
                     f'Updated On: {last_commit}\n'\
                     f'Uptime: {currentTime}\n'\
-                    f'Version: {version}\n'\
+                    f'Pypi Version: {version}\n'\
                     f'OS Uptime: {osUptime}\n'\
                     f'CPU: [{progress_bar(cpuUsage)}] {cpuUsage}%\n'\
                     f'RAM: [{progress_bar(mem_p)}] {mem_p}%\n'\
                     f'Disk: [{progress_bar(disk)}] {disk}%\n'\
                     f'Disk Free: {free}\n'\
                     f'Upload Data: {sent}\n'\
                     f'Download Data: {recv}\n\n'
@@ -186,15 +186,15 @@
         Interval[0].cancel()
         Interval.clear()
     if QbInterval:
         QbInterval[0].cancel()
         QbInterval.clear()
     clean_all()
     srun(["pkill", "-9", "-f", "gunicorn|aria2c|qbittorrent-nox|ffmpeg"])
-    srun("python3 -m pip3 install mirrorbot", shell=True)
+    srun("python3 -m pip3 install mirrorbot -U", shell=True)
     with open(".restartmsg", "w") as f:
         f.truncate(0)
         f.write(f"{restart_message.chat.id}\n{restart_message.message_id}\n")
     osexecl(executable, executable, "-m", "bot")
 
 
 def ping(update, context):
```

### Comparing `mirrorbot-1.0/bot/helper/ext_utils/bot_utils.py` & `mirrorbot-1.1/bot/helper/ext_utils/bot_utils.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/helper/ext_utils/db_handler.py` & `mirrorbot-1.1/bot/helper/ext_utils/db_handler.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/helper/ext_utils/fs_utils.py` & `mirrorbot-1.1/bot/helper/ext_utils/fs_utils.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/helper/ext_utils/html_helper.py` & `mirrorbot-1.1/bot/helper/ext_utils/html_helper.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/helper/ext_utils/queued_starter.py` & `mirrorbot-1.1/bot/helper/ext_utils/queued_starter.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/helper/ext_utils/shortenurl.py` & `mirrorbot-1.1/bot/helper/ext_utils/shortenurl.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/helper/ext_utils/telegraph_helper.py` & `mirrorbot-1.1/bot/helper/ext_utils/telegraph_helper.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/helper/ext_utils/timegap.py` & `mirrorbot-1.1/bot/helper/ext_utils/timegap.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/helper/mirror_utils/download_utils/aria2_download.py` & `mirrorbot-1.1/bot/helper/mirror_utils/download_utils/aria2_download.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/helper/mirror_utils/download_utils/direct_link_generator.py` & `mirrorbot-1.1/bot/helper/mirror_utils/download_utils/direct_link_generator.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/helper/mirror_utils/download_utils/gd_downloader.py` & `mirrorbot-1.1/bot/helper/mirror_utils/download_utils/gd_downloader.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/helper/mirror_utils/download_utils/mega_downloader.py` & `mirrorbot-1.1/bot/helper/mirror_utils/download_utils/mega_downloader.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/helper/mirror_utils/download_utils/qbit_downloader.py` & `mirrorbot-1.1/bot/helper/mirror_utils/download_utils/qbit_downloader.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/helper/mirror_utils/download_utils/telegram_downloader.py` & `mirrorbot-1.1/bot/helper/mirror_utils/download_utils/telegram_downloader.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/helper/mirror_utils/download_utils/yt_dlp_download_helper.py` & `mirrorbot-1.1/bot/helper/mirror_utils/download_utils/yt_dlp_download_helper.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/helper/mirror_utils/status_utils/aria_download_status.py` & `mirrorbot-1.1/bot/helper/mirror_utils/status_utils/aria_download_status.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/helper/mirror_utils/status_utils/clone_status.py` & `mirrorbot-1.1/bot/helper/mirror_utils/status_utils/clone_status.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/helper/mirror_utils/status_utils/convert_status.py` & `mirrorbot-1.1/bot/helper/mirror_utils/status_utils/convert_status.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/helper/mirror_utils/status_utils/extract_status.py` & `mirrorbot-1.1/bot/helper/mirror_utils/status_utils/extract_status.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/helper/mirror_utils/status_utils/gd_download_status.py` & `mirrorbot-1.1/bot/helper/mirror_utils/status_utils/gd_download_status.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/helper/mirror_utils/status_utils/mega_download_status.py` & `mirrorbot-1.1/bot/helper/mirror_utils/status_utils/mega_download_status.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/helper/mirror_utils/status_utils/qbit_download_status.py` & `mirrorbot-1.1/bot/helper/mirror_utils/status_utils/qbit_download_status.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/helper/mirror_utils/status_utils/queue_status.py` & `mirrorbot-1.1/bot/helper/mirror_utils/status_utils/queue_status.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/helper/mirror_utils/status_utils/split_status.py` & `mirrorbot-1.1/bot/helper/mirror_utils/status_utils/split_status.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/helper/mirror_utils/status_utils/telegram_download_status.py` & `mirrorbot-1.1/bot/helper/mirror_utils/status_utils/telegram_download_status.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/helper/mirror_utils/status_utils/tg_upload_status.py` & `mirrorbot-1.1/bot/helper/mirror_utils/status_utils/tg_upload_status.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/helper/mirror_utils/status_utils/upload_status.py` & `mirrorbot-1.1/bot/helper/mirror_utils/status_utils/upload_status.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/helper/mirror_utils/status_utils/yt_dlp_download_status.py` & `mirrorbot-1.1/bot/helper/mirror_utils/status_utils/yt_dlp_download_status.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/helper/mirror_utils/status_utils/zip_status.py` & `mirrorbot-1.1/bot/helper/mirror_utils/status_utils/zip_status.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/helper/mirror_utils/upload_utils/gdriveTools.py` & `mirrorbot-1.1/bot/helper/mirror_utils/upload_utils/gdriveTools.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/helper/mirror_utils/upload_utils/pyrogramEngine.py` & `mirrorbot-1.1/bot/helper/mirror_utils/upload_utils/pyrogramEngine.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/helper/telegram_helper/bot_commands.py` & `mirrorbot-1.1/bot/helper/telegram_helper/bot_commands.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/helper/telegram_helper/button_build.py` & `mirrorbot-1.1/bot/helper/telegram_helper/button_build.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/helper/telegram_helper/filters.py` & `mirrorbot-1.1/bot/helper/telegram_helper/filters.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/helper/telegram_helper/message_utils.py` & `mirrorbot-1.1/bot/helper/telegram_helper/message_utils.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/modules/anilist.py` & `mirrorbot-1.1/bot/modules/anilist.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/modules/authorize.py` & `mirrorbot-1.1/bot/modules/authorize.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/modules/bot_settings.py` & `mirrorbot-1.1/bot/modules/bot_settings.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/modules/broadcast.py` & `mirrorbot-1.1/bot/modules/broadcast.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/modules/bt_select.py` & `mirrorbot-1.1/bot/modules/bt_select.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/modules/cancel_mirror.py` & `mirrorbot-1.1/bot/modules/cancel_mirror.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/modules/clone.py` & `mirrorbot-1.1/bot/modules/clone.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/modules/count.py` & `mirrorbot-1.1/bot/modules/count.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/modules/delete.py` & `mirrorbot-1.1/bot/modules/delete.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/modules/drive_clean.py` & `mirrorbot-1.1/bot/modules/drive_clean.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/modules/eval.py` & `mirrorbot-1.1/bot/modules/eval.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/modules/gmail.py` & `mirrorbot-1.1/bot/modules/gmail.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/modules/hash.py` & `mirrorbot-1.1/bot/modules/hash.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/modules/imdb.py` & `mirrorbot-1.1/bot/modules/imdb.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/modules/list.py` & `mirrorbot-1.1/bot/modules/list.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/modules/listener.py` & `mirrorbot-1.1/bot/modules/listener.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/modules/mediainfo.py` & `mirrorbot-1.1/bot/modules/mediainfo.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/modules/mirror_leech.py` & `mirrorbot-1.1/bot/modules/mirror_leech.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/modules/mirror_status.py` & `mirrorbot-1.1/bot/modules/mirror_status.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/modules/pictures.py` & `mirrorbot-1.1/bot/modules/pictures.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/modules/rss.py` & `mirrorbot-1.1/bot/modules/rss.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/modules/save_msg.py` & `mirrorbot-1.1/bot/modules/save_msg.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/modules/scraper.py` & `mirrorbot-1.1/bot/modules/scraper.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/modules/search.py` & `mirrorbot-1.1/bot/modules/search.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/modules/sel_cat.py` & `mirrorbot-1.1/bot/modules/sel_cat.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/modules/shell.py` & `mirrorbot-1.1/bot/modules/shell.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/modules/speedtest.py` & `mirrorbot-1.1/bot/modules/speedtest.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/modules/users.py` & `mirrorbot-1.1/bot/modules/users.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/modules/users_settings.py` & `mirrorbot-1.1/bot/modules/users_settings.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/modules/wayback.py` & `mirrorbot-1.1/bot/modules/wayback.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/bot/modules/ytdlp.py` & `mirrorbot-1.1/bot/modules/ytdlp.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/mirrorbot.egg-info/SOURCES.txt` & `mirrorbot-1.1/mirrorbot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mirrorbot-1.0/setup.py` & `mirrorbot-1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mirrorbot',
-    version='1.0',
+    version='1.1',
     packages=find_packages(),
     include_package_data=True,
     package_data={
         '': ['*.*']
     },
     install_requires=[
         'aiohttp',
```

