# Comparing `tmp/hoodat_vertex_components-1.6.2.tar.gz` & `tmp/hoodat_vertex_components-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hoodat_vertex_components-1.6.2.tar", max compression
+gzip compressed data, was "hoodat_vertex_components-1.6.4.tar", max compression
```

## Comparing `hoodat_vertex_components-1.6.2.tar` & `hoodat_vertex_components-1.6.4.tar`

### file list

```diff
@@ -1,71 +1,70 @@
--rw-r--r--   0        0        0     1069 2023-02-19 16:42:51.079350 hoodat_vertex_components-1.6.2/LICENSE.txt
--rw-r--r--   0        0        0     2368 2023-02-19 16:42:51.079350 hoodat_vertex_components-1.6.2/README.md
--rw-r--r--   0        0        0       22 2023-02-19 16:42:51.079350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/__init__.py
--rw-r--r--   0        0        0     1919 2023-02-19 16:42:51.079350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/__init__.py
--rw-r--r--   0        0        0       61 2023-02-19 16:42:51.079350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/add_py/Dockerfile
--rw-r--r--   0        0        0      295 2023-02-19 16:42:51.079350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/add_py/add.py
--rw-r--r--   0        0        0      490 2023-02-19 16:42:51.079350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/add_py/component.yaml
--rw-r--r--   0        0        0     1895 2023-02-19 16:42:51.079350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/bytetrack_from_video/Dockerfile
--rw-r--r--   0        0        0     1305 2023-02-19 16:42:51.079350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/bytetrack_from_video/Dockerfile_orig
--rw-r--r--   0        0        0     3423 2023-02-19 16:42:51.079350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/bytetrack_from_video/component.py
--rw-r--r--   0        0        0     5107 2023-02-19 16:42:51.079350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/bytetrack_from_video/component.yaml
--rw-r--r--   0        0        0   154659 2023-02-19 16:42:51.083350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/bytetrack_from_video/friends-Scene-008.mp4
--rw-r--r--   0        0        0    25708 2023-02-19 16:42:51.083350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/bytetrack_from_video/poetry.lock
--rw-r--r--   0        0        0      568 2023-02-19 16:42:51.083350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/bytetrack_from_video/pyproject.toml
--rw-r--r--   0        0        0      160 2023-02-19 16:42:51.083350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/bytetrack_from_video/requirements.txt
--rw-r--r--   0        0        0    14976 2023-02-19 16:42:51.083350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/bytetrack_from_video/tools/demo_track.py
--rw-r--r--   0        0        0     1895 2023-02-19 16:42:51.083350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/bytetrack_from_videos/Dockerfile
--rw-r--r--   0        0        0     5283 2023-02-19 16:42:51.083350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/bytetrack_from_videos/component.py
--rw-r--r--   0        0        0     6323 2023-02-19 16:42:51.083350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/bytetrack_from_videos/component.yaml
--rw-r--r--   0        0        0   154659 2023-02-19 16:42:51.083350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/bytetrack_from_videos/friends-Scene-008.mp4
--rw-r--r--   0        0        0    25708 2023-02-19 16:42:51.083350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/bytetrack_from_videos/poetry.lock
--rw-r--r--   0        0        0      568 2023-02-19 16:42:51.083350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/bytetrack_from_videos/pyproject.toml
--rw-r--r--   0        0        0      160 2023-02-19 16:42:51.083350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/bytetrack_from_videos/requirements.txt
--rw-r--r--   0        0        0    14976 2023-02-19 16:42:51.083350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/bytetrack_from_videos/tools/demo_track.py
--rw-r--r--   0        0        0       70 2023-02-19 16:42:51.083350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/haar_from_frames/Dockerfile
--rw-r--r--   0        0        0     4294 2023-02-19 16:42:51.083350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/haar_from_frames/component.py
--rw-r--r--   0        0        0     5711 2023-02-19 16:42:51.083350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/haar_from_frames/component.yaml
--rw-r--r--   0        0        0      159 2023-02-19 16:42:51.083350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/make_cascade_file/Dockerfile
--rw-r--r--   0        0        0      327 2023-02-19 16:42:51.083350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/make_cascade_file/cascades.csv
--rw-r--r--   0        0        0      798 2023-02-19 16:42:51.083350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/make_cascade_file/component.yaml
--rw-r--r--   0        0        0     1732 2023-02-19 16:42:51.083350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/make_cascade_file/make_cascade_file.py
--rw-r--r--   0        0        0    14340 2023-02-19 16:42:51.083350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/make_cascade_file/poetry.lock
--rw-r--r--   0        0        0      328 2023-02-19 16:42:51.083350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/make_cascade_file/pyproject.toml
--rw-r--r--   0        0        0      707 2023-02-19 16:42:51.083350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/make_cascade_file/tests/test_filter_cascades.py
--rw-r--r--   0        0        0      272 2023-02-19 16:42:51.083350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/pyscenedetect/Dockerfile
--rw-r--r--   0        0        0     5631 2023-02-19 16:42:51.087350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/pyscenedetect/component.py
--rw-r--r--   0        0        0     8128 2023-02-19 16:42:51.087350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/pyscenedetect/component.yaml
--rw-r--r--   0        0        0  2709671 2023-02-19 16:42:51.099350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/pyscenedetect/friends.mp4
--rw-r--r--   0        0        0     4827 2023-02-19 16:42:51.103350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/pyscenedetect/poetry.lock
--rw-r--r--   0        0        0      389 2023-02-19 16:42:51.103350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/pyscenedetect/pyproject.toml
--rw-r--r--   0        0        0      159 2023-02-19 16:42:51.103350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/query_database_output_data/Dockerfile
--rw-r--r--   0        0        0      960 2023-02-19 16:42:51.103350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/query_database_output_data/component.yaml
--rw-r--r--   0        0        0    49727 2023-02-19 16:42:51.103350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/query_database_output_data/poetry.lock
--rw-r--r--   0        0        0      383 2023-02-19 16:42:51.103350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/query_database_output_data/pyproject.toml
--rw-r--r--   0        0        0     1393 2023-02-19 16:42:51.103350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/query_database_output_data/src/query_db.py
--rw-r--r--   0        0        0      159 2023-02-19 16:42:51.103350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/query_database_output_string/Dockerfile
--rw-r--r--   0        0        0      955 2023-02-19 16:42:51.103350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/query_database_output_string/component.yaml
--rw-r--r--   0        0        0    49727 2023-02-19 16:42:51.103350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/query_database_output_string/poetry.lock
--rw-r--r--   0        0        0      383 2023-02-19 16:42:51.103350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/query_database_output_string/pyproject.toml
--rw-r--r--   0        0        0     1756 2023-02-19 16:42:51.103350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/query_database_output_string/src/query_db.py
--rw-r--r--   0        0        0      318 2023-02-19 16:42:51.103350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/stitch_videos/Dockerfile
--rw-r--r--   0        0        0      955 2023-02-19 16:42:51.103350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/stitch_videos/component.py
--rw-r--r--   0        0        0     1967 2023-02-19 16:42:51.103350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/stitch_videos/component.yaml
--rw-r--r--   0        0        0    73030 2023-02-19 16:42:51.103350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/stitch_videos/poetry.lock
--rw-r--r--   0        0        0      422 2023-02-19 16:42:51.103350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/stitch_videos/pyproject.toml
--rw-r--r--   0        0        0    78906 2023-02-19 16:42:51.103350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/stitch_videos/sample/friends-Scene-001.mp4
--rw-r--r--   0        0        0    76382 2023-02-19 16:42:51.103350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/stitch_videos/sample/friends-Scene-002.mp4
--rw-r--r--   0        0        0    92195 2023-02-19 16:42:51.103350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/stitch_videos/sample/friends-Scene-003.mp4
--rw-r--r--   0        0        0      159 2023-02-19 16:42:51.103350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/video_in_database/Dockerfile
--rw-r--r--   0        0        0     4965 2023-02-19 16:42:51.103350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/video_in_database/component.py
--rw-r--r--   0        0        0     6840 2023-02-19 16:42:51.103350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/video_in_database/component.yaml
--rw-r--r--   0        0        0    20204 2023-02-19 16:42:51.103350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/video_in_database/poetry.lock
--rw-r--r--   0        0        0      525 2023-02-19 16:42:51.103350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/video_in_database/pyproject.toml
--rw-r--r--   0        0        0      194 2023-02-19 16:42:51.103350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/video_to_frames/Dockerfile
--rw-r--r--   0        0        0     5490 2023-02-19 16:42:51.103350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/video_to_frames/component.py
--rw-r--r--   0        0        0     7578 2023-02-19 16:42:51.103350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/video_to_frames/component.yaml
--rw-r--r--   0        0        0     1285 2023-02-19 16:42:51.103350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/video_to_frames/poetry.lock
--rw-r--r--   0        0        0      308 2023-02-19 16:42:51.103350 hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/video_to_frames/pyproject.toml
--rw-r--r--   0        0        0      886 2023-02-19 16:42:51.103350 hoodat_vertex_components-1.6.2/pyproject.toml
--rw-r--r--   0        0        0     4289 1970-01-01 00:00:00.000000 hoodat_vertex_components-1.6.2/setup.py
--rw-r--r--   0        0        0     3052 1970-01-01 00:00:00.000000 hoodat_vertex_components-1.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-17 21:44:19.319421 hoodat_vertex_components-1.6.4/LICENSE.txt
+-rw-r--r--   0        0        0     2368 2023-04-17 21:44:19.319421 hoodat_vertex_components-1.6.4/README.md
+-rw-r--r--   0        0        0       22 2023-04-17 21:44:19.319421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/__init__.py
+-rw-r--r--   0        0        0     1919 2023-04-17 21:44:19.319421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/__init__.py
+-rw-r--r--   0        0        0       61 2023-04-17 21:44:19.319421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/add_py/Dockerfile
+-rw-r--r--   0        0        0      295 2023-04-17 21:44:19.319421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/add_py/add.py
+-rw-r--r--   0        0        0      490 2023-04-17 21:44:19.319421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/add_py/component.yaml
+-rw-r--r--   0        0        0     1895 2023-04-17 21:44:19.319421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/bytetrack_from_video/Dockerfile
+-rw-r--r--   0        0        0     1305 2023-04-17 21:44:19.319421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/bytetrack_from_video/Dockerfile_orig
+-rw-r--r--   0        0        0     3423 2023-04-17 21:44:19.319421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/bytetrack_from_video/component.py
+-rw-r--r--   0        0        0     5107 2023-04-17 21:44:19.319421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/bytetrack_from_video/component.yaml
+-rw-r--r--   0        0        0   154659 2023-04-17 21:44:19.319421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/bytetrack_from_video/friends-Scene-008.mp4
+-rw-r--r--   0        0        0    25708 2023-04-17 21:44:19.319421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/bytetrack_from_video/poetry.lock
+-rw-r--r--   0        0        0      568 2023-04-17 21:44:19.319421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/bytetrack_from_video/pyproject.toml
+-rw-r--r--   0        0        0      160 2023-04-17 21:44:19.319421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/bytetrack_from_video/requirements.txt
+-rw-r--r--   0        0        0    14976 2023-04-17 21:44:19.319421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/bytetrack_from_video/tools/demo_track.py
+-rw-r--r--   0        0        0     1895 2023-04-17 21:44:19.319421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/bytetrack_from_videos/Dockerfile
+-rw-r--r--   0        0        0     5505 2023-04-17 21:44:19.319421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/bytetrack_from_videos/component.py
+-rw-r--r--   0        0        0     7736 2023-04-17 21:44:19.319421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/bytetrack_from_videos/component.yaml
+-rw-r--r--   0        0        0   154659 2023-04-17 21:44:19.323421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/bytetrack_from_videos/friends-Scene-008.mp4
+-rw-r--r--   0        0        0    25708 2023-04-17 21:44:19.323421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/bytetrack_from_videos/poetry.lock
+-rw-r--r--   0        0        0      568 2023-04-17 21:44:19.323421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/bytetrack_from_videos/pyproject.toml
+-rw-r--r--   0        0        0      160 2023-04-17 21:44:19.323421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/bytetrack_from_videos/requirements.txt
+-rw-r--r--   0        0        0    14976 2023-04-17 21:44:19.323421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/bytetrack_from_videos/tools/demo_track.py
+-rw-r--r--   0        0        0       70 2023-04-17 21:44:19.323421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/haar_from_frames/Dockerfile
+-rw-r--r--   0        0        0     4294 2023-04-17 21:44:19.323421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/haar_from_frames/component.py
+-rw-r--r--   0        0        0     5711 2023-04-17 21:44:19.323421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/haar_from_frames/component.yaml
+-rw-r--r--   0        0        0      159 2023-04-17 21:44:19.323421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/make_cascade_file/Dockerfile
+-rw-r--r--   0        0        0      327 2023-04-17 21:44:19.323421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/make_cascade_file/cascades.csv
+-rw-r--r--   0        0        0      798 2023-04-17 21:44:19.323421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/make_cascade_file/component.yaml
+-rw-r--r--   0        0        0     1732 2023-04-17 21:44:19.323421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/make_cascade_file/make_cascade_file.py
+-rw-r--r--   0        0        0    14340 2023-04-17 21:44:19.323421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/make_cascade_file/poetry.lock
+-rw-r--r--   0        0        0      328 2023-04-17 21:44:19.323421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/make_cascade_file/pyproject.toml
+-rw-r--r--   0        0        0      707 2023-04-17 21:44:19.323421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/make_cascade_file/tests/test_filter_cascades.py
+-rw-r--r--   0        0        0      272 2023-04-17 21:44:19.323421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/pyscenedetect/Dockerfile
+-rw-r--r--   0        0        0     5631 2023-04-17 21:44:19.323421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/pyscenedetect/component.py
+-rw-r--r--   0        0        0     8128 2023-04-17 21:44:19.323421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/pyscenedetect/component.yaml
+-rw-r--r--   0        0        0  2709671 2023-04-17 21:44:19.339421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/pyscenedetect/friends.mp4
+-rw-r--r--   0        0        0     4827 2023-04-17 21:44:19.339421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/pyscenedetect/poetry.lock
+-rw-r--r--   0        0        0      389 2023-04-17 21:44:19.339421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/pyscenedetect/pyproject.toml
+-rw-r--r--   0        0        0      159 2023-04-17 21:44:19.339421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/query_database_output_data/Dockerfile
+-rw-r--r--   0        0        0      963 2023-04-17 21:44:19.339421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/query_database_output_data/component.yaml
+-rw-r--r--   0        0        0    49727 2023-04-17 21:44:19.339421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/query_database_output_data/poetry.lock
+-rw-r--r--   0        0        0      383 2023-04-17 21:44:19.339421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/query_database_output_data/pyproject.toml
+-rw-r--r--   0        0        0     1393 2023-04-17 21:44:19.339421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/query_database_output_data/src/query_db.py
+-rw-r--r--   0        0        0      159 2023-04-17 21:44:19.339421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/query_database_output_string/Dockerfile
+-rw-r--r--   0        0        0      955 2023-04-17 21:44:19.339421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/query_database_output_string/component.yaml
+-rw-r--r--   0        0        0    49727 2023-04-17 21:44:19.339421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/query_database_output_string/poetry.lock
+-rw-r--r--   0        0        0      383 2023-04-17 21:44:19.339421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/query_database_output_string/pyproject.toml
+-rw-r--r--   0        0        0     1756 2023-04-17 21:44:19.339421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/query_database_output_string/src/query_db.py
+-rw-r--r--   0        0        0      318 2023-04-17 21:44:19.339421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/stitch_videos/Dockerfile
+-rw-r--r--   0        0        0      955 2023-04-17 21:44:19.339421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/stitch_videos/component.py
+-rw-r--r--   0        0        0     1967 2023-04-17 21:44:19.339421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/stitch_videos/component.yaml
+-rw-r--r--   0        0        0    73030 2023-04-17 21:44:19.339421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/stitch_videos/poetry.lock
+-rw-r--r--   0        0        0      422 2023-04-17 21:44:19.339421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/stitch_videos/pyproject.toml
+-rw-r--r--   0        0        0    78906 2023-04-17 21:44:19.339421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/stitch_videos/sample/friends-Scene-001.mp4
+-rw-r--r--   0        0        0    76382 2023-04-17 21:44:19.339421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/stitch_videos/sample/friends-Scene-002.mp4
+-rw-r--r--   0        0        0    92195 2023-04-17 21:44:19.339421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/stitch_videos/sample/friends-Scene-003.mp4
+-rw-r--r--   0        0        0      159 2023-04-17 21:44:19.339421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/video_in_database/Dockerfile
+-rw-r--r--   0        0        0     4965 2023-04-17 21:44:19.339421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/video_in_database/component.py
+-rw-r--r--   0        0        0     6840 2023-04-17 21:44:19.339421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/video_in_database/component.yaml
+-rw-r--r--   0        0        0    20204 2023-04-17 21:44:19.339421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/video_in_database/poetry.lock
+-rw-r--r--   0        0        0      525 2023-04-17 21:44:19.339421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/video_in_database/pyproject.toml
+-rw-r--r--   0        0        0      194 2023-04-17 21:44:19.339421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/video_to_frames/Dockerfile
+-rw-r--r--   0        0        0     5490 2023-04-17 21:44:19.339421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/video_to_frames/component.py
+-rw-r--r--   0        0        0     7578 2023-04-17 21:44:19.339421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/video_to_frames/component.yaml
+-rw-r--r--   0        0        0     1285 2023-04-17 21:44:19.343421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/video_to_frames/poetry.lock
+-rw-r--r--   0        0        0      308 2023-04-17 21:44:19.343421 hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/video_to_frames/pyproject.toml
+-rw-r--r--   0        0        0      886 2023-04-17 21:44:19.343421 hoodat_vertex_components-1.6.4/pyproject.toml
+-rw-r--r--   0        0        0     3052 1970-01-01 00:00:00.000000 hoodat_vertex_components-1.6.4/PKG-INFO
```

### Comparing `hoodat_vertex_components-1.6.2/LICENSE.txt` & `hoodat_vertex_components-1.6.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.2/README.md` & `hoodat_vertex_components-1.6.4/README.md`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/__init__.py` & `hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/__init__.py`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/bytetrack_from_video/Dockerfile` & `hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/bytetrack_from_video/Dockerfile`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/bytetrack_from_video/Dockerfile_orig` & `hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/bytetrack_from_video/Dockerfile_orig`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/bytetrack_from_video/component.py` & `hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/bytetrack_from_video/component.py`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/bytetrack_from_video/component.yaml` & `hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/bytetrack_from_video/component.yaml`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/bytetrack_from_video/friends-Scene-008.mp4` & `hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/bytetrack_from_video/friends-Scene-008.mp4`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/bytetrack_from_video/poetry.lock` & `hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/bytetrack_from_video/poetry.lock`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/bytetrack_from_video/pyproject.toml` & `hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/bytetrack_from_video/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/bytetrack_from_video/tools/demo_track.py` & `hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/bytetrack_from_video/tools/demo_track.py`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/bytetrack_from_videos/Dockerfile` & `hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/bytetrack_from_videos/Dockerfile`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/bytetrack_from_videos/component.py` & `hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/bytetrack_from_videos/component.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,64 +10,68 @@
     input_weights: Input[Artifact],
     output_video_dir: Output[Artifact],
     output_text_file_dataset_dir: Output[Dataset],
     output_video_dir_path: str,
     output_text_file_dataset_dir_path: str,
     device: str = "gpu",  # Must be gpu or cpu
 ):
+    """
+    Run bytetrack on a directory of videos.
+
+    Args:
+        input_video_dir: Input directory of videos.
+        input_weights: Input weights file.
+        output_video_dir: Output directory of videos.
+        output_text_file_dataset_dir: Output directory of text files.
+        output_video_dir_path: Output directory of videos. Must start with /gcs.
+        output_text_file_dataset_dir_path: Output directory of text files. Must start with /gcs.
+        device: Device to use. Must be gpu or cpu.
+
+    Returns:
+        None
+    """
     import os
     import time
     from datetime import timedelta
     import pandas as pd
     import shutil
     from loguru import logger
     from tools.demo_track import make_parser, main, get_exp
 
     start_time = time.time()
 
     ################################
     # Helper functions
     ################################
 
-    def setup_output_path(output_path):
-        if output_path.startswith("gs://"):
-            output_path_gs = output_path
-            output_path_local = output_path.replace("gs://", "/gcs/")
-        elif output_path.startswith("/gcs/"):
-            output_path_gs = output_path.replace("/gcs/", "gs://")
-            output_path_local = output_path
-        else:
-            raise ValueError("output_path should start with either gs:// or /gcs/")
-        return output_path_gs, output_path_local
-
     ################################
     # Setup output paths
     ################################
 
-    output_video_dir_path_gs, output_video_dir_path_local = setup_output_path(
-        output_video_dir_path
-    )
-    os.makedirs(output_video_dir_path_local, exist_ok=True)
-    (
-        output_text_file_dataset_dir_path_gs,
-        output_text_file_dataset_dir_path_local,
-    ) = setup_output_path(output_text_file_dataset_dir_path)
-    os.makedirs(output_text_file_dataset_dir_path_local, exist_ok=True)
+    output_video_dir.path = output_video_dir_path
+    output_text_file_dataset_dir.path = output_text_file_dataset_dir_path
 
-    output_video_dir.uri = output_video_dir_path_gs
-    output_text_file_dataset_dir.uri = output_text_file_dataset_dir_path_gs
+    os.makedirs(output_video_dir.path, exist_ok=True)
+    os.makedirs(output_text_file_dataset_dir.path, exist_ok=True)
 
     # List the videos in the input directory
     file_names = os.listdir(input_video_dir.path)
     file_paths = [
         os.path.join(input_video_dir.path, file_name) for file_name in file_names
     ]
     file_names_and_paths = list(zip(file_names, file_paths))
     logger.info(f"Number of files to process: {len(file_names)}")
 
+    logger.info(
+        f"output_video_dir.path: {output_video_dir.path}, output_video_dir.uri: {output_video_dir.uri}"
+    )
+    logger.info(
+        f"output_text_file_dataset_dir.path: {output_text_file_dataset_dir.path}, output_text_file_dataset_dir.uri: {output_text_file_dataset_dir.uri}"
+    )
+
     ################################
     # Run bytetrack
     ################################
 
     video_processing_times = []
     for file_name_and_path in file_names_and_paths:
         # Log start time
@@ -94,20 +98,24 @@
         exp = get_exp(args.exp_file, args.name)
         main(exp=exp, args=args)
         # Copy outputs to GCS
         source_dir = "/ByteTrack/YOLOX_outputs/yolox_x_mix_det/track_vis"
         source_video = f"{source_dir}/output.mp4"
         source_results = f"{source_dir}/results.txt"
         output_video_path_local = os.path.join(
-            output_video_dir_path_local, file_name_and_path[0]
+            output_video_dir.path, file_name_and_path[0]
         )
+        logger.info(f"output_video_path_local: {output_video_path_local}")
         output_text_file_dataset_path_local = (
-            os.path.join(output_text_file_dataset_dir_path_local, file_name_and_path[0])
+            os.path.join(output_text_file_dataset_dir.path, file_name_and_path[0])
             + ".csv"
         )
+        logger.info(
+            f"output_text_file_dataset_path_local: {output_text_file_dataset_path_local}"
+        )
         shutil.copyfile(source_video, output_video_path_local)
         shutil.copyfile(source_results, output_text_file_dataset_path_local)
         # Log end time
         end_time_this_video = time.time()
         video_processing_time = timedelta(
             seconds=(end_time_this_video - start_time_this_video)
         )
@@ -122,20 +130,20 @@
     # Log total time
     end_time = time.time()
     total_time = timedelta(seconds=(end_time - start_time))
     total_time = total_time - timedelta(microseconds=total_time.microseconds)
     logger.info(f"Total processing time: {str(total_time)}")
 
     # output_text_file_dataset_dir.path = os.path.join(
-    #     output_text_file_dataset_dir_path_local, "data.csv"
+    #     output_text_file_dataset_dir.path, "data.csv"
     # )
 
     # # Combine all the results into a single csv file
     # file_paths = [
-    #     os.path.join(output_text_file_dataset_dir_path_local, file_name)
-    #     for file_name in os.listdir(output_text_file_dataset_dir_path_local)
+    #     os.path.join(output_text_file_dataset_dir.path, file_name)
+    #     for file_name in os.listdir(output_text_file_dataset_dir.path)
     # ]
     # dfs = [pd.read_csv(file_path, header=None) for file_path in file_paths]
     # df_shapes = [df.shape for df in dfs]
     # logger.info(f"df_shapes: {df_shapes}")
     # df = pd.concat(dfs)
     # df.to_csv(output_text_file_dataset.path, index=False)
```

### Comparing `hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/bytetrack_from_videos/friends-Scene-008.mp4` & `hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/bytetrack_from_videos/friends-Scene-008.mp4`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/bytetrack_from_videos/poetry.lock` & `hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/bytetrack_from_videos/poetry.lock`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/bytetrack_from_videos/pyproject.toml` & `hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/bytetrack_from_videos/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/bytetrack_from_videos/tools/demo_track.py` & `hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/bytetrack_from_videos/tools/demo_track.py`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/haar_from_frames/component.py` & `hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/haar_from_frames/component.py`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/haar_from_frames/component.yaml` & `hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/haar_from_frames/component.yaml`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/make_cascade_file/component.yaml` & `hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/make_cascade_file/component.yaml`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/make_cascade_file/make_cascade_file.py` & `hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/make_cascade_file/make_cascade_file.py`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/make_cascade_file/poetry.lock` & `hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/make_cascade_file/poetry.lock`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/make_cascade_file/tests/test_filter_cascades.py` & `hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/make_cascade_file/tests/test_filter_cascades.py`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/pyscenedetect/component.py` & `hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/pyscenedetect/component.py`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/pyscenedetect/component.yaml` & `hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/pyscenedetect/component.yaml`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/pyscenedetect/friends.mp4` & `hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/pyscenedetect/friends.mp4`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/pyscenedetect/poetry.lock` & `hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/pyscenedetect/poetry.lock`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/query_database_output_data/component.yaml` & `hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/query_database_output_data/component.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 description: Query the hoodat database and save the result to a file. Use this when the output is more than one cell
 
 inputs:
 - {name: secret_sql_conn, type: String, default: "projects/176634837938/secrets/hoodat_db_connection_string/versions/latest", description: "The secret that contains the connection string for the database"}
 - {name: query, type: String, default: "SELECT video_id, video_name FROM videos LIMIT 2", description: "Query to run against the database"}
 
 outputs:
-- {name: query_result, type: Data, description: "The result of the query"}
+- {name: query_result, type: Dataset, description: "The result of the query"}
 
 implementation:
   container:
     image: europe-west1-docker.pkg.dev/hoodat-sandbox/hoodat-sandbox-kfp-components/query_database_output_data
     command:
     - sh
     - -c
```

### Comparing `hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/query_database_output_data/poetry.lock` & `hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/query_database_output_data/poetry.lock`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/query_database_output_data/src/query_db.py` & `hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/query_database_output_data/src/query_db.py`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/query_database_output_string/component.yaml` & `hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/query_database_output_string/component.yaml`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/query_database_output_string/poetry.lock` & `hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/query_database_output_string/poetry.lock`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/query_database_output_string/src/query_db.py` & `hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/query_database_output_string/src/query_db.py`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/stitch_videos/component.py` & `hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/stitch_videos/component.py`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/stitch_videos/component.yaml` & `hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/stitch_videos/component.yaml`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/stitch_videos/poetry.lock` & `hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/stitch_videos/poetry.lock`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/stitch_videos/sample/friends-Scene-001.mp4` & `hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/stitch_videos/sample/friends-Scene-001.mp4`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/stitch_videos/sample/friends-Scene-002.mp4` & `hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/stitch_videos/sample/friends-Scene-002.mp4`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/stitch_videos/sample/friends-Scene-003.mp4` & `hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/stitch_videos/sample/friends-Scene-003.mp4`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/video_in_database/component.py` & `hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/video_in_database/component.py`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/video_in_database/component.yaml` & `hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/video_in_database/component.yaml`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/video_in_database/poetry.lock` & `hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/video_in_database/poetry.lock`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/video_in_database/pyproject.toml` & `hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/video_in_database/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/video_to_frames/component.py` & `hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/video_to_frames/component.py`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/video_to_frames/component.yaml` & `hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/video_to_frames/component.yaml`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.2/hoodat_vertex_components/components/video_to_frames/poetry.lock` & `hoodat_vertex_components-1.6.4/hoodat_vertex_components/components/video_to_frames/poetry.lock`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.2/pyproject.toml` & `hoodat_vertex_components-1.6.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "hoodat-vertex-components"
-version = "1.6.2"
+version = "1.6.4"
 description = "Re-usable kfp components for hoodat"
 authors = ["Eugene Brown <efbbrown@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 include = [
     "LICENSE.txt",
 ]
 
 [tool.commitizen]
-version = "1.6.2"
+version = "1.6.4"
 version_files = [
     "pyproject.toml:version",
     "hoodat_vertex_components/__init__.py:__version__",
 ]
 tag_format = "v$major.$minor.$patch$prerelease"
 
 [tool.poetry.dependencies]
```

### Comparing `hoodat_vertex_components-1.6.2/PKG-INFO` & `hoodat_vertex_components-1.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hoodat-vertex-components
-Version: 1.6.2
+Version: 1.6.4
 Summary: Re-usable kfp components for hoodat
 License: MIT
 Author: Eugene Brown
 Author-email: efbbrown@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

