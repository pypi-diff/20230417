# Comparing `tmp/pytubemusic-0.0.1a4.tar.gz` & `tmp/pytubemusic-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytubemusic-0.0.1a4.tar", last modified: Thu Feb 16 08:55:59 2023, max compression
+gzip compressed data, was "pytubemusic-0.1.0.tar", last modified: Mon Apr 17 20:53:50 2023, max compression
```

## Comparing `pytubemusic-0.0.1a4.tar` & `pytubemusic-0.1.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-02-16 08:55:59.221875 pytubemusic-0.0.1a4/
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1075 2023-01-01 00:59:16.000000 pytubemusic-0.0.1a4/LICENSE
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)       25 2023-01-04 10:11:36.000000 pytubemusic-0.0.1a4/MANIFEST.in
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     4893 2023-02-16 08:55:59.221741 pytubemusic-0.0.1a4/PKG-INFO
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     3184 2023-02-16 08:48:01.000000 pytubemusic-0.0.1a4/README.md
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      756 2023-02-16 08:54:11.000000 pytubemusic-0.0.1a4/pyproject.toml
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)       42 2023-01-04 09:45:10.000000 pytubemusic-0.0.1a4/requirements.txt
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)       38 2023-02-16 08:55:59.221911 pytubemusic-0.0.1a4/setup.cfg
-drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-02-16 08:55:59.217820 pytubemusic-0.0.1a4/src/
-drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-02-16 08:55:59.220432 pytubemusic-0.0.1a4/src/pytubemusic/
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-01-01 00:52:45.000000 pytubemusic-0.0.1a4/src/pytubemusic/__init__.py
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     2631 2023-02-14 03:19:48.000000 pytubemusic-0.0.1a4/src/pytubemusic/__main__.py
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1927 2023-02-14 03:55:34.000000 pytubemusic-0.0.1a4/src/pytubemusic/audio.py
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     2155 2023-02-14 04:12:54.000000 pytubemusic-0.0.1a4/src/pytubemusic/logutils.py
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     5872 2023-02-16 08:39:11.000000 pytubemusic-0.0.1a4/src/pytubemusic/track.py
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     3749 2023-02-14 04:12:54.000000 pytubemusic-0.0.1a4/src/pytubemusic/utils.py
-drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-02-16 08:55:59.221442 pytubemusic-0.0.1a4/src/pytubemusic.egg-info/
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     4893 2023-02-16 08:55:59.000000 pytubemusic-0.0.1a4/src/pytubemusic.egg-info/PKG-INFO
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      476 2023-02-16 08:55:59.000000 pytubemusic-0.0.1a4/src/pytubemusic.egg-info/SOURCES.txt
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        1 2023-02-16 08:55:59.000000 pytubemusic-0.0.1a4/src/pytubemusic.egg-info/dependency_links.txt
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)       53 2023-02-16 08:55:59.000000 pytubemusic-0.0.1a4/src/pytubemusic.egg-info/entry_points.txt
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)       42 2023-02-16 08:55:59.000000 pytubemusic-0.0.1a4/src/pytubemusic.egg-info/requires.txt
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)       12 2023-02-16 08:55:59.000000 pytubemusic-0.0.1a4/src/pytubemusic.egg-info/top_level.txt
-drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-02-16 08:55:59.221564 pytubemusic-0.0.1a4/tests/
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1641 2023-02-14 00:54:23.000000 pytubemusic-0.0.1a4/tests/test_utils.py
+drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-04-17 20:53:50.476089 pytubemusic-0.1.0/
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1075 2023-01-01 00:59:16.000000 pytubemusic-0.1.0/LICENSE
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     4799 2023-04-17 20:53:50.475961 pytubemusic-0.1.0/PKG-INFO
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     3092 2023-04-17 20:40:33.000000 pytubemusic-0.1.0/README.md
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      754 2023-04-16 01:37:13.000000 pytubemusic-0.1.0/pyproject.toml
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      132 2023-04-17 20:36:11.000000 pytubemusic-0.1.0/requirements.txt
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)       38 2023-04-17 20:53:50.476125 pytubemusic-0.1.0/setup.cfg
+drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-04-17 20:53:50.472288 pytubemusic-0.1.0/src/
+drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-04-17 20:53:50.474476 pytubemusic-0.1.0/src/pytubemusic/
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-01-01 00:52:45.000000 pytubemusic-0.1.0/src/pytubemusic/__init__.py
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     3428 2023-04-17 20:41:20.000000 pytubemusic-0.1.0/src/pytubemusic/__main__.py
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     2005 2023-04-17 20:36:11.000000 pytubemusic-0.1.0/src/pytubemusic/audio.py
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     3185 2023-04-16 01:35:20.000000 pytubemusic-0.1.0/src/pytubemusic/logutils.py
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     6017 2023-04-17 20:32:15.000000 pytubemusic-0.1.0/src/pytubemusic/track.py
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     3625 2023-04-16 01:34:45.000000 pytubemusic-0.1.0/src/pytubemusic/utils.py
+drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-04-17 20:53:50.475430 pytubemusic-0.1.0/src/pytubemusic/validation/
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1143 2023-04-16 03:47:20.000000 pytubemusic-0.1.0/src/pytubemusic/validation/__init__.py
+drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-04-17 20:53:50.475317 pytubemusic-0.1.0/src/pytubemusic.egg-info/
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     4799 2023-04-17 20:53:50.000000 pytubemusic-0.1.0/src/pytubemusic.egg-info/PKG-INFO
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      503 2023-04-17 20:53:50.000000 pytubemusic-0.1.0/src/pytubemusic.egg-info/SOURCES.txt
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        1 2023-04-17 20:53:50.000000 pytubemusic-0.1.0/src/pytubemusic.egg-info/dependency_links.txt
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)       53 2023-04-17 20:53:50.000000 pytubemusic-0.1.0/src/pytubemusic.egg-info/entry_points.txt
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      132 2023-04-17 20:53:50.000000 pytubemusic-0.1.0/src/pytubemusic.egg-info/requires.txt
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)       12 2023-04-17 20:53:50.000000 pytubemusic-0.1.0/src/pytubemusic.egg-info/top_level.txt
+drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-04-17 20:53:50.475663 pytubemusic-0.1.0/tests/
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1641 2023-02-14 00:54:23.000000 pytubemusic-0.1.0/tests/test_utils.py
```

### Comparing `pytubemusic-0.0.1a4/LICENSE` & `pytubemusic-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytubemusic-0.0.1a4/PKG-INFO` & `pytubemusic-0.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytubemusic
-Version: 0.0.1a4
+Version: 0.1.0
 Summary: A cli that may or may not download albums from a certain website
 License: MIT License
         
         Copyright (c) 2023 James Finnie-Ansley
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -32,17 +32,14 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyTubeMusic
 
 A cli that may or may not download albums from a certain website.
 
-> PyTubeMusic is in alpha. Features are limited and significant API changes are
-> expected
-
 ## Install
 
 ```
 pip install pytubemusic
 ```
 
 **Requires [ffmpeg](https://ffmpeg.org/) to be installed on your machine.**
```

### Comparing `pytubemusic-0.0.1a4/README.md` & `pytubemusic-0.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 # PyTubeMusic
 
 A cli that may or may not download albums from a certain website.
 
-> PyTubeMusic is in alpha. Features are limited and significant API changes are
-> expected
-
 ## Install
 
 ```
 pip install pytubemusic
 ```
 
 **Requires [ffmpeg](https://ffmpeg.org/) to be installed on your machine.**
```

### Comparing `pytubemusic-0.0.1a4/pyproject.toml` & `pytubemusic-0.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pytubemusic"
-version = "0.0.1a4"
+version = "0.1.0"
 description = 'A cli that may or may not download albums from a certain website'
 
 readme = "README.md"
 requires-python = ">=3.11"
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 1 - Planning",
```

### Comparing `pytubemusic-0.0.1a4/src/pytubemusic/__main__.py` & `pytubemusic-0.1.0/src/pytubemusic/__main__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import logging
-import tomllib
 from pathlib import Path
 
+import cowexcept
 from typer import Argument, Option, Typer
 
-from .logutils import log_block, log_call
+from .logutils import log_block, log_call, open_or_panic
 from .track import Track
+from .validation import loadf_or_panic
 
 app = Typer(add_completion=False)
 
 logger = logging.getLogger("pytubemusic")
 logger.setLevel(logging.INFO)
 logger.addHandler(logging.StreamHandler())
 
@@ -17,79 +18,92 @@
 @app.command(
     "album",
     help="Gets album tracks as individual files "
          "from the video associated with the album_data file",
 )
 @log_call(
     on_enter="Building album from '{album_data}'",
-    on_exit="DONE",
+    on_exit="\x1b[32mDONE!\x1b[0m",
     on_error="\x1b[31mProcessing Album Failed.\x1b[0m",
 )
 def make_album(
         album_data: Path = Argument(..., help="The album data"),
         out: Path = Option(
             Path("."),
             "--out", "-o",
             help="The directory album tracks will be written to. "
                  "Defaults to the album name",
         )
 ):
-    with open(album_data, "rb") as f:
-        album_data = tomllib.load(f)
+    prefix = "Processing Album Failed.\n"
+    err_msg = f"{prefix}Cannot open `{album_data}`"
+    with open_or_panic(album_data, "rb", err_msg) as f:
+        err_msg = f"{prefix}Invalid Album TOML format for `{album_data}`."
+        album_data = loadf_or_panic(f, "album", err_msg)
     tracks = list(Track.from_album(**album_data))
     with log_block(on_enter="Exporting Tracks"):
         for track in tracks:
             track.export(out / track.album)
 
 
 @app.command(
     "track",
     help="Gets a single audio file from the "
          "video associated with the track_data file",
 )
 @log_call(
     on_enter="Building track from '{track_data}'",
-    on_exit="DONE",
+    on_exit="\x1b[32mDONE!\x1b[0m",
     on_error="\x1b[31mProcessing Track Failed.\x1b[0m",
 )
 def make_track(
         track_data: Path = Argument(..., help="The track data"),
         out: Path = Option(
             Path("."),
             "--out", "-o",
             help="The directory album tracks will be written to. "
                  "Defaults to the cwd",
         )
 ):
-    with open(track_data, "rb") as f:
-        track_data = tomllib.load(f)
+    prefix = "Processing Track Failed.\n"
+    err_msg = f"{prefix}Cannot open `{track_data}`"
+    with open_or_panic(track_data, "rb", err_msg) as f:
+        err_msg = f"{prefix}Invalid Track TOML format for `{track_data}`."
+        track_data = loadf_or_panic(f, "track", err_msg)
     track = Track.from_video(**track_data)
     track.export(out)
 
 
 @app.command(
     "playlist",
     help="Gets tracks from the videos associated with the playlist",
 )
 @log_call(
     on_enter="Building album from '{playlist_data}'",
-    on_exit="DONE",
+    on_exit="\x1b[32mDONE!\x1b[0m",
     on_error="\x1b[31mProcessing Playlist Failed.\x1b[0m",
 )
 def make_playlist_album(
         playlist_data: Path = Argument(..., help="The track data"),
         out: Path = Option(
             Path("."),
             "--out", "-o",
             help="The directory album tracks will be written to. "
                  "Defaults to the cwd",
         )
 ):
-    with open(playlist_data, "rb") as f:
-        playlist_data = tomllib.load(f)
+    err_msg = f"Processing Playlist Failed.\nCannot open `{playlist_data}`"
+    with open_or_panic(playlist_data, "rb", err_msg) as f:
+        err_msg = f"Processing Playlist Failed.\nInvalid Playlist TOML format."
+        playlist_data = loadf_or_panic(f, "playlist", err_msg)
     tracks = list(Track.from_playlist(**playlist_data))
     with log_block(on_enter="Exporting tracks"):
         for track in tracks:
             track.export(out / track.album)
 
 
+@app.callback(invoke_without_command=True)
+def main():
+    cowexcept.activate()
+
+
 app()
```

### Comparing `pytubemusic-0.0.1a4/src/pytubemusic/audio.py` & `pytubemusic-0.1.0/src/pytubemusic/audio.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import io
 from collections.abc import Mapping
 from datetime import timedelta
 from typing import BinaryIO, Self
 
+import backoff
 from pydub import AudioSegment
 from pytube import YouTube
 
 from pytubemusic.utils import to_microseconds
 
 __all__ = ["Audio"]
 
@@ -42,14 +43,15 @@
             format="mp3",
             tags=metadata,
             parameters=["-b:a", f"{self.bitrate}"],
             cover=cover,
         )
 
     @classmethod
+    @backoff.on_exception(backoff.expo, KeyError, max_tries=5)
     def from_url(cls, url: str) -> Self:
         """
         Downloads audio from the video associated with the URL
 
         :param url: The video URL
         :return: An Audio object
         """
```

### Comparing `pytubemusic-0.0.1a4/src/pytubemusic/track.py` & `pytubemusic-0.1.0/src/pytubemusic/track.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,20 +2,22 @@
 from collections.abc import Iterable, Mapping
 from dataclasses import dataclass
 from datetime import timedelta
 from pathlib import Path
 from tempfile import NamedTemporaryFile
 from typing import Any, Self
 
-from pytube import Playlist
+import backoff
+from pipe_utils import Pipe
+from pytube import Playlist, YouTube
+from pytube.exceptions import PytubeError
 
 from pytubemusic.audio import Audio
 from pytubemusic.logutils import log_call
-from pytubemusic.utils import (Pipe, get_cover, merge_metadata, pathify,
-                               set_ends, thumbnail, to_delta)
+from pytubemusic.utils import *
 
 __all__ = ["Track"]
 
 STR_MAP = Mapping[str, Any]
 TRACK_DATA = Iterable[STR_MAP]
 
 
@@ -82,39 +84,37 @@
         :param url: The URL of the video
         :param track_data: A list of string maps of track data
         :param metadata: A String map of FFMPEG MP3 metadata tags
         :param cover_url: The url to a JPG cover image
         :return: an iterator of Track objects
         """
         audio = Audio.from_url(url)
-        cover = thumbnail(url) if cover_url is None else get_cover(cover_url)
         track_data = (
-            Pipe(track_data)
-            .then(set_ends, audio.duration)
-            .then(merge_metadata, metadata)
-            .result
-        )
+                Pipe(track_data)
+                | (set_ends, audio.duration)
+                | (merge_metadata, metadata)
+        ).get()
         for track in track_data:
             yield cls(
                 audio,
-                cover,
-                to_delta(track.get("start")),
-                to_delta(track.get("end")),
+                thumbnail(url) if cover_url is None else get_cover(cover_url),
+                to_delta(track["start"]),
+                to_delta(track["end"]),
                 track["metadata"],
             )
 
     @classmethod
     @log_call(on_enter="Downloading '{metadata[title]}' from {url}")
     def from_video(
             cls,
             url: str,
             *,
+            metadata: Mapping[str, str],
             start: str = "00:00",
             end: str = None,
-            metadata: Mapping[str, str],
             cover_url: str = None,
     ) -> Self:
         """
         Factory that constructs a Track from a video.
 
         :param url: The URL of the video
         :param metadata: A String map of FFMPEG MP3 metadata tags
@@ -122,51 +122,57 @@
             track. Defaults to 00:00:00.00
         :param end: A H?:M:S.f? timestamp indicating the end time of the track.
             Defaults to the length of the audio
         :param cover_url: The url to a JPG cover image
         :return: A new Track
         """
         audio = Audio.from_url(url)
-        end = to_delta(end) if end is not None else audio.duration
-        if cover_url is None:
-            cover_url = thumbnail(url)
-        else:
-            cover_url = get_cover(cover_url)
-        return cls(audio, cover_url, to_delta(start), end, metadata)
+        return cls(
+            audio,
+            thumbnail(url) if cover_url is None else get_cover(cover_url),
+            to_delta(start),
+            to_delta(end) if end is not None else audio.duration,
+            metadata,
+        )
 
     @classmethod
-    @log_call(on_enter="Downloading '{metadata[album]}' from {url}")
+    @log_call(on_enter="Downloading '{metadata[album]}' from playlist {url}")
     def from_playlist(
             cls,
             url: str,
             *,
-            track_data: Iterable[Mapping[str, Any]] = None,
             metadata: Mapping[str, str],
+            track_data: Iterable[Mapping[str, Any]] = None,
             cover_url: str = None,
     ) -> Iterable[Self]:
         """
         Factory that constructs an Album from a playlist video that contains
         multiple tracks in sequence.
 
         :param url: The URL of the playlist
         :param track_data: A list of string maps of track data
         :param metadata: A String map of FFMPEG MP3 metadata tags
         :param cover_url: The url to a JPG cover image
         :return: an iterator of Track objects
         """
         playlist = Playlist(url)
-        if track_data is None:
-            track_data = [{} for _ in range(len(playlist))]
+        track_data = [{}] * len(playlist) if track_data is None else track_data
         video_data = zip(playlist.videos, track_data)
         for i, (video, data) in enumerate(video_data, start=1):
-            track_metadata = data.pop("metadata") if "metadata" in data else {}
             yield cls.from_video(
                 video.watch_url,
+                cover_url=cover_url,
                 metadata={
                     **metadata,
                     "track": i,
-                    "title": video.title,
-                    **track_metadata,
+                    # Hack to avoid issues with titles not being
+                    # found on playlist videos
+                    "title": get_title(video.watch_url),
+                    **data.get("metadata", {}),
                 },
-                cover_url=cover_url,
-                **data,
+                **{k: v for k, v in data.items() if k != "metadata"},
             )
+
+
+@backoff.on_exception(backoff.expo, PytubeError, max_tries=5)
+def get_title(url):
+    return YouTube(url).title
```

### Comparing `pytubemusic-0.0.1a4/src/pytubemusic/utils.py` & `pytubemusic-0.1.0/src/pytubemusic/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 import urllib.request
 from collections.abc import Iterable, Iterator, Mapping
 from datetime import datetime, timedelta
 from itertools import chain, pairwise
 from pathlib import PurePath
 from tempfile import NamedTemporaryFile
-from typing import Any, Self
+from typing import Any
 
 from pytube import YouTube
 
+__all__ = [
+    "to_delta", "to_timestamp", "to_microseconds", "pathify", "make_track_data",
+    "set_ends", "merge_metadata", "get_cover", "thumbnail",
+]
+
 STR_MAP = Mapping[str, Any]
 TRACK_DATA = Iterable[STR_MAP]
 
 
 def to_delta(timestamp: str) -> timedelta:
     """Converts a H?:M:S.f? timestamp string to a timedelta"""
     if "." in timestamp:
@@ -45,24 +50,14 @@
     """
     Replaces invalid characters in filenames and joins the params to a path
     with the given extension
     """
     return root / (title.replace("/", "\u2044") + ext)
 
 
-class Pipe:
-    def __init__(self, data):
-        """Allows for piped operations to the data via method chaining"""
-        self.result = data
-
-    def then(self, func, *args, **kwargs) -> Self:
-        self.result = func(self.result, *args, **kwargs)
-        return self
-
-
 def make_track_data(
         track_data: list[Mapping],
         end: timedelta,
 ) -> Iterator[Mapping]:
     """
     Adds track number metadata to a list of track data and ensures tracks have
     start and end timestamps
```

### Comparing `pytubemusic-0.0.1a4/src/pytubemusic.egg-info/PKG-INFO` & `pytubemusic-0.1.0/src/pytubemusic.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytubemusic
-Version: 0.0.1a4
+Version: 0.1.0
 Summary: A cli that may or may not download albums from a certain website
 License: MIT License
         
         Copyright (c) 2023 James Finnie-Ansley
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -32,17 +32,14 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyTubeMusic
 
 A cli that may or may not download albums from a certain website.
 
-> PyTubeMusic is in alpha. Features are limited and significant API changes are
-> expected
-
 ## Install
 
 ```
 pip install pytubemusic
 ```
 
 **Requires [ffmpeg](https://ffmpeg.org/) to be installed on your machine.**
```

### Comparing `pytubemusic-0.0.1a4/tests/test_utils.py` & `pytubemusic-0.1.0/tests/test_utils.py`

 * *Files identical despite different names*

