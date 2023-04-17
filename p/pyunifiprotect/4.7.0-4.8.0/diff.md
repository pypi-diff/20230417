# Comparing `tmp/pyunifiprotect-4.7.0.tar.gz` & `tmp/pyunifiprotect-4.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyunifiprotect-4.7.0.tar", last modified: Tue Feb 14 20:19:40 2023, max compression
+gzip compressed data, was "pyunifiprotect-4.8.0.tar", last modified: Sun Apr 16 21:33:33 2023, max compression
```

## Comparing `pyunifiprotect-4.7.0.tar` & `pyunifiprotect-4.8.0.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 20:19:40.131606 pyunifiprotect-4.7.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 20:19:40.119606 pyunifiprotect-4.7.0/.bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      300 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/.bin/format-code
--rwxr-xr-x   0 runner    (1001) docker     (123)      381 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/.bin/install-requirements
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 20:19:40.119606 pyunifiprotect-4.7.0/.bin/lib/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/.bin/lib/common.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      618 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/.bin/lint-code
--rwxr-xr-x   0 runner    (1001) docker     (123)      503 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/.bin/test-code
--rwxr-xr-x   0 runner    (1001) docker     (123)      829 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/.bin/update-requirements
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 20:19:40.119606 pyunifiprotect-4.7.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 20:19:40.119606 pyunifiprotect-4.7.0/.docker/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/.docker/entrypoint.sh
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 20:19:40.119606 pyunifiprotect-4.7.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 20:19:40.123606 pyunifiprotect-4.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/.github/workflows/docker.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/.github/workflows/test-live-AngellusMortis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 20:19:40.123606 pyunifiprotect-4.7.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/LIVE_DATA_CI.md
--rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-02-14 20:19:40.131606 pyunifiprotect-4.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6760 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/TESTDATA.md
--rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 20:19:40.123606 pyunifiprotect-4.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/docs/api.md
--rw-r--r--   0 runner    (1001) docker     (123)    20591 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/docs/cli.md
--rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/docs/dev.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 20:19:40.123606 pyunifiprotect-4.7.0/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/docs/overrides/main.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 20:19:40.123606 pyunifiprotect-4.7.0/docs/overrides/partials/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/docs/overrides/partials/toc-item.html
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 20:19:40.123606 pyunifiprotect-4.7.0/pyunifiprotect/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/pyunifiprotect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/pyunifiprotect/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47657 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/pyunifiprotect/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 20:19:40.123606 pyunifiprotect-4.7.0/pyunifiprotect/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     8505 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/pyunifiprotect/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34254 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/pyunifiprotect/cli/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     7629 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/pyunifiprotect/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15605 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/pyunifiprotect/cli/cameras.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/pyunifiprotect/cli/chimes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/pyunifiprotect/cli/doorlocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/pyunifiprotect/cli/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/pyunifiprotect/cli/lights.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/pyunifiprotect/cli/liveviews.py
--rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/pyunifiprotect/cli/nvr.py
--rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/pyunifiprotect/cli/sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/pyunifiprotect/cli/viewers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 20:19:40.127606 pyunifiprotect-4.7.0/pyunifiprotect/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/pyunifiprotect/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34329 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/pyunifiprotect/data/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    19208 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/pyunifiprotect/data/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/pyunifiprotect/data/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    71362 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/pyunifiprotect/data/devices.py
--rw-r--r--   0 runner    (1001) docker     (123)    32619 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/pyunifiprotect/data/nvr.py
--rw-r--r--   0 runner    (1001) docker     (123)    11444 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/pyunifiprotect/data/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/pyunifiprotect/data/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/pyunifiprotect/data/websocket.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/pyunifiprotect/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/pyunifiprotect/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/pyunifiprotect/release_cache.json
--rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/pyunifiprotect/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 20:19:40.127606 pyunifiprotect-4.7.0/pyunifiprotect/test_util/
--rw-r--r--   0 runner    (1001) docker     (123)    18223 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/pyunifiprotect/test_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8251 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/pyunifiprotect/test_util/anonymize.py
--rw-r--r--   0 runner    (1001) docker     (123)    15311 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/pyunifiprotect/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6740 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/pyunifiprotect/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 20:19:40.123606 pyunifiprotect-4.7.0/pyunifiprotect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-02-14 20:19:40.000000 pyunifiprotect-4.7.0/pyunifiprotect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-02-14 20:19:40.000000 pyunifiprotect-4.7.0/pyunifiprotect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-14 20:19:40.000000 pyunifiprotect-4.7.0/pyunifiprotect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-02-14 20:19:40.000000 pyunifiprotect-4.7.0/pyunifiprotect.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-02-14 20:19:40.000000 pyunifiprotect-4.7.0/pyunifiprotect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-14 20:19:40.000000 pyunifiprotect-4.7.0/pyunifiprotect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-14 20:19:40.131606 pyunifiprotect-4.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 20:19:40.127606 pyunifiprotect-4.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21013 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 20:19:40.127606 pyunifiprotect-4.7.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29621 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/tests/data/test_camera.py
--rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/tests/data/test_chime.py
--rw-r--r--   0 runner    (1001) docker     (123)    24992 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/tests/data/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/tests/data/test_doorlock.py
--rw-r--r--   0 runner    (1001) docker     (123)     8437 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/tests/data/test_light.py
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/tests/data/test_nvr.py
--rw-r--r--   0 runner    (1001) docker     (123)    11232 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/tests/data/test_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/tests/data/test_viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 20:19:40.131606 pyunifiprotect-4.7.0/tests/sample_data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/tests/sample_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/tests/sample_data/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)   239461 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/tests/sample_data/sample_bootstrap.json
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/tests/sample_data/sample_bridge.json
--rw-r--r--   0 runner    (1001) docker     (123)    14428 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/tests/sample_data/sample_camera.json
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/tests/sample_data/sample_camera_heatmap.png
--rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/tests/sample_data/sample_camera_snapshot.png
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/tests/sample_data/sample_camera_thumbnail.png
--rw-r--r--   0 runner    (1001) docker     (123)    50760 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/tests/sample_data/sample_camera_video.mp4
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/tests/sample_data/sample_chime.json
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/tests/sample_data/sample_constants.json
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/tests/sample_data/sample_doorlock.json
--rw-r--r--   0 runner    (1001) docker     (123)     8820 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/tests/sample_data/sample_event_smart_track.json
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/tests/sample_data/sample_light.json
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/tests/sample_data/sample_liveview.json
--rw-r--r--   0 runner    (1001) docker     (123)   854579 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/tests/sample_data/sample_raw_events.json
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/tests/sample_data/sample_sensor.json
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/tests/sample_data/sample_viewport.json
--rw-r--r--   0 runner    (1001) docker     (123)   159864 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/tests/sample_data/sample_ws_messages.json
--rw-r--r--   0 runner    (1001) docker     (123)    23128 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/tests/test_api_polling.py
--rw-r--r--   0 runner    (1001) docker     (123)    16408 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/tests/test_api_ws.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-02-14 20:19:23.000000 pyunifiprotect-4.7.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:33:33.916395 pyunifiprotect-4.8.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:33:33.904394 pyunifiprotect-4.8.0/.bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      300 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/.bin/format-code
+-rwxr-xr-x   0 runner    (1001) docker     (123)      381 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/.bin/install-requirements
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:33:33.904394 pyunifiprotect-4.8.0/.bin/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/.bin/lib/common.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      618 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/.bin/lint-code
+-rwxr-xr-x   0 runner    (1001) docker     (123)      503 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/.bin/test-code
+-rwxr-xr-x   0 runner    (1001) docker     (123)      910 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/.bin/update-requirements
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:33:33.904394 pyunifiprotect-4.8.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:33:33.904394 pyunifiprotect-4.8.0/.docker/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/.docker/entrypoint.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:33:33.900395 pyunifiprotect-4.8.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:33:33.904394 pyunifiprotect-4.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/.github/workflows/docker.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/.github/workflows/test-live-AngellusMortis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:33:33.904394 pyunifiprotect-4.8.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/LIVE_DATA_CI.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-04-16 21:33:33.916395 pyunifiprotect-4.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6760 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/TESTDATA.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7764 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:33:33.908394 pyunifiprotect-4.8.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/docs/api.md
+-rw-r--r--   0 runner    (1001) docker     (123)    20591 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/docs/cli.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/docs/dev.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:33:33.908394 pyunifiprotect-4.8.0/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/docs/overrides/main.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:33:33.908394 pyunifiprotect-4.8.0/docs/overrides/partials/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/docs/overrides/partials/toc-item.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:33:33.908394 pyunifiprotect-4.8.0/pyunifiprotect/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/pyunifiprotect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/pyunifiprotect/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47822 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/pyunifiprotect/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:33:33.908394 pyunifiprotect-4.8.0/pyunifiprotect/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/pyunifiprotect/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34254 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/pyunifiprotect/cli/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7629 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/pyunifiprotect/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15605 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/pyunifiprotect/cli/cameras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/pyunifiprotect/cli/chimes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/pyunifiprotect/cli/doorlocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/pyunifiprotect/cli/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/pyunifiprotect/cli/lights.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/pyunifiprotect/cli/liveviews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/pyunifiprotect/cli/nvr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/pyunifiprotect/cli/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/pyunifiprotect/cli/viewers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:33:33.912395 pyunifiprotect-4.8.0/pyunifiprotect/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/pyunifiprotect/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/pyunifiprotect/data/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19192 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/pyunifiprotect/data/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/pyunifiprotect/data/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72373 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/pyunifiprotect/data/devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33071 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/pyunifiprotect/data/nvr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11503 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/pyunifiprotect/data/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/pyunifiprotect/data/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/pyunifiprotect/data/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/pyunifiprotect/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/pyunifiprotect/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/pyunifiprotect/release_cache.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/pyunifiprotect/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:33:33.912395 pyunifiprotect-4.8.0/pyunifiprotect/test_util/
+-rw-r--r--   0 runner    (1001) docker     (123)    18223 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/pyunifiprotect/test_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8251 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/pyunifiprotect/test_util/anonymize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15373 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/pyunifiprotect/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/pyunifiprotect/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:33:33.908394 pyunifiprotect-4.8.0/pyunifiprotect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-04-16 21:33:33.000000 pyunifiprotect-4.8.0/pyunifiprotect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-16 21:33:33.000000 pyunifiprotect-4.8.0/pyunifiprotect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 21:33:33.000000 pyunifiprotect-4.8.0/pyunifiprotect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-16 21:33:33.000000 pyunifiprotect-4.8.0/pyunifiprotect.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-16 21:33:33.000000 pyunifiprotect-4.8.0/pyunifiprotect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-16 21:33:33.000000 pyunifiprotect-4.8.0/pyunifiprotect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 21:33:33.916395 pyunifiprotect-4.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:33:33.912395 pyunifiprotect-4.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22173 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:33:33.912395 pyunifiprotect-4.8.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29621 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/tests/data/test_camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/tests/data/test_chime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24992 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/tests/data/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/tests/data/test_doorlock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8437 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/tests/data/test_light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/tests/data/test_nvr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11232 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/tests/data/test_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/tests/data/test_viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:33:33.916395 pyunifiprotect-4.8.0/tests/sample_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/tests/sample_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/tests/sample_data/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)   239461 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/tests/sample_data/sample_bootstrap.json
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/tests/sample_data/sample_bridge.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14428 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/tests/sample_data/sample_camera.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/tests/sample_data/sample_camera_heatmap.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/tests/sample_data/sample_camera_snapshot.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/tests/sample_data/sample_camera_thumbnail.png
+-rw-r--r--   0 runner    (1001) docker     (123)    50760 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/tests/sample_data/sample_camera_video.mp4
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/tests/sample_data/sample_chime.json
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/tests/sample_data/sample_constants.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/tests/sample_data/sample_doorlock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8820 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/tests/sample_data/sample_event_smart_track.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/tests/sample_data/sample_light.json
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/tests/sample_data/sample_liveview.json
+-rw-r--r--   0 runner    (1001) docker     (123)   854579 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/tests/sample_data/sample_raw_events.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/tests/sample_data/sample_sensor.json
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/tests/sample_data/sample_viewport.json
+-rw-r--r--   0 runner    (1001) docker     (123)   159864 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/tests/sample_data/sample_ws_messages.json
+-rw-r--r--   0 runner    (1001) docker     (123)    23128 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/tests/test_api_polling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16300 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/tests/test_api_ws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-16 21:33:21.000000 pyunifiprotect-4.8.0/tests/test_utils.py
```

### Comparing `pyunifiprotect-4.7.0/.bin/lib/common.sh` & `pyunifiprotect-4.8.0/.bin/lib/common.sh`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/.bin/lint-code` & `pyunifiprotect-4.8.0/.bin/lint-code`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/.devcontainer/devcontainer.json` & `pyunifiprotect-4.8.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/.github/workflows/ci.yaml` & `pyunifiprotect-4.8.0/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/.github/workflows/docker.yml` & `pyunifiprotect-4.8.0/.github/workflows/docker.yml`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/.github/workflows/docs.yml` & `pyunifiprotect-4.8.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/.github/workflows/pypi.yml` & `pyunifiprotect-4.8.0/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/.github/workflows/test-live-AngellusMortis.yml` & `pyunifiprotect-4.8.0/.github/workflows/test-live-AngellusMortis.yml`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/.gitignore` & `pyunifiprotect-4.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/.vscode/launch.json` & `pyunifiprotect-4.8.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/.vscode/tasks.json` & `pyunifiprotect-4.8.0/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/Dockerfile` & `pyunifiprotect-4.8.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/LICENSE` & `pyunifiprotect-4.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/LIVE_DATA_CI.md` & `pyunifiprotect-4.8.0/LIVE_DATA_CI.md`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/PKG-INFO` & `pyunifiprotect-4.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyunifiprotect
-Version: 4.7.0
+Version: 4.8.0
 Summary: Unofficial UniFi Protect Python API and CLI
 Author-email: Bjarne Riis <bjarne@briis.com>, Christopher Bailey <cbailey@mort.is>
 Maintainer-email: Christopher Bailey <cbailey@mort.is>, "J. Nick Koston" <nick@koston.org>
 License: MIT
 Project-URL: Source Code, https://github.com/AngellusMortis/pyunifiprotect/
 Project-URL: Documentation, https://angellusmortis.github.io/pyunifiprotect/latest/
 Project-URL: Bug Reports, https://github.com/AngellusMortis/pyunifiprotect/issues/
```

### Comparing `pyunifiprotect-4.7.0/README.md` & `pyunifiprotect-4.8.0/README.md`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/TESTDATA.md` & `pyunifiprotect-4.8.0/TESTDATA.md`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/dev-requirements.txt` & `pyunifiprotect-4.8.0/dev-requirements.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,52 @@
 #
-# This file is autogenerated by pip-compile with python 3.10
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.11
+# by the following command:
 #
-#    pip-compile --extra=dev --extra=full --output-file=dev-requirements.txt --pip-args='--root-user-action=ignore -c requirements.txt' pyproject.toml
+#    pip-compile --extra=dev --extra=full --output-file=dev-requirements.txt --pip-args='--root-user-action=ignore -c requirements.txt' --resolver=backtracking pyproject.toml
 #
 aiofiles==23.1.0
     # via pyunifiprotect (pyproject.toml)
 aiohttp==3.8.4
     # via pyunifiprotect (pyproject.toml)
-aioshutil==1.2
+aioshutil==1.3
     # via pyunifiprotect (pyproject.toml)
 aiosignal==1.3.1
     # via aiohttp
 aiosqlite==0.18.0
     # via pyunifiprotect (pyproject.toml)
-astroid==2.14.2
+astroid==2.15.2
     # via pylint
 asttokens==2.2.1
     # via stack-data
 async-timeout==4.0.2
     # via
     #   aiohttp
     #   pyunifiprotect (pyproject.toml)
 asyncify==0.9.1
     # via pyunifiprotect (pyproject.toml)
-attrs==22.2.0
-    # via
-    #   aiohttp
-    #   pytest
+attrs==23.1.0
+    # via aiohttp
 av==10.0.0
     # via pyunifiprotect (pyproject.toml)
-babel==2.11.0
+babel==2.12.1
     # via mkdocs-git-revision-date-localized-plugin
 backcall==0.2.0
     # via ipython
 base36==0.1.1
     # via pyunifiprotect (pyproject.toml)
-black==23.1.0
+black==23.3.0
     # via pyunifiprotect (pyproject.toml)
 build==0.10.0
     # via
     #   pip-tools
     #   pyunifiprotect (pyproject.toml)
 certifi==2022.12.7
     # via requests
-charset-normalizer==3.0.1
+charset-normalizer==3.1.0
     # via
     #   aiohttp
     #   requests
 click==8.1.3
     # via
     #   black
     #   mkdocs
@@ -57,26 +55,24 @@
 colorama==0.4.6
     # via
     #   griffe
     #   mkdocs-material
     #   typer
 commonmark==0.9.1
     # via rich
-coverage[toml]==7.1.0
+coverage[toml]==7.2.3
     # via
     #   pytest-cov
     #   pyunifiprotect (pyproject.toml)
-dateparser==1.1.7
+dateparser==1.1.8
     # via pyunifiprotect (pyproject.toml)
 decorator==5.1.1
     # via ipython
 dill==0.3.6
     # via pylint
-exceptiongroup==1.1.0
-    # via pytest
 execnet==1.9.0
     # via pytest-xdist
 executing==1.2.0
     # via stack-data
 flake8==6.0.0
     # via
     #   flake8-docstrings
@@ -90,27 +86,27 @@
     #   aiosignal
 funkify==0.4.4
     # via asyncify
 ghp-import==2.1.0
     # via mkdocs
 gitdb==4.0.10
     # via gitpython
-gitpython==3.1.30
+gitpython==3.1.31
     # via mkdocs-git-revision-date-localized-plugin
 greenlet==2.0.2
     # via sqlalchemy
-griffe==0.25.4
+griffe==0.27.1
     # via mkdocstrings-python
 idna==3.4
     # via
     #   requests
     #   yarl
 iniconfig==2.0.0
     # via pytest
-ipython==8.10.0
+ipython==8.12.0
     # via pyunifiprotect (pyproject.toml)
 isort==5.12.0
     # via pylint
 jedi==0.18.2
     # via ipython
 jinja2==3.1.2
     # via
@@ -146,225 +142,215 @@
     #   mike
     #   mkdocs-autorefs
     #   mkdocs-git-revision-date-localized-plugin
     #   mkdocs-material
     #   mkdocstrings
 mkdocs-autorefs==0.4.1
     # via mkdocstrings
-mkdocs-git-revision-date-localized-plugin==1.1.0
+mkdocs-git-revision-date-localized-plugin==1.2.0
     # via pyunifiprotect (pyproject.toml)
-mkdocs-include-markdown-plugin==4.0.3
+mkdocs-include-markdown-plugin==4.0.4
     # via pyunifiprotect (pyproject.toml)
-mkdocs-material==9.0.12
+mkdocs-material==9.1.6
     # via pyunifiprotect (pyproject.toml)
 mkdocs-material-extensions==1.1.1
     # via mkdocs-material
-mkdocstrings[python]==0.20.0
+mkdocstrings[python]==0.21.2
     # via
     #   mkdocstrings-python
     #   pyunifiprotect (pyproject.toml)
-mkdocstrings-python==0.8.3
+mkdocstrings-python==0.9.0
     # via mkdocstrings
 multidict==6.0.4
     # via
     #   aiohttp
     #   yarl
-mypy==1.0.0
+mypy==1.2.0
     # via
     #   pyunifiprotect (pyproject.toml)
     #   sqlalchemy
 mypy-extensions==1.0.0
     # via
     #   black
     #   mypy
-orjson==3.8.6
+orjson==3.8.10
     # via pyunifiprotect (pyproject.toml)
-packaging==23.0
+packaging==23.1
     # via
     #   black
     #   build
     #   mkdocs
     #   pytest
     #   pytest-sugar
     #   pyunifiprotect (pyproject.toml)
 parso==0.8.3
     # via jedi
-pathspec==0.11.0
+pathspec==0.11.1
     # via black
 pexpect==4.8.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
-pillow==9.4.0
+pillow==9.5.0
     # via pyunifiprotect (pyproject.toml)
-pip-tools==6.12.2
+pip-tools==6.13.0
     # via pyunifiprotect (pyproject.toml)
-platformdirs==3.0.0
+platformdirs==3.2.0
     # via
     #   black
     #   pylint
 pluggy==1.0.0
     # via pytest
-prompt-toolkit==3.0.36
+prompt-toolkit==3.0.38
     # via ipython
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
 py-cpuinfo==9.0.0
     # via pytest-benchmark
 pycodestyle==2.10.0
     # via flake8
-pydantic==1.10.4
+pydantic==1.10.7
     # via pyunifiprotect (pyproject.toml)
 pydocstyle==6.3.0
     # via
     #   flake8-docstrings
     #   pyunifiprotect (pyproject.toml)
 pyflakes==3.0.1
     # via flake8
-pygments==2.14.0
+pygments==2.15.0
     # via
     #   ipython
     #   mkdocs-material
     #   rich
 pyjwt==2.6.0
     # via pyunifiprotect (pyproject.toml)
-pylint==2.16.2
+pylint==2.17.2
     # via
     #   pylint-strict-informational
     #   pyunifiprotect (pyproject.toml)
 pylint-strict-informational==0.1
     # via pyunifiprotect (pyproject.toml)
-pymdown-extensions==9.9.2
+pymdown-extensions==9.11
     # via
     #   mkdocs-material
     #   mkdocstrings
 pyproject-flake8==6.0.0.post1
     # via pyunifiprotect (pyproject.toml)
 pyproject-hooks==1.0.0
     # via build
-pytest==7.2.1
+pytest==7.3.1
     # via
     #   pytest-asyncio
     #   pytest-benchmark
     #   pytest-cov
     #   pytest-sugar
     #   pytest-timeout
     #   pytest-xdist
     #   pyunifiprotect (pyproject.toml)
-pytest-asyncio==0.20.3
+pytest-asyncio==0.21.0
     # via pyunifiprotect (pyproject.toml)
 pytest-benchmark==4.0.0
     # via pyunifiprotect (pyproject.toml)
 pytest-cov==4.0.0
     # via pyunifiprotect (pyproject.toml)
-pytest-sugar==0.9.6
+pytest-sugar==0.9.7
     # via pyunifiprotect (pyproject.toml)
 pytest-timeout==2.1.0
     # via pyunifiprotect (pyproject.toml)
-pytest-xdist==3.2.0
+pytest-xdist==3.2.1
     # via pyunifiprotect (pyproject.toml)
 python-dateutil==2.8.2
     # via
     #   dateparser
     #   ghp-import
-python-dotenv==0.21.1
+python-dotenv==1.0.0
     # via pyunifiprotect (pyproject.toml)
-pytz==2022.7.1
+pytz==2023.3
     # via
-    #   babel
     #   dateparser
+    #   mkdocs-git-revision-date-localized-plugin
 pytz-deprecation-shim==0.1.0.post0
     # via tzlocal
 pyyaml==6.0
     # via
     #   mike
     #   mkdocs
+    #   pymdown-extensions
     #   pyyaml-env-tag
 pyyaml-env-tag==0.1
     # via mkdocs
-regex==2022.10.31
+regex==2023.3.23
     # via
     #   dateparser
     #   mkdocs-material
 requests==2.28.2
     # via mkdocs-material
 rich==12.6.0
     # via typer
-shellingham==1.5.1
+shellingham==1.5.0.post1
     # via typer
 six==1.16.0
     # via
     #   asttokens
     #   python-dateutil
 smmap==5.0.0
     # via gitdb
 snowballstemmer==2.2.0
     # via pydocstyle
-sqlalchemy[asyncio,mypy]==2.0.3
+sqlalchemy[asyncio,mypy]==2.0.9
     # via pyunifiprotect (pyproject.toml)
 stack-data==0.6.2
     # via ipython
 termcolor==2.2.0
     # via
     #   pytest-sugar
     #   pyunifiprotect (pyproject.toml)
-tomli==2.0.1
-    # via
-    #   black
-    #   build
-    #   coverage
-    #   mypy
-    #   pylint
-    #   pyproject-flake8
-    #   pyproject-hooks
-    #   pytest
-tomlkit==0.11.6
+tomlkit==0.11.7
     # via pylint
 traitlets==5.9.0
     # via
     #   ipython
     #   matplotlib-inline
 typer[all]==0.7.0
     # via pyunifiprotect (pyproject.toml)
-types-aiofiles==22.1.0.7
+types-aiofiles==23.1.0.1
     # via pyunifiprotect (pyproject.toml)
-types-dateparser==1.1.4.6
+types-dateparser==1.1.4.9
     # via pyunifiprotect (pyproject.toml)
-types-pillow==9.4.0.11
+types-pillow==9.5.0.0
     # via pyunifiprotect (pyproject.toml)
-types-termcolor==1.1.6
+types-termcolor==1.1.6.2
     # via pyunifiprotect (pyproject.toml)
-typing-extensions==4.4.0
+typing-extensions==4.5.0
     # via
-    #   astroid
     #   mypy
     #   pydantic
     #   sqlalchemy
     #   xtyping
-tzdata==2022.7
+tzdata==2023.3
     # via
     #   pytz-deprecation-shim
     #   pyunifiprotect (pyproject.toml)
-tzlocal==4.2
+tzlocal==4.3
     # via dateparser
-urllib3==1.26.14
+urllib3==1.26.15
     # via requests
 verspec==0.1.0
     # via mike
-watchdog==2.2.1
+watchdog==3.0.0
     # via mkdocs
 wcwidth==0.2.6
     # via prompt-toolkit
-wheel==0.38.4
+wheel==0.40.0
     # via pip-tools
-wrapt==1.14.1
+wrapt==1.15.0
     # via astroid
-xtyping==0.6.1
+xtyping==0.6.2
     # via asyncify
 yarl==1.8.2
     # via aiohttp
 
 # The following packages are considered to be unsafe in a requirements file:
 # pip
 # setuptools
```

### Comparing `pyunifiprotect-4.7.0/docs/api.md` & `pyunifiprotect-4.8.0/docs/api.md`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/docs/cli.md` & `pyunifiprotect-4.8.0/docs/cli.md`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/docs/dev.md` & `pyunifiprotect-4.8.0/docs/dev.md`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/mkdocs.yml` & `pyunifiprotect-4.8.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/pyproject.toml` & `pyunifiprotect-4.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 [build-system]
 requires = [
-  "setuptools >= 61.0.0", "setuptools_scm[toml]>=6.2",
+  "setuptools>=61.0.0",
+  "setuptools_scm[toml]>=6.2",
   "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyunifiprotect"
 description = "Unofficial UniFi Protect Python API and CLI"
```

### Comparing `pyunifiprotect-4.7.0/pyunifiprotect/api.py` & `pyunifiprotect-4.8.0/pyunifiprotect/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import asyncio
 from datetime import datetime, timedelta
 from http.cookies import Morsel
 from ipaddress import IPv4Address
 import logging
 from pathlib import Path
+from tempfile import gettempdir
 import time
 from typing import Any, Callable, Dict, List, Optional, Set, Type, Union, cast
 from urllib.parse import urljoin
 from uuid import UUID
 
 import aiofiles
 import aiohttp
@@ -500,14 +501,15 @@
     _subscribed_models: Set[ModelType]
     _ignore_stats: bool
     _ws_subscriptions: List[Callable[[WSSubscriptionMessage], None]]
     _bootstrap: Optional[Bootstrap] = None
     _last_update_dt: Optional[datetime] = None
     _connection_host: Optional[Union[IPv4Address, str]] = None
 
+    cache_dir: Path
     ignore_unadopted: bool
 
     def __init__(
         self,
         host: str,
         port: int,
         username: str,
@@ -516,14 +518,15 @@
         session: Optional[aiohttp.ClientSession] = None,
         override_connection_host: bool = False,
         minimum_score: int = 0,
         subscribed_models: Optional[Set[ModelType]] = None,
         ignore_stats: bool = False,
         ignore_unadopted: bool = True,
         debug: bool = False,
+        cache_dir: Optional[Path] = None,
     ) -> None:
         super().__init__(
             host=host,
             port=port,
             username=username,
             password=password,
             verify_ssl=verify_ssl,
@@ -531,14 +534,15 @@
         )
 
         self._minimum_score = minimum_score
         self._subscribed_models = subscribed_models or set()
         self._ignore_stats = ignore_stats
         self._ws_subscriptions = []
         self.ignore_unadopted = ignore_unadopted
+        self.cache_dir = cache_dir or Path(gettempdir()) / "ufp_cache"
 
         if override_connection_host:
             self._connection_host = ip_from_host(self._host)
 
         if debug:
             set_debug()
```

### Comparing `pyunifiprotect-4.7.0/pyunifiprotect/cli/__init__.py` & `pyunifiprotect-4.8.0/pyunifiprotect/cli/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,19 @@
 from pyunifiprotect.cli.lights import app as light_app
 from pyunifiprotect.cli.liveviews import app as liveview_app
 from pyunifiprotect.cli.nvr import app as nvr_app
 from pyunifiprotect.cli.sensors import app as sensor_app
 from pyunifiprotect.cli.viewers import app as viewer_app
 from pyunifiprotect.data import Version, WSPacket
 from pyunifiprotect.test_util import SampleDataGenerator
-from pyunifiprotect.utils import get_local_timezone, profile_ws as profile_ws_job
+from pyunifiprotect.utils import (
+    RELEASE_CACHE,
+    get_local_timezone,
+    profile_ws as profile_ws_job,
+)
 
 _LOGGER = logging.getLogger("pyunifiprotect")
 
 try:
     from IPython import embed
     from termcolor import colored
     from traitlets.config import get_config
@@ -255,11 +259,11 @@
 
     _setup_logger()
 
     loop = asyncio.get_event_loop()
     versions = loop.run_until_complete(callback())
     output = orjson.dumps(sorted([str(v) for v in versions]))
 
-    with open(Path(__file__).parent.parent / "release_cache.json", "wb") as cache_file:
+    with open(RELEASE_CACHE, "wb") as cache_file:
         cache_file.write(output)
 
     typer.echo(output.decode("utf-8"))
```

### Comparing `pyunifiprotect-4.7.0/pyunifiprotect/cli/backup.py` & `pyunifiprotect-4.8.0/pyunifiprotect/cli/backup.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/pyunifiprotect/cli/base.py` & `pyunifiprotect-4.8.0/pyunifiprotect/cli/base.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/pyunifiprotect/cli/cameras.py` & `pyunifiprotect-4.8.0/pyunifiprotect/cli/cameras.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/pyunifiprotect/cli/chimes.py` & `pyunifiprotect-4.8.0/pyunifiprotect/cli/chimes.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/pyunifiprotect/cli/doorlocks.py` & `pyunifiprotect-4.8.0/pyunifiprotect/cli/doorlocks.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/pyunifiprotect/cli/events.py` & `pyunifiprotect-4.8.0/pyunifiprotect/cli/events.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/pyunifiprotect/cli/lights.py` & `pyunifiprotect-4.8.0/pyunifiprotect/cli/lights.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/pyunifiprotect/cli/liveviews.py` & `pyunifiprotect-4.8.0/pyunifiprotect/cli/liveviews.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/pyunifiprotect/cli/nvr.py` & `pyunifiprotect-4.8.0/pyunifiprotect/cli/nvr.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/pyunifiprotect/cli/sensors.py` & `pyunifiprotect-4.8.0/pyunifiprotect/cli/sensors.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/pyunifiprotect/cli/viewers.py` & `pyunifiprotect-4.8.0/pyunifiprotect/cli/viewers.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/pyunifiprotect/data/__init__.py` & `pyunifiprotect-4.8.0/pyunifiprotect/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/pyunifiprotect/data/base.py` & `pyunifiprotect-4.8.0/pyunifiprotect/data/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     is_debug,
     process_datetime,
     serialize_unifi_obj,
     to_snake_case,
 )
 
 if TYPE_CHECKING:
+    from asyncio.events import TimerHandle
     from typing import Self  # requires Python 3.11+
 
     from pydantic.typing import DictStrAny, SetStr
 
     from pyunifiprotect.api import ProtectApiClient
     from pyunifiprotect.data.devices import Bridge
     from pyunifiprotect.data.nvr import Event
@@ -721,14 +722,16 @@
     uptime: Optional[timedelta]
     last_seen: Optional[datetime]
     hardware_revision: Optional[str]
     firmware_version: Optional[str]
     is_updating: bool
     is_ssh_enabled: bool
 
+    _callback_ping: Optional[TimerHandle] = None
+
     @classmethod
     def _get_read_only_fields(cls) -> Set[str]:
         return super()._get_read_only_fields() | {
             "mac",
             "host",
             "type",
             "upSince",
@@ -752,15 +755,17 @@
             data["hardwareRevision"] = str(data["hardwareRevision"])
 
         return super().unifi_dict_to_dict(data)
 
     def _event_callback_ping(self) -> None:
         _LOGGER.debug("Event ping timer started for %s", self.id)
         loop = asyncio.get_event_loop()
-        loop.call_later(EVENT_PING_INTERVAL.total_seconds(), asyncio.create_task, self.emit_message({}))
+        self._callback_ping = loop.call_later(
+            EVENT_PING_INTERVAL.total_seconds(), asyncio.create_task, self.emit_message({})
+        )
 
     async def set_name(self, name: str | None) -> None:
         """Sets name for the device"""
 
         def callback() -> None:
             self.name = name
 
@@ -808,14 +813,16 @@
     can_adopt: bool
     is_attempting_to_connect: bool
     is_connected: bool
     # requires 1.21+
     market_name: Optional[str]
     # requires 2.7.5+
     fw_update_state: Optional[str] = None
+    # requires 2.8.14+
+    nvr_mac: Optional[str] = None
 
     wired_connection_state: Optional[WiredConnectionState] = None
     wifi_connection_state: Optional[WifiConnectionState] = None
     bluetooth_connection_state: Optional[BluetoothConnectionState] = None
     bridge_id: Optional[str]
     is_downloading_firmware: Optional[bool]
```

### Comparing `pyunifiprotect-4.7.0/pyunifiprotect/data/bootstrap.py` & `pyunifiprotect-4.8.0/pyunifiprotect/data/bootstrap.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 from __future__ import annotations
 
 import asyncio
 from copy import deepcopy
 from dataclasses import dataclass
 from datetime import datetime
 import logging
-from pathlib import Path
-from tempfile import gettempdir
 from typing import Any, Dict, List, Optional, Set, Tuple, cast
 from uuid import UUID
 
 from aiohttp.client_exceptions import ServerDisconnectedError
 from pydantic import PrivateAttr, ValidationError
 
 from pyunifiprotect.data.base import (
@@ -63,17 +61,14 @@
 CAMERA_EVENT_ATTR_MAP: Dict[EventType, Tuple[str, str]] = {
     EventType.MOTION: ("last_motion", "last_motion_event_id"),
     EventType.SMART_DETECT: ("last_smart_detect", "last_smart_detect_event_id"),
     EventType.SMART_AUDIO_DETECT: ("last_smart_audio_detect", "last_smart_audio_detect_event_id"),
     EventType.RING: ("last_ring", "last_ring_event_id"),
 }
 
-TMP_RELEASE_CACHE = Path(gettempdir()) / "ufp_cache" / "release_cache.json"
-RELEASE_CACHE = Path(__file__).parent.parent / "release_cache.json"
-
 
 def _remove_stats_keys(data: Dict[str, Any], ignore_stats: bool) -> Dict[str, Any]:
     if ignore_stats:
         for key in STATS_KEYS.intersection(data.keys()):
             del data[key]
     return data
 
@@ -162,14 +157,15 @@
     mac_lookup: dict[str, ProtectDeviceRef] = {}
     id_lookup: dict[str, ProtectDeviceRef] = {}
     _ws_stats: List[WSStat] = PrivateAttr([])
     _has_doorbell: Optional[bool] = PrivateAttr(None)
     _has_smart: Optional[bool] = PrivateAttr(None)
     _has_media: Optional[bool] = PrivateAttr(None)
     _recording_start: Optional[datetime] = PrivateAttr(None)
+    _refresh_tasks: Set[asyncio.Task[None]] = PrivateAttr(set())
 
     @classmethod
     def unifi_dict_to_dict(cls, data: Dict[str, Any]) -> Dict[str, Any]:
         api = cls._get_api(data.get("api"))
         data["macLookup"] = {}
         data["idLookup"] = {}
         for model_type in ModelType.bootstrap_models():
@@ -484,15 +480,17 @@
         msg = ""
         if action["modelKey"] == "event":
             msg = f"Validation error processing event: {action['id']}. Ignoring event."
         else:
             try:
                 model_type = ModelType(action["modelKey"])
                 device_id = action["id"]
-                asyncio.create_task(self.refresh_device(model_type, device_id))
+                task = asyncio.create_task(self.refresh_device(model_type, device_id))
+                self._refresh_tasks.add(task)
+                task.add_done_callback(self._refresh_tasks.discard)
             except (ValueError, IndexError):
                 msg = f"{action['action']} packet caused invalid state. Unable to refresh device."
             else:
                 msg = f"{action['action']} packet caused invalid state. Refreshing device: {model_type} {device_id}"
         _LOGGER.debug("%s Error: %s", msg, err)
 
     async def refresh_device(self, model_type: ModelType, device_id: str) -> None:
```

### Comparing `pyunifiprotect-4.7.0/pyunifiprotect/data/convert.py` & `pyunifiprotect-4.8.0/pyunifiprotect/data/convert.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/pyunifiprotect/data/devices.py` & `pyunifiprotect-4.8.0/pyunifiprotect/data/devices.py`

 * *Files 0% similar despite different names*

```diff
@@ -312,14 +312,16 @@
     d_zoom_stream_id: int
     focus_mode: Optional[FocusMode] = None
     focus_position: int
     touch_focus_x: Optional[int]
     touch_focus_y: Optional[int]
     zoom_position: PercentInt
     mount_position: Optional[MountPosition] = None
+    # requires 2.8.14+
+    is_color_night_vision_enabled: Optional[bool] = None
 
     def unifi_dict(self, data: Optional[Dict[str, Any]] = None, exclude: Optional[Set[str]] = None) -> Dict[str, Any]:
         data = super().unifi_dict(data=data, exclude=exclude)
 
         if "focusMode" in data and data["focusMode"] is None:
             del data["focusMode"]
 
@@ -624,17 +626,29 @@
 
 
 class PrivacyMaskCapability(ProtectBaseObject):
     max_masks: Optional[int]
     rectangle_only: bool
 
 
+class HotplugExtender(ProtectBaseObject):
+    has_flash: Optional[bool] = None
+    has_ir: Optional[bool] = None
+    has_radar: Optional[bool] = None
+    is_attached: Optional[bool] = None
+
+    @classmethod
+    def _get_unifi_remaps(cls) -> Dict[str, str]:
+        return {**super()._get_unifi_remaps(), "hasIR": "hasIr"}
+
+
 class Hotplug(ProtectBaseObject):
     audio: Optional[bool] = None
     video: Optional[bool] = None
+    extender: Optional[HotplugExtender] = None
 
 
 class CameraFeatureFlags(ProtectBaseObject):
     can_adjust_ir_led_level: bool
     can_magic_zoom: bool
     can_optical_zoom: bool
     can_touch_focus: bool
@@ -771,14 +785,18 @@
     # requires 2.6.13+
     homekit_settings: Optional[CameraHomekitSettings] = None
     # requires 2.6.17+
     ap_mgmt_ip: Optional[IPv4Address] = None
     # requires 2.7.5+
     is_waterproof_case_attached: Optional[bool] = None
     last_disconnect: Optional[datetime] = None
+    # requires 2.8.14+
+    is_2k: Optional[bool] = None
+    is_4k: Optional[bool] = None
+    use_global: Optional[bool] = None
 
     # TODO: used for adopting
     # apMac read only
     # apRssi read only
     # elementInfo read only
 
     # TODO:
@@ -794,14 +812,18 @@
     last_smart_audio_detect: Optional[datetime] = None
     last_smart_detect_event_id: Optional[str] = None
     last_smart_audio_detect_event_id: Optional[str] = None
     talkback_stream: Optional[TalkbackStream] = None
     _last_ring_timeout: Optional[datetime] = PrivateAttr(None)
 
     @classmethod
+    def _get_unifi_remaps(cls) -> Dict[str, str]:
+        return {**super()._get_unifi_remaps(), "is2K": "is2k", "is4K": "is4k"}
+
+    @classmethod
     def _get_excluded_changed_fields(cls) -> Set[str]:
         return super()._get_excluded_changed_fields() | {
             "last_ring_event_id",
             "last_smart_detect",
             "last_smart_audio_detect",
             "last_smart_detect_event_id",
             "last_smart_audio_detect_event_id",
@@ -1060,27 +1082,27 @@
 
     @property
     def is_digital_chime(self) -> bool:
         return self.chime_type is ChimeType.DIGITAL
 
     @property
     def high_camera_channel(self) -> Optional[CameraChannel]:
-        if len(self.channels) == 3:
+        if len(self.channels) >= 3:
             return self.channels[0]
         return None
 
     @property
     def medium_camera_channel(self) -> Optional[CameraChannel]:
-        if len(self.channels) == 3:
+        if len(self.channels) >= 3:
             return self.channels[1]
         return None
 
     @property
     def low_camera_channel(self) -> Optional[CameraChannel]:
-        if len(self.channels) == 3:
+        if len(self.channels) >= 3:
             return self.channels[2]
         return None
 
     @property
     def default_camera_channel(self) -> Optional[CameraChannel]:
         for channel in [self.high_camera_channel, self.medium_camera_channel, self.low_camera_channel]:
             if channel is not None and channel.is_rtsp_enabled:
@@ -1146,14 +1168,17 @@
 
         Datetime of screenshot is approximate. It may be +/- a few seconds.
         """
 
         if not self.api.bootstrap.auth_user.can(ModelType.CAMERA, PermissionNode.READ_MEDIA, self):
             raise NotAuthorized(f"Do not have permission to read media for camera: {self.id}")
 
+        if height is None and width is None and self.high_camera_channel is not None:
+            height = self.high_camera_channel.height
+
         return await self.api.get_camera_snapshot(self.id, width, height, dt=dt)
 
     async def get_package_snapshot(
         self,
         width: Optional[int] = None,
         height: Optional[int] = None,
         dt: Optional[datetime] = None,
@@ -1166,14 +1191,17 @@
 
         if not self.feature_flags.has_package_camera:
             raise BadRequest("Device does not have package camera")
 
         if not self.api.bootstrap.auth_user.can(ModelType.CAMERA, PermissionNode.READ_MEDIA, self):
             raise NotAuthorized(f"Do not have permission to read media for camera: {self.id}")
 
+        if height is None and width is None and self.package_camera_channel is not None:
+            height = self.package_camera_channel.height
+
         return await self.api.get_package_camera_snapshot(self.id, width, height, dt=dt)
 
     async def get_video(
         self,
         start: datetime,
         end: datetime,
         channel_index: int = 0,
```

### Comparing `pyunifiprotect-4.7.0/pyunifiprotect/data/nvr.py` & `pyunifiprotect-4.8.0/pyunifiprotect/data/nvr.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """UniFi Protect Data."""
 from __future__ import annotations
 
 from datetime import datetime, timedelta, tzinfo
 from ipaddress import IPv4Address
 import logging
 from pathlib import Path
-from tempfile import gettempdir
 from typing import (
     TYPE_CHECKING,
     Any,
     ClassVar,
     Dict,
     List,
     Literal,
@@ -51,24 +50,22 @@
     SensorType,
     SmartDetectObjectType,
     StorageType,
     Version,
 )
 from pyunifiprotect.data.user import User, UserLocation
 from pyunifiprotect.exceptions import BadRequest, NotAuthorized
-from pyunifiprotect.utils import process_datetime
+from pyunifiprotect.utils import RELEASE_CACHE, process_datetime
 
 if TYPE_CHECKING:
     from pydantic.typing import SetStr
 
 _LOGGER = logging.getLogger(__name__)
 MAX_SUPPORTED_CAMERAS = 256
 MAX_EVENT_HISTORY_IN_STATE_MACHINE = MAX_SUPPORTED_CAMERAS * 2
-TMP_RELEASE_CACHE = Path(gettempdir()) / "ufp_cache" / "release_cache.json"
-RELEASE_CACHE = Path(__file__).parent.parent / "release_cache.json"
 
 
 class NVRLocation(UserLocation):
     is_geofencing_enabled: bool
     radius: int
     model: Optional[ModelType] = None
 
@@ -210,14 +207,15 @@
     metadata: Optional[EventMetadata]
     # requires 2.7.5+
     deleted_at: Optional[datetime] = None
     deletion_type: Optional[Literal["manual", "automatic"]] = None
 
     # TODO:
     # partition
+    # description
 
     _smart_detect_events: Optional[List[Event]] = PrivateAttr(None)
     _smart_detect_track: Optional[SmartDetectTrack] = PrivateAttr(None)
     _smart_detect_zones: Optional[Dict[int, CameraZone]] = PrivateAttr(None)
 
     @classmethod
     def _get_unifi_remaps(cls) -> Dict[str, str]:
@@ -433,14 +431,16 @@
 class StorageInfo(ProtectBaseObject):
     available: int
     is_recycling: bool
     size: int
     type: StorageType
     used: int
     devices: List[StorageDevice]
+    # requires 2.8.14+
+    capability: Optional[str] = None
 
     @classmethod
     def unifi_dict_to_dict(cls, data: Dict[str, Any]) -> Dict[str, Any]:
         if "type" in data:
             storage_type = data.pop("type")
             try:
                 data["type"] = StorageType(storage_type)
@@ -473,15 +473,15 @@
     serial: Optional[str] = None
     firmware: Optional[str] = None
     rpm: Optional[int] = None
     ata: Optional[str] = None
     sata: Optional[str] = None
     action: Optional[str] = None
     healthy: Optional[str] = None
-    reason: Optional[Any] = None
+    reason: Optional[List[Any]] = None
     temperature: Optional[int] = None
     power_on_hours: Optional[int] = None
     life_span: Optional[PercentFloat] = None
     bad_sector: Optional[int] = None
     threshold: Optional[int] = None
     progress: Optional[PercentFloat] = None
     estimate: Optional[timedelta] = None
@@ -501,15 +501,15 @@
             data["estimate"] = timedelta(seconds=data.pop("estimate"))
 
         return super().unifi_dict_to_dict(data)
 
     def unifi_dict(self, data: Optional[Dict[str, Any]] = None, exclude: Optional[Set[str]] = None) -> Dict[str, Any]:
         data = super().unifi_dict(data=data, exclude=exclude)
 
-        # esimtate is actually in seconds, not milliseconds
+        # estimate is actually in seconds, not milliseconds
         if "estimate" in data and data["estimate"] is not None:
             data["estimate"] = data["estimate"] / 1000
 
         if "state" in data and data["state"] == "nodisk":
             delete_keys = [
                 "action",
                 "ata",
@@ -553,14 +553,16 @@
 class UOSSpace(ProtectBaseObject):
     device: str
     total_bytes: int
     used_bytes: int
     action: str
     progress: Optional[PercentFloat] = None
     estimate: Optional[timedelta] = None
+    # requires 2.8.14+
+    health: Optional[str] = None
 
     @classmethod
     def _get_unifi_remaps(cls) -> Dict[str, str]:
         return {
             **super()._get_unifi_remaps(),
             "total_bytes": "totalBytes",
             "used_bytes": "usedBytes",
@@ -712,14 +714,15 @@
 
 
 class NVRFeatureFlags(ProtectBaseObject):
     beta: bool
     dev: bool
     notifications_v2: bool
     homekit_paired: Optional[bool] = None
+    ulp_role_management: Optional[bool] = None
 
 
 class NVR(ProtectDeviceModel):
     can_auto_update: bool
     is_stats_gathering_enabled: bool
     timezone: tzinfo
     version: Version
@@ -768,19 +771,30 @@
     ui_version: Optional[str] = None
     sso_channel: Optional[FirmwareReleaseChannel] = None
     is_stacked: Optional[bool] = None
     is_primary: Optional[bool] = None
     last_drive_slow_event: Optional[datetime] = None
     is_u_core_setup: Optional[bool] = None
     vault_camera_ids: list[str] = []
+    # requires 2.8.14+
+    corruption_state: Optional[str] = None
+    country_code: Optional[str] = None
+    has_gateway: Optional[bool] = None
+    is_vault_registered: Optional[bool] = None
+    public_ip: Optional[IPv4Address] = None
+    ulp_version: Optional[str] = None
+    wan_ip: Optional[IPv4Address] = None
 
     # TODO:
     # errorCode   read only
     # wifiSettings
     # smartDetectAgreement
+    # dbRecoveryOptions
+    # globalCameraSettings
+    # portStatus
 
     @classmethod
     def _get_unifi_remaps(cls) -> Dict[str, str]:
         return {
             **super()._get_unifi_remaps(),
             "recordingRetentionDurationMs": "recordingRetentionDuration",
             "vaultCameras": "vaultCameraIds",
@@ -951,25 +965,25 @@
         """Get if current version of Protect is a prerelease version."""
 
         # only EA versions have `-beta` in versions
         if self.version.is_prerelease:
             return True
 
         # 2.6.14 is an EA version that looks like a release version
-        versions = await self._read_cache_file(TMP_RELEASE_CACHE) or await self._read_cache_file(RELEASE_CACHE)
+        cache_file_path = self.api.cache_dir / "release_cache.json"
+        versions = await self._read_cache_file(cache_file_path) or await self._read_cache_file(RELEASE_CACHE)
         if versions is None or self.version not in versions:
             versions = await self.api.get_release_versions()
             try:
                 _LOGGER.debug("Fetching releases from APT repos...")
-                base = TMP_RELEASE_CACHE.parent
-                tmp = base / "release_cache.tmp.json"
-                await aos.makedirs(base, exist_ok=True)
+                tmp = self.api.cache_dir / "release_cache.tmp.json"
+                await aos.makedirs(self.api.cache_dir, exist_ok=True)
                 async with aiofiles.open(tmp, "wb") as cache_file:
                     await cache_file.write(orjson.dumps([str(v) for v in versions]))
-                await aos.rename(tmp, TMP_RELEASE_CACHE)
+                await aos.rename(tmp, cache_file_path)
             except Exception:  # pylint: disable=broad-except
                 _LOGGER.warning("Failed write cache file.")
 
         return self.version not in versions
 
 
 class LiveviewSlot(ProtectBaseObject):
```

### Comparing `pyunifiprotect-4.7.0/pyunifiprotect/data/types.py` & `pyunifiprotect-4.8.0/pyunifiprotect/data/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,14 +162,16 @@
     #
     MOTION_LIGHT = "lightMotion"
     #
     DOORLOCK_OPEN = "doorlockOpened"
     DOORLOCK_CLOSE = "doorlockClosed"
     DOORLOCK_BATTERY_LOW = "doorlockBatteryLow"
     #
+    DISRUPTED_CONDITIONS = "ringDisruptedConditions"
+    #
     RECORDING_OFF = "recordingOff"
 
     @staticmethod
     def device_events() -> List[str]:
         return [EventType.MOTION.value, EventType.RING.value, EventType.SMART_DETECT.value]
 
     @staticmethod
```

### Comparing `pyunifiprotect-4.7.0/pyunifiprotect/data/user.py` & `pyunifiprotect-4.8.0/pyunifiprotect/data/user.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/pyunifiprotect/data/websocket.py` & `pyunifiprotect-4.8.0/pyunifiprotect/data/websocket.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/pyunifiprotect/exceptions.py` & `pyunifiprotect-4.8.0/pyunifiprotect/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/pyunifiprotect/stream.py` & `pyunifiprotect-4.8.0/pyunifiprotect/stream.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/pyunifiprotect/test_util/__init__.py` & `pyunifiprotect-4.8.0/pyunifiprotect/test_util/__init__.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/pyunifiprotect/test_util/anonymize.py` & `pyunifiprotect-4.8.0/pyunifiprotect/test_util/anonymize.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/pyunifiprotect/utils.py` & `pyunifiprotect-4.8.0/pyunifiprotect/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,16 @@
 
 SNAKE_CASE_MATCH_1 = re.compile("(.)([A-Z0-9][a-z]+)")
 SNAKE_CASE_MATCH_2 = re.compile("__([A-Z0-9])")
 SNAKE_CASE_MATCH_3 = re.compile("([a-z0-9])([A-Z])")
 
 _LOGGER = logging.getLogger(__name__)
 
+RELEASE_CACHE = Path(__file__).parent / "release_cache.json"
+
 
 def set_debug() -> None:
     """Sets ENV variable for UFP_DEBUG to on (True)"""
     os.environ[DEBUG_ENV] = str(True)
 
 
 def set_no_debug() -> None:
```

### Comparing `pyunifiprotect-4.7.0/pyunifiprotect/websocket.py` & `pyunifiprotect-4.8.0/pyunifiprotect/websocket.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     backoff: int
     _auth: CALLBACK_TYPE
     _timeout: float
     _ws_subscriptions: List[Callable[[WSMessage], None]]
     _connect_lock: asyncio.Lock
 
     _headers: Optional[Dict[str, str]] = None
+    _websocket_loop_task: Optional[asyncio.Task[None]] = None
     _timer_task: Optional[asyncio.Task[None]] = None
     _ws_connection: Optional[ClientWebSocketResponse] = None
     _last_connect: float = -1000
     _recent_failures: int = 0
 
     def __init__(
         self,
@@ -155,15 +156,15 @@
         try:
             await asyncio.wait_for(self._connect_lock.acquire(), timeout=0.1)
         except asyncio.TimeoutError:
             _LOGGER.debug("Failed to get connection lock")
 
         start_event = asyncio.Event()
         _LOGGER.debug("Scheduling WS connect...")
-        asyncio.create_task(self._websocket_loop(start_event))
+        self._websocket_loop_task = asyncio.create_task(self._websocket_loop(start_event))
 
         try:
             await asyncio.wait_for(start_event.wait(), timeout=self.timeout_interval)
         except asyncio.TimeoutError:
             _LOGGER.warning("Timed out while waiting for Websocket to connect")
             await self.disconnect()
```

### Comparing `pyunifiprotect-4.7.0/pyunifiprotect.egg-info/PKG-INFO` & `pyunifiprotect-4.8.0/pyunifiprotect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyunifiprotect
-Version: 4.7.0
+Version: 4.8.0
 Summary: Unofficial UniFi Protect Python API and CLI
 Author-email: Bjarne Riis <bjarne@briis.com>, Christopher Bailey <cbailey@mort.is>
 Maintainer-email: Christopher Bailey <cbailey@mort.is>, "J. Nick Koston" <nick@koston.org>
 License: MIT
 Project-URL: Source Code, https://github.com/AngellusMortis/pyunifiprotect/
 Project-URL: Documentation, https://angellusmortis.github.io/pyunifiprotect/latest/
 Project-URL: Bug Reports, https://github.com/AngellusMortis/pyunifiprotect/issues/
```

### Comparing `pyunifiprotect-4.7.0/pyunifiprotect.egg-info/SOURCES.txt` & `pyunifiprotect-4.8.0/pyunifiprotect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/pyunifiprotect.egg-info/requires.txt` & `pyunifiprotect-4.8.0/pyunifiprotect.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/requirements.txt` & `pyunifiprotect-4.8.0/requirements.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 #
-# This file is autogenerated by pip-compile with python 3.10
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.11
+# by the following command:
 #
-#    pip-compile --extra=full --output-file=requirements.txt --pip-args='--root-user-action=ignore' pyproject.toml
+#    pip-compile --extra=full --output-file=requirements.txt --pip-args='--root-user-action=ignore' --resolver=backtracking pyproject.toml
 #
 aiofiles==23.1.0
     # via pyunifiprotect (pyproject.toml)
 aiohttp==3.8.4
     # via pyunifiprotect (pyproject.toml)
-aioshutil==1.2
+aioshutil==1.3
     # via pyunifiprotect (pyproject.toml)
 aiosignal==1.3.1
     # via aiohttp
 aiosqlite==0.18.0
     # via pyunifiprotect (pyproject.toml)
 asttokens==2.2.1
     # via stack-data
 async-timeout==4.0.2
     # via
     #   aiohttp
     #   pyunifiprotect (pyproject.toml)
 asyncify==0.9.1
     # via pyunifiprotect (pyproject.toml)
-attrs==22.2.0
+attrs==23.1.0
     # via aiohttp
 av==10.0.0
     # via pyunifiprotect (pyproject.toml)
 backcall==0.2.0
     # via ipython
-charset-normalizer==3.0.1
+charset-normalizer==3.1.0
     # via aiohttp
 click==8.1.3
     # via typer
 colorama==0.4.6
     # via typer
 commonmark==0.9.1
     # via rich
-dateparser==1.1.7
+dateparser==1.1.8
     # via pyunifiprotect (pyproject.toml)
 decorator==5.1.1
     # via ipython
 executing==1.2.0
     # via stack-data
 frozenlist==1.3.3
     # via
@@ -48,88 +48,88 @@
     #   aiosignal
 funkify==0.4.4
     # via asyncify
 greenlet==2.0.2
     # via sqlalchemy
 idna==3.4
     # via yarl
-ipython==8.10.0
+ipython==8.12.0
     # via pyunifiprotect (pyproject.toml)
 jedi==0.18.2
     # via ipython
 matplotlib-inline==0.1.6
     # via ipython
 multidict==6.0.4
     # via
     #   aiohttp
     #   yarl
-orjson==3.8.6
+orjson==3.8.10
     # via pyunifiprotect (pyproject.toml)
-packaging==23.0
+packaging==23.1
     # via pyunifiprotect (pyproject.toml)
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
-pillow==9.4.0
+pillow==9.5.0
     # via pyunifiprotect (pyproject.toml)
-prompt-toolkit==3.0.36
+prompt-toolkit==3.0.38
     # via ipython
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-pydantic==1.10.4
+pydantic==1.10.7
     # via pyunifiprotect (pyproject.toml)
-pygments==2.14.0
+pygments==2.15.0
     # via
     #   ipython
     #   rich
 pyjwt==2.6.0
     # via pyunifiprotect (pyproject.toml)
 python-dateutil==2.8.2
     # via dateparser
-python-dotenv==0.21.1
+python-dotenv==1.0.0
     # via pyunifiprotect (pyproject.toml)
-pytz==2022.7.1
+pytz==2023.3
     # via dateparser
 pytz-deprecation-shim==0.1.0.post0
     # via tzlocal
-regex==2022.10.31
+regex==2023.3.23
     # via dateparser
 rich==12.6.0
     # via typer
-shellingham==1.5.1
+shellingham==1.5.0.post1
     # via typer
 six==1.16.0
     # via
     #   asttokens
     #   python-dateutil
-sqlalchemy[asyncio]==2.0.3
+sqlalchemy[asyncio]==2.0.9
     # via pyunifiprotect (pyproject.toml)
 stack-data==0.6.2
     # via ipython
 termcolor==2.2.0
     # via pyunifiprotect (pyproject.toml)
 traitlets==5.9.0
     # via
     #   ipython
     #   matplotlib-inline
 typer[all]==0.7.0
     # via pyunifiprotect (pyproject.toml)
-typing-extensions==4.4.0
+typing-extensions==4.5.0
     # via
     #   pydantic
     #   sqlalchemy
     #   xtyping
-tzdata==2022.7
+tzdata==2023.3
     # via pytz-deprecation-shim
-tzlocal==4.2
+tzlocal==4.3
     # via dateparser
 wcwidth==0.2.6
     # via prompt-toolkit
-xtyping==0.6.1
+xtyping==0.6.2
     # via asyncify
 yarl==1.8.2
     # via aiohttp
```

### Comparing `pyunifiprotect-4.7.0/tests/conftest.py` & `pyunifiprotect-4.8.0/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -518,27 +518,44 @@
     "fwUpdateState",
     "isWaterproofCaseAttached",
     "deletedAt",
     "deletionType",
     "lastDisconnect",
     # 2.7.15
     "featureFlags",  # added to chime
+    # 2.8.14+
+    "nvrMac",
+    "useGlobal",
+    "is2K",
+    "is4K",
+    "ulpVersion",
+    "wanIp",
+    "publicIp",
+    "isVaultRegistered",
+    "hasGateway",
+    "corruptionState",
+    "countryCode",
 }
 
 NEW_CAMERA_FEATURE_FLAGS = {
     "audio",
     "audioCodecs",
     "hasInfrared",
     "hotplug",
     "smartDetectAudioTypes",
     "lensType",
     # 2.7.18+
     "isDoorbell",
 }
 
+NEW_NVR_FEATURE_FLAGS = {
+    # 2.8.14+
+    "ulpRoleManagement",
+}
+
 OLD_FIELDS = {
     # remove in 2.7.12
     "avgMotions",
 }
 
 
 def compare_objs(obj_type, expected, actual):
@@ -568,14 +585,16 @@
 
         expected["motionZones"] = actual["motionZones"] = []
         expected["privacyZones"] = actual["privacyZones"] = []
         expected["smartDetectZones"] = actual["smartDetectZones"] = []
         expected["recordingSettings"]["enableMotionDetection"] = expected["recordingSettings"].get(
             "enableMotionDetection"
         )
+        if "isColorNightVisionEnabled" not in expected["ispSettings"]:
+            actual["ispSettings"].pop("isColorNightVisionEnabled", None)
 
         if expected["eventStats"]["motion"].get("recentHours") in [[None], None, []]:
             expected["eventStats"]["motion"].pop("recentHours", None)
             actual["eventStats"]["motion"].pop("recentHours", None)
         if expected["eventStats"]["smart"].get("recentHours") == [[None], None, []]:
             expected["eventStats"]["smart"].pop("recentHours", None)
             actual["eventStats"]["smart"].pop("recentHours", None)
@@ -599,14 +618,15 @@
         if "lastLoginIp" not in expected:
             actual.pop("lastLoginIp", None)
         if "lastLoginTime" not in expected:
             actual.pop("lastLoginTime", None)
     elif obj_type == ModelType.EVENT.value:
         expected.pop("partition", None)
         expected.pop("deletionType", None)
+        expected.pop("description", None)
 
         expected_keys = (expected.get("metadata") or {}).keys()
         actual_keys = (actual.get("metadata") or {}).keys()
         # delete all extra metadata keys, many of which are not modeled
         for key in set(expected_keys).difference(actual_keys):
             del expected["metadata"][key]
     elif obj_type in (ModelType.SENSOR.value, ModelType.DOORLOCK.value):
@@ -618,22 +638,34 @@
         del expected["apRssi"]
         del expected["elementInfo"]
     elif obj_type == ModelType.NVR.value:
         # TODO:
         del expected["errorCode"]
         del expected["wifiSettings"]
         del expected["smartDetectAgreement"]
+        expected.pop("dbRecoveryOptions", None)
+        expected.pop("globalCameraSettings", None)
+        expected.pop("portStatus", None)
+
         expected["ports"]["piongw"] = expected["ports"].get("piongw")
         expected["ports"]["stacking"] = expected["ports"].get("stacking")
         expected["ports"]["emsJsonCLI"] = expected["ports"].get("emsJsonCLI")
 
         if "homekitPaired" in actual["featureFlags"] and "homekitPaired" not in expected["featureFlags"]:
             del actual["featureFlags"]["homekitPaired"]
 
+        if "capability" not in expected["systemInfo"]["storage"]:
+            actual["systemInfo"]["storage"].pop("capability", None)
+
         # float math...
+        cpu_fields = ["averageLoad", "temperature"]
+        for key in cpu_fields:
+            if math.isclose(expected["systemInfo"]["cpu"][key], actual["systemInfo"]["cpu"][key], rel_tol=0.01):
+                expected["systemInfo"]["cpu"][key] = actual["systemInfo"]["cpu"][key]
+
         if expected["systemInfo"].get("ustorage") is not None:
             for index, disk in enumerate(expected["systemInfo"]["ustorage"]["disks"]):
                 actual_disk = actual["systemInfo"]["ustorage"]["disks"][index]
                 estimate = disk.get("estimate")
                 actual_estimate = actual_disk.get("estimate")
                 if estimate is not None and actual_estimate is not None:
                     if math.isclose(estimate, actual_estimate, rel_tol=0.01):
@@ -643,14 +675,18 @@
                 actual_device = actual["systemInfo"]["ustorage"]["space"][index]
                 estimate = device.get("estimate")
                 actual_estimate = actual_device.get("estimate")
                 if estimate is not None and actual_estimate is not None:
                     if math.isclose(estimate, actual_estimate, rel_tol=0.01):
                         actual["systemInfo"]["ustorage"]["space"][index]["estimate"] = estimate
 
+        for flag in NEW_NVR_FEATURE_FLAGS:
+            if flag not in expected["featureFlags"]:
+                del actual["featureFlags"][flag]
+
     if "bluetoothConnectionState" in expected:
         expected["bluetoothConnectionState"]["experienceScore"] = expected["bluetoothConnectionState"].get(
             "experienceScore"
         )
 
     if "wifiConnectionState" in expected:
         expected["wifiConnectionState"]["bssid"] = expected["wifiConnectionState"].get("bssid")
```

### Comparing `pyunifiprotect-4.7.0/tests/data/test_camera.py` & `pyunifiprotect-4.8.0/tests/data/test_camera.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/tests/data/test_chime.py` & `pyunifiprotect-4.8.0/tests/data/test_chime.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/tests/data/test_common.py` & `pyunifiprotect-4.8.0/tests/data/test_common.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/tests/data/test_doorlock.py` & `pyunifiprotect-4.8.0/tests/data/test_doorlock.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/tests/data/test_light.py` & `pyunifiprotect-4.8.0/tests/data/test_light.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/tests/data/test_nvr.py` & `pyunifiprotect-4.8.0/tests/data/test_nvr.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/tests/data/test_sensor.py` & `pyunifiprotect-4.8.0/tests/data/test_sensor.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/tests/data/test_viewer.py` & `pyunifiprotect-4.8.0/tests/data/test_viewer.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/tests/sample_data/constants.py` & `pyunifiprotect-4.8.0/tests/sample_data/constants.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/tests/sample_data/sample_bootstrap.json` & `pyunifiprotect-4.8.0/tests/sample_data/sample_bootstrap.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/tests/sample_data/sample_bridge.json` & `pyunifiprotect-4.8.0/tests/sample_data/sample_bridge.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/tests/sample_data/sample_camera.json` & `pyunifiprotect-4.8.0/tests/sample_data/sample_camera.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/tests/sample_data/sample_camera_heatmap.png` & `pyunifiprotect-4.8.0/tests/sample_data/sample_camera_heatmap.png`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/tests/sample_data/sample_camera_snapshot.png` & `pyunifiprotect-4.8.0/tests/sample_data/sample_camera_snapshot.png`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/tests/sample_data/sample_camera_thumbnail.png` & `pyunifiprotect-4.8.0/tests/sample_data/sample_camera_thumbnail.png`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/tests/sample_data/sample_camera_video.mp4` & `pyunifiprotect-4.8.0/tests/sample_data/sample_camera_video.mp4`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/tests/sample_data/sample_chime.json` & `pyunifiprotect-4.8.0/tests/sample_data/sample_chime.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/tests/sample_data/sample_constants.json` & `pyunifiprotect-4.8.0/tests/sample_data/sample_constants.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/tests/sample_data/sample_doorlock.json` & `pyunifiprotect-4.8.0/tests/sample_data/sample_doorlock.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/tests/sample_data/sample_event_smart_track.json` & `pyunifiprotect-4.8.0/tests/sample_data/sample_event_smart_track.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/tests/sample_data/sample_light.json` & `pyunifiprotect-4.8.0/tests/sample_data/sample_light.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/tests/sample_data/sample_liveview.json` & `pyunifiprotect-4.8.0/tests/sample_data/sample_liveview.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/tests/sample_data/sample_raw_events.json` & `pyunifiprotect-4.8.0/tests/sample_data/sample_raw_events.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/tests/sample_data/sample_sensor.json` & `pyunifiprotect-4.8.0/tests/sample_data/sample_sensor.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/tests/sample_data/sample_viewport.json` & `pyunifiprotect-4.8.0/tests/sample_data/sample_viewport.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/tests/sample_data/sample_ws_messages.json` & `pyunifiprotect-4.8.0/tests/sample_data/sample_ws_messages.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/tests/test_api.py` & `pyunifiprotect-4.8.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/tests/test_api_polling.py` & `pyunifiprotect-4.8.0/tests/test_api_polling.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.7.0/tests/test_api_ws.py` & `pyunifiprotect-4.8.0/tests/test_api_ws.py`

 * *Files 2% similar despite different names*

```diff
@@ -399,16 +399,14 @@
     assert not obj.is_ringing
     with patch("pyunifiprotect.data.bootstrap.utc_now", mock_now):
         protect_client._process_ws_message(msg)
     assert obj.is_ringing
     mock_now.return_value = utc_now() + EVENT_PING_INTERVAL
     assert not obj.is_ringing
 
-    protect_client.emit_message.assert_called_once()
-
 
 @pytest.mark.skipif(not TEST_SENSOR_EXISTS, reason="Missing testdata")
 @patch("pyunifiprotect.data.devices.utc_now")
 @pytest.mark.asyncio
 async def test_ws_emit_alarm_callback(
     mock_now, protect_client_no_debug: ProtectApiClient, now: datetime, sensor, packet: WSPacket
 ):
@@ -437,16 +435,14 @@
     assert not obj.is_alarm_detected
     with patch("pyunifiprotect.data.bootstrap.utc_now", mock_now):
         protect_client._process_ws_message(msg)
     assert obj.is_alarm_detected
     mock_now.return_value = utc_now() + EVENT_PING_INTERVAL
     assert not obj.is_alarm_detected
 
-    protect_client.emit_message.assert_called_once()
-
 
 @pytest.mark.asyncio
 async def test_check_ws_connected(protect_client_ws: ProtectApiClient, caplog: pytest.LogCaptureFixture):
     caplog.set_level(logging.DEBUG)
 
     active_ws = protect_client_ws.check_ws()
```

### Comparing `pyunifiprotect-4.7.0/tests/test_utils.py` & `pyunifiprotect-4.8.0/tests/test_utils.py`

 * *Files identical despite different names*

