# Comparing `tmp/ytpodgen-0.2.5.tar.gz` & `tmp/ytpodgen-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ytpodgen-0.2.5.tar", max compression
+gzip compressed data, was "ytpodgen-0.2.6.tar", max compression
```

## Comparing `ytpodgen-0.2.5.tar` & `ytpodgen-0.2.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1071 2023-03-27 04:22:24.231435 ytpodgen-0.2.5/LICENSE
--rw-r--r--   0        0        0     3019 2023-04-01 03:12:31.866761 ytpodgen-0.2.5/README.md
--rw-r--r--   0        0        0      616 2023-04-10 05:16:14.794097 ytpodgen-0.2.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-27 04:22:24.232397 ytpodgen-0.2.5/ytpodgen/__init__.py
--rw-r--r--   0        0        0     1631 2023-04-10 05:13:17.721804 ytpodgen-0.2.5/ytpodgen/downloader.py
--rw-r--r--   0        0        0     1225 2023-04-10 03:41:14.385965 ytpodgen-0.2.5/ytpodgen/feedgenerator.py
--rw-r--r--   0        0        0     1795 2023-04-08 05:56:06.207718 ytpodgen-0.2.5/ytpodgen/uploader.py
--rw-r--r--   0        0        0     2870 2023-04-10 03:32:52.623757 ytpodgen-0.2.5/ytpodgen/ytpodgen.py
--rw-r--r--   0        0        0     3809 1970-01-01 00:00:00.000000 ytpodgen-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-17 03:41:08.602094 ytpodgen-0.2.6/LICENSE
+-rw-r--r--   0        0        0     3336 2023-04-17 03:41:08.602094 ytpodgen-0.2.6/README.md
+-rw-r--r--   0        0        0      616 2023-04-17 03:41:08.602094 ytpodgen-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-17 03:41:08.606094 ytpodgen-0.2.6/ytpodgen/__init__.py
+-rw-r--r--   0        0        0     1193 2023-04-17 03:41:08.606094 ytpodgen-0.2.6/ytpodgen/downloader.py
+-rw-r--r--   0        0        0     1225 2023-04-17 03:41:08.606094 ytpodgen-0.2.6/ytpodgen/feedgenerator.py
+-rw-r--r--   0        0        0     1795 2023-04-17 03:41:08.606094 ytpodgen-0.2.6/ytpodgen/uploader.py
+-rw-r--r--   0        0        0     2870 2023-04-17 03:41:08.606094 ytpodgen-0.2.6/ytpodgen/ytpodgen.py
+-rw-r--r--   0        0        0     4126 1970-01-01 00:00:00.000000 ytpodgen-0.2.6/PKG-INFO
```

### Comparing `ytpodgen-0.2.5/LICENSE` & `ytpodgen-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ytpodgen-0.2.5/README.md` & `ytpodgen-0.2.6/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -47,21 +47,32 @@
 TITLE=<title> ; #title for your podcast
 HOSTNAME=<hostname> ; #hostname to serve files from
 ytpodgen --title ${TITLE} --hostname ${HOSTNAME}
 ```
 
 This generates `index.rss` file under current directory and exits.
 
+## How to release
+Executing the commands below, and the GitHub Actions publishes new package to PyPI.
+
+```bash
+poetry version <patch/minor/major>
+git add pyproject.toml && git commit -m $(poetry version -s)
+git push origin main
+gh release create --generate-notes "v$(poetry version -s)"
+git fetch --tags origin
+```
+
 ## Why only Cloudflare R2, and not other S3-compatible cloud storage?
 Because:
 
 - It offers free tier for up to 10GB of storage space per month
 - With Cloudflare Worker, basic auth can be applied to the uploaded files that are made public
 
 ## how I configured basic auth on Cloudflare R2 using Cloudflare Workers
 1. connected a custom domain to my R2 bucket, to make the bucket public. [docs](https://developers.cloudflare.com/r2/buckets/public-buckets/)
 2. configured a basic auth worker by following steps described [here](https://qiita.com/AnaKutsu/items/1c8bd0eb938edd3c0e0a).
 3. replaced the plaintext declaration of password with worker env var. [docs](https://developers.cloudflare.com/workers/platform/environment-variables/#environment-variables-via-the-dashboard)
 4. added a trigger(custom domain route) to the basic auth worker. [docs](https://developers.cloudflare.com/workers/platform/triggers/routes/)
 
 ## TODO/IDEAS
-moved to [GitHub issues](https://github.com/harupong/ytpodgen/issues/)
+moved to [GitHub issues](https://github.com/harupong/ytpodgen/issues/)
```

#### html2text {}

```diff
@@ -20,21 +20,25 @@
 ``` TITLE=
  ; #YouTube live URL that ends with "/live" HOSTNAME= ; #hostname to serve
 files from screen -dmS ${TITLE} ytpodgen --upload-r2 --liveurl ${LIVEURL} --
 title ${TITLE} --hostname ${HOSTNAME} ``` ### I just want to generate RSS from
 mp3 files, no download/upload needed ``` TITLE=
  ; #hostname to serve files from ytpodgen --title ${TITLE} --hostname $
 {HOSTNAME} ``` This generates `index.rss` file under current directory and
-exits. ## Why only Cloudflare R2, and not other S3-compatible cloud storage?
-Because: - It offers free tier for up to 10GB of storage space per month - With
-Cloudflare Worker, basic auth can be applied to the uploaded files that are
-made public ## how I configured basic auth on Cloudflare R2 using Cloudflare
-Workers 1. connected a custom domain to my R2 bucket, to make the bucket
-public. [docs](https://developers.cloudflare.com/r2/buckets/public-buckets/) 2.
-configured a basic auth worker by following steps described [here](https://
-qiita.com/AnaKutsu/items/1c8bd0eb938edd3c0e0a). 3. replaced the plaintext
-declaration of password with worker env var. [docs](https://
+exits. ## How to release Executing the commands below, and the GitHub Actions
+publishes new package to PyPI. ```bash poetry version
+inor/major> git add pyproject.toml && git commit -m $(poetry version -s) git
+push origin main gh release create --generate-notes "v$(poetry version -s)" git
+fetch --tags origin ``` ## Why only Cloudflare R2, and not other S3-compatible
+cloud storage? Because: - It offers free tier for up to 10GB of storage space
+per month - With Cloudflare Worker, basic auth can be applied to the uploaded
+files that are made public ## how I configured basic auth on Cloudflare R2
+using Cloudflare Workers 1. connected a custom domain to my R2 bucket, to make
+the bucket public. [docs](https://developers.cloudflare.com/r2/buckets/public-
+buckets/) 2. configured a basic auth worker by following steps described [here]
+(https://qiita.com/AnaKutsu/items/1c8bd0eb938edd3c0e0a). 3. replaced the
+plaintext declaration of password with worker env var. [docs](https://
 developers.cloudflare.com/workers/platform/environment-variables/#environment-
 variables-via-the-dashboard) 4. added a trigger(custom domain route) to the
 basic auth worker. [docs](https://developers.cloudflare.com/workers/platform/
 triggers/routes/) ## TODO/IDEAS moved to [GitHub issues](https://github.com/
 harupong/ytpodgen/issues/)
```

### Comparing `ytpodgen-0.2.5/pyproject.toml` & `ytpodgen-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ytpodgen"
-version = "0.2.5"
+version = "0.2.6"
 description = "turns YouTube live streams into podcasts"
 license = "MIT"
 authors = ["harupong <harupong@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/harupong/ytpodgen"
 
 [tool.poetry.dependencies]
```

### Comparing `ytpodgen-0.2.5/ytpodgen/downloader.py` & `ytpodgen-0.2.6/ytpodgen/downloader.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 
 class Downloader:
     def __init__(self):
         pass
 
     @staticmethod
     def download(title, liveurl):
-        live_from_start = True if Downloader._is_live(liveurl) else False
-
+        live_from_start = True
+        
         # See help(yt_dlp.YoutubeDL) for a list of available options
         # and public functions
         # https://github.com/yt-dlp/yt-dlp/blob/216bcb66d7dce0762767d751dad10650cb57da9d/yt_dlp/YoutubeDL.py#L184
         ydl_opts = {
             # best audio-only format if available,
             # and if not, fall back to best format that contains both video and audio
             "format": "bestaudio/best",
-            "wait_for_video": (60, 60),
+            "wait_for_video": (60, 600),
             "outtmpl": f"{title}_%(epoch>%Y%m%d%H%M%S)s_%(id)s",
             "live_from_start": live_from_start,
             "postprocessors": [
                 {  # Extract audio using ffmpeg
                     "key": "FFmpegExtractAudio",
                     "preferredcodec": "mp3",
                     "preferredquality": "64",
@@ -30,18 +30,7 @@
                 "-ac",
                 "1",  # audio channel mono
             ],
         }
 
         with yt_dlp.YoutubeDL(ydl_opts) as ydl:
             ydl.download(liveurl)
-
-    @staticmethod
-    def _is_live(liveurl):
-        ydl_opts = {}
-        with yt_dlp.YoutubeDL(ydl_opts) as ydl:
-            try:
-                info = ydl.extract_info(liveurl, download=False)
-                live_status = info["live_status"].rstrip("\n")
-                return True if live_status == "is_live" else False
-            except yt_dlp.utils.DownloadError:
-                return False
```

### Comparing `ytpodgen-0.2.5/ytpodgen/feedgenerator.py` & `ytpodgen-0.2.6/ytpodgen/feedgenerator.py`

 * *Files identical despite different names*

### Comparing `ytpodgen-0.2.5/ytpodgen/uploader.py` & `ytpodgen-0.2.6/ytpodgen/uploader.py`

 * *Files identical despite different names*

### Comparing `ytpodgen-0.2.5/ytpodgen/ytpodgen.py` & `ytpodgen-0.2.6/ytpodgen/ytpodgen.py`

 * *Files identical despite different names*

### Comparing `ytpodgen-0.2.5/PKG-INFO` & `ytpodgen-0.2.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytpodgen
-Version: 0.2.5
+Version: 0.2.6
 Summary: turns YouTube live streams into podcasts
 Home-page: https://github.com/harupong/ytpodgen
 License: MIT
 Author: harupong
 Author-email: harupong@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -69,21 +69,33 @@
 TITLE=<title> ; #title for your podcast
 HOSTNAME=<hostname> ; #hostname to serve files from
 ytpodgen --title ${TITLE} --hostname ${HOSTNAME}
 ```
 
 This generates `index.rss` file under current directory and exits.
 
+## How to release
+Executing the commands below, and the GitHub Actions publishes new package to PyPI.
+
+```bash
+poetry version <patch/minor/major>
+git add pyproject.toml && git commit -m $(poetry version -s)
+git push origin main
+gh release create --generate-notes "v$(poetry version -s)"
+git fetch --tags origin
+```
+
 ## Why only Cloudflare R2, and not other S3-compatible cloud storage?
 Because:
 
 - It offers free tier for up to 10GB of storage space per month
 - With Cloudflare Worker, basic auth can be applied to the uploaded files that are made public
 
 ## how I configured basic auth on Cloudflare R2 using Cloudflare Workers
 1. connected a custom domain to my R2 bucket, to make the bucket public. [docs](https://developers.cloudflare.com/r2/buckets/public-buckets/)
 2. configured a basic auth worker by following steps described [here](https://qiita.com/AnaKutsu/items/1c8bd0eb938edd3c0e0a).
 3. replaced the plaintext declaration of password with worker env var. [docs](https://developers.cloudflare.com/workers/platform/environment-variables/#environment-variables-via-the-dashboard)
 4. added a trigger(custom domain route) to the basic auth worker. [docs](https://developers.cloudflare.com/workers/platform/triggers/routes/)
 
 ## TODO/IDEAS
 moved to [GitHub issues](https://github.com/harupong/ytpodgen/issues/)
+
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ytpodgen Version: 0.2.5 Summary: turns YouTube live
+Metadata-Version: 2.1 Name: ytpodgen Version: 0.2.6 Summary: turns YouTube live
 streams into podcasts Home-page: https://github.com/harupong/ytpodgen License:
 MIT Author: harupong Author-email: harupong@gmail.com Requires-Python:
 >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: boto3
 (>=1.26.89,<2.0.0) Requires-Dist: click (>=8.1.3,<9.0.0) Requires-Dist: loguru
 (>=0.6.0,<0.7.0) Requires-Dist: podgen (>=1.1.0,<2.0.0) Requires-Dist: requests
@@ -30,21 +30,25 @@
 ``` TITLE=
  ; #YouTube live URL that ends with "/live" HOSTNAME= ; #hostname to serve
 files from screen -dmS ${TITLE} ytpodgen --upload-r2 --liveurl ${LIVEURL} --
 title ${TITLE} --hostname ${HOSTNAME} ``` ### I just want to generate RSS from
 mp3 files, no download/upload needed ``` TITLE=
  ; #hostname to serve files from ytpodgen --title ${TITLE} --hostname $
 {HOSTNAME} ``` This generates `index.rss` file under current directory and
-exits. ## Why only Cloudflare R2, and not other S3-compatible cloud storage?
-Because: - It offers free tier for up to 10GB of storage space per month - With
-Cloudflare Worker, basic auth can be applied to the uploaded files that are
-made public ## how I configured basic auth on Cloudflare R2 using Cloudflare
-Workers 1. connected a custom domain to my R2 bucket, to make the bucket
-public. [docs](https://developers.cloudflare.com/r2/buckets/public-buckets/) 2.
-configured a basic auth worker by following steps described [here](https://
-qiita.com/AnaKutsu/items/1c8bd0eb938edd3c0e0a). 3. replaced the plaintext
-declaration of password with worker env var. [docs](https://
+exits. ## How to release Executing the commands below, and the GitHub Actions
+publishes new package to PyPI. ```bash poetry version
+inor/major> git add pyproject.toml && git commit -m $(poetry version -s) git
+push origin main gh release create --generate-notes "v$(poetry version -s)" git
+fetch --tags origin ``` ## Why only Cloudflare R2, and not other S3-compatible
+cloud storage? Because: - It offers free tier for up to 10GB of storage space
+per month - With Cloudflare Worker, basic auth can be applied to the uploaded
+files that are made public ## how I configured basic auth on Cloudflare R2
+using Cloudflare Workers 1. connected a custom domain to my R2 bucket, to make
+the bucket public. [docs](https://developers.cloudflare.com/r2/buckets/public-
+buckets/) 2. configured a basic auth worker by following steps described [here]
+(https://qiita.com/AnaKutsu/items/1c8bd0eb938edd3c0e0a). 3. replaced the
+plaintext declaration of password with worker env var. [docs](https://
 developers.cloudflare.com/workers/platform/environment-variables/#environment-
 variables-via-the-dashboard) 4. added a trigger(custom domain route) to the
 basic auth worker. [docs](https://developers.cloudflare.com/workers/platform/
 triggers/routes/) ## TODO/IDEAS moved to [GitHub issues](https://github.com/
 harupong/ytpodgen/issues/)
```

