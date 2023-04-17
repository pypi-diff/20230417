# Comparing `tmp/smartwheel-core-0.0.2.tar.gz` & `tmp/smartwheel-core-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartwheel-core-0.0.2.tar", last modified: Tue Mar 14 12:17:14 2023, max compression
+gzip compressed data, was "smartwheel-core-0.0.3.tar", last modified: Mon Apr 17 06:57:06 2023, max compression
```

## Comparing `smartwheel-core-0.0.2.tar` & `smartwheel-core-0.0.3.tar`

### file list

```diff
@@ -1,124 +1,138 @@
-drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-03-14 12:17:14.160324 smartwheel-core-0.0.2/
--rw-r--r--   0 fitz      (1000) fitz      (1000)    35149 2022-05-16 11:10:38.000000 smartwheel-core-0.0.2/LICENSE
--rw-r--r--   0 fitz      (1000) fitz      (1000)       52 2023-03-14 08:39:34.000000 smartwheel-core-0.0.2/MANIFEST.in
--rw-r--r--   0 fitz      (1000) fitz      (1000)    45151 2023-03-14 12:17:14.160324 smartwheel-core-0.0.2/PKG-INFO
--rw-r--r--   0 fitz      (1000) fitz      (1000)     4001 2023-03-14 11:25:55.000000 smartwheel-core-0.0.2/README.md
--rw-r--r--   0 fitz      (1000) fitz      (1000)     1008 2023-03-14 12:16:21.000000 smartwheel-core-0.0.2/pyproject.toml
--rw-r--r--   0 fitz      (1000) fitz      (1000)       38 2023-03-14 12:17:14.160324 smartwheel-core-0.0.2/setup.cfg
-drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-03-14 12:17:14.129325 smartwheel-core-0.0.2/src/
-drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-03-14 12:17:14.135325 smartwheel-core-0.0.2/src/smartwheel/
--rw-r--r--   0 fitz      (1000) fitz      (1000)       22 2023-03-14 12:16:32.000000 smartwheel-core-0.0.2/src/smartwheel/__init__.py
--rwxr-xr-x   0 fitz      (1000) fitz      (1000)     7912 2023-03-14 10:42:46.000000 smartwheel-core-0.0.2/src/smartwheel/__main__.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)     5615 2023-03-14 10:37:19.000000 smartwheel-core-0.0.2/src/smartwheel/actionengine.py
-drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-03-14 12:17:14.137324 smartwheel-core-0.0.2/src/smartwheel/actions/
--rw-r--r--   0 fitz      (1000) fitz      (1000)        0 2022-05-16 11:10:38.000000 smartwheel-core-0.0.2/src/smartwheel/actions/__init__.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)       95 2023-03-07 10:31:43.000000 smartwheel-core-0.0.2/src/smartwheel/actions/baseaction.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)      338 2023-03-14 09:26:20.000000 smartwheel-core-0.0.2/src/smartwheel/actions/custom.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)     2818 2023-03-14 09:26:29.000000 smartwheel-core-0.0.2/src/smartwheel/actions/keypress.py
-drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-03-14 12:17:14.138325 smartwheel-core-0.0.2/src/smartwheel/actions/wheel/
--rw-r--r--   0 fitz      (1000) fitz      (1000)        0 2022-10-15 10:15:43.000000 smartwheel-core-0.0.2/src/smartwheel/actions/wheel/__init__.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)       93 2023-03-07 10:31:43.000000 smartwheel-core-0.0.2/src/smartwheel/actions/wheel/base.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)      409 2023-03-14 09:26:43.000000 smartwheel-core-0.0.2/src/smartwheel/actions/wheel/module.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)      670 2023-03-14 09:26:50.000000 smartwheel-core-0.0.2/src/smartwheel/actions/wheel/wheel.py
-drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-03-14 12:17:14.139325 smartwheel-core-0.0.2/src/smartwheel/backgrounds/
--rw-r--r--   0 fitz      (1000) fitz      (1000)        0 2023-03-07 16:05:15.000000 smartwheel-core-0.0.2/src/smartwheel/backgrounds/__init__.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)      510 2023-03-14 09:26:58.000000 smartwheel-core-0.0.2/src/smartwheel/backgrounds/base.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)     1437 2023-03-14 09:33:55.000000 smartwheel-core-0.0.2/src/smartwheel/backgrounds/basic.py
-drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-03-14 12:17:14.140324 smartwheel-core-0.0.2/src/smartwheel/backgrounds/config/
--rw-r--r--   0 fitz      (1000) fitz      (1000)      133 2023-03-10 13:03:51.000000 smartwheel-core-0.0.2/src/smartwheel/backgrounds/config/contour.json
--rw-r--r--   0 fitz      (1000) fitz      (1000)       67 2023-03-10 17:35:19.000000 smartwheel-core-0.0.2/src/smartwheel/backgrounds/config/pattern.json
--rw-r--r--   0 fitz      (1000) fitz      (1000)      169 2023-03-10 12:18:32.000000 smartwheel-core-0.0.2/src/smartwheel/backgrounds/config.json
--rw-r--r--   0 fitz      (1000) fitz      (1000)     4936 2023-03-14 09:33:55.000000 smartwheel-core-0.0.2/src/smartwheel/backgrounds/contour.py
-drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-03-14 12:17:14.125325 smartwheel-core-0.0.2/src/smartwheel/cache/
-drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-03-14 12:17:14.140324 smartwheel-core-0.0.2/src/smartwheel/cache/background_contour/
--rw-r--r--   0 fitz      (1000) fitz      (1000)      143 2023-03-14 08:57:54.000000 smartwheel-core-0.0.2/src/smartwheel/cache/background_contour/contour1.json
--rw-r--r--   0 fitz      (1000) fitz      (1000)    29072 2023-03-14 08:57:54.000000 smartwheel-core-0.0.2/src/smartwheel/cache/background_contour/contour1.png
--rw-r--r--   0 fitz      (1000) fitz      (1000)    12153 2023-03-14 11:05:49.000000 smartwheel-core-0.0.2/src/smartwheel/canvas.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)     3585 2023-03-14 11:05:49.000000 smartwheel-core-0.0.2/src/smartwheel/common.py
-drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-03-14 12:17:14.144324 smartwheel-core-0.0.2/src/smartwheel/config/
--rw-r--r--   0 fitz      (1000) fitz      (1000)    13806 2023-03-10 13:03:51.000000 smartwheel-core-0.0.2/src/smartwheel/config/actionengine.json
--rw-r--r--   0 fitz      (1000) fitz      (1000)      724 2023-03-10 13:03:51.000000 smartwheel-core-0.0.2/src/smartwheel/config/bgkeyboard.json
--rw-r--r--   0 fitz      (1000) fitz      (1000)      427 2023-03-10 16:13:31.000000 smartwheel-core-0.0.2/src/smartwheel/config/common.json
--rw-r--r--   0 fitz      (1000) fitz      (1000)     2926 2023-03-11 12:22:23.000000 smartwheel-core-0.0.2/src/smartwheel/config/config.json
--rw-r--r--   0 fitz      (1000) fitz      (1000)      224 2023-03-10 13:03:51.000000 smartwheel-core-0.0.2/src/smartwheel/config/folder.json
--rw-r--r--   0 fitz      (1000) fitz      (1000)     1175 2023-03-10 13:03:51.000000 smartwheel-core-0.0.2/src/smartwheel/config/hue.json
-drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-03-14 12:17:14.145325 smartwheel-core-0.0.2/src/smartwheel/config/internal/
--rw-r--r--   0 fitz      (1000) fitz      (1000)       44 2022-05-16 11:10:38.000000 smartwheel-core-0.0.2/src/smartwheel/config/internal/krita_server.json
--rw-r--r--   0 fitz      (1000) fitz      (1000)      273 2022-10-15 10:15:43.000000 smartwheel-core-0.0.2/src/smartwheel/config/keyboard.json
--rw-r--r--   0 fitz      (1000) fitz      (1000)     2164 2023-03-13 08:43:44.000000 smartwheel-core-0.0.2/src/smartwheel/config/media.json
--rw-r--r--   0 fitz      (1000) fitz      (1000)     1130 2023-03-10 13:03:51.000000 smartwheel-core-0.0.2/src/smartwheel/config/serial.json
--rw-r--r--   0 fitz      (1000) fitz      (1000)      613 2023-03-10 13:03:51.000000 smartwheel-core-0.0.2/src/smartwheel/config/wheel.json
--rw-r--r--   0 fitz      (1000) fitz      (1000)     9887 2023-03-14 09:31:23.000000 smartwheel-core-0.0.2/src/smartwheel/config.py
-drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-03-14 12:17:14.146324 smartwheel-core-0.0.2/src/smartwheel/docs/
-drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-03-14 12:17:14.127324 smartwheel-core-0.0.2/src/smartwheel/docs/_build/
-drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-03-14 12:17:14.127324 smartwheel-core-0.0.2/src/smartwheel/docs/_build/html/
-drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-03-14 12:17:14.147324 smartwheel-core-0.0.2/src/smartwheel/docs/_build/html/_static/
-drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-03-14 12:17:14.127324 smartwheel-core-0.0.2/src/smartwheel/docs/_build/html/_static/css/
-drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-03-14 12:17:14.147324 smartwheel-core-0.0.2/src/smartwheel/docs/_build/html/_static/css/fonts/
--rw-r--r--   0 fitz      (1000) fitz      (1000)   444379 2023-01-12 13:41:03.000000 smartwheel-core-0.0.2/src/smartwheel/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0 fitz      (1000) fitz      (1000)      286 2022-10-15 10:15:55.000000 smartwheel-core-0.0.2/src/smartwheel/docs/_build/html/_static/file.png
--rw-r--r--   0 fitz      (1000) fitz      (1000)       90 2022-10-15 10:15:55.000000 smartwheel-core-0.0.2/src/smartwheel/docs/_build/html/_static/minus.png
--rw-r--r--   0 fitz      (1000) fitz      (1000)       90 2022-10-15 10:15:55.000000 smartwheel-core-0.0.2/src/smartwheel/docs/_build/html/_static/plus.png
--rw-r--r--   0 fitz      (1000) fitz      (1000)     1185 2023-03-07 10:31:43.000000 smartwheel-core-0.0.2/src/smartwheel/docs/conf.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)     1747 2023-03-09 12:41:38.000000 smartwheel-core-0.0.2/src/smartwheel/gui_tools.py
-drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-03-14 12:17:14.128325 smartwheel-core-0.0.2/src/smartwheel/icons/
-drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-03-14 12:17:14.150324 smartwheel-core-0.0.2/src/smartwheel/icons/default/
--rw-r--r--   0 fitz      (1000) fitz      (1000)     5227 2022-05-16 11:10:38.000000 smartwheel-core-0.0.2/src/smartwheel/icons/default/folder.png
--rw-r--r--   0 fitz      (1000) fitz      (1000)    30624 2022-05-16 11:10:38.000000 smartwheel-core-0.0.2/src/smartwheel/icons/default/hue.png
--rw-r--r--   0 fitz      (1000) fitz      (1000)     5386 2022-05-16 11:10:38.000000 smartwheel-core-0.0.2/src/smartwheel/icons/default/hue.svg
--rw-r--r--   0 fitz      (1000) fitz      (1000)    15349 2022-05-16 11:10:38.000000 smartwheel-core-0.0.2/src/smartwheel/icons/default/media.png
--rw-r--r--   0 fitz      (1000) fitz      (1000)     1900 2022-05-16 11:10:38.000000 smartwheel-core-0.0.2/src/smartwheel/icons/default/pause.png
--rw-r--r--   0 fitz      (1000) fitz      (1000)     3297 2022-05-16 11:10:38.000000 smartwheel-core-0.0.2/src/smartwheel/icons/default/play.png
--rw-r--r--   0 fitz      (1000) fitz      (1000)     8682 2022-05-16 11:10:38.000000 smartwheel-core-0.0.2/src/smartwheel/icons/default/round.png
--rw-r--r--   0 fitz      (1000) fitz      (1000)       29 2023-01-16 11:54:26.000000 smartwheel-core-0.0.2/src/smartwheel/launch.json
--rw-r--r--   0 fitz      (1000) fitz      (1000)   242358 2022-05-16 11:10:38.000000 smartwheel-core-0.0.2/src/smartwheel/logo.png
-drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-03-14 12:17:14.128325 smartwheel-core-0.0.2/src/smartwheel/presets/
-drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-03-14 12:17:14.151324 smartwheel-core-0.0.2/src/smartwheel/presets/appearance/
--rw-r--r--   0 fitz      (1000) fitz      (1000)     1195 2023-03-13 06:24:07.000000 smartwheel-core-0.0.2/src/smartwheel/presets/appearance/blackout.json
--rw-r--r--   0 fitz      (1000) fitz      (1000)     1204 2023-03-10 16:18:28.000000 smartwheel-core-0.0.2/src/smartwheel/presets/appearance/classic.json
--rw-r--r--   0 fitz      (1000) fitz      (1000)     1200 2023-03-10 16:18:18.000000 smartwheel-core-0.0.2/src/smartwheel/presets/appearance/polar.json
-drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-03-14 12:17:14.153324 smartwheel-core-0.0.2/src/smartwheel/serialpipe/
--rw-r--r--   0 fitz      (1000) fitz      (1000)        0 2022-05-16 11:10:38.000000 smartwheel-core-0.0.2/src/smartwheel/serialpipe/__init__.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)     9049 2023-03-07 15:47:03.000000 smartwheel-core-0.0.2/src/smartwheel/serialpipe/base.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)     4553 2023-03-14 11:05:52.000000 smartwheel-core-0.0.2/src/smartwheel/serialpipe/bgkeyboard.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)     1829 2023-03-14 09:33:55.000000 smartwheel-core-0.0.2/src/smartwheel/serialpipe/keyboard.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)     1778 2023-03-14 09:30:09.000000 smartwheel-core-0.0.2/src/smartwheel/serialpipe/serial.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)    20828 2023-03-14 10:44:48.000000 smartwheel-core-0.0.2/src/smartwheel/settings.py
-drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-03-14 12:17:14.154324 smartwheel-core-0.0.2/src/smartwheel/settings_handlers/
--rw-r--r--   0 fitz      (1000) fitz      (1000)        0 2023-01-28 07:05:00.000000 smartwheel-core-0.0.2/src/smartwheel/settings_handlers/__init__.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)    12276 2023-03-14 09:30:38.000000 smartwheel-core-0.0.2/src/smartwheel/settings_handlers/actions.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)     2135 2023-03-13 07:05:07.000000 smartwheel-core-0.0.2/src/smartwheel/settings_handlers/base.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)     7820 2023-03-14 09:31:23.000000 smartwheel-core-0.0.2/src/smartwheel/settings_handlers/basic.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)       68 2023-03-06 13:19:17.000000 smartwheel-core-0.0.2/src/smartwheel/settings_handlers/config.json
--rw-r--r--   0 fitz      (1000) fitz      (1000)     5115 2023-03-14 09:31:23.000000 smartwheel-core-0.0.2/src/smartwheel/settings_handlers/modules.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)     5445 2023-03-14 11:05:49.000000 smartwheel-core-0.0.2/src/smartwheel/settings_handlers/preset.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)      412 2023-03-14 09:31:46.000000 smartwheel-core-0.0.2/src/smartwheel/settings_handlers/serial.py
-drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-03-14 12:17:14.155325 smartwheel-core-0.0.2/src/smartwheel/settings_registry/
--rw-r--r--   0 fitz      (1000) fitz      (1000)     4019 2023-03-10 16:15:05.000000 smartwheel-core-0.0.2/src/smartwheel/settings_registry/appearance.json
--rw-r--r--   0 fitz      (1000) fitz      (1000)      368 2023-03-10 12:27:00.000000 smartwheel-core-0.0.2/src/smartwheel/settings_registry/config.json
-drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-03-14 12:17:14.155325 smartwheel-core-0.0.2/src/smartwheel/settings_registry/external/
--rw-r--r--   0 fitz      (1000) fitz      (1000)      672 2023-03-09 19:10:05.000000 smartwheel-core-0.0.2/src/smartwheel/settings_registry/external/contour.json
--rw-r--r--   0 fitz      (1000) fitz      (1000)      448 2023-03-10 16:00:47.000000 smartwheel-core-0.0.2/src/smartwheel/settings_registry/external/pattern.json
--rw-r--r--   0 fitz      (1000) fitz      (1000)     1165 2023-03-14 08:32:47.000000 smartwheel-core-0.0.2/src/smartwheel/settings_registry/general.json
--rw-r--r--   0 fitz      (1000) fitz      (1000)       97 2023-02-04 10:16:56.000000 smartwheel-core-0.0.2/src/smartwheel/settings_registry/serial.json
--rw-r--r--   0 fitz      (1000) fitz      (1000)      590 2023-03-08 19:13:53.000000 smartwheel-core-0.0.2/src/smartwheel/tools.py
-drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-03-14 12:17:14.157324 smartwheel-core-0.0.2/src/smartwheel/ui/
--rw-r--r--   0 fitz      (1000) fitz      (1000)        0 2022-05-16 11:10:38.000000 smartwheel-core-0.0.2/src/smartwheel/ui/__init__.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)      245 2023-03-13 09:01:47.000000 smartwheel-core-0.0.2/src/smartwheel/ui/base.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)     3674 2023-03-14 09:32:38.000000 smartwheel-core-0.0.2/src/smartwheel/ui/files.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)      767 2023-03-14 11:05:52.000000 smartwheel-core-0.0.2/src/smartwheel/ui/folder.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)    11410 2023-03-14 09:32:57.000000 smartwheel-core-0.0.2/src/smartwheel/ui/hue.py
-drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-03-14 12:17:14.158325 smartwheel-core-0.0.2/src/smartwheel/ui/internal/
--rw-r--r--   0 fitz      (1000) fitz      (1000)        0 2022-10-15 10:15:43.000000 smartwheel-core-0.0.2/src/smartwheel/ui/internal/__init__.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)      301 2023-03-07 15:47:03.000000 smartwheel-core-0.0.2/src/smartwheel/ui/internal/baseinternal.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)      410 2023-03-14 11:05:52.000000 smartwheel-core-0.0.2/src/smartwheel/ui/internal/krita_api.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)     2566 2023-03-14 11:05:52.000000 smartwheel-core-0.0.2/src/smartwheel/ui/internal/krita_server.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)     6180 2023-03-14 09:33:55.000000 smartwheel-core-0.0.2/src/smartwheel/ui/media.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)    20571 2023-03-14 10:58:22.000000 smartwheel-core-0.0.2/src/smartwheel/ui/wheel.py
-drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-03-14 12:17:14.159325 smartwheel-core-0.0.2/src/smartwheel_core.egg-info/
--rw-r--r--   0 fitz      (1000) fitz      (1000)    45151 2023-03-14 12:17:14.000000 smartwheel-core-0.0.2/src/smartwheel_core.egg-info/PKG-INFO
--rw-r--r--   0 fitz      (1000) fitz      (1000)     3515 2023-03-14 12:17:14.000000 smartwheel-core-0.0.2/src/smartwheel_core.egg-info/SOURCES.txt
--rw-r--r--   0 fitz      (1000) fitz      (1000)        1 2023-03-14 12:17:14.000000 smartwheel-core-0.0.2/src/smartwheel_core.egg-info/dependency_links.txt
--rw-r--r--   0 fitz      (1000) fitz      (1000)       57 2023-03-14 12:17:14.000000 smartwheel-core-0.0.2/src/smartwheel_core.egg-info/entry_points.txt
--rw-r--r--   0 fitz      (1000) fitz      (1000)      129 2023-03-14 12:17:14.000000 smartwheel-core-0.0.2/src/smartwheel_core.egg-info/requires.txt
--rw-r--r--   0 fitz      (1000) fitz      (1000)       11 2023-03-14 12:17:14.000000 smartwheel-core-0.0.2/src/smartwheel_core.egg-info/top_level.txt
+drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 06:57:06.573902 smartwheel-core-0.0.3/
+-rw-r--r--   0 fitz      (1000) fitz      (1000)    35149 2022-05-16 11:10:38.000000 smartwheel-core-0.0.3/LICENSE
+-rw-r--r--   0 fitz      (1000) fitz      (1000)       65 2023-04-17 06:56:28.000000 smartwheel-core-0.0.3/MANIFEST.in
+-rw-r--r--   0 fitz      (1000) fitz      (1000)    45385 2023-04-17 06:57:06.572903 smartwheel-core-0.0.3/PKG-INFO
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     4235 2023-04-14 15:45:11.000000 smartwheel-core-0.0.3/README.md
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     1008 2023-04-17 06:50:21.000000 smartwheel-core-0.0.3/pyproject.toml
+-rw-r--r--   0 fitz      (1000) fitz      (1000)       38 2023-04-17 06:57:06.573902 smartwheel-core-0.0.3/setup.cfg
+drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 06:57:06.552903 smartwheel-core-0.0.3/src/
+drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 06:57:06.556903 smartwheel-core-0.0.3/src/smartwheel/
+-rw-r--r--   0 fitz      (1000) fitz      (1000)       22 2023-04-17 06:50:38.000000 smartwheel-core-0.0.3/src/smartwheel/__init__.py
+-rwxr-xr-x   0 fitz      (1000) fitz      (1000)    13103 2023-04-15 10:44:17.000000 smartwheel-core-0.0.3/src/smartwheel/__main__.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     5634 2023-04-15 10:36:59.000000 smartwheel-core-0.0.3/src/smartwheel/actionengine.py
+drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 06:57:06.557902 smartwheel-core-0.0.3/src/smartwheel/actions/
+-rw-r--r--   0 fitz      (1000) fitz      (1000)        0 2022-05-16 11:10:38.000000 smartwheel-core-0.0.3/src/smartwheel/actions/__init__.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)       95 2023-03-07 10:31:43.000000 smartwheel-core-0.0.3/src/smartwheel/actions/baseaction.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      338 2023-03-14 09:26:20.000000 smartwheel-core-0.0.3/src/smartwheel/actions/custom.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     2818 2023-03-14 09:26:29.000000 smartwheel-core-0.0.3/src/smartwheel/actions/keypress.py
+drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 06:57:06.558903 smartwheel-core-0.0.3/src/smartwheel/actions/wheel/
+-rw-r--r--   0 fitz      (1000) fitz      (1000)        0 2022-10-15 10:15:43.000000 smartwheel-core-0.0.3/src/smartwheel/actions/wheel/__init__.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)       93 2023-03-07 10:31:43.000000 smartwheel-core-0.0.3/src/smartwheel/actions/wheel/base.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      409 2023-03-14 09:26:43.000000 smartwheel-core-0.0.3/src/smartwheel/actions/wheel/module.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      670 2023-03-14 09:26:50.000000 smartwheel-core-0.0.3/src/smartwheel/actions/wheel/wheel.py
+drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 06:57:06.559903 smartwheel-core-0.0.3/src/smartwheel/backgrounds/
+-rw-r--r--   0 fitz      (1000) fitz      (1000)        0 2023-03-07 16:05:15.000000 smartwheel-core-0.0.3/src/smartwheel/backgrounds/__init__.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      510 2023-03-14 09:26:58.000000 smartwheel-core-0.0.3/src/smartwheel/backgrounds/base.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     1452 2023-03-20 06:26:26.000000 smartwheel-core-0.0.3/src/smartwheel/backgrounds/basic.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      174 2023-04-14 15:52:54.000000 smartwheel-core-0.0.3/src/smartwheel/backgrounds/config_defaults.json
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     4918 2023-04-15 11:28:35.000000 smartwheel-core-0.0.3/src/smartwheel/backgrounds/contour.py
+drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 06:57:06.550902 smartwheel-core-0.0.3/src/smartwheel/cache/
+drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 06:57:06.559903 smartwheel-core-0.0.3/src/smartwheel/cache/background_contour/
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      143 2023-03-14 08:57:54.000000 smartwheel-core-0.0.3/src/smartwheel/cache/background_contour/contour1.json
+-rw-r--r--   0 fitz      (1000) fitz      (1000)    29072 2023-03-14 08:57:54.000000 smartwheel-core-0.0.3/src/smartwheel/cache/background_contour/contour1.png
+-rw-r--r--   0 fitz      (1000) fitz      (1000)    12923 2023-04-15 10:34:20.000000 smartwheel-core-0.0.3/src/smartwheel/canvas.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     8947 2023-04-15 11:00:12.000000 smartwheel-core-0.0.3/src/smartwheel/common.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)    13575 2023-04-15 11:00:58.000000 smartwheel-core-0.0.3/src/smartwheel/config.py
+drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 06:57:06.560902 smartwheel-core-0.0.3/src/smartwheel/defaults/
+-rw-r--r--   0 fitz      (1000) fitz      (1000)    13807 2023-04-14 15:19:42.000000 smartwheel-core-0.0.3/src/smartwheel/defaults/actionengine.json
+drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 06:57:06.561903 smartwheel-core-0.0.3/src/smartwheel/defaults/backgrounds/
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      133 2023-03-10 13:03:51.000000 smartwheel-core-0.0.3/src/smartwheel/defaults/backgrounds/contour.json
+-rw-r--r--   0 fitz      (1000) fitz      (1000)       67 2023-03-10 17:35:19.000000 smartwheel-core-0.0.3/src/smartwheel/defaults/backgrounds/pattern.json
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      428 2023-03-15 11:11:32.000000 smartwheel-core-0.0.3/src/smartwheel/defaults/common.json
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     3387 2023-04-14 17:35:11.000000 smartwheel-core-0.0.3/src/smartwheel/defaults/config.json
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      225 2023-03-15 11:10:38.000000 smartwheel-core-0.0.3/src/smartwheel/defaults/folder.json
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     1142 2023-03-15 11:10:14.000000 smartwheel-core-0.0.3/src/smartwheel/defaults/hue.json
+drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 06:57:06.561903 smartwheel-core-0.0.3/src/smartwheel/defaults/internal/
+-rw-r--r--   0 fitz      (1000) fitz      (1000)       44 2022-05-16 11:10:38.000000 smartwheel-core-0.0.3/src/smartwheel/defaults/internal/krita_server.json
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     2007 2023-03-31 18:58:45.000000 smartwheel-core-0.0.3/src/smartwheel/defaults/media.json
+drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 06:57:06.561903 smartwheel-core-0.0.3/src/smartwheel/defaults/serial/
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      724 2023-03-10 13:03:51.000000 smartwheel-core-0.0.3/src/smartwheel/defaults/serial/bgkeyboard.json
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      273 2022-10-15 10:15:43.000000 smartwheel-core-0.0.3/src/smartwheel/defaults/serial/keyboard.json
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     1131 2023-03-20 11:00:24.000000 smartwheel-core-0.0.3/src/smartwheel/defaults/serial/serial.json
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      613 2023-03-10 13:03:51.000000 smartwheel-core-0.0.3/src/smartwheel/defaults/wheel.json
+drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 06:57:06.562903 smartwheel-core-0.0.3/src/smartwheel/docs/
+drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 06:57:06.550902 smartwheel-core-0.0.3/src/smartwheel/docs/_build/
+drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 06:57:06.550902 smartwheel-core-0.0.3/src/smartwheel/docs/_build/html/
+drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 06:57:06.562903 smartwheel-core-0.0.3/src/smartwheel/docs/_build/html/_static/
+drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 06:57:06.551902 smartwheel-core-0.0.3/src/smartwheel/docs/_build/html/_static/css/
+drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 06:57:06.562903 smartwheel-core-0.0.3/src/smartwheel/docs/_build/html/_static/css/fonts/
+-rw-r--r--   0 fitz      (1000) fitz      (1000)   444379 2023-01-12 13:41:03.000000 smartwheel-core-0.0.3/src/smartwheel/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      286 2022-10-15 10:15:55.000000 smartwheel-core-0.0.3/src/smartwheel/docs/_build/html/_static/file.png
+-rw-r--r--   0 fitz      (1000) fitz      (1000)       90 2022-10-15 10:15:55.000000 smartwheel-core-0.0.3/src/smartwheel/docs/_build/html/_static/minus.png
+-rw-r--r--   0 fitz      (1000) fitz      (1000)       90 2022-10-15 10:15:55.000000 smartwheel-core-0.0.3/src/smartwheel/docs/_build/html/_static/plus.png
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     1185 2023-03-07 10:31:43.000000 smartwheel-core-0.0.3/src/smartwheel/docs/conf.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     2849 2023-04-14 15:39:49.000000 smartwheel-core-0.0.3/src/smartwheel/gui_tools.py
+drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 06:57:06.551902 smartwheel-core-0.0.3/src/smartwheel/icons/
+drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 06:57:06.564902 smartwheel-core-0.0.3/src/smartwheel/icons/default/
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     5227 2022-05-16 11:10:38.000000 smartwheel-core-0.0.3/src/smartwheel/icons/default/folder.png
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     5386 2022-05-16 11:10:38.000000 smartwheel-core-0.0.3/src/smartwheel/icons/default/hue.svg
+-rw-r--r--   0 fitz      (1000) fitz      (1000)    30624 2022-05-16 11:10:38.000000 smartwheel-core-0.0.3/src/smartwheel/icons/default/hue_old.png
+-rw-r--r--   0 fitz      (1000) fitz      (1000)    15349 2022-05-16 11:10:38.000000 smartwheel-core-0.0.3/src/smartwheel/icons/default/media.png
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     1900 2022-05-16 11:10:38.000000 smartwheel-core-0.0.3/src/smartwheel/icons/default/pause.png
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     3297 2022-05-16 11:10:38.000000 smartwheel-core-0.0.3/src/smartwheel/icons/default/play.png
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     8682 2022-05-16 11:10:38.000000 smartwheel-core-0.0.3/src/smartwheel/icons/default/round.png
+drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 06:57:06.565903 smartwheel-core-0.0.3/src/smartwheel/icons/ionicons/
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      397 1985-10-26 08:15:00.000000 smartwheel-core-0.0.3/src/smartwheel/icons/ionicons/close.svg
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      547 1985-10-26 08:15:00.000000 smartwheel-core-0.0.3/src/smartwheel/icons/ionicons/folder.svg
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      269 2023-03-15 10:51:33.000000 smartwheel-core-0.0.3/src/smartwheel/icons/ionicons/hue.svg
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      335 1985-10-26 08:15:00.000000 smartwheel-core-0.0.3/src/smartwheel/icons/ionicons/media.svg
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      294 1985-10-26 08:15:00.000000 smartwheel-core-0.0.3/src/smartwheel/icons/ionicons/pause.svg
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      305 1985-10-26 08:15:00.000000 smartwheel-core-0.0.3/src/smartwheel/icons/ionicons/play.svg
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      917 1985-10-26 08:15:00.000000 smartwheel-core-0.0.3/src/smartwheel/icons/ionicons/settings.svg
+-rw-r--r--   0 fitz      (1000) fitz      (1000)       66 2023-04-14 17:50:58.000000 smartwheel-core-0.0.3/src/smartwheel/launch.json
+-rw-r--r--   0 fitz      (1000) fitz      (1000)   242358 2022-05-16 11:10:38.000000 smartwheel-core-0.0.3/src/smartwheel/logo.png
+drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 06:57:06.551902 smartwheel-core-0.0.3/src/smartwheel/presets/
+drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 06:57:06.566902 smartwheel-core-0.0.3/src/smartwheel/presets/appearance/
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     1289 2023-03-31 18:58:45.000000 smartwheel-core-0.0.3/src/smartwheel/presets/appearance/blackout.json
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     1298 2023-03-31 18:58:45.000000 smartwheel-core-0.0.3/src/smartwheel/presets/appearance/classic.json
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     1294 2023-03-31 18:58:45.000000 smartwheel-core-0.0.3/src/smartwheel/presets/appearance/polar.json
+drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 06:57:06.567902 smartwheel-core-0.0.3/src/smartwheel/serialpipe/
+-rw-r--r--   0 fitz      (1000) fitz      (1000)        0 2022-05-16 11:10:38.000000 smartwheel-core-0.0.3/src/smartwheel/serialpipe/__init__.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     9049 2023-03-07 15:47:03.000000 smartwheel-core-0.0.3/src/smartwheel/serialpipe/base.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     4572 2023-04-15 10:36:27.000000 smartwheel-core-0.0.3/src/smartwheel/serialpipe/bgkeyboard.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     1829 2023-03-14 09:33:55.000000 smartwheel-core-0.0.3/src/smartwheel/serialpipe/keyboard.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     1844 2023-04-15 10:36:09.000000 smartwheel-core-0.0.3/src/smartwheel/serialpipe/serial.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)    23435 2023-04-15 11:25:21.000000 smartwheel-core-0.0.3/src/smartwheel/settings.py
+drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 06:57:06.568903 smartwheel-core-0.0.3/src/smartwheel/settings_handlers/
+-rw-r--r--   0 fitz      (1000) fitz      (1000)        0 2023-01-28 07:05:00.000000 smartwheel-core-0.0.3/src/smartwheel/settings_handlers/__init__.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)    12276 2023-04-14 15:19:42.000000 smartwheel-core-0.0.3/src/smartwheel/settings_handlers/actions.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     2135 2023-03-13 07:05:07.000000 smartwheel-core-0.0.3/src/smartwheel/settings_handlers/base.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     7820 2023-03-20 06:26:26.000000 smartwheel-core-0.0.3/src/smartwheel/settings_handlers/basic.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)       84 2023-03-21 09:13:23.000000 smartwheel-core-0.0.3/src/smartwheel/settings_handlers/config_defaults.json
+-rw-r--r--   0 fitz      (1000) fitz      (1000)    15523 2023-04-14 15:40:07.000000 smartwheel-core-0.0.3/src/smartwheel/settings_handlers/modules.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     5565 2023-03-20 06:26:26.000000 smartwheel-core-0.0.3/src/smartwheel/settings_handlers/preset.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     7846 2023-04-14 15:40:07.000000 smartwheel-core-0.0.3/src/smartwheel/settings_handlers/serial.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     3961 2023-04-14 15:40:07.000000 smartwheel-core-0.0.3/src/smartwheel/settings_handlers/ui.py
+drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 06:57:06.569903 smartwheel-core-0.0.3/src/smartwheel/settings_registry/
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     4261 2023-03-21 10:12:12.000000 smartwheel-core-0.0.3/src/smartwheel/settings_registry/appearance.json
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      492 2023-03-31 18:58:45.000000 smartwheel-core-0.0.3/src/smartwheel/settings_registry/config_defaults.json
+drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 06:57:06.569903 smartwheel-core-0.0.3/src/smartwheel/settings_registry/external/
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      700 2023-04-15 09:06:54.000000 smartwheel-core-0.0.3/src/smartwheel/settings_registry/external/contour.json
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      448 2023-03-10 16:00:47.000000 smartwheel-core-0.0.3/src/smartwheel/settings_registry/external/pattern.json
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      758 2023-03-21 08:32:03.000000 smartwheel-core-0.0.3/src/smartwheel/settings_registry/external/serialmodule.json
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      854 2023-03-31 18:58:45.000000 smartwheel-core-0.0.3/src/smartwheel/settings_registry/external/ui_media.json
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     1165 2023-03-14 08:32:47.000000 smartwheel-core-0.0.3/src/smartwheel/settings_registry/general.json
+-rw-r--r--   0 fitz      (1000) fitz      (1000)       97 2023-03-20 06:30:56.000000 smartwheel-core-0.0.3/src/smartwheel/settings_registry/serial.json
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      169 2023-03-21 10:46:26.000000 smartwheel-core-0.0.3/src/smartwheel/settings_registry/uimodules.json
+-rw-r--r--   0 fitz      (1000) fitz      (1000)       20 2023-04-15 10:14:23.000000 smartwheel-core-0.0.3/src/smartwheel/status.json
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      590 2023-03-08 19:13:53.000000 smartwheel-core-0.0.3/src/smartwheel/tools.py
+drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 06:57:06.570902 smartwheel-core-0.0.3/src/smartwheel/ui/
+-rw-r--r--   0 fitz      (1000) fitz      (1000)        0 2022-05-16 11:10:38.000000 smartwheel-core-0.0.3/src/smartwheel/ui/__init__.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      245 2023-03-13 09:01:47.000000 smartwheel-core-0.0.3/src/smartwheel/ui/base.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     3674 2023-03-14 09:32:38.000000 smartwheel-core-0.0.3/src/smartwheel/ui/files.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      767 2023-03-14 11:05:52.000000 smartwheel-core-0.0.3/src/smartwheel/ui/folder.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)    11410 2023-03-14 09:32:57.000000 smartwheel-core-0.0.3/src/smartwheel/ui/hue.py
+drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 06:57:06.571903 smartwheel-core-0.0.3/src/smartwheel/ui/internal/
+-rw-r--r--   0 fitz      (1000) fitz      (1000)        0 2022-10-15 10:15:43.000000 smartwheel-core-0.0.3/src/smartwheel/ui/internal/__init__.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      301 2023-03-07 15:47:03.000000 smartwheel-core-0.0.3/src/smartwheel/ui/internal/baseinternal.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      410 2023-03-14 11:05:52.000000 smartwheel-core-0.0.3/src/smartwheel/ui/internal/krita_api.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     2566 2023-03-14 11:05:52.000000 smartwheel-core-0.0.3/src/smartwheel/ui/internal/krita_server.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     6126 2023-03-31 18:58:45.000000 smartwheel-core-0.0.3/src/smartwheel/ui/media.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)    20641 2023-03-21 09:07:45.000000 smartwheel-core-0.0.3/src/smartwheel/ui/wheel.py
+drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 06:57:06.572903 smartwheel-core-0.0.3/src/smartwheel_core.egg-info/
+-rw-r--r--   0 fitz      (1000) fitz      (1000)    45385 2023-04-17 06:57:06.000000 smartwheel-core-0.0.3/src/smartwheel_core.egg-info/PKG-INFO
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     4104 2023-04-17 06:57:06.000000 smartwheel-core-0.0.3/src/smartwheel_core.egg-info/SOURCES.txt
+-rw-r--r--   0 fitz      (1000) fitz      (1000)        1 2023-04-17 06:57:06.000000 smartwheel-core-0.0.3/src/smartwheel_core.egg-info/dependency_links.txt
+-rw-r--r--   0 fitz      (1000) fitz      (1000)       57 2023-04-17 06:57:06.000000 smartwheel-core-0.0.3/src/smartwheel_core.egg-info/entry_points.txt
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      129 2023-04-17 06:57:06.000000 smartwheel-core-0.0.3/src/smartwheel_core.egg-info/requires.txt
+-rw-r--r--   0 fitz      (1000) fitz      (1000)       11 2023-04-17 06:57:06.000000 smartwheel-core-0.0.3/src/smartwheel_core.egg-info/top_level.txt
```

### Comparing `smartwheel-core-0.0.2/LICENSE` & `smartwheel-core-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.2/PKG-INFO` & `smartwheel-core-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartwheel-core
-Version: 0.0.2
+Version: 0.0.3
 Summary: Keyboard knob/dial controller with a ton of features
 Author-email: enaix <enaix@protonmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -686,15 +686,15 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 ![smartwheel-core](/extra/render1.jpg)
 
-# Smartwheel Core
+![smartwheel-core logo](/extra/logo.png)
 
 A powerful keyboard knob controller with GUI
 
 ![smartwheel-core ui](/extra/banner.png)
 
 ## Why do I need it?
 
@@ -714,28 +714,38 @@
 
 #### Theming
 
 Smartwheel is fully customizable (you can even create any keybinds if you want)
 
 ## Installation
 
+You may install the prebuilt stable version from the releases.
+
+#### Development build
+
 Make sure that Python 3 is installed
 
 #### Stable version
 
 `pip3 install smartwheel-core`
 
-#### Development build
+#### From Github
 
 `git clone https://github.com/enaix/smartwheel-core.git`
 
 `cd smartwheel-core`
 
 `pip3 install .`
 
+#### Compilation
+
+Nuitka now supports only Python <= 3.10
+
+`./build.sh` or `.\build.bat`
+
 ## We need your help!
 
 I've started working on this project a while ago, but it turned out that it's too big: it won't be possible to finish it without your help. However, it's much easier to implement features one-by-one: you only need basic Python3 (and sometimes PyQt6) knowledge. If you believe in this project and want to contribute, please DM me. Even small fixes, ideas or suggestions are very important.
 
 ## Documentation
 
 Docs are available at readthedocs: https://smartwheel-core.readthedocs.io/en/latest/
@@ -746,35 +756,38 @@
 - [x] Documentation (in progress)
 - [ ] Examples (in progress)
 - [x] Initial encoders support (Linux)
 - [ ] Refactor api
   - [X] Move to PyQt6
   - [X] Add colorable icons
   - [X] Add modules background processes
+  - [ ] Rewrite serial input with new api
+  - [ ] Add media fetching on Windows
   - [ ] Add key combos
   - [ ] Finish folders support
 - [ ] Settings menu (in progress)
   - [X] Basic stuff
   - [X] Custom handlers support (Almost)
   - [X] Saving
   - [X] Theme presets
   - [X] Add color picker
-  - [ ] Better overlays editor
-  - [ ] Actions editor
-  - [ ] Modules import (.zip)
+  - [X] Actions editor
+  - [ ] Sections editor
+  - [ ] Add unified input editor (new input api)
+  - [ ] Better overlays editor (?)
+  - [ ] Modules import (.zip) (?)
 - [ ] Wheel hiding
   - [ ] Hide after timeout
   - [ ] Hide after losing window focus
 - [ ] Packaging
-  - [ ] Configure setup.py
+  - [X] Configure setup.py
   - [ ] Add auto update feature
   - [ ] Hire core doctor!
 - [ ] Windows support
   - [ ] (Platform) Replace AF_UNIX socket with network socket
-  - [ ] (Platform) Replace pynput with winapi
 - [ ] Add fancy blur (?)
 - [ ] Mac support (?)
 
 ## Features progress
 
 - [x] Base structure (Plugins manager)
 - [x] Action engine
@@ -800,16 +813,20 @@
   - [ ] Canvas rotate/scale
   - [ ] Brush
   - [ ] ...
 - [ ] Photoshop integration (?)
 
 ## DIY knob
 
-If you don't have a standalone dial, you may 3D print one: there is a Freecad model in `pad` folder. Sadly, some components don't fit, but I don't have time to fix it right now. DM me if you need the fixed case model.
+If you don't have a standalone dial, you may 3D print one! 
 
-Upd: going to properly remodel it in F360 in the future
+### [smartwheel pad](https://github.com/enaix/smartwheel-pad-mk1)
 
 ## Gallery
 
 Short video (sorry for the poor quality): ![smartwheel.mp4](https://github.com/enaix/smartwheel-core/raw/master/extra/smartwheel.mp4)
 
 Update: added UI overlays ![smartwheel2.mp4](https://github.com/enaix/smartwheel-core/raw/master/extra/simplescreenrecorder-2022-10-10_12.54.42.mp4)
+
+## Resources
+
+Ionicons icon set https://github.com/ionic-team/ionicons
```

### Comparing `smartwheel-core-0.0.2/README.md` & `smartwheel-core-0.0.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ![smartwheel-core](/extra/render1.jpg)
 
-# Smartwheel Core
+![smartwheel-core logo](/extra/logo.png)
 
 A powerful keyboard knob controller with GUI
 
 ![smartwheel-core ui](/extra/banner.png)
 
 ## Why do I need it?
 
@@ -24,28 +24,38 @@
 
 #### Theming
 
 Smartwheel is fully customizable (you can even create any keybinds if you want)
 
 ## Installation
 
+You may install the prebuilt stable version from the releases.
+
+#### Development build
+
 Make sure that Python 3 is installed
 
 #### Stable version
 
 `pip3 install smartwheel-core`
 
-#### Development build
+#### From Github
 
 `git clone https://github.com/enaix/smartwheel-core.git`
 
 `cd smartwheel-core`
 
 `pip3 install .`
 
+#### Compilation
+
+Nuitka now supports only Python <= 3.10
+
+`./build.sh` or `.\build.bat`
+
 ## We need your help!
 
 I've started working on this project a while ago, but it turned out that it's too big: it won't be possible to finish it without your help. However, it's much easier to implement features one-by-one: you only need basic Python3 (and sometimes PyQt6) knowledge. If you believe in this project and want to contribute, please DM me. Even small fixes, ideas or suggestions are very important.
 
 ## Documentation
 
 Docs are available at readthedocs: https://smartwheel-core.readthedocs.io/en/latest/
@@ -56,35 +66,38 @@
 - [x] Documentation (in progress)
 - [ ] Examples (in progress)
 - [x] Initial encoders support (Linux)
 - [ ] Refactor api
   - [X] Move to PyQt6
   - [X] Add colorable icons
   - [X] Add modules background processes
+  - [ ] Rewrite serial input with new api
+  - [ ] Add media fetching on Windows
   - [ ] Add key combos
   - [ ] Finish folders support
 - [ ] Settings menu (in progress)
   - [X] Basic stuff
   - [X] Custom handlers support (Almost)
   - [X] Saving
   - [X] Theme presets
   - [X] Add color picker
-  - [ ] Better overlays editor
-  - [ ] Actions editor
-  - [ ] Modules import (.zip)
+  - [X] Actions editor
+  - [ ] Sections editor
+  - [ ] Add unified input editor (new input api)
+  - [ ] Better overlays editor (?)
+  - [ ] Modules import (.zip) (?)
 - [ ] Wheel hiding
   - [ ] Hide after timeout
   - [ ] Hide after losing window focus
 - [ ] Packaging
-  - [ ] Configure setup.py
+  - [X] Configure setup.py
   - [ ] Add auto update feature
   - [ ] Hire core doctor!
 - [ ] Windows support
   - [ ] (Platform) Replace AF_UNIX socket with network socket
-  - [ ] (Platform) Replace pynput with winapi
 - [ ] Add fancy blur (?)
 - [ ] Mac support (?)
 
 ## Features progress
 
 - [x] Base structure (Plugins manager)
 - [x] Action engine
@@ -110,16 +123,20 @@
   - [ ] Canvas rotate/scale
   - [ ] Brush
   - [ ] ...
 - [ ] Photoshop integration (?)
 
 ## DIY knob
 
-If you don't have a standalone dial, you may 3D print one: there is a Freecad model in `pad` folder. Sadly, some components don't fit, but I don't have time to fix it right now. DM me if you need the fixed case model.
+If you don't have a standalone dial, you may 3D print one! 
 
-Upd: going to properly remodel it in F360 in the future
+### [smartwheel pad](https://github.com/enaix/smartwheel-pad-mk1)
 
 ## Gallery
 
 Short video (sorry for the poor quality): ![smartwheel.mp4](https://github.com/enaix/smartwheel-core/raw/master/extra/smartwheel.mp4)
 
 Update: added UI overlays ![smartwheel2.mp4](https://github.com/enaix/smartwheel-core/raw/master/extra/simplescreenrecorder-2022-10-10_12.54.42.mp4)
+
+## Resources
+
+Ionicons icon set https://github.com/ionic-team/ionicons
```

### Comparing `smartwheel-core-0.0.2/pyproject.toml` & `smartwheel-core-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "smartwheel-core"
-version = "0.0.2"
+version = "0.0.3"
 description = "Keyboard knob/dial controller with a ton of features"
 readme = 'README.md'
 authors = [{ name = "enaix", email = "enaix@protonmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
```

### Comparing `smartwheel-core-0.0.2/src/smartwheel/__main__.py` & `smartwheel-core-0.0.3/src/smartwheel/common.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,234 +1,328 @@
-#!/usr/bin/python3
-# -*- coding: utf-8 -*-
-import importlib
 import json
 import logging
 import os
-import sys
-import weakref
+import time
+from enum import auto, IntEnum, StrEnum
 
-import qdarktheme
-from PyQt6 import QtCore
-from PyQt6.QtCore import QEvent, pyqtSlot
-from PyQt6.QtGui import *
-from PyQt6.QtWidgets import (
-    QApplication,
-    QDockWidget,
-    QGraphicsBlurEffect,
-    QMainWindow,
-    QPushButton,
-    QWidget,
-)
+from PyQt6.QtCore import QObject, pyqtSignal, pyqtSlot
 
 from smartwheel import config
-from smartwheel.canvas import RootCanvas
-from smartwheel.settings import SettingsWindow
 
 
-class WConfig(config.Config):
-    def __init__(self, config_file, launch_config):
-        super(WConfig, self).__init__(config_file, varsWhitelist=["serialModulesLoad"])
-
-        if not self.loadConfig():
-            print("Fatal: error loading main config file. Exiting..")
-            os.exit(1)
-
-        self.launch_config = launch_config
-
-        self.processConfig()
-
-    def processConfig(self):
-        self.c_canvas = config.Config(config_dict=self.c["canvas"])
-        c_geometry = self.c["window"]["geometry"]
-        self.c_canvas["width"] = c_geometry[2] - self.c["window"]["padding"] * 2
-        self.c_canvas["height"] = c_geometry[3] - self.c["window"]["padding"] * 2
-        self.c_canvas["cx"] = c_geometry[2] // 2
-        self.c_canvas["cy"] = c_geometry[3] // 2
-        self.c_canvas["corner_x"] = self.c["window"]["padding"]
-        self.c_canvas["corner_y"] = self.c["window"]["padding"]
-
-
-class RootWindow(QMainWindow):
-    def __init__(self, conf):
-        self.app = QApplication(sys.argv)
-        self.app.setStyleSheet(qdarktheme.load_stylesheet())
-        super(RootWindow, self).__init__()
-        self.conf = conf
-        self.rc = None
-        self.kb = None
-        logging.basicConfig(
-            level=getattr(logging, self.conf.c["canvas"]["logging"].upper(), 2)
-        )
-        self.logger = logging.getLogger(__name__)
+class ConfigManager(QObject):
+    """
+    Global class that manages all config files. This module contains an instance of this class, acting as a singleton
+    """
+
+    save = pyqtSignal()
+    updated = pyqtSignal(str)
+    batchUpdate = pyqtSignal(list)
 
-        self.setWindowFlags(QtCore.Qt.WindowType.FramelessWindowHint)
-        self.setAttribute(QtCore.Qt.WidgetAttribute.WA_Hover, True)
-        # self.mainWindow = QMainWindow(self)
-        # self.mainWindow.setWindowFlags(QtCore.Qt.FramelessWindowHint)
-
-        self.setAutoFillBackground(True)
-        self.setAttribute(QtCore.Qt.WidgetAttribute.WA_TranslucentBackground, True)
-        self.setWindowTitle("SmartWHEEL")
-        self.setWindowIcon(QIcon("logo.png"))
-        self.setGeometry(*self.conf.c["window"]["geometry"])
-        self.loadClasses()
-        self.loadSerial()
-        self.initUI()
-
-        self.settings = SettingsWindow(
-            os.path.join(self.conf["basedir"], "settings_registry", "config.json"),
-            weakref.ref(self),
-            weakref.ref(self.conf),
-            self.conf["basedir"],
-        )
-        # self.settings.show()
+    def __init__(self):
+        super(ConfigManager, self).__init__()
+
+    def __new__(cls):
+        """
+        Singleton implementation
+        """
+        if not hasattr(cls, "instance"):
+            cls.instance = super(ConfigManager, cls).__new__(cls)
+        return cls.instance
 
-        self.show()
-        # self.qp = QPainter(self)
+    @pyqtSlot()
+    def saveConfig(self):
+        """
+        Slot function that executes the saving of all Config objects, must be called from settings module
+        """
+        self.save.emit()
 
-    def initUI(self):
-        self.dock = QDockWidget()
-        self.dock.setMaximumWidth(300)
-        self.dock.setMaximumHeight(300)
-        self.settingsButton = QPushButton("Settings", default=False, autoDefault=False)
-        self.settingsButton.setFocusPolicy(QtCore.Qt.FocusPolicy.NoFocus)
-        self.dock.setWidget(self.settingsButton)
-        self.addDockWidget(QtCore.Qt.DockWidgetArea.BottomDockWidgetArea, self.dock)
-        self.dock.hide()
 
-        self.settingsButton.clicked.connect(self.openSettings)
+class AppState(IntEnum):
+    PreStart = 0
+    InternalModulesInit = 1
+    BrushesInit = 2
+    ModulesInit = 3
+    WheelInit = 4
+    ActionsInit = 5
+    SerialInit = 6
+    WindowInit = 7
+    SettingsRegistryInit = 8
+    SettingsHandlersInit = 9
+    SettingsInit = 10
+    PostStart = 11
+    Loaded = 12
+
+
+class SignalWrapper(QObject):
+    """
+    Wrapper class that contains unique signal
+    """
+
+    signal = pyqtSignal()
+
+
+class ApplicationManager(QObject):
+    """
+    Global class that reports application startup status
+
+    Emits global stateChanged(state) signal and individual self.<state>.signal signals
+    """
+
+    state = AppState.PreStart
+    stateChanged = pyqtSignal(int)
+    # startupSignals = [pyqtSignal() for _ in AppState]
 
-        self.installEventFilter(self)
+    def __init__(self):
+        super(ApplicationManager, self).__init__()
+        self.logger = logging.getLogger(__name__)
 
-        # self.drawBlur()
+        for i in AppState:
+            setattr(self, i.name, SignalWrapper())
+        self.Loaded.signal.connect(self.loadComplete)
 
-    @pyqtSlot()
-    def openSettings(self):
-        self.settings.show()
+        self.stage_time = time.time_ns()
+        self.total_time = self.stage_time
+
+    def __new__(cls):
+        """
+        Singleton implementation
+        """
+        if not hasattr(cls, "instance"):
+            cls.instance = super(ApplicationManager, cls).__new__(cls)
+        return cls.instance
+
+    def updateState(self, state):
+        """
+        Set current startup state
 
-    def eventFilter(self, obj, event):
-        if event.type() == QEvent.Type.HoverEnter:
-            self.dock.show()
-        elif event.type() == QEvent.Type.HoverLeave:
-            self.dock.hide()
-        return super(RootWindow, self).eventFilter(obj, event)
-
-    def drawBlur(self):
-        self.blur_widget = QWidget(self)
-        self.blur_widget.setGeometry(0, 0, *self.conf.c["window"]["geometry"][2:])
-        self.blur_widget.setStyleSheet(
-            "border-radius: {}px;\
-                                       border: 0px solid white;\
-                                       background-color: rgba(0, 0, 0, 0.5);".format(
-                self.conf.c["window"]["geometry"][2] / 6
-            )
+        Parameters
+        ==========
+        state
+            AppState.<state> enum
+        """
+        self.state = state
+        self.stateChanged.emit(self.state)
+        getattr(self, self.state.name).signal.emit()
+
+        if self.state == 0:
+            return
+        new_time = time.time_ns()
+        self.logger.info(
+            "Init: "
+            + AppState(self.state - 1).name
+            + " took "
+            + str((new_time - self.stage_time) // 1000000)
+            + " ms"
         )
-        # self.blur_widget.
-        self.blur_filter = QGraphicsBlurEffect()
-        self.blur_filter.setBlurRadius(15)
-        os.system(
-            "xprop -f _KDE_NET_WM_BLUR_BEHIND_REGION 32c -set _KDE_NET_WM_BLUR_BEHIND_REGION 0 -id "
-            + str(int(self.winId()))
+        self.stage_time = new_time
+
+    @pyqtSlot()
+    def loadComplete(self):
+        final_time = (time.time_ns() - self.total_time) // 1000000
+        self.logger.info(
+            "Init: load complete. Total load time is " + str(final_time) + " ms"
         )
-        # self.blur_widget.setGraphicsEffect(self.blur_filter)
-        self.blur_widget.show()
 
-    def paintEvent(self, event):
-        self.qp = QPainter(self)
-        self.qp.setRenderHint(QPainter.RenderHint.Antialiasing)
-        # self.qp.begin(self)
-        self.draw()
-        self.qp.end()
 
-    def keyPressEvent(self, event):
+class StartupMode(StrEnum):
+    Normal = auto()
+    Update = auto()
+    PostUpdate = auto()
+    Defaults = auto()
+    PostDefaults = auto()
+
+
+class Doctor(QObject):
+    """
+    Medic! This class handles errors and startup modes
+    """
+    def __init__(self):
+        super(Doctor, self).__init__()
+        self.startupMode = StartupMode.Normal
+        self.file = None
+        self.logger = logging.getLogger(__name__)
+
+    def saveStatus(self):
+        """
+        Save current startup status to the file
         """
-        Read keypresses from Qt and pass them to serialpipe
+        if self.startupMode == StartupMode.Normal:
+            if os.path.exists(self.file):
+                os.remove(self.file)
+                return
+        else:
+            status = {"startupMode": self.startupMode.value, "update": False}
+            with open(self.file, "w") as f:
+                json.dump(status, f, indent=4)
+
+    def loadStatus(self, file):
+        """
+        Load previous startup status from file
+
+        Parameters
+        ==========
+        file
+            Input filename
         """
-        if self.serialModules.get("serialpipe.keyboard") is None:  # not initialized yet
+        self.file = file
+        if not os.path.exists(file):
             return
 
-        self.serialModules["serialpipe.keyboard"].handleKeypress(event)
+        try:
+            with open(file, "r") as f:
+                status = json.load(f)
+        except BaseException:
+            self.logger.error("Could not load previous startup status: file corruption. Merging defaults..")
+            self.startupMode = StartupMode.Update
+            return
+
+        if status.get("update", False):
+            self.startupMode = StartupMode.Update
+            self.logger.warning("Note: the app has been updated. Merging the defaults")
+
+        if status.get("startupMode") is not None:
+            try:
+                appStatus = StartupMode(status["startupMode"])
+            except BaseException:
+                self.logger.warning("Could not decode previous startup mode")
+                appStatus = StartupMode.Normal
+            
+            if appStatus == StartupMode.Update:
+                self.startupMode = StartupMode.PostUpdate
+            elif appStatus == StartupMode.Defaults:
+                self.startupMode = StartupMode.PostDefaults
 
-    def keyPressEventLegacy(self, event):
+    def __new__(cls):
         """
-        Old keypress event, dead code
+        Singleton implementation
         """
-        if event.key() == QtCore.Qt.Key_W:
-            self.conf.c["canvas"]["modules"][0]["class"].processKey(True)
-        elif event.key() == QtCore.Qt.Key_A:
-            self.conf.c["canvas"]["modules"][0]["class"].processKey(False)
-        elif event.key() == QtCore.Qt.Key_Up:
-            self.rc.ae.action("scrollUp")
-        elif event.key() == QtCore.Qt.Key_Down:
-            self.rc.ae.action("scrollDown")
-        elif event.key() == QtCore.Qt.Key_Return:
-            self.rc.ae.action("keyAction1")
-        elif event.key() == QtCore.Qt.Key_Q:
-            self.hide()
-            QtCore.QTimer.singleShot(1000, self.show)  # Hide example
-        elif event.key() == QtCore.Qt.Key_Escape:
-            sys.exit(0)
-        self.update()
-
-    def loadSerial(self):
-        """
-        Init main serial connections
-        """
-        # TODO add serial.tools.miniterm in settings
-
-        self.serialModules = {}
-        self.serialModulesNames = []
-
-        for i in self.conf.c["canvas"]["serialModulesLoad"]:
-            mod_name = self.conf.c["canvas"]["serialModules"][i]["name"]
-            mod = importlib.import_module("smartwheel." + mod_name)
+        if not hasattr(cls, "instance"):
+            cls.instance = super(Doctor, cls).__new__(cls)
+        return cls.instance
 
-            try:
-                cls = mod.SConn(
-                    os.path.join(
-                        self.conf["config_dir"],
-                        self.conf.c["canvas"]["serialModules"][i]["config"],
-                    ),
-                    self.rc.ae.callAction,
-                )
-                cls.start()
-                self.serialModules[mod_name] = cls
-                self.serialModulesNames.append(mod_name)
-            except BaseException as e:
-                self.logger.error("Failed to load " + mod_name + ": ", e)
-
-    def loadClasses(self):
-        self.rc = RootCanvas(
-            self.conf.c_canvas, self.conf.launch_config["config_dir"], self.update
-        )
 
-        QGuiApplication.instance().aboutToQuit.connect(self.rc.killThreads)
+class DefaultsManager(QObject):
+    """
+    Global class that manages defaults for config files. Is a singleton
+    """
+
+    def __init__(self):
+        super(DefaultsManager, self).__init__()
+
+    def postInit(self, config_dir, defaults_config_dir):
+        """
+        Post-initialize manager
+
+        Parameters
+        ==========
+        config_dir
+            Common configuration file dir
+        """
+        self.config_dir = config_dir
+        self.defaults_config_dir = defaults_config_dir
+
+    def __new__(cls):
+        """
+        Singleton implementation
+        """
+        if not hasattr(cls, "instance"):
+            cls.instance = super(DefaultsManager, cls).__new__(cls)
+        return cls.instance
 
-    def draw(self):
-        self.rc.draw(self.qp)
 
+class CacheManager(QObject):
+    """
+    Global class that manages cache access. Not inteded to be called from other threads
+    """
 
-def main():
-    dirpath = os.path.dirname(os.path.realpath(__file__))
+    def __init__(self):
+        super(CacheManager, self).__init__()
 
-    if not os.path.exists(dirpath):
-        print(
-            "Please check that configuration files are present in the installation directory"
+    def __new__(cls):
+        """
+        Singleton implementation
+        """
+        if not hasattr(cls, "instance"):
+            cls.instance = super(CacheManager, cls).__new__(cls)
+        return cls.instance
+
+    def initManager(self, conf):
+        self.conf = conf
+        self.conf["cacheDir"] = os.path.join(
+            os.path.dirname(os.path.realpath(__file__)), self.conf["cacheDir"]
         )
 
-    with open(os.path.join(dirpath, "launch.json"), "r") as f:
-        launch_config = json.load(f)
+        if not os.path.exists(self.conf["cacheDir"]):
+            os.mkdir(self.conf["cacheDir"])
 
-    launch_config["config_dir"] = os.path.join(dirpath, launch_config["config_dir"])
+    def load(self, app_name, filename):
+        """
+        Load cache file path and config (optional) from cache. Returns (True, filepath, conf) if found
+
+        Parameters
+        ==========
+        app_name
+            Application name, must be unique
+        filename
+            File to load
+        """
+        if self.conf is None:
+            print("Cache manager is not initialized")
+            return False, None, None
 
-    main_conf_path = os.path.join(launch_config["config_dir"], "config.json")
-    conf = WConfig(main_conf_path, launch_config)
-    conf["config_dir"] = launch_config["config_dir"]
-    conf["basedir"] = dirpath
-    conf.c_canvas["basedir"] = conf["basedir"]
-    root = RootWindow(conf)
-    sys.exit(root.app.exec())
+        appdir = os.path.join(self.conf["cacheDir"], app_name)
+        if not os.path.exists(appdir):
+            os.mkdir(appdir)
 
+        cachepath = os.path.join(appdir, filename)
+        confpath = os.path.join(appdir, filename.split(".")[0] + ".json")
+        cacheconf = None
 
-if __name__ == "__main__":
-    main()
+        if not os.path.exists(cachepath):
+            return False, None, None
+
+        if os.path.exists(confpath):
+            with open(confpath, "r") as f:
+                cacheconf = json.load(f)
+
+        return True, cachepath, cacheconf
+
+    def save(self, app_name, filename, conf=None):
+        """
+        Save to cache. Returns cache filepath to save manually. Note that config object is saved and loaded automatically
+
+        Parameters
+        ==========
+        app_name
+            Application name, must be unique
+        filename
+            File to save
+        conf
+            (Optional) Cache metadata
+        """
+        if self.conf is None:
+            print("Cache manager is not initialized")
+            return None
+
+        appdir = os.path.join(self.conf["cacheDir"], app_name)
+        if not os.path.exists(appdir):
+            os.mkdir(appdir)
+
+        cachepath = os.path.join(appdir, filename)
+        confpath = os.path.join(appdir, filename.split(".")[0] + ".json")
+
+        if conf is not None:
+            with open(confpath, "w") as f:
+                if type(conf) == dict:
+                    json.dump(conf, f)
+                else:
+                    json.dump(conf.c, f)
+
+        return cachepath
+
+
+config_manager = ConfigManager()
+defaults_manager = DefaultsManager()
+app_manager = ApplicationManager()
+cache_manager = CacheManager()
+doctor = Doctor()
```

### Comparing `smartwheel-core-0.0.2/src/smartwheel/actionengine.py` & `smartwheel-core-0.0.3/src/smartwheel/actionengine.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         Parameters
         ----------
         config_file
             Filename
 
         """
         self.conf = config.Config(
-            config_file, self.logger, varsWhitelist=["commandBind"]
+            config_file=config_file, logger=self.logger, varsWhitelist=["commandBind"]
         )
         self.conf.loadConfig()
 
     def importActions(self):
         """
         Import actions from `actions` folder
         """
```

### Comparing `smartwheel-core-0.0.2/src/smartwheel/actions/keypress.py` & `smartwheel-core-0.0.3/src/smartwheel/actions/keypress.py`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.2/src/smartwheel/actions/wheel/wheel.py` & `smartwheel-core-0.0.3/src/smartwheel/actions/wheel/wheel.py`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.2/src/smartwheel/backgrounds/basic.py` & `smartwheel-core-0.0.3/src/smartwheel/backgrounds/basic.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,18 +27,19 @@
         }
 
         self.draw()
 
     def draw(self):
         self.setColor(QColor(self.conf["wheelTextureColor"]))
 
+        tf = QTransform().fromScale(
+            self.conf["patternScale"], self.conf["patternScale"]
+        )
+        self.setTransform(tf)
+
         if self.pattern_map.get(self.conf["patternType"]) is not None:
             self.setStyle(self.pattern_map[self.conf["patternType"]])
         else:
             return
 
-        tf = QTransform()
-        tf.scale(self.conf["patternScale"], self.conf["patternScale"])
-        self.setTransform(tf)
-
 
 brushes = {"pattern": PatternBackground}
```

### Comparing `smartwheel-core-0.0.2/src/smartwheel/backgrounds/contour.py` & `smartwheel-core-0.0.3/src/smartwheel/backgrounds/contour.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,16 +129,15 @@
 
         for p in params:
             if not self.conf.get(p) == conf.get(p):
                 return False
         return True
 
     def updatePixmap(self):
-        pix = self.genContour()
-        self.setTexture(pix)
+        self.setTexture(self.genContour())
 
     def loadPixmap(self):
         if self.conf["useCache"] and not self.conf["randomSeed"]:
             ok, filepath, conf = common.cache_manager.load(
                 "background_contour", "contour1.png"
             )
             if ok and self.checkCache(conf):
```

### Comparing `smartwheel-core-0.0.2/src/smartwheel/cache/background_contour/contour1.png` & `smartwheel-core-0.0.3/src/smartwheel/cache/background_contour/contour1.png`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.2/src/smartwheel/canvas.py` & `smartwheel-core-0.0.3/src/smartwheel/canvas.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,18 +37,19 @@
         self.update_func = update_func
         self.logger = logging.getLogger(__name__)
         self.loadCommonConf()
         self.processCommonConfig()
         # TODO add try catch everywhere
         self.initCacheDir()
         self.loadInternalModules()
-        self.loadBrushes()
         self.startInternalModules()
+        self.loadBrushes()
         self.pool = QThreadPool.globalInstance()
         self.threads = []
+        common.app_manager.updateState(common.AppState.ModulesInit)
         self.wheel_modules = self.loadSections(self.conf["wheelModules"])
         self.cur_wheel_modules = self.wheel_modules
         if self.wheel_modules == 1:
             raise KeyError
         self.loadModules()
         self.tick = 0
         self.loadActionEngine()
@@ -57,32 +58,33 @@
         self.exec_window = 0
         self.exec_times = queue.Queue()
 
         self.startThreads()
 
     def loadCommonConf(self):
         self.common_config = config.Config(
-            os.path.join(self.config_dir, self.conf["commonConfig"]), self.logger
+            os.path.join(self.config_dir, self.conf["commonConfig"]), logger=self.logger
         )
         if not self.common_config.loadConfig():
             self.logger.error("Could not find common config file. Exiting..")
             os._exit(1)
 
         self.common_config["iconsFolder"] = os.path.join(
             self.conf["basedir"], self.common_config["iconsFolder"]
         )
         self.updateIconCache()
 
     def loadModules(self):
         """
-        Read module classes from `modules` config
+        Read main module classes from `modules` config
         """
-        for i in self.conf["modulesLoad"]:
-            self.conf["modules"][i]["class"] = self.importModule(
-                self.conf["modules"][i]
+        common.app_manager.updateState(common.AppState.WheelInit)
+        if 0 in self.conf["modulesLoad"]:
+            self.conf["modules"][0]["class"] = self.importModule(
+                self.conf["modules"][0]
             )
 
     def importModule(self, meta):
         """
         Import a single module class
 
         Parameters
@@ -129,32 +131,37 @@
                 mod = MDict(mod_dict)
             if parent_mod is not None:
                 mod["parent"] = weakref.ref(parent_mod)
             # elif mod is None:
             #    print("Error importing module ", mod["name"], ": No such module. Aborting...",sep="")
             #    return 1
             mod_class = self.loadWheelModule(mod)
-            if i["name"] == "ui.folder":
+            if mod_class is not None and i["name"] == "ui.folder":
                 mod_class["class"].wrapper_pointer = weakref.ref(mod_class)
             mods.append(mod_class)
         return mods
 
     def initCacheDir(self):
         common.cache_manager.initManager(self.conf)
 
     def loadBrushes(self):
+        common.app_manager.updateState(common.AppState.BrushesInit)
         b_config = os.path.join(
             self.conf["basedir"], self.conf["brushes_dir"], "config.json"
         )
-        if not os.path.exists(b_config):
-            self.logger.error("Missing " + b_config + " file")
-            os._exit(1)
+        b_defaults = os.path.join(
+            self.conf["basedir"], self.conf["brushes_dir"], "config_defaults.json"
+        )
 
-        with open(b_config, "r") as f:
-            self.brushes_conf = json.load(f)
+        self.brushes_conf = config.Config(
+            config_file=b_config, default_config_file=b_defaults, disableSaving=True
+        )
+        ok = self.brushes_conf.loadConfig()
+        if not ok:
+            os._exit(1)
 
         self.brushes = {}
         self.conf["brush_configs"] = {}
 
         for mod_name in self.brushes_conf["brushes_modules"]:
             brush = importlib.import_module(
                 "smartwheel." + self.conf["brushes_dir"] + "." + mod_name
@@ -163,15 +170,15 @@
             for k in b_dict:
                 if self.brushes.get(k) is not None:
                     self.logger.warning("Brush " + k + " is defined twice. Overriding")
 
                 self.conf["brush_configs"][k] = config.Config(
                     os.path.join(
                         self.conf["basedir"],
-                        self.conf["brushes_dir"],
+                        self.config_dir,
                         self.brushes_conf["brushes_config_dir"],
                         self.brushes_conf["brushes_config"][k],
                     )
                 )
                 self.conf["brush_configs"][k].loadConfig()
 
                 self.brushes[k] = b_dict[k](
@@ -192,14 +199,20 @@
             self.common_config["wheelWidth"] = self.conf["width"] // 4
         self.common_config["configDir"] = self.config_dir
 
         # Merging configs in order to make settings editable on-the-fly
         merge_dicts(self.conf, self.common_config)
 
     def loadWheelModule(self, module):
+        for i, key in enumerate(self.conf["modules"]):
+            if module["name"] == key["name"]:
+                if not i in self.conf["modulesLoad"]:
+                    module["class"] = None
+                    return module
+
         mod = importlib.import_module("smartwheel." + module["name"])
         if module.get("config", None) is not None:
             ui = mod.UIElem(os.path.join(self.config_dir, module["config"]), self.conf)
 
             if hasattr(ui, "updateSignal"):
                 ui.updateSignal.connect(self.updateCanvas)
 
@@ -238,14 +251,15 @@
             # return None
         else:
             self.cur_wheel_modules = caller["modules"]
             # return caller["modules"]
         self.conf["modules"][0]["class"].reloadModules(self.cur_wheel_modules)
 
     def loadInternalModules(self):
+        common.app_manager.updateState(common.AppState.InternalModulesInit)
         self.conf["internal"] = {}
         for i in self.conf["internalModulesLoad"]:
             mod = self.conf["internalModules"][i]
             if mod.get("config") is not None:
                 cnf = os.path.join(self.config_dir, mod["config"])
             else:
                 cnf = None
@@ -270,37 +284,41 @@
     def getWheelModule(self):
         i = self.conf["modules"][0]["class"].getCurModule()
         if i >= len(self.cur_wheel_modules):
             return None
         return self.cur_wheel_modules[i]
 
     def loadActionEngine(self):
+        common.app_manager.updateState(common.AppState.ActionsInit)
         self.ae = ActionEngine(
             self.wheel_modules,
             os.path.join(self.config_dir, self.conf["actionEngineConfig"]),
             self.conf,
         )
         self.ae.current_module_list_getter = self.getCurModList
         self.ae.current_module_getter = self.conf["modules"][0]["class"].getCurModule
         self.ae.canvas = weakref.ref(self)
         self.ae.wheel = weakref.ref(self.conf["modules"][0]["class"])
 
     def updateIconCache(self):
         """
         Will only be called if icon color has been changed
         """
-        res1 = gui_tools.icon_managers["wheel"].setIconColor(
-            self.common_config["wheelIconColor"]
-        )
-        return (
-            gui_tools.icon_managers["sections"].setIconColor(
-                self.common_config["sectionsIconColor"]
-            )
-            or res1
-        )
+        colors = [
+            self.common_config["wheelIconColor"],
+            self.common_config["sectionsIconColor"],
+            self.conf["toolsIconColor"],
+        ]
+        keys = ["wheel", "sections", "tools"]
+
+        res = False
+
+        for i in range(len(keys)):
+            res = gui_tools.icon_managers[keys[i]].setIconColor(colors[i]) or res
+        return res
 
     def calculateSmoothFPS(self, new_time):
         """
         Calculate the average render time out of n frames
 
         Parameters
         ==========
@@ -335,42 +353,44 @@
         Parameters
         ----------
         qp
             QPainter object
         """
         # for i in self.conf["modulesLoad"]:
         #    self.conf["modules"][i]["class"].draw(qp)
+        if self.conf["stabilizeFPS"]:
+            sleep_time = max(1 / self.conf["fps"] - self.exec_time, 0)
+        else:
+            sleep_time = 1 / self.conf["fps"]
+
+        time.sleep(sleep_time)
+
+        start_time = time.time_ns()
+
         self.conf["modules"][0]["class"].draw(qp)  # render wheel
+
+        e_time = (time.time_ns() - start_time) / 1000000000  # seconds
+
+        if self.conf["stabilizeFPS"]:
+            if self.conf["logFPS"]:
+                self.logger.info(
+                    "FPS(AVG): "
+                    + str(round(1 / max(sleep_time + self.exec_time, 0.0000001), 1))
+                )
+            self.calculateSmoothFPS(e_time)
+
+        else:
+            if self.conf["logFPS"]:
+                self.logger.info("FPS: " + str(round(1 / (sleep_time + e_time), 1)))
+
         m = self.getWheelModule()
+        cache = self.updateIconCache()
         if (
             self.conf["modules"][0]["class"].is_anim_running
             or (
                 m is not None
                 and hasattr(m["class"], "is_anim_running")
                 and m["class"].is_anim_running
             )
-            or self.updateIconCache()
+            or cache
         ):
-            if self.conf["stabilizeFPS"]:
-                sleep_time = max(1 / self.conf["fps"] - self.exec_time, 0)
-            else:
-                sleep_time = 1 / self.conf["fps"]
-
-            time.sleep(sleep_time)
-
-            start_time = time.time()
-
-            self.update_func()  # TODO add another update event
-
-            e_time = (time.time() - start_time) * 1000
-
-            if self.conf["stabilizeFPS"]:
-                if self.conf["logFPS"]:
-                    self.logger.info(
-                        "FPS(AVG): "
-                        + str(round(1 / max(sleep_time + self.exec_time, 0.0000001), 1))
-                    )
-                self.calculateSmoothFPS(e_time)
-
-            else:
-                if self.conf["logFPS"]:
-                    self.logger.info("FPS: " + str(round(1 / (sleep_time + e_time), 1)))
+            self.update_func()
```

### Comparing `smartwheel-core-0.0.2/src/smartwheel/config/actionengine.json` & `smartwheel-core-0.0.3/src/smartwheel/defaults/actionengine.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -856,8 +856,8 @@
 00003570: 3a20 226d 6f64 756c 6522 2c0a 2020 2020  : "module",.    
 00003580: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003590: 2020 2020 2263 6865 636b 5374 6174 6522      "checkState"
 000035a0: 3a20 7472 7565 0a20 2020 2020 2020 2020  : true.         
 000035b0: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
 000035c0: 2020 2020 2020 2020 2020 2020 205d 0a20               ]. 
 000035d0: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
-000035e0: 2020 2020 205d 0a20 2020 207d 0a7d            ].    }.}
+000035e0: 2020 2020 205d 0a20 2020 207d 0a7d 0a         ].    }.}.
```

### Comparing `smartwheel-core-0.0.2/src/smartwheel/config/bgkeyboard.json` & `smartwheel-core-0.0.3/src/smartwheel/defaults/serial/bgkeyboard.json`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.2/src/smartwheel/config/config.json` & `smartwheel-core-0.0.3/src/smartwheel/defaults/config.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9622962962962962%*

 * *Differences: {"'canvas'": "{'modules': {0: {'title': 'Wheel', 'description': 'Main wheel module, cannot be "*

 * *             "disabled'}, 1: {'title': 'Media', 'description': 'Control music/volume', 'registry': "*

 * *             "'ui_media'}, 2: {'title': 'Color picker', 'description': 'HSL wheel picker'}}, "*

 * *             "'serialModules': {0: {'handler': 'serialmodule', 'registry': 'serialmodule'}}, "*

 * *             "'modulesLoad': {insert: [(1, 1), (2, 2)]}, 'settingsIcon': 'settings.svg', "*

 * *             "'serialConfigDir': ' […]*

```diff
@@ -11,14 +11,15 @@
         ],
         "actionModulesLoad": [
             0,
             1
         ],
         "brushes_dir": "backgrounds",
         "cacheDir": "cache",
+        "closeIcon": "close.svg",
         "commonConfig": "common.json",
         "fps": 60,
         "fpsFramesSmooth": 10,
         "internalModules": [
             {
                 "config": "internal/krita_server.json",
                 "name": "ui.internal.krita_server"
@@ -32,33 +33,45 @@
             1
         ],
         "logFPS": false,
         "logging": "INFO",
         "modules": [
             {
                 "config": "wheel.json",
-                "name": "ui.wheel"
+                "description": "Main wheel module, cannot be disabled",
+                "name": "ui.wheel",
+                "title": "Wheel"
             },
             {
                 "config": "media.json",
-                "name": "ui.media"
+                "description": "Control music/volume",
+                "name": "ui.media",
+                "registry": "ui_media",
+                "title": "Media"
             },
             {
                 "config": "hue.json",
-                "name": "ui.hue"
+                "description": "HSL wheel picker",
+                "name": "ui.hue",
+                "title": "Color picker"
             }
         ],
         "modulesLoad": [
-            0
+            0,
+            1,
+            2
         ],
+        "serialConfigDir": "serial",
         "serialModules": [
             {
                 "config": "serial.json",
                 "description": "Serial keyboard/encoder",
+                "handler": "serialmodule",
                 "name": "serialpipe.serial",
+                "registry": "serialmodule",
                 "title": "Serial"
             },
             {
                 "config": "keyboard.json",
                 "description": "Basic keyboard input from window",
                 "name": "serialpipe.keyboard",
                 "title": "Simple keyboard"
@@ -70,15 +83,18 @@
                 "title": "Background keyboard"
             }
         ],
         "serialModulesLoad": [
             0,
             2
         ],
+        "settingsIcon": "settings.svg",
         "stabilizeFPS": true,
+        "toolsBackgroundColor": "#ffffff",
+        "toolsIconColor": "#000000",
         "wheelActionModules": [
             {
                 "name": "actions.wheel.module"
             },
             {
                 "name": "actions.wheel.wheel"
             }
```

### Comparing `smartwheel-core-0.0.2/src/smartwheel/config/hue.json` & `smartwheel-core-0.0.3/src/smartwheel/defaults/hue.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.925%*

 * *Differences: {"'icon_path'": "'hue.svg'", 'delete': "['roundIconPath']"}*

```diff
@@ -31,14 +31,13 @@
     "colorDotDarkStrokeColor": "#000000",
     "colorDotLightStrokeColor": "#ffffff",
     "colorDotLightnessThreshold": 100,
     "colorDotStrokeWidth": 2,
     "colorWidgetMaxWidth": 80,
     "colorWidgetPadding": 10,
     "colorWidgetShape": "hybrid",
-    "icon_path": "hue.png",
+    "icon_path": "hue.svg",
     "isHSLPaddingFixed": false,
     "isHSLSelectionWidthFixed": false,
     "isHSLWidthFixed": false,
-    "roundIconPath": "round.png",
     "widthAnimDuration": 100
 }
```

### Comparing `smartwheel-core-0.0.2/src/smartwheel/config/media.json` & `smartwheel-core-0.0.3/src/smartwheel/defaults/media.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.2727272727272727%*

 * *Differences: {"'bottomTextFont'": "'Ubuntu'",*

 * * "'bottomTextSize'": '12',*

 * * "'icon_path'": "'media.svg'",*

 * * "'icons'": "['play.svg', 'pause.svg']",*

 * * "'seekTextFont'": "'Ubuntu'",*

 * * "'seekTextSize'": '14',*

 * * "'textHeaderFont'": "'Ubuntu'",*

 * * "'textHeaderSize'": '14',*

 * * 'delete': "['style']"}*

```diff
@@ -57,25 +57,20 @@
                 "key": "next",
                 "key_class": "media",
                 "repeat": 0,
                 "type": "updown"
             }
         ]
     },
-    "icon_path": "media.png",
+    "bottomTextFont": "Ubuntu",
+    "bottomTextSize": 12,
+    "icon_path": "media.svg",
     "icons": [
-        "play.png",
-        "pause.png"
+        "play.svg",
+        "pause.svg"
     ],
     "mediaFetchSleep": 0.01,
-    "style": {
-        "bottomTextColor": "#cccccc",
-        "bottomTextFont": "Ubuntu",
-        "bottomTextSize": 12,
-        "seekTextColor": "#cccccc",
-        "seekTextFont": "Ubuntu",
-        "seekTextSize": 14,
-        "textHeaderColor": "#ffffff",
-        "textHeaderFont": "Ubuntu",
-        "textHeaderSize": 14
-    }
+    "seekTextFont": "Ubuntu",
+    "seekTextSize": 14,
+    "textHeaderFont": "Ubuntu",
+    "textHeaderSize": 14
 }
```

### Comparing `smartwheel-core-0.0.2/src/smartwheel/config/serial.json` & `smartwheel-core-0.0.3/src/smartwheel/defaults/serial/serial.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -64,8 +64,8 @@
 000003f0: 2020 2020 2020 2020 2020 7b0a 2020 2020            {.    
 00000400: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000410: 2273 7472 696e 6722 3a20 2265 6e63 315f  "string": "enc1_
 00000420: 646f 7562 6c65 636c 6963 6b5f 7363 726f  doubleclick_scro
 00000430: 6c6c 2064 6f77 6e22 0a20 2020 2020 2020  ll down".       
 00000440: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
 00000450: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
-00000460: 207d 0a20 2020 205d 0a7d                  }.    ].}
+00000460: 207d 0a20 2020 205d 0a7d 0a               }.    ].}.
```

### Comparing `smartwheel-core-0.0.2/src/smartwheel/config/wheel.json` & `smartwheel-core-0.0.3/src/smartwheel/defaults/wheel.json`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.2/src/smartwheel/config.py` & `smartwheel-core-0.0.3/src/smartwheel/config.py`

 * *Files 21% similar despite different names*

```diff
@@ -21,51 +21,67 @@
     """
 
     updated = pyqtSignal()
 
     def __init__(
         self,
         config_file=None,
+        default_config_file=None,
         config_dict=None,
         logger=None,
         ignoreNewVars=True,
         varsWhitelist=[],
         varsBlacklist=[],
         updateFunc=None,
+        disableSaving=False,
     ):
         """
         Initialize Config object
         Note: the config file needs to be loaded manually by calling loadConfig()
 
         Parameters
         ==========
         config_file
             (Optional) Path to the configuration file
+        default_config_file
+            (Optional) Path to the default configuration file, `defaults/...` dir if not specified
         config_dict
-            (Optional) Dict containing initial values. Overwritten if config_file is specified.
+            (Optional) Dict containing initial values. Overwritten if config_file is specified
         logger
             logger.Logger instance (recommended, will print to stdout if not given)
         ignoreNewVars
             (Optional) Drop new variables while saving (in order not to write runtime variables to config)
         varsWhitelist
             (Optional) List of keys that override ignoreNewVars option (all new children variables of any depth will be saved)
         varsBlacklist
             (Optional) List of keys that contain runtime variables, new children variables of any depth are ignored
         updateFunc
             (Optional) Update function to call when settings are updated. Use only if signals are not supported
+        disableSaving
+            (Optional) Do not save config file automatically. False by default
         """
         super(Config, self).__init__()
         self.config_file = config_file
+        self.default_config_file = default_config_file
+
+        if self.default_config_file is None and self.config_file is not None:
+            self.default_config_file = self.config_file.replace(
+                common.defaults_manager.config_dir,
+                common.defaults_manager.defaults_config_dir,
+                1,
+            )
+
         # self.c = self.loadConfig()
         self.c = config_dict
         self.logger = logger
         self.ignoreNew = ignoreNewVars
         self.whitelist = varsWhitelist
         self.blacklist = varsBlacklist
         self.updateFunc = updateFunc
+        self.disableSaving = disableSaving
         self.links = []  # Storing source dicts to allow updating the variables
 
         common.config_manager.save.connect(self.saveConfig)
         common.config_manager.updated.connect(self.__updated)
         common.config_manager.batchUpdate.connect(self.__batchUpdate)
 
     def __fetchkey(self, key):
@@ -201,120 +217,166 @@
 
     def items(self):
         """
         Call the builtin dictionary items method
         """
         return self.c.items()
 
-    def loadConfig(self, immediate=False):
+    def createConfig(self):
+        """
+        Create config file and underlying file structure if it does not exist
+
+        Returns True if config has been loaded from defaults
+        """
+        if self.default_config_file is None:
+            return False
+
+        if os.path.exists(self.config_file):
+            return False
+
+        os.makedirs(os.path.dirname(self.config_file), exist_ok=True)
+        ok, defaults = self.loadConfig(
+            immediate=True, override=self.default_config_file
+        )
+        if not ok:
+            return
+
+        self.c = defaults
+
+        with open(self.config_file, "w") as f:
+            json.dump(defaults, f, indent=4)
+
+        return True
+
+    def loadConfig(self, immediate=False, override=None):
         """
         Load the config from file, returns True if it is loaded successfully
 
         Parameters
         ==========
         immediate
             If false (default), the function applies the config and does not return it's copy. True - it returns (bool, dict) without applying it
+        override
+            (Optional) Override config file path with given one
         """
         if self.config_file is None:
             if immediate:
                 return True, self.c
             return True
 
+        config_file = self.config_file
+        if override is not None:
+            config_file = override
+
+        if not override and not immediate:
+            if self.createConfig():
+                return True
+
         try:
-            with open(self.config_file, "r") as f:
+            with open(config_file, "r") as f:
                 if immediate:
                     return True, json.load(f)
                 self.c = json.load(f)
+                if common.doctor.startupMode == common.StartupMode.Update:
+                    self.mergeDefaults()
+                elif common.doctor.startupMode == common.StartupMode.Defaults:
+                    self.loadDefaults()
         except BaseException as e:
             if self.logger is not None:
                 self.logger.error("Could not load config file:")
                 self.logger.error(str(e))
             else:
                 print("Could not load config file:")
                 print(str(e))
 
             if immediate:
                 return False, None
             return False
 
         return True
 
-    def listIter(self, new, old, dropNew=True):
+    def listIter(self, new, old, dropNew=True, preserveOld=False):
         """
         Recursively iterate through the list and update old config value iff it is present in config file
 
         Parameters
         ==========
         new
             New values (saved from the application)
         old
             Old values from the json config file
         dropNew
             (Optional) Drop new variables
+        preserveOld
+            (Optional) Preserve old variables (update only missing)
         """
         if dropNew and not len(new) == len(old):
             return
 
         # We need to unset the old list in order to prevent duplications errors
         if not dropNew and len(new) < len(old):
             for i in range(len(new), len(old)):
                 del old[i]
 
         for i in range(len(new)):
             if i < len(old):
                 if type(new[i]) == type(old[i]):
                     if type(new[i]) == dict:
-                        self.dictIter(new[i], old[i], dropNew)
+                        self.dictIter(new[i], old[i], dropNew, preserveOld)
                     elif type(new[i]) == list:
-                        self.listIter(new[i], old[i], dropNew)
+                        self.listIter(new[i], old[i], dropNew, preserveOld)
                     else:
-                        old[i] = new[i]
+                        if not preserveOld:
+                            old[i] = new[i]
             elif not dropNew:
                 old.append(new[i])
             else:
                 return
 
-    def dictIter(self, new, old, dropNew=True):
+    def dictIter(self, new, old, dropNew=True, preserveOld=False):
         """
         Recursively iterate through the dict and update old config value iff it is present in config file
 
         Parameters
         ==========
         new
             New values (saved from the application)
         old
             Old values from the json config file
         dropNew
             (Optional) Drop new variables
+        preserveOld
+            (Optional) Preserve old variables (update only missing)
         """
         for key, val in new.items():
             if old.get(key) is not None and type(val) == type(old[key]):
                 drop = dropNew
                 if dropNew and key in self.whitelist:
                     drop = False
                 elif not dropNew and key in self.blacklist:
                     drop = True
 
                 if type(val) == dict:
-                    self.dictIter(new[key], old[key], drop)
+                    self.dictIter(new[key], old[key], drop, preserveOld)
                 elif type(val) == list:
-                    self.listIter(val, old[key], drop)
+                    self.listIter(val, old[key], drop, preserveOld)
                 else:
-                    old[key] = val
+                    if not preserveOld:
+                        old[key] = val
                     # print(key)
             elif not dropNew:
                 old[key] = val
 
     @pyqtSlot()
     def saveConfig(self):
         """
         Save the config file
         Note: new variables are dropped by default (we need to purge runtime variables)
         """
-        if self.config_file is None:
+        if self.config_file is None or self.disableSaving:
             return
 
         # We need to drop runtime variables, so we need to load the json file again
         ok, old_values = self.loadConfig(immediate=True)
 
         if not ok:
             if self.logger is not None:
@@ -325,7 +387,49 @@
             return
 
         # recursively iterate over the dictionary
         self.dictIter(self.c, old_values, dropNew=self.ignoreNew)
 
         with open(self.config_file, "w") as f:
             json.dump(old_values, f, indent=4)
+
+    def mergeDefaults(self):
+        """
+        Refresh config file with default variables. Is invoked in case of an update or config error
+        """
+        if self.default_config_file is None or self.config_file is None:
+            return
+
+        ok, defaults = self.loadConfig(immediate=True, override=self.default_config_file)
+
+        if not ok:
+            if self.logger is not None:
+                self.logger.error("Failed to merge defaults")
+            else:
+                print("Failed to merge defaults")
+            return
+
+        # Default refresh strategy
+        self.dictIter(defaults, self.c, dropNew=False, preserveOld=True)
+        self.dictIter(self.c, defaults, dropNew=self.ignoreNew)
+
+        with open(self.config_file, "w") as f:
+            json.dump(defaults, f, indent=4)
+
+    def loadDefaults(self):
+        """
+        Reload config file from defaults
+        """
+        if self.default_config_file is None or self.config_file is None:
+            return
+
+        ok, defaults = self.loadConfig(immediate=True, override=self.default_config_file)
+
+        if not ok:
+            if self.logger is not None:
+                self.logger.error("Failed to merge defaults")
+            else:
+                print("Failed to merge defaults")
+            return
+
+        with open(self.config_file, "w") as f:
+            json.dump(defaults, f, indent=4)
```

### Comparing `smartwheel-core-0.0.2/src/smartwheel/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg` & `smartwheel-core-0.0.3/src/smartwheel/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.2/src/smartwheel/docs/conf.py` & `smartwheel-core-0.0.3/src/smartwheel/docs/conf.py`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.2/src/smartwheel/icons/default/folder.png` & `smartwheel-core-0.0.3/src/smartwheel/icons/default/folder.png`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.2/src/smartwheel/icons/default/hue.png` & `smartwheel-core-0.0.3/src/smartwheel/icons/default/hue_old.png`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.2/src/smartwheel/icons/default/hue.svg` & `smartwheel-core-0.0.3/src/smartwheel/icons/default/hue.svg`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.2/src/smartwheel/icons/default/media.png` & `smartwheel-core-0.0.3/src/smartwheel/icons/default/media.png`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.2/src/smartwheel/icons/default/pause.png` & `smartwheel-core-0.0.3/src/smartwheel/icons/default/pause.png`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.2/src/smartwheel/icons/default/play.png` & `smartwheel-core-0.0.3/src/smartwheel/icons/default/play.png`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.2/src/smartwheel/icons/default/round.png` & `smartwheel-core-0.0.3/src/smartwheel/icons/default/round.png`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.2/src/smartwheel/logo.png` & `smartwheel-core-0.0.3/src/smartwheel/logo.png`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.2/src/smartwheel/presets/appearance/blackout.json` & `smartwheel-core-0.0.3/src/smartwheel/presets/appearance/blackout.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9833333333333334%*

 * *Differences: {"'props'": "{'ui.wheel.overlayCirclesOpacity': 0.5, 'canvas.toolsIconColor': '#ffffff', "*

 * *            "'canvas.toolsBackgroundColor': '#000000'}"}*

```diff
@@ -2,26 +2,28 @@
     "name": "blackout",
     "props": {
         "canvas.brush_configs.contour.backgroundColor": "#ffffff",
         "canvas.brush_configs.contour.generator": "Trigonometric",
         "canvas.brush_configs.contour.seed": 42,
         "canvas.brush_configs.pattern.patternScale": 1.0,
         "canvas.brush_configs.pattern.patternType": "None",
+        "canvas.toolsBackgroundColor": "#000000",
+        "canvas.toolsIconColor": "#ffffff",
         "common.bgWheelColor": "#000000",
         "common.majorTextColor": "#ffffff",
         "common.sectionsIconColor": "#ffffff",
         "common.selectionWheelBG": "#000000",
         "common.selectionWheelFG": "#000000",
         "common.wheelIconColor": "#ffffff",
         "common.wheelTextureColor": "#000000",
         "ui.wheel.backgroundStyle": "pattern",
         "ui.wheel.drawOverlayCircles": true,
         "ui.wheel.drawOverlayRects": false,
         "ui.wheel.overlayCirclesColor": "#2a2a2a",
-        "ui.wheel.overlayCirclesOpacity": 0.2,
+        "ui.wheel.overlayCirclesOpacity": 0.5,
         "ui.wheel.overlayCirclesWidth": 10,
         "ui.wheel.overlayRectsColor": "#262626",
         "ui.wheel.overlayRectsOpacity": 0.2,
         "ui.wheel.overlayRectsWidth": 20,
         "ui.wheel.pointerColor": "#1eff00",
         "ui.wheel.wheelShadowColor": "#000000"
     },
```

### Comparing `smartwheel-core-0.0.2/src/smartwheel/presets/appearance/classic.json` & `smartwheel-core-0.0.3/src/smartwheel/presets/appearance/classic.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9866666666666667%*

 * *Differences: {"'props'": "{'canvas.toolsIconColor': '#ffffff', 'canvas.toolsBackgroundColor': '#161616'}"}*

```diff
@@ -2,14 +2,16 @@
     "name": "classic",
     "props": {
         "canvas.brush_configs.contour.backgroundColor": "#ffffff",
         "canvas.brush_configs.contour.generator": "Trigonometric",
         "canvas.brush_configs.contour.seed": 42,
         "canvas.brush_configs.pattern.patternScale": 1.0,
         "canvas.brush_configs.pattern.patternType": "Diagonal (right)",
+        "canvas.toolsBackgroundColor": "#161616",
+        "canvas.toolsIconColor": "#ffffff",
         "common.bgWheelColor": "#171717",
         "common.majorTextColor": "#ffffff",
         "common.sectionsIconColor": "#ffffff",
         "common.selectionWheelBG": "#171717",
         "common.selectionWheelFG": "#cccccc",
         "common.wheelIconColor": "#ffffff",
         "common.wheelTextureColor": "#404040",
```

### Comparing `smartwheel-core-0.0.2/src/smartwheel/presets/appearance/polar.json` & `smartwheel-core-0.0.3/src/smartwheel/presets/appearance/polar.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9833333333333334%*

 * *Differences: {"'props'": "{'common.bgWheelColor': '#ffffff', 'canvas.toolsIconColor': '#000000', "*

 * *            "'canvas.toolsBackgroundColor': '#ffffff'}"}*

```diff
@@ -2,15 +2,17 @@
     "name": "polar",
     "props": {
         "canvas.brush_configs.contour.backgroundColor": "#ffffff",
         "canvas.brush_configs.contour.generator": "Trigonometric",
         "canvas.brush_configs.contour.seed": 42,
         "canvas.brush_configs.pattern.patternScale": 1.0,
         "canvas.brush_configs.pattern.patternType": "Diagonal (right)",
-        "common.bgWheelColor": "#171717",
+        "canvas.toolsBackgroundColor": "#ffffff",
+        "canvas.toolsIconColor": "#000000",
+        "common.bgWheelColor": "#ffffff",
         "common.majorTextColor": "#000000",
         "common.sectionsIconColor": "#262626",
         "common.selectionWheelBG": "#f0f0f0",
         "common.selectionWheelFG": "#000000",
         "common.wheelIconColor": "#262626",
         "common.wheelTextureColor": "#e2e2e2",
         "ui.wheel.backgroundStyle": "contour",
```

### Comparing `smartwheel-core-0.0.2/src/smartwheel/serialpipe/base.py` & `smartwheel-core-0.0.3/src/smartwheel/serialpipe/base.py`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.2/src/smartwheel/serialpipe/bgkeyboard.py` & `smartwheel-core-0.0.3/src/smartwheel/serialpipe/bgkeyboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         self.logger = logging.getLogger(__name__)
         self.config_file = config_file
         self.call = call_signal
         self.loadConfig()
         self.loadKeys()
 
     def loadConfig(self):
-        self.conf = config.Config(self.config_file, self.logger)
+        self.conf = config.Config(config_file=self.config_file, logger=self.logger)
         self.conf.loadConfig()
 
     def loadKeys(self):
         """
         Initialize dicts of keys to quickly find them
         """
         self.keys = {
```

### Comparing `smartwheel-core-0.0.2/src/smartwheel/serialpipe/keyboard.py` & `smartwheel-core-0.0.3/src/smartwheel/serialpipe/keyboard.py`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.2/src/smartwheel/serialpipe/serial.py` & `smartwheel-core-0.0.3/src/smartwheel/serialpipe/serial.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,15 +15,17 @@
         self.conf = None
         self.config_file = config_file
         self.call = call_signal
         self.logger = logging.getLogger(__name__)
         self.loadConfig()
 
     def loadConfig(self):
-        self.conf = config.Config(self.config_file, self.logger)
+        self.conf = config.Config(
+            config_file=self.config_file, logger=self.logger, varsWhitelist=["binds"]
+        )
         self.conf.loadConfig()
 
     def serialCall(self, string):
         """
         Parse serial call from string
 
         Parameters
```

### Comparing `smartwheel-core-0.0.2/src/smartwheel/settings.py` & `smartwheel-core-0.0.3/src/smartwheel/settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,28 +15,33 @@
     QPushButton,
     QScrollArea,
     QSizePolicy,
     QSpacerItem,
     QTabWidget,
     QVBoxLayout,
     QWidget,
+    QComboBox,
 )
 
-from smartwheel import common
+from smartwheel import common, config
 
 
 class SettingsWindow(QWidget):
-    def __init__(self, config_file, main_class, conf_class, basedir, parent=None):
+    def __init__(
+        self, config_file, defaults_file, main_class, conf_class, basedir, parent=None
+    ):
         """
         Init SettingsWindow
 
         Parameters
         ==========
         config_file
-            Path to settings registry
+            Path to settings registry config
+        defaults_file
+            Path to settings registry default config
         main_class
             Weakref to RootWindow object
         conf_class
             Weakref to WConfig object
         """
         super(SettingsWindow, self).__init__(parent)
         self.setWindowTitle("Settings")
@@ -44,39 +49,50 @@
         self.conf = None
         self.handlers_conf = None
         self.handlers = None
         self.basedir = basedir
         self.settings = {}
         self.external_reg = {}
         self.logger = logging.getLogger(__name__)
-        self.loadConfig(config_file)
+        self.loadConfig(config_file, defaults_file)
         self.setConfigHook(main_class, conf_class)
         self.loadSettingsHandlers(
             os.path.join(self.basedir, self.conf["settings_handlers_dir"])
         )
         self.preset_tabs = {}
+        self.preset_controllers = {}
+        self.presets_index_mapping = {}
         self.conf["presets"] = {}
         self.linked_widgets = {}
         self.presets_queue = LifoQueue()
         self.presets_update_queue = []
         self.isLoaded = False
+        self.externalRegistries = {}
 
         self.initLayout()
 
-    def loadConfig(self, config_file):
+    def loadConfig(self, config_file, defaults_file):
         """
         Import settings registry
 
         Parameters
         ==========
         config_file
             Settings registry config.json file
+        defaults_file
+            Default config file
         """
-        with open(config_file, "r") as f:
-            self.conf = json.load(f)
+        common.app_manager.updateState(common.AppState.SettingsRegistryInit)
+        self.conf = config.Config(
+            config_file=config_file,
+            default_config_file=defaults_file,
+            disableSaving=True,
+        )
+        if not self.conf.loadConfig():
+            os._exit(1)
 
         if self.conf.get("tabs") is not None:
             for i in range(len(self.conf["tabs"])):
                 with open(
                     os.path.join(
                         self.basedir,
                         "settings_registry",
@@ -116,18 +132,19 @@
         self.settings["actionengine"] = main_class().rc.ae.conf
 
         # Parsing serial modules
         self.settings["serial"] = {}
         serial = main_class().serialModules
 
         for name in main_class().serialModulesNames:
+            key = name.split(".")[-1:][0]
             if hasattr(serial[name], "conf"):
-                self.settings["serial"][name] = serial[name].conf
+                self.settings["serial"][key] = serial[name].conf
             else:
-                self.logger.error("serialpipe." + name + " has no conf attribute")
+                self.logger.error("serialpipe." + key + " has no conf attribute")
 
         # Parsing canvas section modules
         self.settings["modules"] = {}
         main_modules = main_class().rc.conf["modules"]
         wheel_modules = main_class().rc.wheel_modules
 
         for i, modules in enumerate([main_modules, wheel_modules]):
@@ -146,21 +163,23 @@
         Init settings handlers from the directory
 
         Parameters
         ==========
         handlers_dir
             Directory containing settings handlers, must contain config.json file
         """
+        common.app_manager.updateState(common.AppState.SettingsHandlersInit)
         s_config = os.path.join(handlers_dir, "config.json")
-        if not os.path.exists(s_config):
+        s_default = os.path.join(handlers_dir, "config_defaults.json")
+        self.handlers_conf = config.Config(
+            config_file=s_config, default_config_file=s_default, disableSaving=True
+        )
+        if not self.handlers_conf.loadConfig():
             self.logger.error("Missing " + s_config + " file")
-            os.exit(1)
-
-        with open(s_config, "r") as f:
-            self.handlers_conf = json.load(f)
+            os._exit(1)
 
         self.handlers = {}
         for mod_name in self.handlers_conf["handlers_modules"]:
             handler = importlib.import_module(
                 "smartwheel." + self.conf["settings_handlers_dir"] + "." + mod_name
             )
             h_dict = handler.handlers
@@ -289,21 +308,25 @@
         if self.settings.get(module) is None:
             self.logger.error("Could not get value: no module " + str(module))
             return
 
         props = prop.split(".")
 
         if self.dictWalk(self.settings[module], props, value, index):
+            name = module + "." + prop
+            if index is not None:
+                name += "." + str(index)
+            self.setCustom(name)
+
             if self.isLoaded:
                 common.config_manager.updated.emit(props[-1:][0])
+                self.main_class().update()
             else:
                 self.presets_update_queue.append(props[-1:][0])
 
-            self.main_class().update()
-
     def savePreset(self, index, name, title, filepath):
         """
         Save the specified preset
 
         Parameters
         ==========
         index
@@ -341,40 +364,54 @@
         Parameters
         ==========
         index
             Settings tab index
         name
             Preset internal name
         """
+        if not self.isLoaded:
+            self.presets_queue.put((index, name))
+            return
+
         preset = self.conf["presets"][str(index)][name]
 
         for key, value in preset["props"].items():
             p_elem = self.preset_tabs[index].get(key)
             if p_elem is None:
-                if not self.isLoaded:
-                    self.presets_queue.put((index, name))
-                else:
-                    self.logger.warning(
-                        "Could not find "
-                        + key
-                        + " widget from preset "
-                        + preset["title"]
-                    )
+                self.logger.warning(
+                    "Could not find " + key + " widget from preset " + preset["title"]
+                )
                 continue
 
             elem, handler = p_elem
 
             ok = handler.updateValue(elem(), value)
             if not ok:
                 self.logger.warning(
                     "Could not set "
                     + key
                     + " widget value from preset "
                     + preset["title"]
                 )
+            #else:
+            #    self.presetValueSet.connect(self.preset_controllers[index]().setCustom)
+
+    def setCustom(self, name):
+        """
+        Set custom preset on settings edit
+
+        Parameters
+        ==========
+        name
+            Internal preset name
+        """
+        index = self.presets_index_mapping.get(name)
+        if index is None:
+            return
+        self.preset_controllers[index]().setCurrentText("Custom")
 
     @pyqtSlot(str)
     def showLinkedWidgets(self, text):
         """
         Show/hide linked widgets of the external registry selector. Intended to work with QComboBox
 
         Parameters
@@ -435,26 +472,31 @@
                 wid.setProperty("prop", elem["prop"])
                 prop_preset += "." + elem["prop"]
 
             if elem.get("index") is not None:
                 wid.setProperty("index", elem["index"])
                 prop_preset += "." + str(elem["index"])
 
+            if elem["type"] == "preset":
+                self.preset_controllers[index] = weakref.ref(wid.findChild(QComboBox))
+
             if (
                 tab["conf"].get("enable_presets", False)
                 and elem.get("preset", False)
                 and not prop_preset == ""
             ):
                 wid.setProperty("preset_property", prop_preset)
 
                 self.preset_tabs[index][prop_preset] = (
                     weakref.ref(wid),
                     self.handlers[elem["type"]],
                 )
 
+                self.presets_index_mapping[prop_preset] = index
+
             if registriesName is not None:
                 ok = self.handlers[elem["type"]].linkElem(wid, registriesName)
                 if not ok:
                     self.logger.warning(
                         "Element type "
                         + elem["type"]
                         + " does not support linking extra registries"
@@ -483,14 +525,39 @@
             if label is not None:
                 form.addRow(label, widWrapper)
             else:
                 form.addRow(widWrapper)
 
         return form.rowCount() - 1, wid
 
+    def initExtraRegistries(self):
+        for reg, value in self.external_reg.items():
+            if value.get("inPlace", False):
+                continue
+
+            scroll = QScrollArea()
+            scroll.setVerticalScrollBarPolicy(Qt.ScrollBarPolicy.ScrollBarAlwaysOn)
+            scroll.setHorizontalScrollBarPolicy(Qt.ScrollBarPolicy.ScrollBarAlwaysOff)
+            scroll.setWidgetResizable(True)
+            wrapper = QWidget()
+            wrapper.setSizePolicy(
+                QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum
+            )
+            form = QFormLayout()
+
+            for elem in value["items"]:
+                tab = {"conf": {"enable_presets": False}}
+                index = None
+                self.processItem(elem, index, form, tab)
+
+            wrapper.setLayout(form)
+            scroll.setWidget(wrapper)
+            scroll.setWindowTitle("Settings")
+            self.externalRegistries[reg] = scroll
+
     def initTab(self, index):
         """
         Parse registry and generate elements
 
         Parameters
         ==========
         index
@@ -593,14 +660,17 @@
 
         return scroll
 
     def initLayout(self):
         """
         Generate layout
         """
+        common.app_manager.updateState(common.AppState.SettingsInit)
+        self.initExtraRegistries()
+
         baseLayout = QVBoxLayout(self)
 
         tabWidget = QTabWidget()
         for i in range(len(self.conf["tabs"])):
             scroll = self.initTab(i)
             tabWidget.addTab(scroll, self.conf["tabs"][i]["name"])
 
@@ -625,15 +695,16 @@
         bottomPanel.addWidget(applyButton)
         bottomPanel.addWidget(okButton)
 
         baseLayout.addLayout(bottomPanel)
 
         self.setLayout(baseLayout)
 
+        self.isLoaded = True
+
         while not self.presets_queue.empty():
             self.loadPreset(*self.presets_queue.get())
 
-        self.isLoaded = True
-
         # updating properties
-        if self.presets_update_queue:
+        if not self.presets_update_queue == []:
             common.config_manager.batchUpdate.emit(self.presets_update_queue)
+            self.main_class().update()
```

### Comparing `smartwheel-core-0.0.2/src/smartwheel/settings_handlers/actions.py` & `smartwheel-core-0.0.3/src/smartwheel/settings_handlers/actions.py`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.2/src/smartwheel/settings_handlers/base.py` & `smartwheel-core-0.0.3/src/smartwheel/settings_handlers/base.py`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.2/src/smartwheel/settings_handlers/basic.py` & `smartwheel-core-0.0.3/src/smartwheel/settings_handlers/basic.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,15 +191,15 @@
 
         ok, value = self.value_getter(elem["module"], elem["prop"])
         if ok:
             wid.setChecked(value)
         else:
             self.logger.warning("Could not get value for " + elem["name"])
 
-        wid.clicked.connect(self.setBool)
+        wid.toggled.connect(self.setBool)
 
         return wid
 
     @pyqtSlot(bool)
     def setBool(self, value):
         caller = self.sender()
         self.value_setter(caller, value)
```

### Comparing `smartwheel-core-0.0.2/src/smartwheel/settings_handlers/modules.py` & `smartwheel-core-0.0.3/src/smartwheel/settings_handlers/ui.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,127 +1,47 @@
 import logging
+import math
 
-from PyQt6.QtCore import Qt, pyqtSlot
-from PyQt6.QtGui import QFont
-from PyQt6.QtWidgets import (
-    QCheckBox,
-    QGridLayout,
-    QHBoxLayout,
-    QLabel,
-    QPushButton,
-    QSizePolicy,
-    QSpacerItem,
-    QVBoxLayout,
-    QWidget,
-)
+from PyQt6.QtCore import pyqtSlot
+from PyQt6.QtWidgets import QComboBox, QGridLayout, QSizePolicy, QVBoxLayout, QWidget
 
 from smartwheel.settings_handlers.base import BaseHandler
 
 
-class ModulesLoader(BaseHandler):
+class UIModulesLoader(BaseHandler):
     """
-    Common modules picker
+    UI modules loader
     """
 
     def __init__(self, value_getter, value_setter, parent_obj=None):
-        super(ModulesLoader, self).__init__(value_getter, value_setter, parent_obj)
+        super(UIModulesLoader, self).__init__(value_getter, value_setter, parent_obj)
         self.logger = logging.getLogger(__name__)
 
     def initElem(self, elem):
         """
-        Initialize modules picker, should not be called directly from settings.py
-
-        Parameters
-        ==========
-        elem
-            Dict containing modules {"modules": [{"name": "internalName", "title": ..., "description": ...,}, ...], "modulesLoad": [0, 1, ...]}
-        """
-        layout = QGridLayout()
-
-        font = QFont()
-        font.setBold(True)
-
-        labels = [QLabel(x) for x in ["Enabled", "Title", "Description", "Options"]]
-
-        for i in range(len(labels)):
-            labels[i].setFont(font)
-            layout.addWidget(labels[i], 0, i, Qt.AlignmentFlag.AlignLeft)
-
-        # layout.setColumnStretch(10, 0)
-
-        for i, mod in enumerate(elem["modules"]):
-            check = QCheckBox()
-            options = QPushButton("...")
-
-            check.setProperty("name", mod["name"])
-
-            if i in elem["modulesLoad"]:
-                check.setChecked(True)
-
-            for j, s in enumerate(["title", "description"]):
-                label = QLabel(mod[s])
-
-                layout.addWidget(label, i + 1, j + 1, Qt.AlignmentFlag.AlignLeft)
-
-            layout.addWidget(check, i + 1, 0, Qt.AlignmentFlag.AlignLeft)
-            layout.addWidget(options, i + 1, 3, Qt.AlignmentFlag.AlignLeft)
-
-            for j in range(1, 4):
-                if layout.itemAtPosition(i + 1, j) is not None:
-                    check.clicked.connect(
-                        layout.itemAtPosition(i + 1, j).widget().setEnabled
-                    )
-                    if not check.isChecked():
-                        layout.itemAtPosition(i + 1, j).widget().setDisabled(True)
-
-        vbox = QVBoxLayout()
-        vbox.addLayout(layout)
-
-        spacer = QSpacerItem(
-            40, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum
-        )
-        vbox.addSpacerItem(spacer)
-
-        wrapper = QWidget()
-        wrapper.setSizePolicy(QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
-        wrapper.setLayout(vbox)
-
-        return wrapper
-
-
-class SerialLoader(BaseHandler):
-    """
-    Serial modules picker
-    """
-
-    def __init__(self, value_getter, value_setter, parent_obj=None):
-        super(SerialLoader, self).__init__(value_getter, value_setter, parent_obj)
-        self.logger = logging.getLogger(__name__)
-
-    def initElem(self, elem):
-        """
-        Load serial modules picker
+        Load ui modules picker
 
         Parameters
         ==========
         elem
             Element from config
         """
-        ok, modules = self.value_getter("canvas", "serialModules")
+        ok, modules = self.value_getter("canvas", "modules")
         if not ok:
-            self.logger.error("Could not get serial modules")
+            self.logger.error("Could not get ui modules")
             return None
 
-        ok, modulesLoad = self.value_getter("canvas", "serialModulesLoad")
+        ok, modulesLoad = self.value_getter("canvas", "modulesLoad")
         if not ok:
-            self.logger.error("Could not get loaded serial modules")
+            self.logger.error("Could not get loaded ui modules")
             return None
 
         elem["modules"] = modules
         elem["modulesLoad"] = modulesLoad
+        elem["disabled"] = [0]
 
         picker = self.parent_obj().handlers["modules"].initElem(elem)
         if picker is None:
             self.logger.error("Could not initialize modules picker")
             return None
 
         layout = picker.findChild(QVBoxLayout).findChild(QGridLayout)
@@ -137,22 +57,22 @@
 
     @pyqtSlot(bool)
     def setEnabled(self, enabled):
         caller = self.sender()
 
         name = caller.property("name")
 
-        ok, modules = self.value_getter("canvas", "serialModules")
+        ok, modules = self.value_getter("canvas", "modules")
         if not ok:
-            self.logger.error("Could not get serial modules")
+            self.logger.error("Could not get ui modules")
             return
 
-        ok, modulesLoad = self.value_getter("canvas", "serialModulesLoad")
+        ok, modulesLoad = self.value_getter("canvas", "modulesLoad")
         if not ok:
-            self.logger.error("Could not get loaded serial modules")
+            self.logger.error("Could not get loaded ui modules")
             return
 
         index = None
         for i in range(len(modules)):
             if modules[i]["name"] == name:
                 index = i
                 break
@@ -164,11 +84,55 @@
         if enabled:
             m_set = set(modulesLoad)
             m_set.add(index)
             modulesLoad = list(m_set)
         else:
             modulesLoad.remove(index)
 
-        self.value_setter(module="canvas", prop="serialModulesLoad", value=modulesLoad)
+        self.value_setter(module="canvas", prop="modulesLoad", value=modulesLoad)
+
+
+class SelectorWheel(QWidget):
+    def __init__(self, n_sections):
+        super(SelectorWheel, self).__init__()
+        self.combos = []
+
+        for a in range(0, 360, 360 // n_sections):
+            combo = QComboBox(parent=self)
+            # combo.setSizePolicy(QSizePolicy.Policy.Fixed, QSizePolicy.Policy.Fixed)
+            # combo.setFixedSize(10, 10)
+            combo.move(
+                self.x() + int(100 + 100 * math.cos(math.radians(a))),
+                self.y() + int(100 + 100 * math.sin(math.radians(a))),
+            )
+            self.combos.append(combo)
+
+
+class WheelPicker(BaseHandler):
+    """
+    Wheel sections picker
+    """
+
+    def __init__(self, value_getter, value_setter, parent_obj=None):
+        super(WheelPicker, self).__init__(value_getter, value_setter, parent_obj)
+        self.logger = logging.getLogger(__name__)
+
+    def initElem(self, elem):
+        """
+        Initialize picker
+
+        Parameters
+        ==========
+        elem
+            Wheel elem config
+        """
+        ok, num_sections = self.value_getter("common", "selectionWheelEntries")
+        if not ok:
+            self.logger.warning("Could not get selection wheel entries number")
+            return
+
+        wrapper = SelectorWheel(num_sections)
+
+        return wrapper
 
 
-handlers = {"modules": ModulesLoader, "serial": SerialLoader}
+handlers = {"uimodules": UIModulesLoader, "sections": WheelPicker}
```

### Comparing `smartwheel-core-0.0.2/src/smartwheel/settings_handlers/preset.py` & `smartwheel-core-0.0.3/src/smartwheel/settings_handlers/preset.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,18 @@
 
         wid.currentIndexChanged.connect(self.setPreset)
 
         ok, value = self.value_getter(elem["module"], elem["prop"])
         if not ok:
             value = "Custom"
 
+        wid.blockSignals(True)
         wid.setCurrentText(value)
+        wid.blockSignals(False)
+        wid.currentIndexChanged.emit(wid.currentIndex())
 
         save = QPushButton("Save")
         save.setProperty("combo", weakref.ref(wid))
         save.clicked.connect(self.savePreset)
 
         layout.addWidget(wid)
         layout.addWidget(save)
```

### Comparing `smartwheel-core-0.0.2/src/smartwheel/settings_registry/appearance.json` & `smartwheel-core-0.0.3/src/smartwheel/settings_registry/appearance.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9981060606060607%*

 * *Differences: {"'items'": "{3: {'options': {insert: [(9, OrderedDict([('name', 'Tools icon color'), ('type', "*

 * *            "'color'), ('module', 'canvas'), ('prop', 'toolsIconColor'), ('preset', True)])), (10, "*

 * *            "OrderedDict([('name', 'Tools background color'), ('type', 'color'), ('module', "*

 * *            "'canvas'), ('prop', 'toolsBackgroundColor'), ('preset', True)]))]}}}"}*

```diff
@@ -186,14 +186,28 @@
                 },
                 {
                     "module": "common",
                     "name": "Main text color",
                     "preset": true,
                     "prop": "majorTextColor",
                     "type": "color"
+                },
+                {
+                    "module": "canvas",
+                    "name": "Tools icon color",
+                    "preset": true,
+                    "prop": "toolsIconColor",
+                    "type": "color"
+                },
+                {
+                    "module": "canvas",
+                    "name": "Tools background color",
+                    "preset": true,
+                    "prop": "toolsBackgroundColor",
+                    "type": "color"
                 }
             ]
         },
         {
             "name": "Background",
             "options": [
                 {
```

### Comparing `smartwheel-core-0.0.2/src/smartwheel/settings_registry/general.json` & `smartwheel-core-0.0.3/src/smartwheel/settings_registry/general.json`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.2/src/smartwheel/tools.py` & `smartwheel-core-0.0.3/src/smartwheel/tools.py`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.2/src/smartwheel/ui/files.py` & `smartwheel-core-0.0.3/src/smartwheel/ui/files.py`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.2/src/smartwheel/ui/folder.py` & `smartwheel-core-0.0.3/src/smartwheel/ui/folder.py`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.2/src/smartwheel/ui/hue.py` & `smartwheel-core-0.0.3/src/smartwheel/ui/hue.py`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.2/src/smartwheel/ui/internal/krita_server.py` & `smartwheel-core-0.0.3/src/smartwheel/ui/internal/krita_server.py`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.2/src/smartwheel/ui/media.py` & `smartwheel-core-0.0.3/src/smartwheel/ui/media.py`

 * *Files 6% similar despite different names*

```diff
@@ -162,36 +162,36 @@
             text,
         )
 
     def drawHeaderText(self, qp, t):
         self.drawText(
             qp,
             self.conf["majorTextColor"],
-            self.conf["style"]["textHeaderFont"],
-            self.conf["style"]["textHeaderSize"],
+            self.conf["textHeaderFont"],
+            self.conf["textHeaderSize"],
             1,
             t,
         )
 
     def drawBottomText(self, qp, t):
         self.drawText(
             qp,
             self.conf["majorTextColor"],
-            self.conf["style"]["bottomTextFont"],
-            self.conf["style"]["bottomTextSize"],
+            self.conf["bottomTextFont"],
+            self.conf["bottomTextSize"],
             2,
             t,
         )
 
     def drawTrackSeek(self, qp, t1, t2):
         self.drawText(
             qp,
             self.conf["majorTextColor"],
-            self.conf["style"]["seekTextFont"],
-            self.conf["style"]["seekTextSize"],
+            self.conf["seekTextFont"],
+            self.conf["seekTextSize"],
             3,
             t1 + " / " + t2,
         )
 
     def draw(self, qp, offset):
         self.updateVars(offset)
         qp.drawPixmap(
```

### Comparing `smartwheel-core-0.0.2/src/smartwheel/ui/wheel.py` & `smartwheel-core-0.0.3/src/smartwheel/ui/wheel.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,25 +30,25 @@
             self.scale_pixmap()
             self.color_pixmap()
 
     def load_module(self):
         # mod = importlib.import_module(self.module["name"])
         # ui = mod.UIElem(self.module["config"], self.parent.conf)
         # self.module["class"] = ui
-        if self.module["class"].icon_path is None:
+        if self.module["class"] is None or self.module["class"].icon_path is None:
             self.pixmap = None  # QImage(os.path.join(self.parent().conf["iconsFolder"], "folder.png"))
         else:
             self.pixmap = QPixmap(
                 os.path.join(
                     self.parent().conf["iconsFolder"], self.module["class"].icon_path
                 )
             )
 
     def draw_module(self, qp, opacity):
-        if self.module is not None:
+        if self.module is not None and self.module["class"] is not None:
             qp.setOpacity(opacity)
             self.module["class"].draw(qp, self.parent()._sections_pos)
             qp.setOpacity(1.0)
 
     def update_vars(self):
         self.delta = self.parent()._angle - self.init_angle
 
@@ -514,14 +514,15 @@
                             * circleWidth
                             // 3
                         ),
                     ),
                     self.conf["overlayCirclesWidth"],
                     self.conf["overlayCirclesWidth"],
                 )
+
         if self.conf["drawOverlayRects"]:
             self.qp.setPen(
                 QPen(
                     QColor(self.conf["overlayRectsColor"]),
                     self.conf["overlayRectsWidth"],
                     Qt.PenStyle.SolidLine,
                 )
```

### Comparing `smartwheel-core-0.0.2/src/smartwheel_core.egg-info/PKG-INFO` & `smartwheel-core-0.0.3/src/smartwheel_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartwheel-core
-Version: 0.0.2
+Version: 0.0.3
 Summary: Keyboard knob/dial controller with a ton of features
 Author-email: enaix <enaix@protonmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -686,15 +686,15 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 ![smartwheel-core](/extra/render1.jpg)
 
-# Smartwheel Core
+![smartwheel-core logo](/extra/logo.png)
 
 A powerful keyboard knob controller with GUI
 
 ![smartwheel-core ui](/extra/banner.png)
 
 ## Why do I need it?
 
@@ -714,28 +714,38 @@
 
 #### Theming
 
 Smartwheel is fully customizable (you can even create any keybinds if you want)
 
 ## Installation
 
+You may install the prebuilt stable version from the releases.
+
+#### Development build
+
 Make sure that Python 3 is installed
 
 #### Stable version
 
 `pip3 install smartwheel-core`
 
-#### Development build
+#### From Github
 
 `git clone https://github.com/enaix/smartwheel-core.git`
 
 `cd smartwheel-core`
 
 `pip3 install .`
 
+#### Compilation
+
+Nuitka now supports only Python <= 3.10
+
+`./build.sh` or `.\build.bat`
+
 ## We need your help!
 
 I've started working on this project a while ago, but it turned out that it's too big: it won't be possible to finish it without your help. However, it's much easier to implement features one-by-one: you only need basic Python3 (and sometimes PyQt6) knowledge. If you believe in this project and want to contribute, please DM me. Even small fixes, ideas or suggestions are very important.
 
 ## Documentation
 
 Docs are available at readthedocs: https://smartwheel-core.readthedocs.io/en/latest/
@@ -746,35 +756,38 @@
 - [x] Documentation (in progress)
 - [ ] Examples (in progress)
 - [x] Initial encoders support (Linux)
 - [ ] Refactor api
   - [X] Move to PyQt6
   - [X] Add colorable icons
   - [X] Add modules background processes
+  - [ ] Rewrite serial input with new api
+  - [ ] Add media fetching on Windows
   - [ ] Add key combos
   - [ ] Finish folders support
 - [ ] Settings menu (in progress)
   - [X] Basic stuff
   - [X] Custom handlers support (Almost)
   - [X] Saving
   - [X] Theme presets
   - [X] Add color picker
-  - [ ] Better overlays editor
-  - [ ] Actions editor
-  - [ ] Modules import (.zip)
+  - [X] Actions editor
+  - [ ] Sections editor
+  - [ ] Add unified input editor (new input api)
+  - [ ] Better overlays editor (?)
+  - [ ] Modules import (.zip) (?)
 - [ ] Wheel hiding
   - [ ] Hide after timeout
   - [ ] Hide after losing window focus
 - [ ] Packaging
-  - [ ] Configure setup.py
+  - [X] Configure setup.py
   - [ ] Add auto update feature
   - [ ] Hire core doctor!
 - [ ] Windows support
   - [ ] (Platform) Replace AF_UNIX socket with network socket
-  - [ ] (Platform) Replace pynput with winapi
 - [ ] Add fancy blur (?)
 - [ ] Mac support (?)
 
 ## Features progress
 
 - [x] Base structure (Plugins manager)
 - [x] Action engine
@@ -800,16 +813,20 @@
   - [ ] Canvas rotate/scale
   - [ ] Brush
   - [ ] ...
 - [ ] Photoshop integration (?)
 
 ## DIY knob
 
-If you don't have a standalone dial, you may 3D print one: there is a Freecad model in `pad` folder. Sadly, some components don't fit, but I don't have time to fix it right now. DM me if you need the fixed case model.
+If you don't have a standalone dial, you may 3D print one! 
 
-Upd: going to properly remodel it in F360 in the future
+### [smartwheel pad](https://github.com/enaix/smartwheel-pad-mk1)
 
 ## Gallery
 
 Short video (sorry for the poor quality): ![smartwheel.mp4](https://github.com/enaix/smartwheel-core/raw/master/extra/smartwheel.mp4)
 
 Update: added UI overlays ![smartwheel2.mp4](https://github.com/enaix/smartwheel-core/raw/master/extra/simplescreenrecorder-2022-10-10_12.54.42.mp4)
+
+## Resources
+
+Ionicons icon set https://github.com/ionic-team/ionicons
```

### Comparing `smartwheel-core-0.0.2/src/smartwheel_core.egg-info/SOURCES.txt` & `smartwheel-core-0.0.3/src/smartwheel_core.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -8,77 +8,89 @@
 src/smartwheel/canvas.py
 src/smartwheel/common.py
 src/smartwheel/config.py
 src/smartwheel/gui_tools.py
 src/smartwheel/launch.json
 src/smartwheel/logo.png
 src/smartwheel/settings.py
+src/smartwheel/status.json
 src/smartwheel/tools.py
 src/smartwheel/actions/__init__.py
 src/smartwheel/actions/baseaction.py
 src/smartwheel/actions/custom.py
 src/smartwheel/actions/keypress.py
 src/smartwheel/actions/wheel/__init__.py
 src/smartwheel/actions/wheel/base.py
 src/smartwheel/actions/wheel/module.py
 src/smartwheel/actions/wheel/wheel.py
 src/smartwheel/backgrounds/__init__.py
 src/smartwheel/backgrounds/base.py
 src/smartwheel/backgrounds/basic.py
-src/smartwheel/backgrounds/config.json
+src/smartwheel/backgrounds/config_defaults.json
 src/smartwheel/backgrounds/contour.py
-src/smartwheel/backgrounds/config/contour.json
-src/smartwheel/backgrounds/config/pattern.json
 src/smartwheel/cache/background_contour/contour1.json
 src/smartwheel/cache/background_contour/contour1.png
-src/smartwheel/config/actionengine.json
-src/smartwheel/config/bgkeyboard.json
-src/smartwheel/config/common.json
-src/smartwheel/config/config.json
-src/smartwheel/config/folder.json
-src/smartwheel/config/hue.json
-src/smartwheel/config/keyboard.json
-src/smartwheel/config/media.json
-src/smartwheel/config/serial.json
-src/smartwheel/config/wheel.json
-src/smartwheel/config/internal/krita_server.json
+src/smartwheel/defaults/actionengine.json
+src/smartwheel/defaults/common.json
+src/smartwheel/defaults/config.json
+src/smartwheel/defaults/folder.json
+src/smartwheel/defaults/hue.json
+src/smartwheel/defaults/media.json
+src/smartwheel/defaults/wheel.json
+src/smartwheel/defaults/backgrounds/contour.json
+src/smartwheel/defaults/backgrounds/pattern.json
+src/smartwheel/defaults/internal/krita_server.json
+src/smartwheel/defaults/serial/bgkeyboard.json
+src/smartwheel/defaults/serial/keyboard.json
+src/smartwheel/defaults/serial/serial.json
 src/smartwheel/docs/conf.py
 src/smartwheel/docs/_build/html/_static/file.png
 src/smartwheel/docs/_build/html/_static/minus.png
 src/smartwheel/docs/_build/html/_static/plus.png
 src/smartwheel/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
 src/smartwheel/icons/default/folder.png
-src/smartwheel/icons/default/hue.png
 src/smartwheel/icons/default/hue.svg
+src/smartwheel/icons/default/hue_old.png
 src/smartwheel/icons/default/media.png
 src/smartwheel/icons/default/pause.png
 src/smartwheel/icons/default/play.png
 src/smartwheel/icons/default/round.png
+src/smartwheel/icons/ionicons/close.svg
+src/smartwheel/icons/ionicons/folder.svg
+src/smartwheel/icons/ionicons/hue.svg
+src/smartwheel/icons/ionicons/media.svg
+src/smartwheel/icons/ionicons/pause.svg
+src/smartwheel/icons/ionicons/play.svg
+src/smartwheel/icons/ionicons/settings.svg
 src/smartwheel/presets/appearance/blackout.json
 src/smartwheel/presets/appearance/classic.json
 src/smartwheel/presets/appearance/polar.json
 src/smartwheel/serialpipe/__init__.py
 src/smartwheel/serialpipe/base.py
 src/smartwheel/serialpipe/bgkeyboard.py
 src/smartwheel/serialpipe/keyboard.py
 src/smartwheel/serialpipe/serial.py
 src/smartwheel/settings_handlers/__init__.py
 src/smartwheel/settings_handlers/actions.py
 src/smartwheel/settings_handlers/base.py
 src/smartwheel/settings_handlers/basic.py
-src/smartwheel/settings_handlers/config.json
+src/smartwheel/settings_handlers/config_defaults.json
 src/smartwheel/settings_handlers/modules.py
 src/smartwheel/settings_handlers/preset.py
 src/smartwheel/settings_handlers/serial.py
+src/smartwheel/settings_handlers/ui.py
 src/smartwheel/settings_registry/appearance.json
-src/smartwheel/settings_registry/config.json
+src/smartwheel/settings_registry/config_defaults.json
 src/smartwheel/settings_registry/general.json
 src/smartwheel/settings_registry/serial.json
+src/smartwheel/settings_registry/uimodules.json
 src/smartwheel/settings_registry/external/contour.json
 src/smartwheel/settings_registry/external/pattern.json
+src/smartwheel/settings_registry/external/serialmodule.json
+src/smartwheel/settings_registry/external/ui_media.json
 src/smartwheel/ui/__init__.py
 src/smartwheel/ui/base.py
 src/smartwheel/ui/files.py
 src/smartwheel/ui/folder.py
 src/smartwheel/ui/hue.py
 src/smartwheel/ui/media.py
 src/smartwheel/ui/wheel.py
```

