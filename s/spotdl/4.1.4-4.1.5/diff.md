# Comparing `tmp/spotdl-4.1.4.tar.gz` & `tmp/spotdl-4.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotdl-4.1.4.tar", max compression
+gzip compressed data, was "spotdl-4.1.5.tar", max compression
```

## Comparing `spotdl-4.1.4.tar` & `spotdl-4.1.5.tar`

### file list

```diff
@@ -1,54 +1,56 @@
--rw-r--r--   0        0        0     1074 2023-04-06 15:40:24.068964 spotdl-4.1.4/LICENSE
--rw-r--r--   0        0        0     5814 2023-04-06 15:40:24.068964 spotdl-4.1.4/README.md
--rw-r--r--   0        0        0     2745 2023-04-06 15:40:24.076964 spotdl-4.1.4/pyproject.toml
--rw-r--r--   0        0        0     4668 2023-04-06 15:40:24.076964 spotdl-4.1.4/spotdl/__init__.py
--rw-r--r--   0        0        0      209 2023-04-06 15:40:24.076964 spotdl-4.1.4/spotdl/__main__.py
--rw-r--r--   0        0        0       58 2023-04-06 15:40:24.076964 spotdl-4.1.4/spotdl/_version.py
--rw-r--r--   0        0        0      186 2023-04-06 15:40:24.076964 spotdl-4.1.4/spotdl/console/__init__.py
--rw-r--r--   0        0        0      598 2023-04-06 15:40:24.076964 spotdl-4.1.4/spotdl/console/download.py
--rw-r--r--   0        0        0     3869 2023-04-06 15:40:24.076964 spotdl-4.1.4/spotdl/console/entry_point.py
--rw-r--r--   0        0        0     4695 2023-04-06 15:40:24.076964 spotdl-4.1.4/spotdl/console/meta.py
--rw-r--r--   0        0        0     2759 2023-04-06 15:40:24.076964 spotdl-4.1.4/spotdl/console/save.py
--rw-r--r--   0        0        0     4896 2023-04-06 15:40:24.076964 spotdl-4.1.4/spotdl/console/sync.py
--rw-r--r--   0        0        0     1702 2023-04-06 15:40:24.076964 spotdl-4.1.4/spotdl/console/url.py
--rw-r--r--   0        0        0     3041 2023-04-06 15:40:24.076964 spotdl-4.1.4/spotdl/console/web.py
--rw-r--r--   0        0        0       80 2023-04-06 15:40:24.076964 spotdl-4.1.4/spotdl/download/__init__.py
--rw-r--r--   0        0        0    26228 2023-04-06 15:40:24.076964 spotdl-4.1.4/spotdl/download/downloader.py
--rw-r--r--   0        0        0    13137 2023-04-06 15:40:24.076964 spotdl-4.1.4/spotdl/download/progress_handler.py
--rw-r--r--   0        0        0       54 2023-04-06 15:40:24.076964 spotdl-4.1.4/spotdl/providers/__init__.py
--rw-r--r--   0        0        0      396 2023-04-06 15:40:24.076964 spotdl-4.1.4/spotdl/providers/audio/__init__.py
--rw-r--r--   0        0        0    11033 2023-04-06 15:40:24.076964 spotdl-4.1.4/spotdl/providers/audio/base.py
--rw-r--r--   0        0        0     1840 2023-04-06 15:40:24.076964 spotdl-4.1.4/spotdl/providers/audio/youtube.py
--rw-r--r--   0        0        0     3111 2023-04-06 15:40:24.076964 spotdl-4.1.4/spotdl/providers/audio/ytmusic.py
--rw-r--r--   0        0        0      382 2023-04-06 15:40:24.076964 spotdl-4.1.4/spotdl/providers/lyrics/__init__.py
--rw-r--r--   0        0        0     3304 2023-04-06 15:40:24.076964 spotdl-4.1.4/spotdl/providers/lyrics/azlyrics.py
--rw-r--r--   0        0        0     3404 2023-04-06 15:40:24.076964 spotdl-4.1.4/spotdl/providers/lyrics/base.py
--rw-r--r--   0        0        0     3091 2023-04-06 15:40:24.076964 spotdl-4.1.4/spotdl/providers/lyrics/genius.py
--rw-r--r--   0        0        0     2765 2023-04-06 15:40:24.076964 spotdl-4.1.4/spotdl/providers/lyrics/musixmatch.py
--rw-r--r--   0        0        0     1689 2023-04-06 15:40:24.076964 spotdl-4.1.4/spotdl/providers/lyrics/synced.py
--rw-r--r--   0        0        0       38 2023-04-06 15:40:24.076964 spotdl-4.1.4/spotdl/types/__init__.py
--rw-r--r--   0        0        0     3451 2023-04-06 15:40:24.076964 spotdl-4.1.4/spotdl/types/album.py
--rw-r--r--   0        0        0     3101 2023-04-06 15:40:24.076964 spotdl-4.1.4/spotdl/types/artist.py
--rw-r--r--   0        0        0     3657 2023-04-06 15:40:24.076964 spotdl-4.1.4/spotdl/types/options.py
--rw-r--r--   0        0        0     4199 2023-04-06 15:40:24.076964 spotdl-4.1.4/spotdl/types/playlist.py
--rw-r--r--   0        0        0     2186 2023-04-06 15:40:24.076964 spotdl-4.1.4/spotdl/types/result.py
--rw-r--r--   0        0        0     3230 2023-04-06 15:40:24.076964 spotdl-4.1.4/spotdl/types/saved.py
--rw-r--r--   0        0        0     9758 2023-04-06 15:40:24.076964 spotdl-4.1.4/spotdl/types/song.py
--rw-r--r--   0        0        0      103 2023-04-06 15:40:24.076964 spotdl-4.1.4/spotdl/utils/__init__.py
--rw-r--r--   0        0        0     1001 2023-04-06 15:40:24.076964 spotdl-4.1.4/spotdl/utils/archive.py
--rw-r--r--   0        0        0    18627 2023-04-06 15:40:24.076964 spotdl-4.1.4/spotdl/utils/arguments.py
--rw-r--r--   0        0        0     6675 2023-04-06 15:40:24.076964 spotdl-4.1.4/spotdl/utils/config.py
--rw-r--r--   0        0        0     3109 2023-04-06 15:40:24.076964 spotdl-4.1.4/spotdl/utils/console.py
--rw-r--r--   0        0        0      571 2023-04-06 15:40:24.076964 spotdl-4.1.4/spotdl/utils/downloader.py
--rw-r--r--   0        0        0    11688 2023-04-06 15:40:24.076964 spotdl-4.1.4/spotdl/utils/ffmpeg.py
--rw-r--r--   0        0        0    14130 2023-04-06 15:40:24.076964 spotdl-4.1.4/spotdl/utils/formatter.py
--rw-r--r--   0        0        0     7018 2023-04-06 15:40:24.076964 spotdl-4.1.4/spotdl/utils/github.py
--rw-r--r--   0        0        0     5364 2023-04-06 15:40:24.076964 spotdl-4.1.4/spotdl/utils/logging.py
--rw-r--r--   0        0        0     4095 2023-04-06 15:40:24.076964 spotdl-4.1.4/spotdl/utils/m3u.py
--rw-r--r--   0        0        0    21866 2023-04-06 15:40:24.076964 spotdl-4.1.4/spotdl/utils/matching.py
--rw-r--r--   0        0        0    15344 2023-04-06 15:40:24.076964 spotdl-4.1.4/spotdl/utils/metadata.py
--rw-r--r--   0        0        0    15064 2023-04-06 15:40:24.076964 spotdl-4.1.4/spotdl/utils/search.py
--rw-r--r--   0        0        0     5660 2023-04-06 15:40:24.076964 spotdl-4.1.4/spotdl/utils/spotify.py
--rw-r--r--   0        0        0    28221 2023-04-06 15:40:24.076964 spotdl-4.1.4/spotdl/utils/static.py
--rw-r--r--   0        0        0    15281 2023-04-06 15:40:24.080964 spotdl-4.1.4/spotdl/utils/web.py
--rw-r--r--   0        0        0     8043 1970-01-01 00:00:00.000000 spotdl-4.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-04-17 18:38:54.557097 spotdl-4.1.5/LICENSE
+-rw-r--r--   0        0        0     5921 2023-04-17 18:38:54.557097 spotdl-4.1.5/README.md
+-rw-r--r--   0        0        0     2745 2023-04-17 18:38:54.561097 spotdl-4.1.5/pyproject.toml
+-rw-r--r--   0        0        0     4668 2023-04-17 18:38:54.561097 spotdl-4.1.5/spotdl/__init__.py
+-rw-r--r--   0        0        0      209 2023-04-17 18:38:54.561097 spotdl-4.1.5/spotdl/__main__.py
+-rw-r--r--   0        0        0       58 2023-04-17 18:38:54.561097 spotdl-4.1.5/spotdl/_version.py
+-rw-r--r--   0        0        0      186 2023-04-17 18:38:54.561097 spotdl-4.1.5/spotdl/console/__init__.py
+-rw-r--r--   0        0        0      598 2023-04-17 18:38:54.561097 spotdl-4.1.5/spotdl/console/download.py
+-rw-r--r--   0        0        0     3869 2023-04-17 18:38:54.561097 spotdl-4.1.5/spotdl/console/entry_point.py
+-rw-r--r--   0        0        0     5995 2023-04-17 18:38:54.561097 spotdl-4.1.5/spotdl/console/meta.py
+-rw-r--r--   0        0        0     2759 2023-04-17 18:38:54.561097 spotdl-4.1.5/spotdl/console/save.py
+-rw-r--r--   0        0        0     4896 2023-04-17 18:38:54.561097 spotdl-4.1.5/spotdl/console/sync.py
+-rw-r--r--   0        0        0     1702 2023-04-17 18:38:54.561097 spotdl-4.1.5/spotdl/console/url.py
+-rw-r--r--   0        0        0     3041 2023-04-17 18:38:54.561097 spotdl-4.1.5/spotdl/console/web.py
+-rw-r--r--   0        0        0       80 2023-04-17 18:38:54.561097 spotdl-4.1.5/spotdl/download/__init__.py
+-rw-r--r--   0        0        0    26849 2023-04-17 18:38:54.561097 spotdl-4.1.5/spotdl/download/downloader.py
+-rw-r--r--   0        0        0    13137 2023-04-17 18:38:54.561097 spotdl-4.1.5/spotdl/download/progress_handler.py
+-rw-r--r--   0        0        0       54 2023-04-17 18:38:54.561097 spotdl-4.1.5/spotdl/providers/__init__.py
+-rw-r--r--   0        0        0      465 2023-04-17 18:38:54.561097 spotdl-4.1.5/spotdl/providers/audio/__init__.py
+-rw-r--r--   0        0        0    10831 2023-04-17 18:38:54.561097 spotdl-4.1.5/spotdl/providers/audio/base.py
+-rw-r--r--   0        0        0     2665 2023-04-17 18:38:54.561097 spotdl-4.1.5/spotdl/providers/audio/sliderkz.py
+-rw-r--r--   0        0        0     1840 2023-04-17 18:38:54.561097 spotdl-4.1.5/spotdl/providers/audio/youtube.py
+-rw-r--r--   0        0        0     2789 2023-04-17 18:38:54.561097 spotdl-4.1.5/spotdl/providers/audio/ytmusic.py
+-rw-r--r--   0        0        0      382 2023-04-17 18:38:54.561097 spotdl-4.1.5/spotdl/providers/lyrics/__init__.py
+-rw-r--r--   0        0        0     3304 2023-04-17 18:38:54.561097 spotdl-4.1.5/spotdl/providers/lyrics/azlyrics.py
+-rw-r--r--   0        0        0     3529 2023-04-17 18:38:54.561097 spotdl-4.1.5/spotdl/providers/lyrics/base.py
+-rw-r--r--   0        0        0     3091 2023-04-17 18:38:54.561097 spotdl-4.1.5/spotdl/providers/lyrics/genius.py
+-rw-r--r--   0        0        0     2765 2023-04-17 18:38:54.561097 spotdl-4.1.5/spotdl/providers/lyrics/musixmatch.py
+-rw-r--r--   0        0        0     1689 2023-04-17 18:38:54.561097 spotdl-4.1.5/spotdl/providers/lyrics/synced.py
+-rw-r--r--   0        0        0       38 2023-04-17 18:38:54.561097 spotdl-4.1.5/spotdl/types/__init__.py
+-rw-r--r--   0        0        0     3451 2023-04-17 18:38:54.561097 spotdl-4.1.5/spotdl/types/album.py
+-rw-r--r--   0        0        0     3101 2023-04-17 18:38:54.561097 spotdl-4.1.5/spotdl/types/artist.py
+-rw-r--r--   0        0        0     3615 2023-04-17 18:38:54.561097 spotdl-4.1.5/spotdl/types/options.py
+-rw-r--r--   0        0        0     4199 2023-04-17 18:38:54.561097 spotdl-4.1.5/spotdl/types/playlist.py
+-rw-r--r--   0        0        0     2186 2023-04-17 18:38:54.561097 spotdl-4.1.5/spotdl/types/result.py
+-rw-r--r--   0        0        0     3230 2023-04-17 18:38:54.561097 spotdl-4.1.5/spotdl/types/saved.py
+-rw-r--r--   0        0        0     9758 2023-04-17 18:38:54.561097 spotdl-4.1.5/spotdl/types/song.py
+-rw-r--r--   0        0        0      103 2023-04-17 18:38:54.561097 spotdl-4.1.5/spotdl/utils/__init__.py
+-rw-r--r--   0        0        0     1001 2023-04-17 18:38:54.565097 spotdl-4.1.5/spotdl/utils/archive.py
+-rw-r--r--   0        0        0    18452 2023-04-17 18:38:54.565097 spotdl-4.1.5/spotdl/utils/arguments.py
+-rw-r--r--   0        0        0     6650 2023-04-17 18:38:54.565097 spotdl-4.1.5/spotdl/utils/config.py
+-rw-r--r--   0        0        0     3109 2023-04-17 18:38:54.565097 spotdl-4.1.5/spotdl/utils/console.py
+-rw-r--r--   0        0        0      571 2023-04-17 18:38:54.565097 spotdl-4.1.5/spotdl/utils/downloader.py
+-rw-r--r--   0        0        0    11688 2023-04-17 18:38:54.565097 spotdl-4.1.5/spotdl/utils/ffmpeg.py
+-rw-r--r--   0        0        0    14159 2023-04-17 18:38:54.565097 spotdl-4.1.5/spotdl/utils/formatter.py
+-rw-r--r--   0        0        0     7018 2023-04-17 18:38:54.565097 spotdl-4.1.5/spotdl/utils/github.py
+-rw-r--r--   0        0        0     5364 2023-04-17 18:38:54.565097 spotdl-4.1.5/spotdl/utils/logging.py
+-rw-r--r--   0        0        0      940 2023-04-17 18:38:54.565097 spotdl-4.1.5/spotdl/utils/lrc.py
+-rw-r--r--   0        0        0     4144 2023-04-17 18:38:54.565097 spotdl-4.1.5/spotdl/utils/m3u.py
+-rw-r--r--   0        0        0    23312 2023-04-17 18:38:54.565097 spotdl-4.1.5/spotdl/utils/matching.py
+-rw-r--r--   0        0        0    15525 2023-04-17 18:38:54.565097 spotdl-4.1.5/spotdl/utils/metadata.py
+-rw-r--r--   0        0        0    15207 2023-04-17 18:38:54.565097 spotdl-4.1.5/spotdl/utils/search.py
+-rw-r--r--   0        0        0     5660 2023-04-17 18:38:54.565097 spotdl-4.1.5/spotdl/utils/spotify.py
+-rw-r--r--   0        0        0    28221 2023-04-17 18:38:54.565097 spotdl-4.1.5/spotdl/utils/static.py
+-rw-r--r--   0        0        0    15281 2023-04-17 18:38:54.565097 spotdl-4.1.5/spotdl/utils/web.py
+-rw-r--r--   0        0        0     8150 1970-01-01 00:00:00.000000 spotdl-4.1.5/PKG-INFO
```

### Comparing `spotdl-4.1.4/LICENSE` & `spotdl-4.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.4/README.md` & `spotdl-4.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -109,14 +109,18 @@
 
 - `save`: Saves only the metadata from Spotify without downloading anything.
     - Usage:
         `spotdl save [query] --save-file {filename}.spotdl`
 
 - `web`: Starts a web interface instead of using the command line. However, it has limited features and only supports downloading single songs.
 
+- `url`: Get direct download link for each song from the query.
+    - Usage:
+        `spotdl web [query]`
+
 - `sync`: Updates directories. Compares the directory with the current state of the playlist. Newly added songs will be downloaded and removed songs will be deleted. No other songs will be downloaded and no other files will be deleted.
 
     - Usage:
         `spotdl sync [query] --save-file {filename}.spotdl`
 
         This create a new **sync** file, to update the directory in the future, use:
```

### Comparing `spotdl-4.1.4/pyproject.toml` & `spotdl-4.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spotdl"
-version = "4.1.4"
+version = "4.1.5"
 description = "Download your Spotify playlists and songs along with album art and metadata"
 license = "MIT"
 authors = ["spotDL Team <spotdladmins@googlegroups.com>"]
 maintainers = ["xnetcat <xnetcat.dev@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/spotDL/spotify-downloader.git"
 homepage = "https://github.com/spotDL/spotify-downloader/"
```

### Comparing `spotdl-4.1.4/spotdl/__init__.py` & `spotdl-4.1.5/spotdl/__init__.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.4/spotdl/console/download.py` & `spotdl-4.1.5/spotdl/console/download.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.4/spotdl/console/entry_point.py` & `spotdl-4.1.5/spotdl/console/entry_point.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.4/spotdl/console/meta.py` & `spotdl-4.1.5/spotdl/console/meta.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import logging
 from pathlib import Path
 from typing import List
 
 from spotdl.download.downloader import Downloader
 from spotdl.types.song import Song
 from spotdl.utils.ffmpeg import FFMPEG_FORMATS
+from spotdl.utils.lrc import generate_lrc
 from spotdl.utils.metadata import embed_metadata, get_file_metadata
 from spotdl.utils.search import QueryError, get_search_results, reinit_song
 
 __all__ = ["meta"]
 
 logger = logging.getLogger(__name__)
 
@@ -61,14 +62,32 @@
                 song_meta.get("artist")
                 and song_meta.get("artists")
                 and song_meta.get("name")
                 and song_meta.get("lyrics")
                 and song_meta.get("album_art")
             ):
                 logger.info("Song already has metadata: %s", file.name)
+                if downloader.settings["generate_lrc"]:
+                    lrc_file = file.with_suffix(".lrc")
+                    if lrc_file.exists():
+                        logger.info("Lrc file already exists for %s", file.name)
+                        return None
+
+                    song = Song.from_missing_data(
+                        name=song_meta["name"],
+                        artists=song_meta["artists"],
+                        artist=song_meta["artist"],
+                    )
+
+                    generate_lrc(song, file)
+                    if lrc_file.exists():
+                        logger.info("Saved lrc file for %s", song.display_name)
+                    else:
+                        logger.info("Could not find lrc file for %s", song.display_name)
+
                 return None
 
         # Same as above
         if (
             not song_meta
             or None
             in [
@@ -110,14 +129,26 @@
             song.lyrics = song_meta.get("lyrics")
 
         # Apply metadata to the song
         embed_metadata(file, song)
 
         logger.info("Applied metadata to %s", file.name)
 
+        if downloader.settings["generate_lrc"]:
+            lrc_file = file.with_suffix(".lrc")
+            if lrc_file.exists():
+                logger.info("Lrc file already exists for %s", file.name)
+                return None
+
+            generate_lrc(song, file)
+            if lrc_file.exists():
+                logger.info("Saved lrc file for %s", song.display_name)
+            else:
+                logger.info("Could not find lrc file for %s", song.display_name)
+
         return None
 
     async def pool_worker(file_path: Path) -> None:
         async with downloader.semaphore:
             # The following function calls blocking code, which would block whole event loop.
             # Therefore it has to be called in a separate thread via ThreadPoolExecutor. This
             # is not a problem, since GIL is released for the I/O operations, so it shouldn't
```

### Comparing `spotdl-4.1.4/spotdl/console/save.py` & `spotdl-4.1.5/spotdl/console/save.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.4/spotdl/console/sync.py` & `spotdl-4.1.5/spotdl/console/sync.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.4/spotdl/console/url.py` & `spotdl-4.1.5/spotdl/console/url.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.4/spotdl/console/web.py` & `spotdl-4.1.5/spotdl/console/web.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.4/spotdl/download/downloader.py` & `spotdl-4.1.5/spotdl/download/downloader.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,33 +9,33 @@
 import shutil
 import sys
 import traceback
 from argparse import Namespace
 from pathlib import Path
 from typing import Dict, List, Optional, Tuple, Type, Union
 
-from syncedlyrics import search as syncedlyrics_search
-from syncedlyrics.utils import is_lrc_valid, save_lrc_file
 from yt_dlp.postprocessor.modify_chapters import ModifyChaptersPP
 from yt_dlp.postprocessor.sponsorblock import SponsorBlockPP
 
 from spotdl.download.progress_handler import ProgressHandler
 from spotdl.providers.audio import AudioProvider, YouTube, YouTubeMusic
+from spotdl.providers.audio.sliderkz import SliderKZ
 from spotdl.providers.lyrics import AzLyrics, Genius, LyricsProvider, MusixMatch, Synced
 from spotdl.types.options import DownloaderOptionalOptions, DownloaderOptions
 from spotdl.types.song import Song
 from spotdl.utils.archive import Archive
 from spotdl.utils.config import (
     DOWNLOADER_OPTIONS,
     create_settings_type,
     get_errors_path,
     get_temp_path,
 )
 from spotdl.utils.ffmpeg import FFmpegError, convert, get_ffmpeg_path
 from spotdl.utils.formatter import create_file_name
+from spotdl.utils.lrc import generate_lrc
 from spotdl.utils.m3u import gen_m3u_files
 from spotdl.utils.metadata import MetadataError, embed_metadata
 from spotdl.utils.search import gather_known_songs, reinit_song, songs_from_albums
 
 __all__ = [
     "AUDIO_PROVIDERS",
     "LYRICS_PROVIDERS",
@@ -43,14 +43,15 @@
     "DownloaderError",
     "SPONSOR_BLOCK_CATEGORIES",
 ]
 
 AUDIO_PROVIDERS: Dict[str, Type[AudioProvider]] = {
     "youtube": YouTube,
     "youtube-music": YouTubeMusic,
+    "slider-kz": SliderKZ,
 }
 
 LYRICS_PROVIDERS: Dict[str, Type[LyricsProvider]] = {
     "genius": Genius,
     "musixmatch": MusixMatch,
     "azlyrics": AzLyrics,
     "synced": Synced,
@@ -174,15 +175,14 @@
 
             self.audio_providers.append(
                 audio_class(
                     output_format=self.settings["format"],
                     cookie_file=self.settings["cookie_file"],
                     search_query=self.settings["search_query"],
                     filter_results=self.settings["filter_results"],
-                    geo_bypass=self.settings["geo_bypass"],
                 )
             )
 
         # Initialize list of errors
         self.errors: List[str] = []
 
         # Initialize archive
@@ -373,186 +373,196 @@
         ### Returns
         - tuple with the song and the path to the downloaded file if successful.
 
         ### Notes
         - This function is synchronous.
         """
 
-        reinitialized = False
-        try:
-            # Create the output file path
-            output_file = create_file_name(
-                song,
-                self.settings["output"],
-                self.settings["format"],
-                self.settings["restrict"],
-            )
-        except Exception:
-            song = reinit_song(song)
-            output_file = create_file_name(
-                song,
-                self.settings["output"],
-                self.settings["format"],
-                self.settings["restrict"],
-            )
+        # Check if song has name/artist and url/song_id
+        if not (song.name and (song.artists or song.artist)) and not (
+            song.url and song.song_id
+        ):
+            logger.error("Song is missing required fields: %s", song.display_name)
+            self.errors.append(f"Song is missing required fields: {song.display_name}")
 
-            reinitialized = True
+            return song, None
 
         # Initalize the progress tracker
         display_progress_tracker = self.progress_handler.get_new_tracker(song)
 
-        # Create the temp folder path
-        temp_folder = get_temp_path()
+        try:
+            reinitialized = False
+            try:
+                # Create the output file path
+                output_file = create_file_name(
+                    song,
+                    self.settings["output"],
+                    self.settings["format"],
+                    self.settings["restrict"],
+                )
+            except Exception:
+                song = reinit_song(song)
 
-        # Check if there is an already existing song file, with the same spotify URL in its
-        # metadata, but saved under a different name. If so, save its path.
-        dup_song_paths: List[Path] = self.known_songs.get(song.url, [])
-
-        # Remove files from the list that have the same path as the output file
-        dup_song_paths = [
-            dup_song_path
-            for dup_song_path in dup_song_paths
-            if (dup_song_path.absolute() != output_file.absolute())
-            and dup_song_path.exists()
-        ]
+                output_file = create_file_name(
+                    song,
+                    self.settings["output"],
+                    self.settings["format"],
+                    self.settings["restrict"],
+                )
 
-        file_exists = output_file.exists() or dup_song_paths
-        if dup_song_paths:
-            logger.debug(
-                "Found duplicate songs for %s at %s", song.display_name, dup_song_paths
-            )
+                reinitialized = True
 
-        # If the file already exists and we don't want to overwrite it,
-        # we can skip the download
-        if file_exists and self.settings["overwrite"] == "skip":
-            logger.info(
-                "Skipping %s (file already exists) %s",
-                song.display_name,
-                "(duplicate)" if dup_song_paths else "",
-            )
+            # Create the temp folder path
+            temp_folder = get_temp_path()
 
-            display_progress_tracker.notify_download_skip()
-            return song, output_file
-
-        # Check if we have all the metadata
-        # and that the song object is not a placeholder
-        # If it's None extract the current metadata
-        # And reinitialize the song object
-        # Force song reinitialization if we are fetching albums
-        # they have most metadata but not all
-        if (
-            (song.name is None and song.url)
-            or (self.settings["fetch_albums"] and reinitialized is False)
-            or None
-            in [
-                song.genres,
-                song.disc_count,
-                song.tracks_count,
-                song.track_number,
-                song.album_id,
-                song.album_artist,
+            # Check if there is an already existing song file, with the same spotify URL in its
+            # metadata, but saved under a different name. If so, save its path.
+            dup_song_paths: List[Path] = self.known_songs.get(song.url, [])
+
+            # Remove files from the list that have the same path as the output file
+            dup_song_paths = [
+                dup_song_path
+                for dup_song_path in dup_song_paths
+                if (dup_song_path.absolute() != output_file.absolute())
+                and dup_song_path.exists()
             ]
-        ):
-            song = reinit_song(song)
-            reinitialized = True
-
-        # Don't skip if the file exists and overwrite is set to force
-        if file_exists and self.settings["overwrite"] == "force":
-            logger.info(
-                "Overwriting %s %s",
-                song.display_name,
-                " (duplicate)" if dup_song_paths else "",
-            )
 
-            # If the duplicate song path is not None, we can delete the old file
-            for dup_song_path in dup_song_paths:
-                try:
-                    logger.info("Removing duplicate file: %s", dup_song_path)
-
-                    dup_song_path.unlink()
-                except (PermissionError, OSError) as exc:
-                    logger.debug(
-                        "Could not remove duplicate file: %s, error: %s",
-                        dup_song_path,
-                        exc,
-                    )
-
-        # Find song lyrics and add them to the song object
-        lyrics = self.search_lyrics(song)
-        if lyrics is None:
-            logger.debug(
-                "No lyrics found for %s, lyrics providers: %s",
-                song.display_name,
-                ", ".join([lprovider.name for lprovider in self.lyrics_providers]),
-            )
-        else:
-            song.lyrics = lyrics
-
-        # If the file already exists and we want to overwrite the metadata,
-        # we can skip the download
-        if file_exists and self.settings["overwrite"] == "metadata":
-            most_recent_duplicate: Optional[Path] = None
+            file_exists = output_file.exists() or dup_song_paths
             if dup_song_paths:
-                # Get the most recent duplicate song path and remove the rest
-                most_recent_duplicate = max(
+                logger.debug(
+                    "Found duplicate songs for %s at %s",
+                    song.display_name,
                     dup_song_paths,
-                    key=lambda dup_song_path: dup_song_path.stat().st_mtime,
                 )
 
-                # Remove the rest of the duplicate song paths
-                for old_song_path in dup_song_paths:
-                    if most_recent_duplicate == old_song_path:
-                        continue
+            # If the file already exists and we don't want to overwrite it,
+            # we can skip the download
+            if file_exists and self.settings["overwrite"] == "skip":
+                logger.info(
+                    "Skipping %s (file already exists) %s",
+                    song.display_name,
+                    "(duplicate)" if dup_song_paths else "",
+                )
+
+                display_progress_tracker.notify_download_skip()
+                return song, output_file
+
+            # Check if we have all the metadata
+            # and that the song object is not a placeholder
+            # If it's None extract the current metadata
+            # And reinitialize the song object
+            # Force song reinitialization if we are fetching albums
+            # they have most metadata but not all
+            if (
+                (song.name is None and song.url)
+                or (self.settings["fetch_albums"] and reinitialized is False)
+                or None
+                in [
+                    song.genres,
+                    song.disc_count,
+                    song.tracks_count,
+                    song.track_number,
+                    song.album_id,
+                    song.album_artist,
+                ]
+            ):
+                song = reinit_song(song)
+                reinitialized = True
+
+            # Don't skip if the file exists and overwrite is set to force
+            if file_exists and self.settings["overwrite"] == "force":
+                logger.info(
+                    "Overwriting %s %s",
+                    song.display_name,
+                    " (duplicate)" if dup_song_paths else "",
+                )
 
+                # If the duplicate song path is not None, we can delete the old file
+                for dup_song_path in dup_song_paths:
                     try:
-                        logger.info("Removing duplicate file: %s", old_song_path)
-                        old_song_path.unlink()
+                        logger.info("Removing duplicate file: %s", dup_song_path)
+
+                        dup_song_path.unlink()
                     except (PermissionError, OSError) as exc:
                         logger.debug(
                             "Could not remove duplicate file: %s, error: %s",
-                            old_song_path,
+                            dup_song_path,
                             exc,
                         )
 
-                # Move the old file to the new location
-                if most_recent_duplicate:
-                    most_recent_duplicate.replace(
-                        output_file.with_suffix(f".{self.settings['format']}")
+            # Find song lyrics and add them to the song object
+            lyrics = self.search_lyrics(song)
+            if lyrics is None:
+                logger.debug(
+                    "No lyrics found for %s, lyrics providers: %s",
+                    song.display_name,
+                    ", ".join([lprovider.name for lprovider in self.lyrics_providers]),
+                )
+            else:
+                song.lyrics = lyrics
+
+            # If the file already exists and we want to overwrite the metadata,
+            # we can skip the download
+            if file_exists and self.settings["overwrite"] == "metadata":
+                most_recent_duplicate: Optional[Path] = None
+                if dup_song_paths:
+                    # Get the most recent duplicate song path and remove the rest
+                    most_recent_duplicate = max(
+                        dup_song_paths,
+                        key=lambda dup_song_path: dup_song_path.stat().st_mtime,
                     )
 
-            # Update the metadata
-            embed_metadata(output_file=output_file, song=song)
+                    # Remove the rest of the duplicate song paths
+                    for old_song_path in dup_song_paths:
+                        if most_recent_duplicate == old_song_path:
+                            continue
+
+                        try:
+                            logger.info("Removing duplicate file: %s", old_song_path)
+                            old_song_path.unlink()
+                        except (PermissionError, OSError) as exc:
+                            logger.debug(
+                                "Could not remove duplicate file: %s, error: %s",
+                                old_song_path,
+                                exc,
+                            )
+
+                    # Move the old file to the new location
+                    if most_recent_duplicate:
+                        most_recent_duplicate.replace(
+                            output_file.with_suffix(f".{self.settings['format']}")
+                        )
 
-            logger.info(
-                f"Updated metadata for {song.display_name}"
-                f", moved to new location: {output_file}"
-                if most_recent_duplicate
-                else ""
-            )
+                # Update the metadata
+                embed_metadata(output_file=output_file, song=song)
 
-            display_progress_tracker.notify_complete()
+                logger.info(
+                    f"Updated metadata for {song.display_name}"
+                    f", moved to new location: {output_file}"
+                    if most_recent_duplicate
+                    else ""
+                )
 
-            return song, output_file
+                display_progress_tracker.notify_complete()
 
-        # Create the output directory if it doesn't exist
-        output_file.parent.mkdir(parents=True, exist_ok=True)
+                return song, output_file
 
-        try:
+            # Create the output directory if it doesn't exist
+            output_file.parent.mkdir(parents=True, exist_ok=True)
             if song.download_url is None:
                 download_url = self.search(song)
             else:
                 download_url = song.download_url
 
             # Initialize audio downloader
             audio_downloader = AudioProvider(
                 output_format=self.settings["format"],
                 cookie_file=self.settings["cookie_file"],
                 search_query=self.settings["search_query"],
                 filter_results=self.settings["filter_results"],
-                geo_bypass=self.settings["geo_bypass"],
             )
 
             logger.debug("Downloading %s using %s", song.display_name, download_url)
 
             # Add progress hook to the audio provider
             audio_downloader.audio_handler.add_progress_hook(
                 display_progress_tracker.yt_dlp_progress_hook
@@ -576,39 +586,48 @@
 
                 raise DownloaderError(
                     f"yt-dlp failed to get metadata for: {song.name} - {song.artist}"
                 )
 
             display_progress_tracker.notify_download_complete()
 
-            # Ignore the bitrate if the bitrate is set to auto for m4a/opus
-            # or if bitrate is set to disabled
-            if self.settings["bitrate"] == "disable":
-                bitrate = None
-            elif self.settings["bitrate"] == "auto" or self.settings["bitrate"] is None:
-                # Ignore the bitrate if the input and output formats are the same
-                # and the input format is m4a/opus
-                if (temp_file.suffix == ".m4a" and output_file.suffix == ".m4a") or (
-                    temp_file.suffix == ".opus" and output_file.suffix == ".opus"
-                ):
+            # Copy the downloaded file to the output file
+            # if the temp file and output file have the same extension
+            # and the bitrate is set to auto or disable
+            if (
+                self.settings["bitrate"] in ["auto", "disable", None]
+                and temp_file.suffix == output_file.suffix
+            ):
+                temp_file.replace(output_file)
+                success = True
+                result = None
+            else:
+                if self.settings["bitrate"] in ["auto", None]:
+                    # Use the bitrate from the download info if it exists
+                    # otherwise use `copy`
+                    bitrate = (
+                        f"{int(download_info['abr'])}k"
+                        if download_info.get("abr")
+                        else "copy"
+                    )
+                elif self.settings["bitrate"] == "disable":
                     bitrate = None
                 else:
-                    bitrate = f"{int(download_info['abr'])}k"
-            else:
-                bitrate = str(self.settings["bitrate"])
+                    bitrate = str(self.settings["bitrate"])
 
-            success, result = convert(
-                input_file=temp_file,
-                output_file=output_file,
-                ffmpeg=self.ffmpeg,
-                output_format=self.settings["format"],
-                bitrate=bitrate,
-                ffmpeg_args=self.settings["ffmpeg_args"],
-                progress_handler=display_progress_tracker.ffmpeg_progress_hook,
-            )
+                # Convert the downloaded file to the output format
+                success, result = convert(
+                    input_file=temp_file,
+                    output_file=output_file,
+                    ffmpeg=self.ffmpeg,
+                    output_format=self.settings["format"],
+                    bitrate=bitrate,
+                    ffmpeg_args=self.settings["ffmpeg_args"],
+                    progress_handler=display_progress_tracker.ffmpeg_progress_hook,
+                )
 
             # Remove the temp file
             if temp_file.exists():
                 try:
                     temp_file.unlink()
                 except (PermissionError, OSError) as exc:
                     logger.debug(
@@ -690,27 +709,15 @@
                 embed_metadata(output_file, song, self.settings["id3_separator"])
             except Exception as exception:
                 raise MetadataError(
                     "Failed to embed metadata to the song"
                 ) from exception
 
             if self.settings["generate_lrc"]:
-                if song.lyrics and is_lrc_valid(song.lyrics):
-                    lrc_data = song.lyrics
-                else:
-                    try:
-                        lrc_data = syncedlyrics_search(song.display_name)
-                    except Exception:
-                        lrc_data = None
-
-                if lrc_data:
-                    save_lrc_file(str(output_file.with_suffix(".lrc")), lrc_data)
-                    logger.debug("Saved lrc file for %s", song.display_name)
-                else:
-                    logger.debug("No lrc file found for %s", song.display_name)
+                generate_lrc(song, output_file)
 
             display_progress_tracker.notify_complete()
 
             # Add the song to the known songs
             self.known_songs.get(song.url, []).append(output_file)
 
             logger.info('Downloaded "%s": %s', song.display_name, song.download_url)
```

### Comparing `spotdl-4.1.4/spotdl/download/progress_handler.py` & `spotdl-4.1.5/spotdl/download/progress_handler.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.4/spotdl/providers/audio/base.py` & `spotdl-4.1.5/spotdl/providers/audio/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,35 +66,30 @@
 
     def __init__(
         self,
         output_format: str = "mp3",
         cookie_file: Optional[str] = None,
         search_query: Optional[str] = None,
         filter_results: bool = True,
-        geo_bypass: bool = False,
     ) -> None:
         """
         Base class for audio providers.
 
         ### Arguments
         - output_directory: The directory to save the downloaded songs to.
         - output_format: The format to save the downloaded songs in.
         - cookie_file: The path to a file containing cookies to be used by YTDL.
         - search_query: The query to use when searching for songs.
         - filter_results: Whether to filter results.
-
-        ### Errors
-        - raises `NotImplementedError` if self.name is not set.
         """
 
         self.output_format = output_format
         self.cookie_file = cookie_file
         self.search_query = search_query
         self.filter_results = filter_results
-        self.geo_bypass = geo_bypass
 
         if self.output_format == "m4a":
             ytdl_format = "bestaudio[ext=m4a]/bestaudio/best"
         elif self.output_format == "opus":
             ytdl_format = "bestaudio[ext=webm]/bestaudio/best"
         else:
             ytdl_format = "bestaudio"
@@ -105,15 +100,14 @@
                 "quiet": True,
                 "no_warnings": True,
                 "encoding": "UTF-8",
                 "logger": YTDLLogger(),
                 "cookiefile": self.cookie_file,
                 "outtmpl": f"{get_temp_path()}/%(id)s.%(ext)s",
                 "retries": 5,
-                "geo_bypass": self.geo_bypass,
             }
         )
 
     def get_results(self, search_term: str, **kwargs) -> List[Result]:
         """
         Get results from audio provider.
```

### Comparing `spotdl-4.1.4/spotdl/providers/audio/youtube.py` & `spotdl-4.1.5/spotdl/providers/audio/youtube.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.4/spotdl/providers/audio/ytmusic.py` & `spotdl-4.1.5/spotdl/providers/audio/ytmusic.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 """
 YTMusic module for downloading and searching songs.
 """
 
 from typing import Any, Dict, List
 
-from requests import session
-from yt_dlp.utils import GeoUtils
 from ytmusicapi import YTMusic
 
 from spotdl.providers.audio.base import ISRC_REGEX, AudioProvider
 from spotdl.types.result import Result
 from spotdl.utils.formatter import parse_duration
 
 __all__ = ["YouTubeMusic"]
@@ -33,21 +31,15 @@
         ### Arguments
         - args: Arguments passed to the `AudioProvider` class.
         - kwargs: Keyword arguments passed to the `AudioProvider` class.
         """
 
         super().__init__(*args, **kwargs)
 
-        client_session = session()
-        if kwargs.get("geo_bypass"):
-            client_session.headers.update(
-                {"X-Forwarded-For": GeoUtils.random_ipv4("US")}  # type: ignore
-            )
-
-        self.client = YTMusic(language="de", requests_session=client_session)  # type: ignore
+        self.client = YTMusic(language="de")
 
     def get_results(self, search_term: str, **kwargs) -> List[Result]:
         """
         Get results from YouTube Music API and simplify them
 
         ### Arguments
         - search_term: The search term to search for.
```

### Comparing `spotdl-4.1.4/spotdl/providers/lyrics/azlyrics.py` & `spotdl-4.1.5/spotdl/providers/lyrics/azlyrics.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.4/spotdl/providers/lyrics/base.py` & `spotdl-4.1.5/spotdl/providers/lyrics/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -75,16 +75,20 @@
 
         ### Returns
         - The lyrics of the song or None if no lyrics were found.
         """
         try:
             results = self.get_results(name, artists, **kwargs)
         except Exception as exc:
-            logger.error(
-                "Failed to get results for %s - %s: %s", name, ", ".join(artists), exc
+            logger.debug(
+                "%s: Failed to get results for %s - %s: %s",
+                self.name,
+                name,
+                ", ".join(artists),
+                exc,
             )
             return None
 
         if not results:
             return None
 
         results_with_score = {}
@@ -101,15 +105,17 @@
         # Only return lyrics if the title match is at least 55%
         if score < 55:
             return None
 
         try:
             return self.extract_lyrics(url, **kwargs)
         except Exception as exc:
-            logger.error("Failed to extract lyrics from %s: %s", url, exc)
+            logger.debug(
+                "%s: Failed to extract lyrics from %s: %s", self.name, url, exc
+            )
             return None
 
     @property
     def name(self) -> str:
         """
         Returns the name of the lyrics provider.
         """
```

### Comparing `spotdl-4.1.4/spotdl/providers/lyrics/genius.py` & `spotdl-4.1.5/spotdl/providers/lyrics/genius.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.4/spotdl/providers/lyrics/musixmatch.py` & `spotdl-4.1.5/spotdl/providers/lyrics/musixmatch.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.4/spotdl/providers/lyrics/synced.py` & `spotdl-4.1.5/spotdl/providers/lyrics/synced.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.4/spotdl/types/album.py` & `spotdl-4.1.5/spotdl/types/album.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.4/spotdl/types/artist.py` & `spotdl-4.1.5/spotdl/types/artist.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.4/spotdl/types/options.py` & `spotdl-4.1.5/spotdl/types/options.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,14 @@
     load_config: bool
     log_level: str
     simple_tui: bool
     fetch_albums: bool
     id3_separator: str
     ytm_data: bool
     add_unavailable: bool
-    geo_bypass: bool
     generate_lrc: bool
     force_update_metadata: bool
 
 
 class WebOptions(TypedDict):
     """
     Options used for initializing the Web server.
@@ -136,15 +135,14 @@
     load_config: bool
     log_level: str
     simple_tui: bool
     fetch_albums: bool
     id3_separator: str
     ytm_data: bool
     add_unavailable: bool
-    geo_bypass: bool
     generate_lrc: bool
     force_update_metadata: bool
 
 
 class WebOptionalOptions(TypedDict, total=False):
     """
     Options used for initializing the Web server.
```

### Comparing `spotdl-4.1.4/spotdl/types/playlist.py` & `spotdl-4.1.5/spotdl/types/playlist.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.4/spotdl/types/result.py` & `spotdl-4.1.5/spotdl/types/result.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.4/spotdl/types/saved.py` & `spotdl-4.1.5/spotdl/types/saved.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.4/spotdl/types/song.py` & `spotdl-4.1.5/spotdl/types/song.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.4/spotdl/utils/archive.py` & `spotdl-4.1.5/spotdl/utils/archive.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.4/spotdl/utils/arguments.py` & `spotdl-4.1.5/spotdl/utils/arguments.py`

 * *Files 1% similar despite different names*

```diff
@@ -329,21 +329,21 @@
     # Add m3u argument
     parser.add_argument(
         "--m3u",
         type=str,
         nargs="?",
         help=(
             "Name of the m3u file to save the songs to. "
-            "Defaults to {list[0]}.m3u "
+            "Defaults to {list[0]}.m3u8 "
             "If you want to generate a m3u for each list in the query use {list}, "
             "If you want to generate a m3u file based on the first list in the query use {list[0]}"
             ", (0 is the first list in the query, 1 is the second, etc. "
             "songs don't count towards the list number) "
         ),
-        const="{list[0]}.m3u",
+        const="{list[0]}.m3u8",
     )
 
     # Add cookie file argument
     parser.add_argument(
         "--cookie-file",
         help="Path to cookies file.",
         type=str,
@@ -545,22 +545,14 @@
     parser.add_argument(
         "--simple-tui",
         action="store_const",
         const=True,
         help="Use a simple tui.",
     )
 
-    # Add geo bypass argument
-    parser.add_argument(
-        "--geo-bypass",
-        action="store_const",
-        const=True,
-        help="Bypass geo restrictions.",
-    )
-
 
 def parse_other_options(parser: _ArgumentGroup):
     """
     Parse other options from the command line.
 
     ### Arguments
     - parser: The argument parser to add the options to.
```

### Comparing `spotdl-4.1.4/spotdl/utils/config.py` & `spotdl-4.1.5/spotdl/utils/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -255,15 +255,14 @@
     "load_config": True,
     "log_level": "INFO",
     "simple_tui": False,
     "fetch_albums": False,
     "id3_separator": "/",
     "ytm_data": False,
     "add_unavailable": False,
-    "geo_bypass": False,
     "generate_lrc": False,
     "force_update_metadata": False,
 }
 
 WEB_OPTIONS: WebOptions = {
     "web_use_output_dir": False,
     "port": 8800,
```

### Comparing `spotdl-4.1.4/spotdl/utils/console.py` & `spotdl-4.1.5/spotdl/utils/console.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.4/spotdl/utils/downloader.py` & `spotdl-4.1.5/spotdl/utils/downloader.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.4/spotdl/utils/ffmpeg.py` & `spotdl-4.1.5/spotdl/utils/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.4/spotdl/utils/formatter.py` & `spotdl-4.1.5/spotdl/utils/formatter.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,15 +221,15 @@
         "{album-artist}": song.album_artist,
         "{genre}": song.genres[0] if song.genres else "",
         "{disc-number}": song.disc_number,
         "{disc-count}": song.disc_count,
         "{duration}": song.duration,
         "{year}": song.year,
         "{original-date}": song.date,
-        "{track-number}": f"{song.track_number:02d}",
+        "{track-number}": f"{song.track_number:02d}" if song.track_number else "",
         "{tracks-count}": song.tracks_count,
         "{isrc}": song.isrc,
         "{track-id}": song.song_id,
         "{publisher}": song.publisher,
         "{output-ext}": file_extension,
         "{list-name}": song.list_name,
         "{list-position}": str(song.list_position).zfill(len(str(song.list_length))),
```

### Comparing `spotdl-4.1.4/spotdl/utils/github.py` & `spotdl-4.1.5/spotdl/utils/github.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.4/spotdl/utils/logging.py` & `spotdl-4.1.5/spotdl/utils/logging.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.4/spotdl/utils/m3u.py` & `spotdl-4.1.5/spotdl/utils/m3u.py`

 * *Files 15% similar despite different names*

```diff
@@ -50,42 +50,42 @@
     file_name: Optional[str],
     template: str,
     file_extension: str,
     restrict: bool = False,
     short: bool = False,
 ):
     """
-    Create an m3u filename from the query.
+    Create an m3u8 filename from the query.
 
     ### Arguments
     - query: the query
     - file_name: the file name to use
     - song_list: the list of songs
     - template: the output file template to use
     - file_extension: the file extension to use
     - restrict: whether to sanitize the filename
     - short: whether to use the short version of the template
     """
 
     # If no file name is provided, use the first list's name
     if not file_name:
-        file_name = "{list[0]}.m3u"
+        file_name = "{list[0]}.m3u8"
 
-    # If file_name ends with a slash. Does not have a m3u name with extension
+    # If file_name ends with a slash. Does not have a m3u8 name with extension
     # at the end of the template, append `{list[0]}`` to it
     if (
         file_name.endswith("/")
         or file_name.endswith(r"\\")
         or file_name.endswith("\\\\")
     ):
-        file_name += "/{list[0]}.m3u"
+        file_name += "/{list[0]}.m3u8"
 
-    # Check if the file name ends with .m3u
-    if not file_name.endswith(".m3u"):
-        file_name += ".m3u"
+    # Check if the file name ends with .m3u or .m3u8
+    if not file_name.endswith(".m3u") or not file_name.endswith(".m3u8"):
+        file_name += ".m3u8"
 
     lists_object: Dict[str, List[Song]] = {}
     for song in songs:
         if song.list_name is None:
             continue
 
         if song.list_name not in lists_object:
```

### Comparing `spotdl-4.1.4/spotdl/utils/matching.py` & `spotdl-4.1.5/spotdl/utils/matching.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,33 +13,47 @@
     create_song_title,
     ratio,
     slugify,
 )
 from spotdl.utils.logging import MATCH
 
 __all__ = [
+    "FORBIDDEN_WORDS",
     "fill_string",
     "create_clean_string",
     "sort_string",
     "based_sort",
     "check_common_word",
+    "check_forbidden_words",
     "create_match_strings",
     "get_best_matches",
     "calc_main_artist_match",
     "calc_artists_match",
     "artists_match_fixup1",
     "artists_match_fixup2",
     "artists_match_fixup3",
     "calc_name_match",
     "calc_time_match",
     "calc_album_match",
 ]
 
 logger = logging.getLogger(__name__)
 
+FORBIDDEN_WORDS = [
+    "bassboosted",
+    "remix",
+    "remastered",
+    "remaster",
+    "reverb",
+    "bassboost",
+    "live",
+    "acoustic",
+    "8daudio",
+]
+
 
 def debug(song_id: str, result_id: str, message: str) -> None:
     """
     Log a message with MATCH level
 
     ### Arguments
     - message: message to log
@@ -174,14 +188,37 @@
     for word in sentence_words:
         if word != "" and word in to_check:
             return True
 
     return False
 
 
+def check_forbidden_words(song: Song, result: Result) -> Tuple[bool, List[str]]:
+    """
+    Check if a forbidden word is present in the result name
+
+    ### Arguments
+    - song: song to match
+    - result: result to match
+
+    ### Returns
+    - True if forbidden word is present in result name, False otherwise
+    """
+
+    song_name = slugify(song.name).replace("-", "")
+    to_check = slugify(result.name).replace("-", "")
+
+    words = []
+    for word in FORBIDDEN_WORDS:
+        if word in to_check and word not in song_name:
+            words.append(word)
+
+    return len(words) > 0, words
+
+
 def create_match_strings(
     song: Song, result: Result, search_query: Optional[str] = None
 ) -> Tuple[str, str]:
     """
     Create strings based on song and result to match
     fill strings with missing artists
 
@@ -613,15 +650,17 @@
     if not result.album:
         return 0.0
 
     return ratio(slugify(song.album_name), slugify(result.album))
 
 
 def order_results(
-    results: List[Result], song: Song, search_query: Optional[str] = None
+    results: List[Result],
+    song: Song,
+    search_query: Optional[str] = None,
 ) -> Dict[Result, float]:
     """
     Order results.
 
     ### Arguments
     - results: The results to order.
     - song: The song to order for.
@@ -691,14 +730,27 @@
             f"Artists match after fixup3: {artists_match}",
         )
 
         debug(song.song_id, result.result_id, f"Final artists match: {artists_match}")
 
         # Calculate name match
         name_match = calc_name_match(song, result, search_query)
+        debug(song.song_id, result.result_id, f"Initial name match: {name_match}")
+
+        # Check if result contains forbidden words
+        contains_fwords, found_fwords = check_forbidden_words(song, result)
+        if contains_fwords:
+            for _ in found_fwords:
+                name_match -= 15
+
+        debug(
+            song.song_id,
+            result.result_id,
+            f"Contains forbidden words: {contains_fwords}, {found_fwords}",
+        )
         debug(song.song_id, result.result_id, f"Final name match: {name_match}")
 
         # Calculate album match
         album_match = calc_album_match(song, result)
         debug(song.song_id, result.result_id, f"Final album match: {album_match}")
 
         # Calculate time match
@@ -711,15 +763,15 @@
                 song.song_id,
                 result.result_id,
                 "Skipping result due to name match lower than 50%",
             )
             continue
 
         # Ignore results with artists match lower than 70%
-        if artists_match < 70:
+        if artists_match < 70 and result.source != "slider.kz":
             debug(
                 song.song_id,
                 result.result_id,
                 "Skipping result due to artists match lower than 70%",
             )
             continue
 
@@ -749,18 +801,22 @@
             debug(
                 song.song_id,
                 result.result_id,
                 "Skipping result due to time match < 50% and average match < 75%",
             )
             continue
 
-        if not result.isrc_search and average_match <= 85 >= time_match:
+        if (
+            not result.isrc_search and average_match <= 85 >= time_match
+        ) or result.source == "slider.kz":
             # Don't add time to avg match if average match is not the best
-            # (lower than 85%)
+            # (lower than 85%), always include time match if result is from
+            # slider.kz
             average_match = (average_match + time_match) / 2
+
             debug(
                 song.song_id,
                 result.result_id,
                 f"Average match /w time match: {average_match}",
             )
 
         average_match = min(average_match, 100)
```

### Comparing `spotdl-4.1.4/spotdl/utils/metadata.py` & `spotdl-4.1.5/spotdl/utils/metadata.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,18 +15,20 @@
 from pathlib import Path
 from typing import Any, Dict, Optional
 
 import requests
 from mutagen._file import File
 from mutagen.flac import Picture
 from mutagen.id3 import ID3
-from mutagen.id3._frames import APIC, COMM, USLT, WOAS
+from mutagen.id3._frames import APIC, COMM, SYLT, USLT, WOAS
+from mutagen.id3._specs import Encoding
 from mutagen.mp4 import MP4Cover
 
 from spotdl.types.song import Song
+from spotdl.utils.formatter import to_ms
 
 __all__ = [
     "MetadataError",
     "M4A_TAG_PRESET",
     "MP3_TAG_PRESET",
     "TAG_PRESET",
     "TAG_TO_SONG",
@@ -152,15 +154,17 @@
                 f"Unrecognized file format for {output_file} from {song.url}"
             )
     except Exception as exc:
         raise MetadataError("Unable to load file.") from exc
 
     # Embed basic metadata
     audio_file[tag_preset["artist"]] = song.artists
-    audio_file[tag_preset["albumartist"]] = song.artist
+    audio_file[tag_preset["albumartist"]] = (
+        song.album_artist if song.album_artist else song.artist
+    )
     audio_file[tag_preset["title"]] = song.name
     audio_file[tag_preset["date"]] = song.date
     audio_file[tag_preset["originaldate"]] = song.date
     audio_file[tag_preset["encodedby"]] = song.publisher
 
     # Embed metadata that isn't always present
     album_name = song.album_name
@@ -285,50 +289,52 @@
 
     lyrics = song.lyrics
     if not lyrics:
         return audio_file
 
     tag_preset = TAG_PRESET if encoding != "m4a" else M4A_TAG_PRESET
 
-    if encoding == "mp3":
-        audio_file.add(USLT(encoding=3, text=song.lyrics))
-    else:
-        audio_file[tag_preset["lyrics"]] = song.lyrics
-
     # Check if the lyrics are in lrc format
     # using regex on the first 5 lines
-    # lrc_lines = lyrics.splitlines()[:5]
-    # lrc_lines = [line for line in lrc_lines if line and LRC_REGEX.match(line)]
+    lrc_lines = lyrics.splitlines()[:5]
+    lrc_lines = [line for line in lrc_lines if line and LRC_REGEX.match(line)]
 
-    # if len(lrc_lines) == 0:
-    #     # Lyrics are not in lrc format
-    #     # Embed them normally
-    #     if encoding == "mp3":
-    #         audio_file.add(USLT(encoding=3, text=song.lyrics))
-    #     else:
-    #         audio_file[tag_preset["lyrics"]] = song.lyrics
-    # else:
-    #     # Lyrics are in lrc format
-    #     # Embed them as SYLT id3 tag
-    #     if encoding == "mp3":
-    #         lrc_data = []
-    #         for line in lyrics.splitlines():
-    #             time_tag = line.split("]", 1)[0] + "]"
-    #             text = line.replace(time_tag, "")
-
-    #             time_tag = time_tag.replace("[", "")
-    #             time_tag = time_tag.replace("]", "")
-    #             time_tag = time_tag.replace(".", ":")
-    #             minute, sec, millisecond = time_tag.split(":")
-    #             time = to_ms(min=minute, sec=sec, ms=millisecond)
-    #             lrc_data.append((text, time))
-
-    #         audio_file.add(SYLT(encoding=3, text=lrc_data, format=1, type=1))
-    #     else:
-    #         audio_file[tag_preset["lyrics"]] = song.lyrics
+    if len(lrc_lines) == 0:
+        # Lyrics are not in lrc format
+        # Embed them normally
+        if encoding == "mp3":
+            audio_file.add(USLT(encoding=Encoding.UTF8, text=song.lyrics))
+        else:
+            audio_file[tag_preset["lyrics"]] = song.lyrics
+    else:
+        # Lyrics are in lrc format
+        # Embed them as SYLT id3 tag
+        if encoding == "mp3":
+            lrc_data = []
+            for line in lyrics.splitlines():
+                time_tag = line.split("]", 1)[0] + "]"
+                text = line.replace(time_tag, "")
+
+                time_tag = time_tag.replace("[", "")
+                time_tag = time_tag.replace("]", "")
+                time_tag = time_tag.replace(".", ":")
+                time_tag_vals = time_tag.split(":")
+                if len(time_tag_vals) != 3:
+                    continue
+
+                minute, sec, millisecond = time_tag_vals
+                time = to_ms(min=minute, sec=sec, ms=millisecond)
+                lrc_data.append((text, time))
+
+            audio_file.add(USLT(encoding=3, text=song.lyrics))
+            audio_file.add(
+                SYLT(encoding=Encoding.UTF8, text=lrc_data, format=2, type=1)
+            )
+        else:
+            audio_file[tag_preset["lyrics"]] = song.lyrics
 
     return audio_file
 
 
 def get_file_metadata(path: Path, id3_separator: str = "/") -> Optional[Dict[str, Any]]:
     """
     Get song metadata.
```

### Comparing `spotdl-4.1.4/spotdl/utils/search.py` & `spotdl-4.1.5/spotdl/utils/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -283,14 +283,18 @@
     ### Returns
     - Updated song object
     """
 
     data = song.json
     if data.get("url"):
         new_data = Song.from_url(data["url"]).json
+    elif data.get("song_id"):
+        new_data = Song.from_url(
+            "https://open.spotify.com/track/" + data["song_id"]
+        ).json
     elif data.get("name") and data.get("artist"):
         new_data = Song.from_search_term(data["name"]).json
     else:
         raise QueryError("Song object is missing required data to be reinitialized")
 
     for key in Song.__dataclass_fields__:  # type: ignore # pylint: disable=E1101
         val = data.get(key)
```

### Comparing `spotdl-4.1.4/spotdl/utils/spotify.py` & `spotdl-4.1.5/spotdl/utils/spotify.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.4/spotdl/utils/static.py` & `spotdl-4.1.5/spotdl/utils/static.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.4/spotdl/utils/web.py` & `spotdl-4.1.5/spotdl/utils/web.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.4/PKG-INFO` & `spotdl-4.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotdl
-Version: 4.1.4
+Version: 4.1.5
 Summary: Download your Spotify playlists and songs along with album art and metadata
 Home-page: https://github.com/spotDL/spotify-downloader/
 License: MIT
 Keywords: spotify,downloader,spotdl,music
 Author: spotDL Team
 Author-email: spotdladmins@googlegroups.com
 Maintainer: xnetcat
@@ -160,14 +160,18 @@
 
 - `save`: Saves only the metadata from Spotify without downloading anything.
     - Usage:
         `spotdl save [query] --save-file {filename}.spotdl`
 
 - `web`: Starts a web interface instead of using the command line. However, it has limited features and only supports downloading single songs.
 
+- `url`: Get direct download link for each song from the query.
+    - Usage:
+        `spotdl web [query]`
+
 - `sync`: Updates directories. Compares the directory with the current state of the playlist. Newly added songs will be downloaded and removed songs will be deleted. No other songs will be downloaded and no other files will be deleted.
 
     - Usage:
         `spotdl sync [query] --save-file {filename}.spotdl`
 
         This create a new **sync** file, to update the directory in the future, use:
```

