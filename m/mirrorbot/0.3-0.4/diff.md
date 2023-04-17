# Comparing `tmp/mirrorbot-0.3.tar.gz` & `tmp/mirrorbot-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mirrorbot-0.3.tar", last modified: Mon Apr 17 06:27:52 2023, max compression
+gzip compressed data, was "mirrorbot-0.4.tar", last modified: Mon Apr 17 08:49:03 2023, max compression
```

## Comparing `mirrorbot-0.3.tar` & `mirrorbot-0.4.tar`

### file list

```diff
@@ -1,52 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:27:52.584776 mirrorbot-0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-17 06:27:39.000000 mirrorbot-0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-17 06:27:52.584776 mirrorbot-0.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:27:52.580776 mirrorbot-0.3/bot/
--rw-r--r--   0 runner    (1001) docker     (123)    33015 2023-04-17 06:27:39.000000 mirrorbot-0.3/bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26588 2023-04-17 06:27:39.000000 mirrorbot-0.3/bot/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:27:52.584776 mirrorbot-0.3/bot/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 06:27:39.000000 mirrorbot-0.3/bot/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17216 2023-04-17 06:27:39.000000 mirrorbot-0.3/bot/modules/anilist.py
--rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-04-17 06:27:39.000000 mirrorbot-0.3/bot/modules/authorize.py
--rw-r--r--   0 runner    (1001) docker     (123)    57929 2023-04-17 06:27:39.000000 mirrorbot-0.3/bot/modules/bot_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-17 06:27:39.000000 mirrorbot-0.3/bot/modules/broadcast.py
--rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-04-17 06:27:39.000000 mirrorbot-0.3/bot/modules/bt_select.py
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-04-17 06:27:39.000000 mirrorbot-0.3/bot/modules/cancel_mirror.py
--rw-r--r--   0 runner    (1001) docker     (123)    23774 2023-04-17 06:27:39.000000 mirrorbot-0.3/bot/modules/clone.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-17 06:27:39.000000 mirrorbot-0.3/bot/modules/count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-17 06:27:39.000000 mirrorbot-0.3/bot/modules/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-17 06:27:39.000000 mirrorbot-0.3/bot/modules/drive_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-04-17 06:27:39.000000 mirrorbot-0.3/bot/modules/eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-04-17 06:27:39.000000 mirrorbot-0.3/bot/modules/gmail.py
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-04-17 06:27:39.000000 mirrorbot-0.3/bot/modules/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)    10523 2023-04-17 06:27:39.000000 mirrorbot-0.3/bot/modules/imdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-04-17 06:27:39.000000 mirrorbot-0.3/bot/modules/list.py
--rw-r--r--   0 runner    (1001) docker     (123)    35580 2023-04-17 06:27:39.000000 mirrorbot-0.3/bot/modules/listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-04-17 06:27:39.000000 mirrorbot-0.3/bot/modules/mediainfo.py
--rw-r--r--   0 runner    (1001) docker     (123)    24324 2023-04-17 06:27:39.000000 mirrorbot-0.3/bot/modules/mirror_leech.py
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-04-17 06:27:39.000000 mirrorbot-0.3/bot/modules/mirror_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-04-17 06:27:39.000000 mirrorbot-0.3/bot/modules/pictures.py
--rw-r--r--   0 runner    (1001) docker     (123)    12419 2023-04-17 06:27:39.000000 mirrorbot-0.3/bot/modules/rss.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-17 06:27:39.000000 mirrorbot-0.3/bot/modules/save_msg.py
--rw-r--r--   0 runner    (1001) docker     (123)    18977 2023-04-17 06:27:39.000000 mirrorbot-0.3/bot/modules/scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)    12477 2023-04-17 06:27:39.000000 mirrorbot-0.3/bot/modules/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     6625 2023-04-17 06:27:39.000000 mirrorbot-0.3/bot/modules/sel_cat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-04-17 06:27:39.000000 mirrorbot-0.3/bot/modules/shell.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-04-17 06:27:39.000000 mirrorbot-0.3/bot/modules/speedtest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-04-17 06:27:39.000000 mirrorbot-0.3/bot/modules/users.py
--rw-r--r--   0 runner    (1001) docker     (123)    34924 2023-04-17 06:27:39.000000 mirrorbot-0.3/bot/modules/users_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4929 2023-04-17 06:27:39.000000 mirrorbot-0.3/bot/modules/wayback.py
--rw-r--r--   0 runner    (1001) docker     (123)    21193 2023-04-17 06:27:39.000000 mirrorbot-0.3/bot/modules/ytdlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:27:52.584776 mirrorbot-0.3/mirrorbot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-17 06:27:52.000000 mirrorbot-0.3/mirrorbot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-17 06:27:52.000000 mirrorbot-0.3/mirrorbot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 06:27:52.000000 mirrorbot-0.3/mirrorbot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-17 06:27:52.000000 mirrorbot-0.3/mirrorbot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-17 06:27:52.000000 mirrorbot-0.3/mirrorbot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-17 06:27:52.000000 mirrorbot-0.3/mirrorbot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 06:27:52.584776 mirrorbot-0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-04-17 06:27:39.000000 mirrorbot-0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:27:52.584776 mirrorbot-0.3/web/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 06:27:39.000000 mirrorbot-0.3/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-17 06:27:39.000000 mirrorbot-0.3/web/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    20479 2023-04-17 06:27:39.000000 mirrorbot-0.3/web/wserver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:49:03.260564 mirrorbot-0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-17 08:48:49.000000 mirrorbot-0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-17 08:49:03.260564 mirrorbot-0.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:49:03.252564 mirrorbot-0.4/bot/
+-rw-r--r--   0 runner    (1001) docker     (123)    33015 2023-04-17 08:48:49.000000 mirrorbot-0.4/bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26588 2023-04-17 08:48:49.000000 mirrorbot-0.4/bot/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:49:03.256564 mirrorbot-0.4/bot/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 08:48:49.000000 mirrorbot-0.4/bot/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17216 2023-04-17 08:48:49.000000 mirrorbot-0.4/bot/modules/anilist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-04-17 08:48:49.000000 mirrorbot-0.4/bot/modules/authorize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57929 2023-04-17 08:48:49.000000 mirrorbot-0.4/bot/modules/bot_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-17 08:48:49.000000 mirrorbot-0.4/bot/modules/broadcast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-04-17 08:48:49.000000 mirrorbot-0.4/bot/modules/bt_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-04-17 08:48:49.000000 mirrorbot-0.4/bot/modules/cancel_mirror.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23774 2023-04-17 08:48:49.000000 mirrorbot-0.4/bot/modules/clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-17 08:48:49.000000 mirrorbot-0.4/bot/modules/count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-17 08:48:49.000000 mirrorbot-0.4/bot/modules/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-17 08:48:49.000000 mirrorbot-0.4/bot/modules/drive_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-04-17 08:48:49.000000 mirrorbot-0.4/bot/modules/eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-04-17 08:48:49.000000 mirrorbot-0.4/bot/modules/gmail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-04-17 08:48:49.000000 mirrorbot-0.4/bot/modules/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10523 2023-04-17 08:48:49.000000 mirrorbot-0.4/bot/modules/imdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-04-17 08:48:49.000000 mirrorbot-0.4/bot/modules/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35580 2023-04-17 08:48:49.000000 mirrorbot-0.4/bot/modules/listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-04-17 08:48:49.000000 mirrorbot-0.4/bot/modules/mediainfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24324 2023-04-17 08:48:49.000000 mirrorbot-0.4/bot/modules/mirror_leech.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-04-17 08:48:49.000000 mirrorbot-0.4/bot/modules/mirror_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-04-17 08:48:49.000000 mirrorbot-0.4/bot/modules/pictures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12419 2023-04-17 08:48:49.000000 mirrorbot-0.4/bot/modules/rss.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-17 08:48:49.000000 mirrorbot-0.4/bot/modules/save_msg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18977 2023-04-17 08:48:49.000000 mirrorbot-0.4/bot/modules/scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12477 2023-04-17 08:48:49.000000 mirrorbot-0.4/bot/modules/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6625 2023-04-17 08:48:49.000000 mirrorbot-0.4/bot/modules/sel_cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-04-17 08:48:49.000000 mirrorbot-0.4/bot/modules/shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-04-17 08:48:49.000000 mirrorbot-0.4/bot/modules/speedtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-04-17 08:48:49.000000 mirrorbot-0.4/bot/modules/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34924 2023-04-17 08:48:49.000000 mirrorbot-0.4/bot/modules/users_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4929 2023-04-17 08:48:49.000000 mirrorbot-0.4/bot/modules/wayback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21193 2023-04-17 08:48:49.000000 mirrorbot-0.4/bot/modules/ytdlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:49:03.260564 mirrorbot-0.4/mirrorbot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-17 08:49:03.000000 mirrorbot-0.4/mirrorbot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-17 08:49:03.000000 mirrorbot-0.4/mirrorbot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 08:49:03.000000 mirrorbot-0.4/mirrorbot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-17 08:49:03.000000 mirrorbot-0.4/mirrorbot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-17 08:49:03.000000 mirrorbot-0.4/mirrorbot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-17 08:49:03.000000 mirrorbot-0.4/mirrorbot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:49:03.260564 mirrorbot-0.4/qBittorrent/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 08:48:49.000000 mirrorbot-0.4/qBittorrent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:49:03.260564 mirrorbot-0.4/qBittorrent/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 08:48:49.000000 mirrorbot-0.4/qBittorrent/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 08:49:03.260564 mirrorbot-0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-17 08:48:49.000000 mirrorbot-0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:49:03.260564 mirrorbot-0.4/web/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 08:48:49.000000 mirrorbot-0.4/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-17 08:48:49.000000 mirrorbot-0.4/web/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20479 2023-04-17 08:48:49.000000 mirrorbot-0.4/web/wserver.py
```

### Comparing `mirrorbot-0.3/LICENSE` & `mirrorbot-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.3/bot/__init__.py` & `mirrorbot-0.4/bot/__init__.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.3/bot/__main__.py` & `mirrorbot-0.4/bot/__main__.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.3/bot/modules/anilist.py` & `mirrorbot-0.4/bot/modules/anilist.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.3/bot/modules/authorize.py` & `mirrorbot-0.4/bot/modules/authorize.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.3/bot/modules/bot_settings.py` & `mirrorbot-0.4/bot/modules/bot_settings.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.3/bot/modules/broadcast.py` & `mirrorbot-0.4/bot/modules/broadcast.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.3/bot/modules/bt_select.py` & `mirrorbot-0.4/bot/modules/bt_select.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.3/bot/modules/cancel_mirror.py` & `mirrorbot-0.4/bot/modules/cancel_mirror.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.3/bot/modules/clone.py` & `mirrorbot-0.4/bot/modules/clone.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.3/bot/modules/count.py` & `mirrorbot-0.4/bot/modules/count.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.3/bot/modules/delete.py` & `mirrorbot-0.4/bot/modules/delete.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.3/bot/modules/drive_clean.py` & `mirrorbot-0.4/bot/modules/drive_clean.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.3/bot/modules/eval.py` & `mirrorbot-0.4/bot/modules/eval.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.3/bot/modules/gmail.py` & `mirrorbot-0.4/bot/modules/gmail.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.3/bot/modules/hash.py` & `mirrorbot-0.4/bot/modules/hash.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.3/bot/modules/imdb.py` & `mirrorbot-0.4/bot/modules/imdb.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.3/bot/modules/list.py` & `mirrorbot-0.4/bot/modules/list.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.3/bot/modules/listener.py` & `mirrorbot-0.4/bot/modules/listener.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.3/bot/modules/mediainfo.py` & `mirrorbot-0.4/bot/modules/mediainfo.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.3/bot/modules/mirror_leech.py` & `mirrorbot-0.4/bot/modules/mirror_leech.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.3/bot/modules/mirror_status.py` & `mirrorbot-0.4/bot/modules/mirror_status.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.3/bot/modules/pictures.py` & `mirrorbot-0.4/bot/modules/pictures.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.3/bot/modules/rss.py` & `mirrorbot-0.4/bot/modules/rss.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.3/bot/modules/save_msg.py` & `mirrorbot-0.4/bot/modules/save_msg.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.3/bot/modules/scraper.py` & `mirrorbot-0.4/bot/modules/scraper.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.3/bot/modules/search.py` & `mirrorbot-0.4/bot/modules/search.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.3/bot/modules/sel_cat.py` & `mirrorbot-0.4/bot/modules/sel_cat.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.3/bot/modules/shell.py` & `mirrorbot-0.4/bot/modules/shell.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.3/bot/modules/speedtest.py` & `mirrorbot-0.4/bot/modules/speedtest.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.3/bot/modules/users.py` & `mirrorbot-0.4/bot/modules/users.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.3/bot/modules/users_settings.py` & `mirrorbot-0.4/bot/modules/users_settings.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.3/bot/modules/wayback.py` & `mirrorbot-0.4/bot/modules/wayback.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.3/bot/modules/ytdlp.py` & `mirrorbot-0.4/bot/modules/ytdlp.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.3/mirrorbot.egg-info/SOURCES.txt` & `mirrorbot-0.4/mirrorbot.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -36,10 +36,12 @@
 bot/modules/ytdlp.py
 mirrorbot.egg-info/PKG-INFO
 mirrorbot.egg-info/SOURCES.txt
 mirrorbot.egg-info/dependency_links.txt
 mirrorbot.egg-info/entry_points.txt
 mirrorbot.egg-info/requires.txt
 mirrorbot.egg-info/top_level.txt
+qBittorrent/__init__.py
+qBittorrent/config/__init__.py
 web/__init__.py
 web/nodes.py
 web/wserver.py
```

### Comparing `mirrorbot-0.3/setup.py` & `mirrorbot-0.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mirrorbot',
-    version='0.3',
+    version='0.4',
     packages=find_packages(),
+    include_package_data=True,
+    package_data={
+        '': ['*.*']
+    },
     install_requires=[
         'aiohttp',
         'anytree',
         'aria2p',
         'asgiref',
         'asyncio',
         'beautifulsoup4',
@@ -46,13 +50,12 @@
         'urllib3',
         'waybackpy',
         'xattr',
         'yt-dlp'
     ],
     entry_points={
         'console_scripts': [
-            'your_package_name=bot.__main__:main'
+            'your_package_name=bot.main:main'
         ]
     },
     python_requires='>=3.9'
 )
-
```

### Comparing `mirrorbot-0.3/web/nodes.py` & `mirrorbot-0.4/web/nodes.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.3/web/wserver.py` & `mirrorbot-0.4/web/wserver.py`

 * *Files identical despite different names*

