# Comparing `tmp/mirrorbot-0.5.tar.gz` & `tmp/mirrorbot-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mirrorbot-0.5.tar", last modified: Mon Apr 17 10:07:13 2023, max compression
+gzip compressed data, was "mirrorbot-0.6.tar", last modified: Mon Apr 17 14:04:28 2023, max compression
```

## Comparing `mirrorbot-0.5.tar` & `mirrorbot-0.6.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:07:13.902906 mirrorbot-0.5/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-17 10:07:13.902906 mirrorbot-0.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:07:13.894905 mirrorbot-0.5/bot/
--rw-r--r--   0 runner    (1001) docker     (123)    33015 2023-04-17 10:07:02.000000 mirrorbot-0.5/bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26588 2023-04-17 10:07:02.000000 mirrorbot-0.5/bot/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:07:13.898906 mirrorbot-0.5/bot/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 10:07:02.000000 mirrorbot-0.5/bot/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17216 2023-04-17 10:07:02.000000 mirrorbot-0.5/bot/modules/anilist.py
--rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-04-17 10:07:02.000000 mirrorbot-0.5/bot/modules/authorize.py
--rw-r--r--   0 runner    (1001) docker     (123)    57929 2023-04-17 10:07:02.000000 mirrorbot-0.5/bot/modules/bot_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-17 10:07:02.000000 mirrorbot-0.5/bot/modules/broadcast.py
--rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-04-17 10:07:02.000000 mirrorbot-0.5/bot/modules/bt_select.py
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-04-17 10:07:02.000000 mirrorbot-0.5/bot/modules/cancel_mirror.py
--rw-r--r--   0 runner    (1001) docker     (123)    23774 2023-04-17 10:07:02.000000 mirrorbot-0.5/bot/modules/clone.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-17 10:07:02.000000 mirrorbot-0.5/bot/modules/count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-17 10:07:02.000000 mirrorbot-0.5/bot/modules/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-17 10:07:02.000000 mirrorbot-0.5/bot/modules/drive_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-04-17 10:07:02.000000 mirrorbot-0.5/bot/modules/eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-04-17 10:07:02.000000 mirrorbot-0.5/bot/modules/gmail.py
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-04-17 10:07:02.000000 mirrorbot-0.5/bot/modules/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)    10523 2023-04-17 10:07:02.000000 mirrorbot-0.5/bot/modules/imdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-04-17 10:07:02.000000 mirrorbot-0.5/bot/modules/list.py
--rw-r--r--   0 runner    (1001) docker     (123)    35580 2023-04-17 10:07:02.000000 mirrorbot-0.5/bot/modules/listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-04-17 10:07:02.000000 mirrorbot-0.5/bot/modules/mediainfo.py
--rw-r--r--   0 runner    (1001) docker     (123)    24324 2023-04-17 10:07:02.000000 mirrorbot-0.5/bot/modules/mirror_leech.py
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-04-17 10:07:02.000000 mirrorbot-0.5/bot/modules/mirror_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-04-17 10:07:02.000000 mirrorbot-0.5/bot/modules/pictures.py
--rw-r--r--   0 runner    (1001) docker     (123)    12419 2023-04-17 10:07:02.000000 mirrorbot-0.5/bot/modules/rss.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-17 10:07:02.000000 mirrorbot-0.5/bot/modules/save_msg.py
--rw-r--r--   0 runner    (1001) docker     (123)    18977 2023-04-17 10:07:02.000000 mirrorbot-0.5/bot/modules/scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)    12477 2023-04-17 10:07:02.000000 mirrorbot-0.5/bot/modules/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     6625 2023-04-17 10:07:02.000000 mirrorbot-0.5/bot/modules/sel_cat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-04-17 10:07:02.000000 mirrorbot-0.5/bot/modules/shell.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-04-17 10:07:02.000000 mirrorbot-0.5/bot/modules/speedtest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-04-17 10:07:02.000000 mirrorbot-0.5/bot/modules/users.py
--rw-r--r--   0 runner    (1001) docker     (123)    34924 2023-04-17 10:07:02.000000 mirrorbot-0.5/bot/modules/users_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4929 2023-04-17 10:07:02.000000 mirrorbot-0.5/bot/modules/wayback.py
--rw-r--r--   0 runner    (1001) docker     (123)    21193 2023-04-17 10:07:02.000000 mirrorbot-0.5/bot/modules/ytdlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:07:13.902906 mirrorbot-0.5/mirrorbot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-17 10:07:13.000000 mirrorbot-0.5/mirrorbot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-17 10:07:13.000000 mirrorbot-0.5/mirrorbot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 10:07:13.000000 mirrorbot-0.5/mirrorbot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-17 10:07:13.000000 mirrorbot-0.5/mirrorbot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-17 10:07:13.000000 mirrorbot-0.5/mirrorbot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-17 10:07:13.000000 mirrorbot-0.5/mirrorbot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 10:07:13.902906 mirrorbot-0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-17 10:07:02.000000 mirrorbot-0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:04:28.750020 mirrorbot-0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-17 14:04:28.750020 mirrorbot-0.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:04:28.746020 mirrorbot-0.6/bot/
+-rw-r--r--   0 runner    (1001) docker     (123)    60945 2023-04-17 14:04:19.000000 mirrorbot-0.6/bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26588 2023-04-17 14:04:19.000000 mirrorbot-0.6/bot/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:04:28.750020 mirrorbot-0.6/bot/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 14:04:19.000000 mirrorbot-0.6/bot/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17216 2023-04-17 14:04:19.000000 mirrorbot-0.6/bot/modules/anilist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-04-17 14:04:19.000000 mirrorbot-0.6/bot/modules/authorize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57929 2023-04-17 14:04:19.000000 mirrorbot-0.6/bot/modules/bot_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-17 14:04:19.000000 mirrorbot-0.6/bot/modules/broadcast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-04-17 14:04:19.000000 mirrorbot-0.6/bot/modules/bt_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-04-17 14:04:19.000000 mirrorbot-0.6/bot/modules/cancel_mirror.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23774 2023-04-17 14:04:19.000000 mirrorbot-0.6/bot/modules/clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-17 14:04:19.000000 mirrorbot-0.6/bot/modules/count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-17 14:04:19.000000 mirrorbot-0.6/bot/modules/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-17 14:04:19.000000 mirrorbot-0.6/bot/modules/drive_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-04-17 14:04:19.000000 mirrorbot-0.6/bot/modules/eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-04-17 14:04:19.000000 mirrorbot-0.6/bot/modules/gmail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-04-17 14:04:19.000000 mirrorbot-0.6/bot/modules/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10523 2023-04-17 14:04:19.000000 mirrorbot-0.6/bot/modules/imdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-04-17 14:04:19.000000 mirrorbot-0.6/bot/modules/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35580 2023-04-17 14:04:19.000000 mirrorbot-0.6/bot/modules/listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-04-17 14:04:19.000000 mirrorbot-0.6/bot/modules/mediainfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24324 2023-04-17 14:04:19.000000 mirrorbot-0.6/bot/modules/mirror_leech.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-04-17 14:04:19.000000 mirrorbot-0.6/bot/modules/mirror_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-04-17 14:04:19.000000 mirrorbot-0.6/bot/modules/pictures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12419 2023-04-17 14:04:19.000000 mirrorbot-0.6/bot/modules/rss.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-17 14:04:19.000000 mirrorbot-0.6/bot/modules/save_msg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18977 2023-04-17 14:04:19.000000 mirrorbot-0.6/bot/modules/scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12477 2023-04-17 14:04:19.000000 mirrorbot-0.6/bot/modules/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6625 2023-04-17 14:04:19.000000 mirrorbot-0.6/bot/modules/sel_cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-04-17 14:04:19.000000 mirrorbot-0.6/bot/modules/shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-04-17 14:04:19.000000 mirrorbot-0.6/bot/modules/speedtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-04-17 14:04:19.000000 mirrorbot-0.6/bot/modules/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34924 2023-04-17 14:04:19.000000 mirrorbot-0.6/bot/modules/users_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4929 2023-04-17 14:04:19.000000 mirrorbot-0.6/bot/modules/wayback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21193 2023-04-17 14:04:19.000000 mirrorbot-0.6/bot/modules/ytdlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:04:28.750020 mirrorbot-0.6/mirrorbot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-17 14:04:28.000000 mirrorbot-0.6/mirrorbot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-17 14:04:28.000000 mirrorbot-0.6/mirrorbot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 14:04:28.000000 mirrorbot-0.6/mirrorbot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-17 14:04:28.000000 mirrorbot-0.6/mirrorbot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-17 14:04:28.000000 mirrorbot-0.6/mirrorbot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-17 14:04:28.000000 mirrorbot-0.6/mirrorbot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 14:04:28.750020 mirrorbot-0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-17 14:04:19.000000 mirrorbot-0.6/setup.py
```

### Comparing `mirrorbot-0.5/bot/__main__.py` & `mirrorbot-0.6/bot/__main__.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.5/bot/modules/anilist.py` & `mirrorbot-0.6/bot/modules/anilist.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.5/bot/modules/authorize.py` & `mirrorbot-0.6/bot/modules/authorize.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.5/bot/modules/bot_settings.py` & `mirrorbot-0.6/bot/modules/bot_settings.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.5/bot/modules/broadcast.py` & `mirrorbot-0.6/bot/modules/broadcast.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.5/bot/modules/bt_select.py` & `mirrorbot-0.6/bot/modules/bt_select.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.5/bot/modules/cancel_mirror.py` & `mirrorbot-0.6/bot/modules/cancel_mirror.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.5/bot/modules/clone.py` & `mirrorbot-0.6/bot/modules/clone.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.5/bot/modules/count.py` & `mirrorbot-0.6/bot/modules/count.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.5/bot/modules/delete.py` & `mirrorbot-0.6/bot/modules/delete.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.5/bot/modules/drive_clean.py` & `mirrorbot-0.6/bot/modules/drive_clean.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.5/bot/modules/eval.py` & `mirrorbot-0.6/bot/modules/eval.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.5/bot/modules/gmail.py` & `mirrorbot-0.6/bot/modules/gmail.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.5/bot/modules/hash.py` & `mirrorbot-0.6/bot/modules/hash.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.5/bot/modules/imdb.py` & `mirrorbot-0.6/bot/modules/imdb.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.5/bot/modules/list.py` & `mirrorbot-0.6/bot/modules/list.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.5/bot/modules/listener.py` & `mirrorbot-0.6/bot/modules/listener.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.5/bot/modules/mediainfo.py` & `mirrorbot-0.6/bot/modules/mediainfo.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.5/bot/modules/mirror_leech.py` & `mirrorbot-0.6/bot/modules/mirror_leech.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.5/bot/modules/mirror_status.py` & `mirrorbot-0.6/bot/modules/mirror_status.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.5/bot/modules/pictures.py` & `mirrorbot-0.6/bot/modules/pictures.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.5/bot/modules/rss.py` & `mirrorbot-0.6/bot/modules/rss.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.5/bot/modules/save_msg.py` & `mirrorbot-0.6/bot/modules/save_msg.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.5/bot/modules/scraper.py` & `mirrorbot-0.6/bot/modules/scraper.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.5/bot/modules/search.py` & `mirrorbot-0.6/bot/modules/search.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.5/bot/modules/sel_cat.py` & `mirrorbot-0.6/bot/modules/sel_cat.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.5/bot/modules/shell.py` & `mirrorbot-0.6/bot/modules/shell.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.5/bot/modules/speedtest.py` & `mirrorbot-0.6/bot/modules/speedtest.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.5/bot/modules/users.py` & `mirrorbot-0.6/bot/modules/users.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.5/bot/modules/users_settings.py` & `mirrorbot-0.6/bot/modules/users_settings.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.5/bot/modules/wayback.py` & `mirrorbot-0.6/bot/modules/wayback.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.5/bot/modules/ytdlp.py` & `mirrorbot-0.6/bot/modules/ytdlp.py`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.5/mirrorbot.egg-info/SOURCES.txt` & `mirrorbot-0.6/mirrorbot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mirrorbot-0.5/setup.py` & `mirrorbot-0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mirrorbot',
-    version='0.5',
+    version='0.6',
     packages=find_packages(),
     include_package_data=True,
     package_data={
         '': ['*.*']
     },
     install_requires=[
         'aiohttp',
```

