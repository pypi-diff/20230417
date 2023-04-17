# Comparing `tmp/twtvt-2023.4.15.post3.tar.gz` & `tmp/twtvt-2023.4.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twtvt-2023.4.15.post3.tar", max compression
+gzip compressed data, was "twtvt-2023.4.17.tar", max compression
```

## Comparing `twtvt-2023.4.15.post3.tar` & `twtvt-2023.4.17.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1017 2023-04-15 14:50:13.568083 twtvt-2023.4.15.post3/README.md
--rw-r--r--   0        0        0     1465 2023-04-15 14:50:37.808502 twtvt-2023.4.15.post3/pyproject.toml
--rw-r--r--   0        0        0      120 2023-04-15 14:50:13.568083 twtvt-2023.4.15.post3/twtvt/__init__.py
--rw-r--r--   0        0        0      110 2023-04-15 14:50:13.568083 twtvt-2023.4.15.post3/twtvt/__main__.py
--rw-r--r--   0        0        0       41 2023-04-15 14:50:13.568083 twtvt-2023.4.15.post3/twtvt/cli/__init__.py
--rw-r--r--   0        0        0     1172 2023-04-15 14:50:13.568083 twtvt-2023.4.15.post3/twtvt/cli/commands.py
--rw-r--r--   0        0        0       79 2023-04-15 14:50:13.568083 twtvt-2023.4.15.post3/twtvt/main.py
--rw-r--r--   0        0        0        0 2023-04-15 14:50:13.568083 twtvt-2023.4.15.post3/twtvt/tests/__init__.py
--rw-r--r--   0        0        0       47 2023-04-15 14:50:13.568083 twtvt-2023.4.15.post3/twtvt/tests/sample_test.py
--rw-r--r--   0        0        0      238 2023-04-15 14:50:13.568083 twtvt-2023.4.15.post3/twtvt/utils/__init__.py
--rw-r--r--   0        0        0     4603 2023-04-15 14:50:13.568083 twtvt-2023.4.15.post3/twtvt/utils/download_video.py
--rw-r--r--   0        0        0      249 2023-04-15 14:50:13.568083 twtvt-2023.4.15.post3/twtvt/utils/logger.py
--rw-r--r--   0        0        0     1354 2023-04-15 14:50:13.568083 twtvt-2023.4.15.post3/twtvt/utils/monsnode_parser.py
--rw-r--r--   0        0        0     7831 2023-04-15 14:50:13.568083 twtvt-2023.4.15.post3/twtvt/utils/twitter_parser.py
--rw-r--r--   0        0        0      566 2023-04-15 14:50:13.568083 twtvt-2023.4.15.post3/twtvt/utils/uri_validator.py
--rw-r--r--   0        0        0     1690 1970-01-01 00:00:00.000000 twtvt-2023.4.15.post3/PKG-INFO
+-rw-r--r--   0        0        0     1017 2023-04-17 06:38:46.115317 twtvt-2023.4.17/README.md
+-rw-r--r--   0        0        0     1463 2023-04-17 06:39:10.563368 twtvt-2023.4.17/pyproject.toml
+-rw-r--r--   0        0        0      120 2023-04-17 06:38:46.115317 twtvt-2023.4.17/twtvt/__init__.py
+-rw-r--r--   0        0        0      110 2023-04-17 06:38:46.115317 twtvt-2023.4.17/twtvt/__main__.py
+-rw-r--r--   0        0        0       41 2023-04-17 06:38:46.115317 twtvt-2023.4.17/twtvt/cli/__init__.py
+-rw-r--r--   0        0        0     1172 2023-04-17 06:38:46.115317 twtvt-2023.4.17/twtvt/cli/commands.py
+-rw-r--r--   0        0        0       79 2023-04-17 06:38:46.115317 twtvt-2023.4.17/twtvt/main.py
+-rw-r--r--   0        0        0        0 2023-04-17 06:38:46.115317 twtvt-2023.4.17/twtvt/tests/__init__.py
+-rw-r--r--   0        0        0       47 2023-04-17 06:38:46.115317 twtvt-2023.4.17/twtvt/tests/sample_test.py
+-rw-r--r--   0        0        0      238 2023-04-17 06:38:46.115317 twtvt-2023.4.17/twtvt/utils/__init__.py
+-rw-r--r--   0        0        0     4727 2023-04-17 06:38:46.115317 twtvt-2023.4.17/twtvt/utils/download_video.py
+-rw-r--r--   0        0        0      249 2023-04-17 06:38:46.115317 twtvt-2023.4.17/twtvt/utils/logger.py
+-rw-r--r--   0        0        0     1354 2023-04-17 06:38:46.115317 twtvt-2023.4.17/twtvt/utils/monsnode_parser.py
+-rw-r--r--   0        0        0     7831 2023-04-17 06:38:46.115317 twtvt-2023.4.17/twtvt/utils/twitter_parser.py
+-rw-r--r--   0        0        0      566 2023-04-17 06:38:46.115317 twtvt-2023.4.17/twtvt/utils/uri_validator.py
+-rw-r--r--   0        0        0     1684 1970-01-01 00:00:00.000000 twtvt-2023.4.17/PKG-INFO
```

### Comparing `twtvt-2023.4.15.post3/README.md` & `twtvt-2023.4.17/README.md`

 * *Files identical despite different names*

### Comparing `twtvt-2023.4.15.post3/pyproject.toml` & `twtvt-2023.4.17/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "twtvt"
-version = "2023.04.15-3"
+version = "2023.04.17"
 description = ""
 authors = []
 readme = "README.md"
 [[tool.poetry.packages]]
 include = "twtvt"
 
 [tool.pyright]
```

### Comparing `twtvt-2023.4.15.post3/twtvt/cli/commands.py` & `twtvt-2023.4.17/twtvt/cli/commands.py`

 * *Files identical despite different names*

### Comparing `twtvt-2023.4.15.post3/twtvt/utils/download_video.py` & `twtvt-2023.4.17/twtvt/utils/download_video.py`

 * *Files 5% similar despite different names*

```diff
@@ -97,23 +97,26 @@
     with open(f'{output}/links-{int(time.time())}-{len(links)}_videos.txt', 'w') as f:
         f.write('\n'.join(links))
 
 
 def _download_videos(video_links: tuple[str], output: str, cookies_from_browser: Optional[str]):
     for index, video_link in enumerate(video_links):
         logger.info(f'Downloading video from {video_link} ({index + 1}/{len(video_links)})')
-        _download_video(video_link, output, cookies_from_browser)
+        try:
+            _download_video(video_link, output, cookies_from_browser)
+        except Exception as e:
+            logger.error(f'Failed to download video from {video_link}: {e}')
 
 
 @retry(
     reraise=True,
     before_sleep=before_sleep_log(logger, logging.DEBUG),
     after=after_log(logger, logging.INFO),
-    stop=stop_after_attempt(60),
-    wait=wait_fixed(5),
+    stop=stop_after_attempt(5),
+    wait=wait_fixed(3),
 )
 def _download_video(video_link: str, output: str, cookies_from_browser: Optional[str]):
     ydl_opts: dict[str, Union[str, bool, tuple[Optional[str]]]] = {
         'nocheckcertificate': True,
     }
     ydl_opts['outtmpl'] = f'{output}/%(title)s.%(upload_date>%Y-%m-%d)s.%(id)s.%(ext)s'
     if cookies_from_browser:
```

### Comparing `twtvt-2023.4.15.post3/twtvt/utils/monsnode_parser.py` & `twtvt-2023.4.17/twtvt/utils/monsnode_parser.py`

 * *Files identical despite different names*

### Comparing `twtvt-2023.4.15.post3/twtvt/utils/twitter_parser.py` & `twtvt-2023.4.17/twtvt/utils/twitter_parser.py`

 * *Files identical despite different names*

### Comparing `twtvt-2023.4.15.post3/twtvt/utils/uri_validator.py` & `twtvt-2023.4.17/twtvt/utils/uri_validator.py`

 * *Files identical despite different names*

### Comparing `twtvt-2023.4.15.post3/PKG-INFO` & `twtvt-2023.4.17/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twtvt
-Version: 2023.4.15.post3
+Version: 2023.4.17
 Summary: 
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
```

