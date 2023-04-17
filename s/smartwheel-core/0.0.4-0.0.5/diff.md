# Comparing `tmp/smartwheel-core-0.0.4.tar.gz` & `tmp/smartwheel-core-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartwheel-core-0.0.4.tar", last modified: Mon Apr 17 07:38:24 2023, max compression
+gzip compressed data, was "smartwheel-core-0.0.5.tar", last modified: Mon Apr 17 08:38:43 2023, max compression
```

## Comparing `smartwheel-core-0.0.4.tar` & `smartwheel-core-0.0.5.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 07:38:24.968529 smartwheel-core-0.0.4/
--rw-r--r--   0 fitz      (1000) fitz      (1000)    35149 2022-05-16 11:10:38.000000 smartwheel-core-0.0.4/LICENSE
--rw-r--r--   0 fitz      (1000) fitz      (1000)       65 2023-04-17 06:56:28.000000 smartwheel-core-0.0.4/MANIFEST.in
--rw-r--r--   0 fitz      (1000) fitz      (1000)    45385 2023-04-17 07:38:24.967529 smartwheel-core-0.0.4/PKG-INFO
--rw-r--r--   0 fitz      (1000) fitz      (1000)     4235 2023-04-14 15:45:11.000000 smartwheel-core-0.0.4/README.md
--rw-r--r--   0 fitz      (1000) fitz      (1000)     1008 2023-04-17 07:36:57.000000 smartwheel-core-0.0.4/pyproject.toml
--rw-r--r--   0 fitz      (1000) fitz      (1000)       38 2023-04-17 07:38:24.968529 smartwheel-core-0.0.4/setup.cfg
-drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 07:38:24.947529 smartwheel-core-0.0.4/src/
-drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 07:38:24.951529 smartwheel-core-0.0.4/src/smartwheel/
--rw-r--r--   0 fitz      (1000) fitz      (1000)       22 2023-04-17 07:37:10.000000 smartwheel-core-0.0.4/src/smartwheel/__init__.py
--rwxr-xr-x   0 fitz      (1000) fitz      (1000)    13103 2023-04-15 10:44:17.000000 smartwheel-core-0.0.4/src/smartwheel/__main__.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)     5634 2023-04-15 10:36:59.000000 smartwheel-core-0.0.4/src/smartwheel/actionengine.py
-drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 07:38:24.954529 smartwheel-core-0.0.4/src/smartwheel/actions/
--rw-r--r--   0 fitz      (1000) fitz      (1000)        0 2022-05-16 11:10:38.000000 smartwheel-core-0.0.4/src/smartwheel/actions/__init__.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)       95 2023-03-07 10:31:43.000000 smartwheel-core-0.0.4/src/smartwheel/actions/baseaction.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)      338 2023-03-14 09:26:20.000000 smartwheel-core-0.0.4/src/smartwheel/actions/custom.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)     2818 2023-03-14 09:26:29.000000 smartwheel-core-0.0.4/src/smartwheel/actions/keypress.py
-drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 07:38:24.954529 smartwheel-core-0.0.4/src/smartwheel/actions/wheel/
--rw-r--r--   0 fitz      (1000) fitz      (1000)        0 2022-10-15 10:15:43.000000 smartwheel-core-0.0.4/src/smartwheel/actions/wheel/__init__.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)       93 2023-03-07 10:31:43.000000 smartwheel-core-0.0.4/src/smartwheel/actions/wheel/base.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)      409 2023-03-14 09:26:43.000000 smartwheel-core-0.0.4/src/smartwheel/actions/wheel/module.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)      670 2023-03-14 09:26:50.000000 smartwheel-core-0.0.4/src/smartwheel/actions/wheel/wheel.py
-drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 07:38:24.955529 smartwheel-core-0.0.4/src/smartwheel/backgrounds/
--rw-r--r--   0 fitz      (1000) fitz      (1000)        0 2023-03-07 16:05:15.000000 smartwheel-core-0.0.4/src/smartwheel/backgrounds/__init__.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)      510 2023-03-14 09:26:58.000000 smartwheel-core-0.0.4/src/smartwheel/backgrounds/base.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)     1452 2023-03-20 06:26:26.000000 smartwheel-core-0.0.4/src/smartwheel/backgrounds/basic.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)      174 2023-04-14 15:52:54.000000 smartwheel-core-0.0.4/src/smartwheel/backgrounds/config_defaults.json
--rw-r--r--   0 fitz      (1000) fitz      (1000)     4918 2023-04-15 11:28:35.000000 smartwheel-core-0.0.4/src/smartwheel/backgrounds/contour.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)    12923 2023-04-15 10:34:20.000000 smartwheel-core-0.0.4/src/smartwheel/canvas.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)     8947 2023-04-15 11:00:12.000000 smartwheel-core-0.0.4/src/smartwheel/common.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)    13575 2023-04-15 11:00:58.000000 smartwheel-core-0.0.4/src/smartwheel/config.py
-drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 07:38:24.956529 smartwheel-core-0.0.4/src/smartwheel/defaults/
--rw-r--r--   0 fitz      (1000) fitz      (1000)    13807 2023-04-14 15:19:42.000000 smartwheel-core-0.0.4/src/smartwheel/defaults/actionengine.json
-drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 07:38:24.956529 smartwheel-core-0.0.4/src/smartwheel/defaults/backgrounds/
--rw-r--r--   0 fitz      (1000) fitz      (1000)      133 2023-03-10 13:03:51.000000 smartwheel-core-0.0.4/src/smartwheel/defaults/backgrounds/contour.json
--rw-r--r--   0 fitz      (1000) fitz      (1000)       67 2023-03-10 17:35:19.000000 smartwheel-core-0.0.4/src/smartwheel/defaults/backgrounds/pattern.json
--rw-r--r--   0 fitz      (1000) fitz      (1000)      428 2023-03-15 11:11:32.000000 smartwheel-core-0.0.4/src/smartwheel/defaults/common.json
--rw-r--r--   0 fitz      (1000) fitz      (1000)     3387 2023-04-14 17:35:11.000000 smartwheel-core-0.0.4/src/smartwheel/defaults/config.json
--rw-r--r--   0 fitz      (1000) fitz      (1000)      225 2023-03-15 11:10:38.000000 smartwheel-core-0.0.4/src/smartwheel/defaults/folder.json
--rw-r--r--   0 fitz      (1000) fitz      (1000)     1142 2023-03-15 11:10:14.000000 smartwheel-core-0.0.4/src/smartwheel/defaults/hue.json
-drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 07:38:24.957529 smartwheel-core-0.0.4/src/smartwheel/defaults/internal/
--rw-r--r--   0 fitz      (1000) fitz      (1000)       44 2022-05-16 11:10:38.000000 smartwheel-core-0.0.4/src/smartwheel/defaults/internal/krita_server.json
--rw-r--r--   0 fitz      (1000) fitz      (1000)     2007 2023-03-31 18:58:45.000000 smartwheel-core-0.0.4/src/smartwheel/defaults/media.json
-drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 07:38:24.957529 smartwheel-core-0.0.4/src/smartwheel/defaults/serial/
--rw-r--r--   0 fitz      (1000) fitz      (1000)      724 2023-03-10 13:03:51.000000 smartwheel-core-0.0.4/src/smartwheel/defaults/serial/bgkeyboard.json
--rw-r--r--   0 fitz      (1000) fitz      (1000)      273 2022-10-15 10:15:43.000000 smartwheel-core-0.0.4/src/smartwheel/defaults/serial/keyboard.json
--rw-r--r--   0 fitz      (1000) fitz      (1000)     1131 2023-03-20 11:00:24.000000 smartwheel-core-0.0.4/src/smartwheel/defaults/serial/serial.json
--rw-r--r--   0 fitz      (1000) fitz      (1000)      613 2023-03-10 13:03:51.000000 smartwheel-core-0.0.4/src/smartwheel/defaults/wheel.json
-drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 07:38:24.957529 smartwheel-core-0.0.4/src/smartwheel/docs/
-drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 07:38:24.946529 smartwheel-core-0.0.4/src/smartwheel/docs/_build/
-drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 07:38:24.946529 smartwheel-core-0.0.4/src/smartwheel/docs/_build/html/
-drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 07:38:24.958529 smartwheel-core-0.0.4/src/smartwheel/docs/_build/html/_static/
-drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 07:38:24.946529 smartwheel-core-0.0.4/src/smartwheel/docs/_build/html/_static/css/
-drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 07:38:24.958529 smartwheel-core-0.0.4/src/smartwheel/docs/_build/html/_static/css/fonts/
--rw-r--r--   0 fitz      (1000) fitz      (1000)   444379 2023-01-12 13:41:03.000000 smartwheel-core-0.0.4/src/smartwheel/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0 fitz      (1000) fitz      (1000)      286 2022-10-15 10:15:55.000000 smartwheel-core-0.0.4/src/smartwheel/docs/_build/html/_static/file.png
--rw-r--r--   0 fitz      (1000) fitz      (1000)       90 2022-10-15 10:15:55.000000 smartwheel-core-0.0.4/src/smartwheel/docs/_build/html/_static/minus.png
--rw-r--r--   0 fitz      (1000) fitz      (1000)       90 2022-10-15 10:15:55.000000 smartwheel-core-0.0.4/src/smartwheel/docs/_build/html/_static/plus.png
--rw-r--r--   0 fitz      (1000) fitz      (1000)     1185 2023-03-07 10:31:43.000000 smartwheel-core-0.0.4/src/smartwheel/docs/conf.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)     2849 2023-04-14 15:39:49.000000 smartwheel-core-0.0.4/src/smartwheel/gui_tools.py
-drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 07:38:24.946529 smartwheel-core-0.0.4/src/smartwheel/icons/
-drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 07:38:24.959529 smartwheel-core-0.0.4/src/smartwheel/icons/default/
--rw-r--r--   0 fitz      (1000) fitz      (1000)     5227 2022-05-16 11:10:38.000000 smartwheel-core-0.0.4/src/smartwheel/icons/default/folder.png
--rw-r--r--   0 fitz      (1000) fitz      (1000)     5386 2022-05-16 11:10:38.000000 smartwheel-core-0.0.4/src/smartwheel/icons/default/hue.svg
--rw-r--r--   0 fitz      (1000) fitz      (1000)    30624 2022-05-16 11:10:38.000000 smartwheel-core-0.0.4/src/smartwheel/icons/default/hue_old.png
--rw-r--r--   0 fitz      (1000) fitz      (1000)    15349 2022-05-16 11:10:38.000000 smartwheel-core-0.0.4/src/smartwheel/icons/default/media.png
--rw-r--r--   0 fitz      (1000) fitz      (1000)     1900 2022-05-16 11:10:38.000000 smartwheel-core-0.0.4/src/smartwheel/icons/default/pause.png
--rw-r--r--   0 fitz      (1000) fitz      (1000)     3297 2022-05-16 11:10:38.000000 smartwheel-core-0.0.4/src/smartwheel/icons/default/play.png
--rw-r--r--   0 fitz      (1000) fitz      (1000)     8682 2022-05-16 11:10:38.000000 smartwheel-core-0.0.4/src/smartwheel/icons/default/round.png
-drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 07:38:24.960529 smartwheel-core-0.0.4/src/smartwheel/icons/ionicons/
--rw-r--r--   0 fitz      (1000) fitz      (1000)      397 1985-10-26 08:15:00.000000 smartwheel-core-0.0.4/src/smartwheel/icons/ionicons/close.svg
--rw-r--r--   0 fitz      (1000) fitz      (1000)      547 1985-10-26 08:15:00.000000 smartwheel-core-0.0.4/src/smartwheel/icons/ionicons/folder.svg
--rw-r--r--   0 fitz      (1000) fitz      (1000)      269 2023-03-15 10:51:33.000000 smartwheel-core-0.0.4/src/smartwheel/icons/ionicons/hue.svg
--rw-r--r--   0 fitz      (1000) fitz      (1000)      335 1985-10-26 08:15:00.000000 smartwheel-core-0.0.4/src/smartwheel/icons/ionicons/media.svg
--rw-r--r--   0 fitz      (1000) fitz      (1000)      294 1985-10-26 08:15:00.000000 smartwheel-core-0.0.4/src/smartwheel/icons/ionicons/pause.svg
--rw-r--r--   0 fitz      (1000) fitz      (1000)      305 1985-10-26 08:15:00.000000 smartwheel-core-0.0.4/src/smartwheel/icons/ionicons/play.svg
--rw-r--r--   0 fitz      (1000) fitz      (1000)      917 1985-10-26 08:15:00.000000 smartwheel-core-0.0.4/src/smartwheel/icons/ionicons/settings.svg
--rw-r--r--   0 fitz      (1000) fitz      (1000)       66 2023-04-14 17:50:58.000000 smartwheel-core-0.0.4/src/smartwheel/launch.json
--rw-r--r--   0 fitz      (1000) fitz      (1000)   242358 2022-05-16 11:10:38.000000 smartwheel-core-0.0.4/src/smartwheel/logo.png
-drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 07:38:24.947529 smartwheel-core-0.0.4/src/smartwheel/presets/
-drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 07:38:24.961529 smartwheel-core-0.0.4/src/smartwheel/presets/appearance/
--rw-r--r--   0 fitz      (1000) fitz      (1000)     1289 2023-03-31 18:58:45.000000 smartwheel-core-0.0.4/src/smartwheel/presets/appearance/blackout.json
--rw-r--r--   0 fitz      (1000) fitz      (1000)     1298 2023-03-31 18:58:45.000000 smartwheel-core-0.0.4/src/smartwheel/presets/appearance/classic.json
--rw-r--r--   0 fitz      (1000) fitz      (1000)     1294 2023-03-31 18:58:45.000000 smartwheel-core-0.0.4/src/smartwheel/presets/appearance/polar.json
-drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 07:38:24.962529 smartwheel-core-0.0.4/src/smartwheel/serialpipe/
--rw-r--r--   0 fitz      (1000) fitz      (1000)        0 2022-05-16 11:10:38.000000 smartwheel-core-0.0.4/src/smartwheel/serialpipe/__init__.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)     9049 2023-03-07 15:47:03.000000 smartwheel-core-0.0.4/src/smartwheel/serialpipe/base.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)     4572 2023-04-15 10:36:27.000000 smartwheel-core-0.0.4/src/smartwheel/serialpipe/bgkeyboard.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)     1829 2023-03-14 09:33:55.000000 smartwheel-core-0.0.4/src/smartwheel/serialpipe/keyboard.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)     1844 2023-04-15 10:36:09.000000 smartwheel-core-0.0.4/src/smartwheel/serialpipe/serial.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)    23435 2023-04-15 11:25:21.000000 smartwheel-core-0.0.4/src/smartwheel/settings.py
-drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 07:38:24.963529 smartwheel-core-0.0.4/src/smartwheel/settings_handlers/
--rw-r--r--   0 fitz      (1000) fitz      (1000)        0 2023-01-28 07:05:00.000000 smartwheel-core-0.0.4/src/smartwheel/settings_handlers/__init__.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)    12276 2023-04-14 15:19:42.000000 smartwheel-core-0.0.4/src/smartwheel/settings_handlers/actions.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)     2135 2023-03-13 07:05:07.000000 smartwheel-core-0.0.4/src/smartwheel/settings_handlers/base.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)     7820 2023-03-20 06:26:26.000000 smartwheel-core-0.0.4/src/smartwheel/settings_handlers/basic.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)       84 2023-03-21 09:13:23.000000 smartwheel-core-0.0.4/src/smartwheel/settings_handlers/config_defaults.json
--rw-r--r--   0 fitz      (1000) fitz      (1000)    15523 2023-04-14 15:40:07.000000 smartwheel-core-0.0.4/src/smartwheel/settings_handlers/modules.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)     5565 2023-03-20 06:26:26.000000 smartwheel-core-0.0.4/src/smartwheel/settings_handlers/preset.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)     7846 2023-04-14 15:40:07.000000 smartwheel-core-0.0.4/src/smartwheel/settings_handlers/serial.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)     3961 2023-04-14 15:40:07.000000 smartwheel-core-0.0.4/src/smartwheel/settings_handlers/ui.py
-drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 07:38:24.964529 smartwheel-core-0.0.4/src/smartwheel/settings_registry/
--rw-r--r--   0 fitz      (1000) fitz      (1000)     4261 2023-03-21 10:12:12.000000 smartwheel-core-0.0.4/src/smartwheel/settings_registry/appearance.json
--rw-r--r--   0 fitz      (1000) fitz      (1000)      492 2023-03-31 18:58:45.000000 smartwheel-core-0.0.4/src/smartwheel/settings_registry/config_defaults.json
-drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 07:38:24.964529 smartwheel-core-0.0.4/src/smartwheel/settings_registry/external/
--rw-r--r--   0 fitz      (1000) fitz      (1000)      700 2023-04-15 09:06:54.000000 smartwheel-core-0.0.4/src/smartwheel/settings_registry/external/contour.json
--rw-r--r--   0 fitz      (1000) fitz      (1000)      448 2023-03-10 16:00:47.000000 smartwheel-core-0.0.4/src/smartwheel/settings_registry/external/pattern.json
--rw-r--r--   0 fitz      (1000) fitz      (1000)      758 2023-03-21 08:32:03.000000 smartwheel-core-0.0.4/src/smartwheel/settings_registry/external/serialmodule.json
--rw-r--r--   0 fitz      (1000) fitz      (1000)      854 2023-03-31 18:58:45.000000 smartwheel-core-0.0.4/src/smartwheel/settings_registry/external/ui_media.json
--rw-r--r--   0 fitz      (1000) fitz      (1000)     1165 2023-03-14 08:32:47.000000 smartwheel-core-0.0.4/src/smartwheel/settings_registry/general.json
--rw-r--r--   0 fitz      (1000) fitz      (1000)       97 2023-03-20 06:30:56.000000 smartwheel-core-0.0.4/src/smartwheel/settings_registry/serial.json
--rw-r--r--   0 fitz      (1000) fitz      (1000)      169 2023-03-21 10:46:26.000000 smartwheel-core-0.0.4/src/smartwheel/settings_registry/uimodules.json
--rw-r--r--   0 fitz      (1000) fitz      (1000)       20 2023-04-15 10:14:23.000000 smartwheel-core-0.0.4/src/smartwheel/status.json
--rw-r--r--   0 fitz      (1000) fitz      (1000)      590 2023-03-08 19:13:53.000000 smartwheel-core-0.0.4/src/smartwheel/tools.py
-drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 07:38:24.965529 smartwheel-core-0.0.4/src/smartwheel/ui/
--rw-r--r--   0 fitz      (1000) fitz      (1000)        0 2022-05-16 11:10:38.000000 smartwheel-core-0.0.4/src/smartwheel/ui/__init__.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)      245 2023-03-13 09:01:47.000000 smartwheel-core-0.0.4/src/smartwheel/ui/base.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)     3674 2023-03-14 09:32:38.000000 smartwheel-core-0.0.4/src/smartwheel/ui/files.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)      779 2023-04-17 07:29:53.000000 smartwheel-core-0.0.4/src/smartwheel/ui/folder.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)    11410 2023-03-14 09:32:57.000000 smartwheel-core-0.0.4/src/smartwheel/ui/hue.py
-drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 07:38:24.966529 smartwheel-core-0.0.4/src/smartwheel/ui/internal/
--rw-r--r--   0 fitz      (1000) fitz      (1000)        0 2022-10-15 10:15:43.000000 smartwheel-core-0.0.4/src/smartwheel/ui/internal/__init__.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)      297 2023-04-17 07:30:55.000000 smartwheel-core-0.0.4/src/smartwheel/ui/internal/baseinternal.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)      406 2023-04-17 07:30:35.000000 smartwheel-core-0.0.4/src/smartwheel/ui/internal/krita_api.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)     2570 2023-04-17 07:30:15.000000 smartwheel-core-0.0.4/src/smartwheel/ui/internal/krita_server.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)     6126 2023-03-31 18:58:45.000000 smartwheel-core-0.0.4/src/smartwheel/ui/media.py
--rw-r--r--   0 fitz      (1000) fitz      (1000)    20641 2023-03-21 09:07:45.000000 smartwheel-core-0.0.4/src/smartwheel/ui/wheel.py
-drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 07:38:24.967529 smartwheel-core-0.0.4/src/smartwheel_core.egg-info/
--rw-r--r--   0 fitz      (1000) fitz      (1000)    45385 2023-04-17 07:38:24.000000 smartwheel-core-0.0.4/src/smartwheel_core.egg-info/PKG-INFO
--rw-r--r--   0 fitz      (1000) fitz      (1000)     3997 2023-04-17 07:38:24.000000 smartwheel-core-0.0.4/src/smartwheel_core.egg-info/SOURCES.txt
--rw-r--r--   0 fitz      (1000) fitz      (1000)        1 2023-04-17 07:38:24.000000 smartwheel-core-0.0.4/src/smartwheel_core.egg-info/dependency_links.txt
--rw-r--r--   0 fitz      (1000) fitz      (1000)       57 2023-04-17 07:38:24.000000 smartwheel-core-0.0.4/src/smartwheel_core.egg-info/entry_points.txt
--rw-r--r--   0 fitz      (1000) fitz      (1000)      129 2023-04-17 07:38:24.000000 smartwheel-core-0.0.4/src/smartwheel_core.egg-info/requires.txt
--rw-r--r--   0 fitz      (1000) fitz      (1000)       11 2023-04-17 07:38:24.000000 smartwheel-core-0.0.4/src/smartwheel_core.egg-info/top_level.txt
+drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 08:38:43.948961 smartwheel-core-0.0.5/
+-rw-r--r--   0 fitz      (1000) fitz      (1000)    35149 2022-05-16 11:10:38.000000 smartwheel-core-0.0.5/LICENSE
+-rw-r--r--   0 fitz      (1000) fitz      (1000)       65 2023-04-17 06:56:28.000000 smartwheel-core-0.0.5/MANIFEST.in
+-rw-r--r--   0 fitz      (1000) fitz      (1000)    45380 2023-04-17 08:38:43.948961 smartwheel-core-0.0.5/PKG-INFO
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     4230 2023-04-17 08:37:14.000000 smartwheel-core-0.0.5/README.md
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     1008 2023-04-17 08:37:28.000000 smartwheel-core-0.0.5/pyproject.toml
+-rw-r--r--   0 fitz      (1000) fitz      (1000)       38 2023-04-17 08:38:43.948961 smartwheel-core-0.0.5/setup.cfg
+drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 08:38:43.925961 smartwheel-core-0.0.5/src/
+drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 08:38:43.931961 smartwheel-core-0.0.5/src/smartwheel/
+-rw-r--r--   0 fitz      (1000) fitz      (1000)       22 2023-04-17 08:37:40.000000 smartwheel-core-0.0.5/src/smartwheel/__init__.py
+-rwxr-xr-x   0 fitz      (1000) fitz      (1000)    13103 2023-04-15 10:44:17.000000 smartwheel-core-0.0.5/src/smartwheel/__main__.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     5634 2023-04-15 10:36:59.000000 smartwheel-core-0.0.5/src/smartwheel/actionengine.py
+drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 08:38:43.932961 smartwheel-core-0.0.5/src/smartwheel/actions/
+-rw-r--r--   0 fitz      (1000) fitz      (1000)        0 2022-05-16 11:10:38.000000 smartwheel-core-0.0.5/src/smartwheel/actions/__init__.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)       95 2023-03-07 10:31:43.000000 smartwheel-core-0.0.5/src/smartwheel/actions/baseaction.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      338 2023-03-14 09:26:20.000000 smartwheel-core-0.0.5/src/smartwheel/actions/custom.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     2818 2023-03-14 09:26:29.000000 smartwheel-core-0.0.5/src/smartwheel/actions/keypress.py
+drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 08:38:43.932961 smartwheel-core-0.0.5/src/smartwheel/actions/wheel/
+-rw-r--r--   0 fitz      (1000) fitz      (1000)        0 2022-10-15 10:15:43.000000 smartwheel-core-0.0.5/src/smartwheel/actions/wheel/__init__.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)       93 2023-03-07 10:31:43.000000 smartwheel-core-0.0.5/src/smartwheel/actions/wheel/base.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      409 2023-03-14 09:26:43.000000 smartwheel-core-0.0.5/src/smartwheel/actions/wheel/module.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      670 2023-03-14 09:26:50.000000 smartwheel-core-0.0.5/src/smartwheel/actions/wheel/wheel.py
+drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 08:38:43.933961 smartwheel-core-0.0.5/src/smartwheel/backgrounds/
+-rw-r--r--   0 fitz      (1000) fitz      (1000)        0 2023-03-07 16:05:15.000000 smartwheel-core-0.0.5/src/smartwheel/backgrounds/__init__.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      510 2023-03-14 09:26:58.000000 smartwheel-core-0.0.5/src/smartwheel/backgrounds/base.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     1452 2023-03-20 06:26:26.000000 smartwheel-core-0.0.5/src/smartwheel/backgrounds/basic.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      174 2023-04-14 15:52:54.000000 smartwheel-core-0.0.5/src/smartwheel/backgrounds/config_defaults.json
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     4918 2023-04-15 11:28:35.000000 smartwheel-core-0.0.5/src/smartwheel/backgrounds/contour.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)    12923 2023-04-15 10:34:20.000000 smartwheel-core-0.0.5/src/smartwheel/canvas.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     8946 2023-04-17 08:33:30.000000 smartwheel-core-0.0.5/src/smartwheel/common.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)    13575 2023-04-15 11:00:58.000000 smartwheel-core-0.0.5/src/smartwheel/config.py
+drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 08:38:43.934961 smartwheel-core-0.0.5/src/smartwheel/defaults/
+-rw-r--r--   0 fitz      (1000) fitz      (1000)    13807 2023-04-14 15:19:42.000000 smartwheel-core-0.0.5/src/smartwheel/defaults/actionengine.json
+drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 08:38:43.935961 smartwheel-core-0.0.5/src/smartwheel/defaults/backgrounds/
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      133 2023-03-10 13:03:51.000000 smartwheel-core-0.0.5/src/smartwheel/defaults/backgrounds/contour.json
+-rw-r--r--   0 fitz      (1000) fitz      (1000)       67 2023-03-10 17:35:19.000000 smartwheel-core-0.0.5/src/smartwheel/defaults/backgrounds/pattern.json
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      428 2023-03-15 11:11:32.000000 smartwheel-core-0.0.5/src/smartwheel/defaults/common.json
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     3387 2023-04-14 17:35:11.000000 smartwheel-core-0.0.5/src/smartwheel/defaults/config.json
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      225 2023-03-15 11:10:38.000000 smartwheel-core-0.0.5/src/smartwheel/defaults/folder.json
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     1142 2023-03-15 11:10:14.000000 smartwheel-core-0.0.5/src/smartwheel/defaults/hue.json
+drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 08:38:43.935961 smartwheel-core-0.0.5/src/smartwheel/defaults/internal/
+-rw-r--r--   0 fitz      (1000) fitz      (1000)       44 2022-05-16 11:10:38.000000 smartwheel-core-0.0.5/src/smartwheel/defaults/internal/krita_server.json
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     2007 2023-03-31 18:58:45.000000 smartwheel-core-0.0.5/src/smartwheel/defaults/media.json
+drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 08:38:43.935961 smartwheel-core-0.0.5/src/smartwheel/defaults/serial/
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      724 2023-03-10 13:03:51.000000 smartwheel-core-0.0.5/src/smartwheel/defaults/serial/bgkeyboard.json
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      273 2022-10-15 10:15:43.000000 smartwheel-core-0.0.5/src/smartwheel/defaults/serial/keyboard.json
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     1131 2023-03-20 11:00:24.000000 smartwheel-core-0.0.5/src/smartwheel/defaults/serial/serial.json
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      613 2023-03-10 13:03:51.000000 smartwheel-core-0.0.5/src/smartwheel/defaults/wheel.json
+drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 08:38:43.936961 smartwheel-core-0.0.5/src/smartwheel/docs/
+drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 08:38:43.923961 smartwheel-core-0.0.5/src/smartwheel/docs/_build/
+drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 08:38:43.923961 smartwheel-core-0.0.5/src/smartwheel/docs/_build/html/
+drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 08:38:43.936961 smartwheel-core-0.0.5/src/smartwheel/docs/_build/html/_static/
+drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 08:38:43.924961 smartwheel-core-0.0.5/src/smartwheel/docs/_build/html/_static/css/
+drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 08:38:43.936961 smartwheel-core-0.0.5/src/smartwheel/docs/_build/html/_static/css/fonts/
+-rw-r--r--   0 fitz      (1000) fitz      (1000)   444379 2023-01-12 13:41:03.000000 smartwheel-core-0.0.5/src/smartwheel/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      286 2022-10-15 10:15:55.000000 smartwheel-core-0.0.5/src/smartwheel/docs/_build/html/_static/file.png
+-rw-r--r--   0 fitz      (1000) fitz      (1000)       90 2022-10-15 10:15:55.000000 smartwheel-core-0.0.5/src/smartwheel/docs/_build/html/_static/minus.png
+-rw-r--r--   0 fitz      (1000) fitz      (1000)       90 2022-10-15 10:15:55.000000 smartwheel-core-0.0.5/src/smartwheel/docs/_build/html/_static/plus.png
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     1185 2023-03-07 10:31:43.000000 smartwheel-core-0.0.5/src/smartwheel/docs/conf.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     2849 2023-04-14 15:39:49.000000 smartwheel-core-0.0.5/src/smartwheel/gui_tools.py
+drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 08:38:43.924961 smartwheel-core-0.0.5/src/smartwheel/icons/
+drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 08:38:43.938961 smartwheel-core-0.0.5/src/smartwheel/icons/default/
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     5227 2022-05-16 11:10:38.000000 smartwheel-core-0.0.5/src/smartwheel/icons/default/folder.png
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     5386 2022-05-16 11:10:38.000000 smartwheel-core-0.0.5/src/smartwheel/icons/default/hue.svg
+-rw-r--r--   0 fitz      (1000) fitz      (1000)    30624 2022-05-16 11:10:38.000000 smartwheel-core-0.0.5/src/smartwheel/icons/default/hue_old.png
+-rw-r--r--   0 fitz      (1000) fitz      (1000)    15349 2022-05-16 11:10:38.000000 smartwheel-core-0.0.5/src/smartwheel/icons/default/media.png
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     1900 2022-05-16 11:10:38.000000 smartwheel-core-0.0.5/src/smartwheel/icons/default/pause.png
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     3297 2022-05-16 11:10:38.000000 smartwheel-core-0.0.5/src/smartwheel/icons/default/play.png
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     8682 2022-05-16 11:10:38.000000 smartwheel-core-0.0.5/src/smartwheel/icons/default/round.png
+drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 08:38:43.939961 smartwheel-core-0.0.5/src/smartwheel/icons/ionicons/
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      397 1985-10-26 08:15:00.000000 smartwheel-core-0.0.5/src/smartwheel/icons/ionicons/close.svg
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      547 1985-10-26 08:15:00.000000 smartwheel-core-0.0.5/src/smartwheel/icons/ionicons/folder.svg
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      269 2023-03-15 10:51:33.000000 smartwheel-core-0.0.5/src/smartwheel/icons/ionicons/hue.svg
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      335 1985-10-26 08:15:00.000000 smartwheel-core-0.0.5/src/smartwheel/icons/ionicons/media.svg
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      294 1985-10-26 08:15:00.000000 smartwheel-core-0.0.5/src/smartwheel/icons/ionicons/pause.svg
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      305 1985-10-26 08:15:00.000000 smartwheel-core-0.0.5/src/smartwheel/icons/ionicons/play.svg
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      917 1985-10-26 08:15:00.000000 smartwheel-core-0.0.5/src/smartwheel/icons/ionicons/settings.svg
+-rw-r--r--   0 fitz      (1000) fitz      (1000)       66 2023-04-14 17:50:58.000000 smartwheel-core-0.0.5/src/smartwheel/launch.json
+-rw-r--r--   0 fitz      (1000) fitz      (1000)   242358 2022-05-16 11:10:38.000000 smartwheel-core-0.0.5/src/smartwheel/logo.png
+drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 08:38:43.924961 smartwheel-core-0.0.5/src/smartwheel/presets/
+drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 08:38:43.940961 smartwheel-core-0.0.5/src/smartwheel/presets/appearance/
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     1289 2023-03-31 18:58:45.000000 smartwheel-core-0.0.5/src/smartwheel/presets/appearance/blackout.json
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     1298 2023-03-31 18:58:45.000000 smartwheel-core-0.0.5/src/smartwheel/presets/appearance/classic.json
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     1294 2023-03-31 18:58:45.000000 smartwheel-core-0.0.5/src/smartwheel/presets/appearance/polar.json
+drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 08:38:43.941961 smartwheel-core-0.0.5/src/smartwheel/serialpipe/
+-rw-r--r--   0 fitz      (1000) fitz      (1000)        0 2022-05-16 11:10:38.000000 smartwheel-core-0.0.5/src/smartwheel/serialpipe/__init__.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     9049 2023-03-07 15:47:03.000000 smartwheel-core-0.0.5/src/smartwheel/serialpipe/base.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     4572 2023-04-15 10:36:27.000000 smartwheel-core-0.0.5/src/smartwheel/serialpipe/bgkeyboard.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     1829 2023-03-14 09:33:55.000000 smartwheel-core-0.0.5/src/smartwheel/serialpipe/keyboard.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     1844 2023-04-15 10:36:09.000000 smartwheel-core-0.0.5/src/smartwheel/serialpipe/serial.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)    23435 2023-04-15 11:25:21.000000 smartwheel-core-0.0.5/src/smartwheel/settings.py
+drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 08:38:43.943961 smartwheel-core-0.0.5/src/smartwheel/settings_handlers/
+-rw-r--r--   0 fitz      (1000) fitz      (1000)        0 2023-01-28 07:05:00.000000 smartwheel-core-0.0.5/src/smartwheel/settings_handlers/__init__.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)    12276 2023-04-14 15:19:42.000000 smartwheel-core-0.0.5/src/smartwheel/settings_handlers/actions.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     2135 2023-03-13 07:05:07.000000 smartwheel-core-0.0.5/src/smartwheel/settings_handlers/base.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     7820 2023-03-20 06:26:26.000000 smartwheel-core-0.0.5/src/smartwheel/settings_handlers/basic.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)       84 2023-03-21 09:13:23.000000 smartwheel-core-0.0.5/src/smartwheel/settings_handlers/config_defaults.json
+-rw-r--r--   0 fitz      (1000) fitz      (1000)    15523 2023-04-14 15:40:07.000000 smartwheel-core-0.0.5/src/smartwheel/settings_handlers/modules.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     5565 2023-03-20 06:26:26.000000 smartwheel-core-0.0.5/src/smartwheel/settings_handlers/preset.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     7846 2023-04-14 15:40:07.000000 smartwheel-core-0.0.5/src/smartwheel/settings_handlers/serial.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     3961 2023-04-14 15:40:07.000000 smartwheel-core-0.0.5/src/smartwheel/settings_handlers/ui.py
+drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 08:38:43.944961 smartwheel-core-0.0.5/src/smartwheel/settings_registry/
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     4261 2023-03-21 10:12:12.000000 smartwheel-core-0.0.5/src/smartwheel/settings_registry/appearance.json
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      492 2023-03-31 18:58:45.000000 smartwheel-core-0.0.5/src/smartwheel/settings_registry/config_defaults.json
+drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 08:38:43.945961 smartwheel-core-0.0.5/src/smartwheel/settings_registry/external/
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      700 2023-04-15 09:06:54.000000 smartwheel-core-0.0.5/src/smartwheel/settings_registry/external/contour.json
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      448 2023-03-10 16:00:47.000000 smartwheel-core-0.0.5/src/smartwheel/settings_registry/external/pattern.json
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      758 2023-03-21 08:32:03.000000 smartwheel-core-0.0.5/src/smartwheel/settings_registry/external/serialmodule.json
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      854 2023-03-31 18:58:45.000000 smartwheel-core-0.0.5/src/smartwheel/settings_registry/external/ui_media.json
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     1165 2023-03-14 08:32:47.000000 smartwheel-core-0.0.5/src/smartwheel/settings_registry/general.json
+-rw-r--r--   0 fitz      (1000) fitz      (1000)       97 2023-03-20 06:30:56.000000 smartwheel-core-0.0.5/src/smartwheel/settings_registry/serial.json
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      169 2023-03-21 10:46:26.000000 smartwheel-core-0.0.5/src/smartwheel/settings_registry/uimodules.json
+-rw-r--r--   0 fitz      (1000) fitz      (1000)       20 2023-04-15 10:14:23.000000 smartwheel-core-0.0.5/src/smartwheel/status.json
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      590 2023-03-08 19:13:53.000000 smartwheel-core-0.0.5/src/smartwheel/tools.py
+drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 08:38:43.946961 smartwheel-core-0.0.5/src/smartwheel/ui/
+-rw-r--r--   0 fitz      (1000) fitz      (1000)        0 2022-05-16 11:10:38.000000 smartwheel-core-0.0.5/src/smartwheel/ui/__init__.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      245 2023-03-13 09:01:47.000000 smartwheel-core-0.0.5/src/smartwheel/ui/base.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     3674 2023-03-14 09:32:38.000000 smartwheel-core-0.0.5/src/smartwheel/ui/files.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      779 2023-04-17 07:29:53.000000 smartwheel-core-0.0.5/src/smartwheel/ui/folder.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)    11410 2023-03-14 09:32:57.000000 smartwheel-core-0.0.5/src/smartwheel/ui/hue.py
+drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 08:38:43.947961 smartwheel-core-0.0.5/src/smartwheel/ui/internal/
+-rw-r--r--   0 fitz      (1000) fitz      (1000)        0 2022-10-15 10:15:43.000000 smartwheel-core-0.0.5/src/smartwheel/ui/internal/__init__.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      297 2023-04-17 07:30:55.000000 smartwheel-core-0.0.5/src/smartwheel/ui/internal/baseinternal.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      406 2023-04-17 07:30:35.000000 smartwheel-core-0.0.5/src/smartwheel/ui/internal/krita_api.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     2570 2023-04-17 07:30:15.000000 smartwheel-core-0.0.5/src/smartwheel/ui/internal/krita_server.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     6126 2023-03-31 18:58:45.000000 smartwheel-core-0.0.5/src/smartwheel/ui/media.py
+-rw-r--r--   0 fitz      (1000) fitz      (1000)    20641 2023-03-21 09:07:45.000000 smartwheel-core-0.0.5/src/smartwheel/ui/wheel.py
+drwxr-xr-x   0 fitz      (1000) fitz      (1000)        0 2023-04-17 08:38:43.948961 smartwheel-core-0.0.5/src/smartwheel_core.egg-info/
+-rw-r--r--   0 fitz      (1000) fitz      (1000)    45380 2023-04-17 08:38:43.000000 smartwheel-core-0.0.5/src/smartwheel_core.egg-info/PKG-INFO
+-rw-r--r--   0 fitz      (1000) fitz      (1000)     3997 2023-04-17 08:38:43.000000 smartwheel-core-0.0.5/src/smartwheel_core.egg-info/SOURCES.txt
+-rw-r--r--   0 fitz      (1000) fitz      (1000)        1 2023-04-17 08:38:43.000000 smartwheel-core-0.0.5/src/smartwheel_core.egg-info/dependency_links.txt
+-rw-r--r--   0 fitz      (1000) fitz      (1000)       57 2023-04-17 08:38:43.000000 smartwheel-core-0.0.5/src/smartwheel_core.egg-info/entry_points.txt
+-rw-r--r--   0 fitz      (1000) fitz      (1000)      129 2023-04-17 08:38:43.000000 smartwheel-core-0.0.5/src/smartwheel_core.egg-info/requires.txt
+-rw-r--r--   0 fitz      (1000) fitz      (1000)       11 2023-04-17 08:38:43.000000 smartwheel-core-0.0.5/src/smartwheel_core.egg-info/top_level.txt
```

### Comparing `smartwheel-core-0.0.4/LICENSE` & `smartwheel-core-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.4/PKG-INFO` & `smartwheel-core-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartwheel-core
-Version: 0.0.4
+Version: 0.0.5
 Summary: Keyboard knob/dial controller with a ton of features
 Author-email: enaix <enaix@protonmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -746,15 +746,15 @@
 
 I've started working on this project a while ago, but it turned out that it's too big: it won't be possible to finish it without your help. However, it's much easier to implement features one-by-one: you only need basic Python3 (and sometimes PyQt6) knowledge. If you believe in this project and want to contribute, please DM me. Even small fixes, ideas or suggestions are very important.
 
 ## Documentation
 
 Docs are available at readthedocs: https://smartwheel-core.readthedocs.io/en/latest/
 
-## Release 0.1.0
+## Release 1.0.0
 
 - [x] Stable version (Linux)
 - [x] Documentation (in progress)
 - [ ] Examples (in progress)
 - [x] Initial encoders support (Linux)
 - [ ] Refactor api
   - [X] Move to PyQt6
@@ -776,15 +776,15 @@
   - [ ] Better overlays editor (?)
   - [ ] Modules import (.zip) (?)
 - [ ] Wheel hiding
   - [ ] Hide after timeout
   - [ ] Hide after losing window focus
 - [ ] Packaging
   - [X] Configure setup.py
-  - [ ] Add auto update feature
+  - [X] Add update feature
   - [ ] Hire core doctor!
 - [ ] Windows support
   - [ ] (Platform) Replace AF_UNIX socket with network socket
 - [ ] Add fancy blur (?)
 - [ ] Mac support (?)
 
 ## Features progress
```

### Comparing `smartwheel-core-0.0.4/README.md` & `smartwheel-core-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
 I've started working on this project a while ago, but it turned out that it's too big: it won't be possible to finish it without your help. However, it's much easier to implement features one-by-one: you only need basic Python3 (and sometimes PyQt6) knowledge. If you believe in this project and want to contribute, please DM me. Even small fixes, ideas or suggestions are very important.
 
 ## Documentation
 
 Docs are available at readthedocs: https://smartwheel-core.readthedocs.io/en/latest/
 
-## Release 0.1.0
+## Release 1.0.0
 
 - [x] Stable version (Linux)
 - [x] Documentation (in progress)
 - [ ] Examples (in progress)
 - [x] Initial encoders support (Linux)
 - [ ] Refactor api
   - [X] Move to PyQt6
@@ -86,15 +86,15 @@
   - [ ] Better overlays editor (?)
   - [ ] Modules import (.zip) (?)
 - [ ] Wheel hiding
   - [ ] Hide after timeout
   - [ ] Hide after losing window focus
 - [ ] Packaging
   - [X] Configure setup.py
-  - [ ] Add auto update feature
+  - [X] Add update feature
   - [ ] Hire core doctor!
 - [ ] Windows support
   - [ ] (Platform) Replace AF_UNIX socket with network socket
 - [ ] Add fancy blur (?)
 - [ ] Mac support (?)
 
 ## Features progress
```

### Comparing `smartwheel-core-0.0.4/pyproject.toml` & `smartwheel-core-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "smartwheel-core"
-version = "0.0.4"
+version = "0.0.5"
 description = "Keyboard knob/dial controller with a ton of features"
 readme = 'README.md'
 authors = [{ name = "enaix", email = "enaix@protonmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
```

### Comparing `smartwheel-core-0.0.4/src/smartwheel/__main__.py` & `smartwheel-core-0.0.5/src/smartwheel/__main__.py`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.4/src/smartwheel/actionengine.py` & `smartwheel-core-0.0.5/src/smartwheel/actionengine.py`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.4/src/smartwheel/actions/keypress.py` & `smartwheel-core-0.0.5/src/smartwheel/actions/keypress.py`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.4/src/smartwheel/actions/wheel/wheel.py` & `smartwheel-core-0.0.5/src/smartwheel/actions/wheel/wheel.py`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.4/src/smartwheel/backgrounds/basic.py` & `smartwheel-core-0.0.5/src/smartwheel/backgrounds/basic.py`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.4/src/smartwheel/backgrounds/contour.py` & `smartwheel-core-0.0.5/src/smartwheel/backgrounds/contour.py`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.4/src/smartwheel/canvas.py` & `smartwheel-core-0.0.5/src/smartwheel/canvas.py`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.4/src/smartwheel/common.py` & `smartwheel-core-0.0.5/src/smartwheel/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 import logging
 import os
 import time
-from enum import auto, IntEnum, StrEnum
+from enum import auto, IntEnum, Enum
 
 from PyQt6.QtCore import QObject, pyqtSignal, pyqtSlot
 
 from smartwheel import config
 
 
 class ConfigManager(QObject):
@@ -120,15 +120,15 @@
     def loadComplete(self):
         final_time = (time.time_ns() - self.total_time) // 1000000
         self.logger.info(
             "Init: load complete. Total load time is " + str(final_time) + " ms"
         )
 
 
-class StartupMode(StrEnum):
+class StartupMode(str, Enum):
     Normal = auto()
     Update = auto()
     PostUpdate = auto()
     Defaults = auto()
     PostDefaults = auto()
```

### Comparing `smartwheel-core-0.0.4/src/smartwheel/config.py` & `smartwheel-core-0.0.5/src/smartwheel/config.py`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.4/src/smartwheel/defaults/actionengine.json` & `smartwheel-core-0.0.5/src/smartwheel/defaults/actionengine.json`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.4/src/smartwheel/defaults/config.json` & `smartwheel-core-0.0.5/src/smartwheel/defaults/config.json`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.4/src/smartwheel/defaults/hue.json` & `smartwheel-core-0.0.5/src/smartwheel/defaults/hue.json`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.4/src/smartwheel/defaults/media.json` & `smartwheel-core-0.0.5/src/smartwheel/defaults/media.json`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.4/src/smartwheel/defaults/serial/bgkeyboard.json` & `smartwheel-core-0.0.5/src/smartwheel/defaults/serial/bgkeyboard.json`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.4/src/smartwheel/defaults/serial/serial.json` & `smartwheel-core-0.0.5/src/smartwheel/defaults/serial/serial.json`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.4/src/smartwheel/defaults/wheel.json` & `smartwheel-core-0.0.5/src/smartwheel/defaults/wheel.json`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.4/src/smartwheel/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg` & `smartwheel-core-0.0.5/src/smartwheel/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.4/src/smartwheel/docs/conf.py` & `smartwheel-core-0.0.5/src/smartwheel/docs/conf.py`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.4/src/smartwheel/gui_tools.py` & `smartwheel-core-0.0.5/src/smartwheel/gui_tools.py`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.4/src/smartwheel/icons/default/folder.png` & `smartwheel-core-0.0.5/src/smartwheel/icons/default/folder.png`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.4/src/smartwheel/icons/default/hue.svg` & `smartwheel-core-0.0.5/src/smartwheel/icons/default/hue.svg`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.4/src/smartwheel/icons/default/hue_old.png` & `smartwheel-core-0.0.5/src/smartwheel/icons/default/hue_old.png`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.4/src/smartwheel/icons/default/media.png` & `smartwheel-core-0.0.5/src/smartwheel/icons/default/media.png`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.4/src/smartwheel/icons/default/pause.png` & `smartwheel-core-0.0.5/src/smartwheel/icons/default/pause.png`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.4/src/smartwheel/icons/default/play.png` & `smartwheel-core-0.0.5/src/smartwheel/icons/default/play.png`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.4/src/smartwheel/icons/default/round.png` & `smartwheel-core-0.0.5/src/smartwheel/icons/default/round.png`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.4/src/smartwheel/icons/ionicons/folder.svg` & `smartwheel-core-0.0.5/src/smartwheel/icons/ionicons/folder.svg`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.4/src/smartwheel/icons/ionicons/settings.svg` & `smartwheel-core-0.0.5/src/smartwheel/icons/ionicons/settings.svg`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.4/src/smartwheel/logo.png` & `smartwheel-core-0.0.5/src/smartwheel/logo.png`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.4/src/smartwheel/presets/appearance/blackout.json` & `smartwheel-core-0.0.5/src/smartwheel/presets/appearance/blackout.json`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.4/src/smartwheel/presets/appearance/classic.json` & `smartwheel-core-0.0.5/src/smartwheel/presets/appearance/classic.json`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.4/src/smartwheel/presets/appearance/polar.json` & `smartwheel-core-0.0.5/src/smartwheel/presets/appearance/polar.json`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.4/src/smartwheel/serialpipe/base.py` & `smartwheel-core-0.0.5/src/smartwheel/serialpipe/base.py`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.4/src/smartwheel/serialpipe/bgkeyboard.py` & `smartwheel-core-0.0.5/src/smartwheel/serialpipe/bgkeyboard.py`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.4/src/smartwheel/serialpipe/keyboard.py` & `smartwheel-core-0.0.5/src/smartwheel/serialpipe/keyboard.py`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.4/src/smartwheel/serialpipe/serial.py` & `smartwheel-core-0.0.5/src/smartwheel/serialpipe/serial.py`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.4/src/smartwheel/settings.py` & `smartwheel-core-0.0.5/src/smartwheel/settings.py`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.4/src/smartwheel/settings_handlers/actions.py` & `smartwheel-core-0.0.5/src/smartwheel/settings_handlers/actions.py`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.4/src/smartwheel/settings_handlers/base.py` & `smartwheel-core-0.0.5/src/smartwheel/settings_handlers/base.py`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.4/src/smartwheel/settings_handlers/basic.py` & `smartwheel-core-0.0.5/src/smartwheel/settings_handlers/basic.py`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.4/src/smartwheel/settings_handlers/modules.py` & `smartwheel-core-0.0.5/src/smartwheel/settings_handlers/modules.py`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.4/src/smartwheel/settings_handlers/preset.py` & `smartwheel-core-0.0.5/src/smartwheel/settings_handlers/preset.py`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.4/src/smartwheel/settings_handlers/serial.py` & `smartwheel-core-0.0.5/src/smartwheel/settings_handlers/serial.py`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.4/src/smartwheel/settings_handlers/ui.py` & `smartwheel-core-0.0.5/src/smartwheel/settings_handlers/ui.py`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.4/src/smartwheel/settings_registry/appearance.json` & `smartwheel-core-0.0.5/src/smartwheel/settings_registry/appearance.json`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.4/src/smartwheel/settings_registry/external/contour.json` & `smartwheel-core-0.0.5/src/smartwheel/settings_registry/external/contour.json`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.4/src/smartwheel/settings_registry/external/serialmodule.json` & `smartwheel-core-0.0.5/src/smartwheel/settings_registry/external/serialmodule.json`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.4/src/smartwheel/settings_registry/external/ui_media.json` & `smartwheel-core-0.0.5/src/smartwheel/settings_registry/external/ui_media.json`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.4/src/smartwheel/settings_registry/general.json` & `smartwheel-core-0.0.5/src/smartwheel/settings_registry/general.json`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.4/src/smartwheel/tools.py` & `smartwheel-core-0.0.5/src/smartwheel/tools.py`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.4/src/smartwheel/ui/files.py` & `smartwheel-core-0.0.5/src/smartwheel/ui/files.py`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.4/src/smartwheel/ui/folder.py` & `smartwheel-core-0.0.5/src/smartwheel/ui/folder.py`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.4/src/smartwheel/ui/hue.py` & `smartwheel-core-0.0.5/src/smartwheel/ui/hue.py`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.4/src/smartwheel/ui/internal/krita_server.py` & `smartwheel-core-0.0.5/src/smartwheel/ui/internal/krita_server.py`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.4/src/smartwheel/ui/media.py` & `smartwheel-core-0.0.5/src/smartwheel/ui/media.py`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.4/src/smartwheel/ui/wheel.py` & `smartwheel-core-0.0.5/src/smartwheel/ui/wheel.py`

 * *Files identical despite different names*

### Comparing `smartwheel-core-0.0.4/src/smartwheel_core.egg-info/PKG-INFO` & `smartwheel-core-0.0.5/src/smartwheel_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartwheel-core
-Version: 0.0.4
+Version: 0.0.5
 Summary: Keyboard knob/dial controller with a ton of features
 Author-email: enaix <enaix@protonmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -746,15 +746,15 @@
 
 I've started working on this project a while ago, but it turned out that it's too big: it won't be possible to finish it without your help. However, it's much easier to implement features one-by-one: you only need basic Python3 (and sometimes PyQt6) knowledge. If you believe in this project and want to contribute, please DM me. Even small fixes, ideas or suggestions are very important.
 
 ## Documentation
 
 Docs are available at readthedocs: https://smartwheel-core.readthedocs.io/en/latest/
 
-## Release 0.1.0
+## Release 1.0.0
 
 - [x] Stable version (Linux)
 - [x] Documentation (in progress)
 - [ ] Examples (in progress)
 - [x] Initial encoders support (Linux)
 - [ ] Refactor api
   - [X] Move to PyQt6
@@ -776,15 +776,15 @@
   - [ ] Better overlays editor (?)
   - [ ] Modules import (.zip) (?)
 - [ ] Wheel hiding
   - [ ] Hide after timeout
   - [ ] Hide after losing window focus
 - [ ] Packaging
   - [X] Configure setup.py
-  - [ ] Add auto update feature
+  - [X] Add update feature
   - [ ] Hire core doctor!
 - [ ] Windows support
   - [ ] (Platform) Replace AF_UNIX socket with network socket
 - [ ] Add fancy blur (?)
 - [ ] Mac support (?)
 
 ## Features progress
```

### Comparing `smartwheel-core-0.0.4/src/smartwheel_core.egg-info/SOURCES.txt` & `smartwheel-core-0.0.5/src/smartwheel_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

