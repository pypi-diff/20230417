# Comparing `tmp/boris-behav-obs-8.9.6.tar.gz` & `tmp/boris-behav-obs-8.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boris-behav-obs-8.9.6.tar", last modified: Tue Dec  6 17:14:51 2022, max compression
+gzip compressed data, was "boris-behav-obs-8.9.8.tar", last modified: Tue Dec 13 12:48:03 2022, max compression
```

## Comparing `boris-behav-obs-8.9.6.tar` & `boris-behav-obs-8.9.8.tar`

### file list

```diff
@@ -1,113 +1,112 @@
-drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2022-12-06 17:14:51.062952 boris-behav-obs-8.9.6/
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    35141 2020-12-05 15:42:21.000000 boris-behav-obs-8.9.6/LICENSE.TXT
--rw-rw-r--   0 olivier   (1000) olivier   (1000)       39 2020-12-05 15:42:21.000000 boris-behav-obs-8.9.6/MANIFEST.in
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     4169 2022-12-06 17:14:51.062952 boris-behav-obs-8.9.6/PKG-INFO
--rw-rw-r--   0 olivier   (1000) olivier   (1000)      771 2022-10-26 20:33:46.000000 boris-behav-obs-8.9.6/README.TXT
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     2339 2022-12-01 09:33:04.000000 boris-behav-obs-8.9.6/README.rst
-drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2022-12-06 17:14:51.062952 boris-behav-obs-8.9.6/boris/
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    35141 2020-12-05 15:42:21.000000 boris-behav-obs-8.9.6/boris/LICENSE.TXT
--rw-rw-r--   0 olivier   (1000) olivier   (1000)      788 2022-02-24 22:32:52.000000 boris-behav-obs-8.9.6/boris/README.TXT
--rw-rw-r--   0 olivier   (1000) olivier   (1000)      773 2022-02-24 22:32:52.000000 boris-behav-obs-8.9.6/boris/__init__.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)      764 2022-10-26 20:33:46.000000 boris-behav-obs-8.9.6/boris/__main__.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     5586 2022-10-26 21:12:06.000000 boris-behav-obs-8.9.6/boris/about.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    24024 2022-10-26 20:33:46.000000 boris-behav-obs-8.9.6/boris/add_modifier.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     9093 2020-12-05 15:42:21.000000 boris-behav-obs-8.9.6/boris/add_modifier.ui
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     9748 2020-12-05 15:42:21.000000 boris-behav-obs-8.9.6/boris/add_modifier_ui.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    14204 2022-12-01 09:33:04.000000 boris-behav-obs-8.9.6/boris/advanced_event_filtering.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    38313 2022-10-26 20:33:46.000000 boris-behav-obs-8.9.6/boris/behav_coding_map_creator.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    11996 2022-12-01 09:33:04.000000 boris-behav-obs-8.9.6/boris/behavior_binary_table.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     7214 2022-10-26 20:33:46.000000 boris-behav-obs-8.9.6/boris/behaviors_coding_map.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    14009 2022-02-24 22:32:52.000000 boris-behav-obs-8.9.6/boris/boris_cli.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     1604 2022-10-26 20:33:46.000000 boris-behav-obs-8.9.6/boris/cmd_arguments.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    10576 2022-10-26 20:33:46.000000 boris-behav-obs-8.9.6/boris/coding_pad.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    14927 2022-11-08 09:18:58.000000 boris-behav-obs-8.9.6/boris/config.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    14552 2022-10-27 21:41:29.000000 boris-behav-obs-8.9.6/boris/config_file.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    16405 2022-10-26 20:33:50.000000 boris-behav-obs-8.9.6/boris/connections.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    11967 2022-10-26 20:33:46.000000 boris-behav-obs-8.9.6/boris/converters.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     8745 2020-12-05 15:42:21.000000 boris-behav-obs-8.9.6/boris/converters_ui.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)   207987 2022-12-01 22:41:59.000000 boris-behav-obs-8.9.6/boris/core.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     1767 2022-10-26 20:33:46.000000 boris-behav-obs-8.9.6/boris/core.qrc
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    44495 2022-10-26 20:33:46.000000 boris-behav-obs-8.9.6/boris/core.ui
--rw-rw-r--   0 olivier   (1000) olivier   (1000)   819259 2022-10-26 20:33:46.000000 boris-behav-obs-8.9.6/boris/core_qrc.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    66063 2022-10-26 20:33:46.000000 boris-behav-obs-8.9.6/boris/core_ui.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    13371 2022-10-29 21:24:49.000000 boris-behav-obs-8.9.6/boris/db_functions.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)      707 2022-11-08 09:16:44.000000 boris-behav-obs-8.9.6/boris/dev.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    24428 2022-10-26 20:33:50.000000 boris-behav-obs-8.9.6/boris/dialog.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     6962 2022-10-26 20:33:46.000000 boris-behav-obs-8.9.6/boris/duration_widget.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     5771 2022-10-26 20:33:46.000000 boris-behav-obs-8.9.6/boris/edit_event.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     4637 2020-12-05 15:42:21.000000 boris-behav-obs-8.9.6/boris/edit_event.ui
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     5003 2020-12-05 15:42:21.000000 boris-behav-obs-8.9.6/boris/edit_event_ui.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    36166 2022-11-11 09:44:21.000000 boris-behav-obs-8.9.6/boris/event_operations.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     2008 2022-10-26 20:33:46.000000 boris-behav-obs-8.9.6/boris/events_cursor.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    26693 2022-12-01 22:42:23.000000 boris-behav-obs-8.9.6/boris/events_snapshots.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     5300 2022-02-24 22:32:52.000000 boris-behav-obs-8.9.6/boris/exclusion_matrix.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    34483 2022-12-06 17:07:48.000000 boris-behav-obs-8.9.6/boris/export_events.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    65321 2022-12-06 17:07:48.000000 boris-behav-obs-8.9.6/boris/export_observation.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    20367 2022-10-26 20:33:46.000000 boris-behav-obs-8.9.6/boris/geometric_measurement.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     2088 2022-10-26 20:33:46.000000 boris-behav-obs-8.9.6/boris/gui_utilities.py
-drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2022-12-06 17:14:51.062952 boris-behav-obs-8.9.6/boris/icons/
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    90406 2022-12-06 17:11:11.000000 boris-behav-obs-8.9.6/boris/icons/logo_eye.ico
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     2482 2022-10-26 20:33:46.000000 boris-behav-obs-8.9.6/boris/image_overlay.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     6129 2022-10-26 20:33:46.000000 boris-behav-obs-8.9.6/boris/import_observations.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    22510 2022-12-01 22:43:58.000000 boris-behav-obs-8.9.6/boris/irr.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     9306 2022-12-01 22:44:31.000000 boris-behav-obs-8.9.6/boris/latency.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    28326 2022-10-26 20:33:46.000000 boris-behav-obs-8.9.6/boris/map_creator.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     5784 2022-10-26 20:33:46.000000 boris-behav-obs-8.9.6/boris/media_file.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     6593 2022-10-26 20:33:46.000000 boris-behav-obs-8.9.6/boris/menu_options.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     4553 2022-10-26 20:33:46.000000 boris-behav-obs-8.9.6/boris/modifiers_coding_map.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    76409 2022-10-26 20:33:46.000000 boris-behav-obs-8.9.6/boris/mpv.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    82561 2022-10-26 20:37:36.000000 boris-behav-obs-8.9.6/boris/mpv2.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    43038 2022-12-01 09:33:04.000000 boris-behav-obs-8.9.6/boris/observation.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    24553 2022-12-01 09:33:04.000000 boris-behav-obs-8.9.6/boris/observation.ui
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    73851 2022-12-06 17:07:48.000000 boris-behav-obs-8.9.6/boris/observation_operations.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    27726 2022-12-01 09:33:04.000000 boris-behav-obs-8.9.6/boris/observation_ui.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    10238 2022-10-26 20:33:46.000000 boris-behav-obs-8.9.6/boris/observations_list.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    10154 2022-10-26 20:33:46.000000 boris-behav-obs-8.9.6/boris/otx_parser.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     7542 2022-12-01 09:33:04.000000 boris-behav-obs-8.9.6/boris/param_panel.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    11013 2022-11-08 10:56:37.000000 boris-behav-obs-8.9.6/boris/param_panel.ui
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    11704 2022-11-08 10:56:45.000000 boris-behav-obs-8.9.6/boris/param_panel_ui.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     4865 2022-10-26 20:42:07.000000 boris-behav-obs-8.9.6/boris/player_dock_widget.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    16379 2022-10-26 20:33:46.000000 boris-behav-obs-8.9.6/boris/plot_data_module.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    22155 2022-11-08 11:19:34.000000 boris-behav-obs-8.9.6/boris/plot_events.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     8451 2022-10-26 20:33:46.000000 boris-behav-obs-8.9.6/boris/plot_events_rt.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     8022 2022-10-26 20:33:46.000000 boris-behav-obs-8.9.6/boris/plot_spectrogram_rt.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     7180 2022-10-26 20:33:46.000000 boris-behav-obs-8.9.6/boris/plot_waveform_rt.py
-drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2022-12-06 17:14:51.062952 boris-behav-obs-8.9.6/boris/portion/
--rw-rw-r--   0 olivier   (1000) olivier   (1000)      602 2021-01-07 23:08:44.000000 boris-behav-obs-8.9.6/boris/portion/__init__.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     1588 2020-11-26 10:59:07.000000 boris-behav-obs-8.9.6/boris/portion/const.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    11282 2020-11-26 10:59:07.000000 boris-behav-obs-8.9.6/boris/portion/dict.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     2174 2020-11-26 10:59:07.000000 boris-behav-obs-8.9.6/boris/portion/func.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    20299 2020-11-26 10:59:07.000000 boris-behav-obs-8.9.6/boris/portion/interval.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     6371 2020-11-26 10:59:07.000000 boris-behav-obs-8.9.6/boris/portion/io.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    10307 2022-11-07 22:02:32.000000 boris-behav-obs-8.9.6/boris/preferences.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    17479 2022-11-07 22:02:32.000000 boris-behav-obs-8.9.6/boris/preferences.ui
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    18974 2022-11-07 22:02:32.000000 boris-behav-obs-8.9.6/boris/preferences_ui.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    76893 2022-10-26 20:33:46.000000 boris-behav-obs-8.9.6/boris/project.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    35853 2022-10-26 20:33:46.000000 boris-behav-obs-8.9.6/boris/project.ui
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    62672 2022-12-01 09:33:04.000000 boris-behav-obs-8.9.6/boris/project_functions.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    37059 2022-10-26 20:33:46.000000 boris-behav-obs-8.9.6/boris/project_import_export.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     7742 2022-10-26 20:33:46.000000 boris-behav-obs-8.9.6/boris/project_server.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    35683 2022-10-26 20:33:46.000000 boris-behav-obs-8.9.6/boris/project_ui.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    12238 2022-10-26 20:33:46.000000 boris-behav-obs-8.9.6/boris/select_modifiers.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     7398 2022-11-11 09:44:21.000000 boris-behav-obs-8.9.6/boris/select_observations.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    10254 2022-12-06 17:07:48.000000 boris-behav-obs-8.9.6/boris/select_subj_behav.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     6913 2022-10-26 20:33:46.000000 boris-behav-obs-8.9.6/boris/state_events.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     3459 2022-10-26 20:33:46.000000 boris-behav-obs-8.9.6/boris/subjects_pad.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     9501 2022-12-01 09:33:04.000000 boris-behav-obs-8.9.6/boris/synthetic_time_budget.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    49795 2022-11-22 08:48:39.000000 boris-behav-obs-8.9.6/boris/time_budget_functions.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    42666 2022-12-01 09:33:04.000000 boris-behav-obs-8.9.6/boris/time_budget_widget.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    12182 2022-12-01 22:46:07.000000 boris-behav-obs-8.9.6/boris/transitions.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    36777 2022-11-07 22:02:32.000000 boris-behav-obs-8.9.6/boris/utilities.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)      792 2022-12-01 22:47:17.000000 boris-behav-obs-8.9.6/boris/version.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     5725 2022-10-26 20:33:46.000000 boris-behav-obs-8.9.6/boris/video_equalizer.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     9762 2022-10-26 20:33:46.000000 boris-behav-obs-8.9.6/boris/video_equalizer_ui.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     7314 2022-10-26 20:33:46.000000 boris-behav-obs-8.9.6/boris/video_operations.py
-drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2022-12-06 17:14:51.062952 boris-behav-obs-8.9.6/boris_behav_obs.egg-info/
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     4169 2022-12-06 17:14:50.000000 boris-behav-obs-8.9.6/boris_behav_obs.egg-info/PKG-INFO
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     2445 2022-12-06 17:14:50.000000 boris-behav-obs-8.9.6/boris_behav_obs.egg-info/SOURCES.txt
--rw-rw-r--   0 olivier   (1000) olivier   (1000)        1 2022-12-06 17:14:50.000000 boris-behav-obs-8.9.6/boris_behav_obs.egg-info/dependency_links.txt
--rw-rw-r--   0 olivier   (1000) olivier   (1000)       38 2022-12-06 17:14:50.000000 boris-behav-obs-8.9.6/boris_behav_obs.egg-info/entry_points.txt
--rw-rw-r--   0 olivier   (1000) olivier   (1000)      120 2022-12-06 17:14:50.000000 boris-behav-obs-8.9.6/boris_behav_obs.egg-info/requires.txt
--rw-rw-r--   0 olivier   (1000) olivier   (1000)        6 2022-12-06 17:14:50.000000 boris-behav-obs-8.9.6/boris_behav_obs.egg-info/top_level.txt
--rw-rw-r--   0 olivier   (1000) olivier   (1000)       38 2022-12-06 17:14:51.062952 boris-behav-obs-8.9.6/setup.cfg
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     2290 2022-12-06 17:13:32.000000 boris-behav-obs-8.9.6/setup.py
+drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2022-12-13 12:48:03.284079 boris-behav-obs-8.9.8/
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    35141 2022-05-06 13:42:08.000000 boris-behav-obs-8.9.8/LICENSE.TXT
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)       39 2022-05-06 13:42:08.000000 boris-behav-obs-8.9.8/MANIFEST.in
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     3456 2022-12-13 12:48:03.284079 boris-behav-obs-8.9.8/PKG-INFO
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)      771 2022-11-17 15:28:11.000000 boris-behav-obs-8.9.8/README.TXT
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     2339 2022-11-25 16:16:52.000000 boris-behav-obs-8.9.8/README.rst
+drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2022-12-13 12:48:03.284079 boris-behav-obs-8.9.8/boris/
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    35141 2022-05-06 13:42:08.000000 boris-behav-obs-8.9.8/boris/LICENSE.TXT
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)      788 2022-05-06 13:42:08.000000 boris-behav-obs-8.9.8/boris/README.TXT
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)      773 2022-05-06 13:42:08.000000 boris-behav-obs-8.9.8/boris/__init__.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)      764 2022-11-17 15:28:11.000000 boris-behav-obs-8.9.8/boris/__main__.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     5586 2022-11-17 15:28:11.000000 boris-behav-obs-8.9.8/boris/about.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    24024 2022-11-17 15:28:11.000000 boris-behav-obs-8.9.8/boris/add_modifier.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     9093 2022-05-06 13:42:08.000000 boris-behav-obs-8.9.8/boris/add_modifier.ui
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     9748 2022-05-06 13:42:08.000000 boris-behav-obs-8.9.8/boris/add_modifier_ui.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    14204 2022-11-23 11:03:30.000000 boris-behav-obs-8.9.8/boris/advanced_event_filtering.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    38313 2022-11-17 15:28:11.000000 boris-behav-obs-8.9.8/boris/behav_coding_map_creator.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    11996 2022-11-23 12:01:21.000000 boris-behav-obs-8.9.8/boris/behavior_binary_table.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     7214 2022-11-17 15:28:11.000000 boris-behav-obs-8.9.8/boris/behaviors_coding_map.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    14009 2022-05-06 13:42:08.000000 boris-behav-obs-8.9.8/boris/boris_cli.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     1604 2022-11-17 15:28:11.000000 boris-behav-obs-8.9.8/boris/cmd_arguments.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    10576 2022-11-17 15:28:11.000000 boris-behav-obs-8.9.8/boris/coding_pad.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    14927 2022-11-17 15:28:11.000000 boris-behav-obs-8.9.8/boris/config.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    14552 2022-11-17 15:28:11.000000 boris-behav-obs-8.9.8/boris/config_file.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    16405 2022-11-17 15:28:11.000000 boris-behav-obs-8.9.8/boris/connections.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    11967 2022-11-17 15:28:11.000000 boris-behav-obs-8.9.8/boris/converters.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     8745 2022-05-06 13:42:08.000000 boris-behav-obs-8.9.8/boris/converters_ui.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)   207987 2022-12-02 09:06:43.000000 boris-behav-obs-8.9.8/boris/core.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     1767 2022-11-17 15:28:11.000000 boris-behav-obs-8.9.8/boris/core.qrc
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    44495 2022-11-17 15:28:11.000000 boris-behav-obs-8.9.8/boris/core.ui
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)   819259 2022-11-17 15:28:11.000000 boris-behav-obs-8.9.8/boris/core_qrc.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    66063 2022-11-17 15:28:11.000000 boris-behav-obs-8.9.8/boris/core_ui.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    13456 2022-12-13 12:47:11.000000 boris-behav-obs-8.9.8/boris/db_functions.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    24428 2022-11-17 15:28:11.000000 boris-behav-obs-8.9.8/boris/dialog.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     6962 2022-11-17 15:28:11.000000 boris-behav-obs-8.9.8/boris/duration_widget.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     5771 2022-11-17 15:28:11.000000 boris-behav-obs-8.9.8/boris/edit_event.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     4637 2022-05-06 13:42:08.000000 boris-behav-obs-8.9.8/boris/edit_event.ui
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     5003 2022-05-06 13:42:08.000000 boris-behav-obs-8.9.8/boris/edit_event_ui.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    36166 2022-11-17 15:28:11.000000 boris-behav-obs-8.9.8/boris/event_operations.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     2008 2022-11-17 15:28:11.000000 boris-behav-obs-8.9.8/boris/events_cursor.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    27493 2022-12-12 14:52:16.000000 boris-behav-obs-8.9.8/boris/events_snapshots.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     5300 2022-05-06 13:42:08.000000 boris-behav-obs-8.9.8/boris/exclusion_matrix.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    34544 2022-12-13 10:51:37.000000 boris-behav-obs-8.9.8/boris/export_events.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    65321 2022-12-02 15:10:25.000000 boris-behav-obs-8.9.8/boris/export_observation.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    20367 2022-11-17 15:28:11.000000 boris-behav-obs-8.9.8/boris/geometric_measurement.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     2088 2022-11-17 15:28:11.000000 boris-behav-obs-8.9.8/boris/gui_utilities.py
+drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2022-12-13 12:48:03.284079 boris-behav-obs-8.9.8/boris/icons/
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    90406 2022-12-12 10:23:39.000000 boris-behav-obs-8.9.8/boris/icons/logo_eye.ico
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     2482 2022-11-17 15:28:11.000000 boris-behav-obs-8.9.8/boris/image_overlay.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     6129 2022-11-17 15:28:11.000000 boris-behav-obs-8.9.8/boris/import_observations.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    22510 2022-12-02 09:06:43.000000 boris-behav-obs-8.9.8/boris/irr.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     9306 2022-12-02 09:06:43.000000 boris-behav-obs-8.9.8/boris/latency.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    28326 2022-11-17 15:28:11.000000 boris-behav-obs-8.9.8/boris/map_creator.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     5784 2022-11-17 15:28:11.000000 boris-behav-obs-8.9.8/boris/media_file.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     6593 2022-11-17 15:28:11.000000 boris-behav-obs-8.9.8/boris/menu_options.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     4553 2022-11-17 15:28:11.000000 boris-behav-obs-8.9.8/boris/modifiers_coding_map.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    76409 2022-11-17 15:28:11.000000 boris-behav-obs-8.9.8/boris/mpv.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    82561 2022-11-17 15:28:11.000000 boris-behav-obs-8.9.8/boris/mpv2.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    43038 2022-11-29 08:52:54.000000 boris-behav-obs-8.9.8/boris/observation.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    24553 2022-11-29 14:28:18.000000 boris-behav-obs-8.9.8/boris/observation.ui
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    73851 2022-12-02 14:26:34.000000 boris-behav-obs-8.9.8/boris/observation_operations.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    27726 2022-11-29 08:44:56.000000 boris-behav-obs-8.9.8/boris/observation_ui.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    10238 2022-11-17 15:28:11.000000 boris-behav-obs-8.9.8/boris/observations_list.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    10154 2022-11-17 15:28:11.000000 boris-behav-obs-8.9.8/boris/otx_parser.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     7542 2022-11-23 11:02:44.000000 boris-behav-obs-8.9.8/boris/param_panel.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    11013 2022-11-17 15:28:11.000000 boris-behav-obs-8.9.8/boris/param_panel.ui
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    11704 2022-11-17 15:28:11.000000 boris-behav-obs-8.9.8/boris/param_panel_ui.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     4865 2022-11-17 15:28:11.000000 boris-behav-obs-8.9.8/boris/player_dock_widget.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    16379 2022-11-17 15:28:11.000000 boris-behav-obs-8.9.8/boris/plot_data_module.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    22155 2022-11-17 15:28:11.000000 boris-behav-obs-8.9.8/boris/plot_events.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     8451 2022-11-17 15:28:11.000000 boris-behav-obs-8.9.8/boris/plot_events_rt.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     8022 2022-11-17 15:28:11.000000 boris-behav-obs-8.9.8/boris/plot_spectrogram_rt.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     7180 2022-11-17 15:28:11.000000 boris-behav-obs-8.9.8/boris/plot_waveform_rt.py
+drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2022-12-13 12:48:03.284079 boris-behav-obs-8.9.8/boris/portion/
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)      602 2022-05-06 13:42:08.000000 boris-behav-obs-8.9.8/boris/portion/__init__.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     1588 2022-05-06 13:42:08.000000 boris-behav-obs-8.9.8/boris/portion/const.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    11282 2022-05-06 13:42:08.000000 boris-behav-obs-8.9.8/boris/portion/dict.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     2174 2022-05-06 13:42:08.000000 boris-behav-obs-8.9.8/boris/portion/func.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    20299 2022-05-06 13:42:08.000000 boris-behav-obs-8.9.8/boris/portion/interval.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     6371 2022-05-06 13:42:08.000000 boris-behav-obs-8.9.8/boris/portion/io.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    10307 2022-11-17 15:28:11.000000 boris-behav-obs-8.9.8/boris/preferences.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    17479 2022-11-17 15:28:11.000000 boris-behav-obs-8.9.8/boris/preferences.ui
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    18974 2022-11-17 15:28:11.000000 boris-behav-obs-8.9.8/boris/preferences_ui.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    76893 2022-11-17 15:28:11.000000 boris-behav-obs-8.9.8/boris/project.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    35853 2022-11-17 15:28:11.000000 boris-behav-obs-8.9.8/boris/project.ui
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    62721 2022-12-13 11:07:47.000000 boris-behav-obs-8.9.8/boris/project_functions.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    37059 2022-11-17 15:28:11.000000 boris-behav-obs-8.9.8/boris/project_import_export.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     7742 2022-11-17 15:28:11.000000 boris-behav-obs-8.9.8/boris/project_server.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    35683 2022-11-17 15:28:11.000000 boris-behav-obs-8.9.8/boris/project_ui.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    12238 2022-11-17 15:28:11.000000 boris-behav-obs-8.9.8/boris/select_modifiers.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     7398 2022-11-17 15:28:11.000000 boris-behav-obs-8.9.8/boris/select_observations.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    10254 2022-12-02 15:18:45.000000 boris-behav-obs-8.9.8/boris/select_subj_behav.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     6913 2022-11-17 15:28:11.000000 boris-behav-obs-8.9.8/boris/state_events.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     3459 2022-11-17 15:28:11.000000 boris-behav-obs-8.9.8/boris/subjects_pad.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     9501 2022-11-23 12:02:55.000000 boris-behav-obs-8.9.8/boris/synthetic_time_budget.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    49795 2022-11-21 13:42:23.000000 boris-behav-obs-8.9.8/boris/time_budget_functions.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    42666 2022-11-23 11:57:05.000000 boris-behav-obs-8.9.8/boris/time_budget_widget.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    12182 2022-12-02 09:06:43.000000 boris-behav-obs-8.9.8/boris/transitions.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    36777 2022-11-17 15:28:11.000000 boris-behav-obs-8.9.8/boris/utilities.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)      792 2022-12-13 12:47:42.000000 boris-behav-obs-8.9.8/boris/version.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     5725 2022-11-17 15:28:11.000000 boris-behav-obs-8.9.8/boris/video_equalizer.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     9762 2022-11-17 15:28:11.000000 boris-behav-obs-8.9.8/boris/video_equalizer_ui.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     7314 2022-11-17 15:28:11.000000 boris-behav-obs-8.9.8/boris/video_operations.py
+drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2022-12-13 12:48:03.284079 boris-behav-obs-8.9.8/boris_behav_obs.egg-info/
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     3456 2022-12-13 12:48:02.000000 boris-behav-obs-8.9.8/boris_behav_obs.egg-info/PKG-INFO
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     2432 2022-12-13 12:48:03.000000 boris-behav-obs-8.9.8/boris_behav_obs.egg-info/SOURCES.txt
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)        1 2022-12-13 12:48:02.000000 boris-behav-obs-8.9.8/boris_behav_obs.egg-info/dependency_links.txt
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)       37 2022-12-13 12:48:02.000000 boris-behav-obs-8.9.8/boris_behav_obs.egg-info/entry_points.txt
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)      120 2022-12-13 12:48:03.000000 boris-behav-obs-8.9.8/boris_behav_obs.egg-info/requires.txt
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)        6 2022-12-13 12:48:03.000000 boris-behav-obs-8.9.8/boris_behav_obs.egg-info/top_level.txt
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)       38 2022-12-13 12:48:03.284079 boris-behav-obs-8.9.8/setup.cfg
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     2290 2022-12-12 10:23:39.000000 boris-behav-obs-8.9.8/setup.py
```

### Comparing `boris-behav-obs-8.9.6/LICENSE.TXT` & `boris-behav-obs-8.9.8/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/PKG-INFO` & `boris-behav-obs-8.9.8/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,116 +1,119 @@
 Metadata-Version: 2.1
 Name: boris-behav-obs
-Version: 8.9.6
+Version: 8.9.8
 Summary: BORIS - Behavioral Observation Research Interactive Software
 Home-page: http://www.boris.unito.it
 Author: Olivier Friard - Marco Gamba
 Author-email: olivier.friard@unito.it
 License: UNKNOWN
 Project-URL: Documentation, https://boris.readthedocs.io/en/latest/
 Project-URL: Changelog, https://github.com/olivierfriard/BORIS/wiki/BORIS-change-log-v.8
 Project-URL: Source code, https://github.com/olivierfriard/BORIS
 Project-URL: Issues, https://github.com/olivierfriard/BORIS/issues
-Description: ===============================================================
-        Behavioral Observation Research Interactive Software (BORIS)
-        ===============================================================
-        
-        BORIS is an easy-to-use event logging software for video/audio coding or live observations.
-        
-        BORIS is a free and open-source software available for GNU/Linux and Windows.
-        
-        It provides also some analysis tools like time budget.
-        
-        The BORIS paper has more than `1000 citations in peer-reviewed scientific publications <http://www.boris.unito.it/pages/citations.html>`_.
-        
-        See http://www.boris.unito.it
-        
-        
-        .. image:: https://img.shields.io/badge/Made%20with-Python-1f425f.svg
-         :target: https://www.python.org/
-        
-        .. image:: https://static.pepy.tech/personalized-badge/boris-behav-obs?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads
-         :target: https://pepy.tech/project/boris-behav-obs
-        
-        
-        
-        
-        
-        
-        Documentation
-        -------------------------------------
-        
-        The official documentation is hosted here:
-        http://boris.readthedocs.io/
-        
-        The documentation provides a good starting point for learning how to use BORIS.
-        
-        Some video tutorials are available:
-        https://www.youtube.com/channel/UCo-Jyvzawwp0bRMEor4aLVQ
-        
-        
-        
-        
-        
-        Bug reports and feature requests
-        --------------------------------------
-        
-        To search for bugs, report them or request a feature, please use the github tracker:
-        https://github.com/olivierfriard/BORIS/issues
-        
-        
-        
-        
-        
-        Citing BORIS
-        --------------------------------------
-        
-        Please acknowledge and cite the use of this software and its authors when
-        results are used in publications or published elsewhere. You can use the
-        following BibTex entry
-        
-        ::
-        
-            @article {MEE3:MEE312584,
-            author = {Friard, Olivier and Gamba, Marco},
-            title = {BORIS: a free, versatile open-source event-logging software for video/audio coding and live observations},
-            journal = {Methods in Ecology and Evolution},
-            issn = {2041-210X},
-            url = {http://dx.doi.org/10.1111/2041-210X.12584},
-            doi = {10.1111/2041-210X.12584},
-            pages = {1324--1330},
-            keywords = {behavioural analysis, behaviour coding, coding scheme, ethology, observational data, ttime-budget},
-            year = {2016},
-            }
-        
-        
-        
-        
-        
-        
-        
-        
-        
-        Licence
-        -----------------------------
-        
-        Distributed with a `GPL v.3 license <LICENSE.TXT>`_
-        
-        
-        Copyright (C) 2012-2022 Olivier Friard
-        
-        
-        
-        
-        
 Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
+License-File: LICENSE.TXT
+
+===============================================================
+Behavioral Observation Research Interactive Software (BORIS)
+===============================================================
+
+BORIS is an easy-to-use event logging software for video/audio coding or live observations.
+
+BORIS is a free and open-source software available for GNU/Linux and Windows.
+
+It provides also some analysis tools like time budget.
+
+The BORIS paper has more than `1000 citations in peer-reviewed scientific publications <http://www.boris.unito.it/pages/citations.html>`_.
+
+See http://www.boris.unito.it
+
+
+.. image:: https://img.shields.io/badge/Made%20with-Python-1f425f.svg
+ :target: https://www.python.org/
+
+.. image:: https://static.pepy.tech/personalized-badge/boris-behav-obs?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads
+ :target: https://pepy.tech/project/boris-behav-obs
+
+
+
+
+
+
+Documentation
+-------------------------------------
+
+The official documentation is hosted here:
+http://boris.readthedocs.io/
+
+The documentation provides a good starting point for learning how to use BORIS.
+
+Some video tutorials are available:
+https://www.youtube.com/channel/UCo-Jyvzawwp0bRMEor4aLVQ
+
+
+
+
+
+Bug reports and feature requests
+--------------------------------------
+
+To search for bugs, report them or request a feature, please use the github tracker:
+https://github.com/olivierfriard/BORIS/issues
+
+
+
+
+
+Citing BORIS
+--------------------------------------
+
+Please acknowledge and cite the use of this software and its authors when
+results are used in publications or published elsewhere. You can use the
+following BibTex entry
+
+::
+
+    @article {MEE3:MEE312584,
+    author = {Friard, Olivier and Gamba, Marco},
+    title = {BORIS: a free, versatile open-source event-logging software for video/audio coding and live observations},
+    journal = {Methods in Ecology and Evolution},
+    issn = {2041-210X},
+    url = {http://dx.doi.org/10.1111/2041-210X.12584},
+    doi = {10.1111/2041-210X.12584},
+    pages = {1324--1330},
+    keywords = {behavioural analysis, behaviour coding, coding scheme, ethology, observational data, ttime-budget},
+    year = {2016},
+    }
+
+
+
+
+
+
+
+
+
+Licence
+-----------------------------
+
+Distributed with a `GPL v.3 license <LICENSE.TXT>`_
+
+
+Copyright (C) 2012-2022 Olivier Friard
+
+
+
+
+
+
```

### Comparing `boris-behav-obs-8.9.6/README.TXT` & `boris-behav-obs-8.9.8/README.TXT`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/README.rst` & `boris-behav-obs-8.9.8/README.rst`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/LICENSE.TXT` & `boris-behav-obs-8.9.8/boris/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/README.TXT` & `boris-behav-obs-8.9.8/boris/README.TXT`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/__init__.py` & `boris-behav-obs-8.9.8/boris/__init__.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/__main__.py` & `boris-behav-obs-8.9.8/boris/__main__.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/about.py` & `boris-behav-obs-8.9.8/boris/about.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/add_modifier.py` & `boris-behav-obs-8.9.8/boris/add_modifier.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/add_modifier.ui` & `boris-behav-obs-8.9.8/boris/add_modifier.ui`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/add_modifier_ui.py` & `boris-behav-obs-8.9.8/boris/add_modifier_ui.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/advanced_event_filtering.py` & `boris-behav-obs-8.9.8/boris/advanced_event_filtering.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/behav_coding_map_creator.py` & `boris-behav-obs-8.9.8/boris/behav_coding_map_creator.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/behavior_binary_table.py` & `boris-behav-obs-8.9.8/boris/behavior_binary_table.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/behaviors_coding_map.py` & `boris-behav-obs-8.9.8/boris/behaviors_coding_map.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/boris_cli.py` & `boris-behav-obs-8.9.8/boris/boris_cli.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/cmd_arguments.py` & `boris-behav-obs-8.9.8/boris/cmd_arguments.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/coding_pad.py` & `boris-behav-obs-8.9.8/boris/coding_pad.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/config.py` & `boris-behav-obs-8.9.8/boris/config.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/config_file.py` & `boris-behav-obs-8.9.8/boris/config_file.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/connections.py` & `boris-behav-obs-8.9.8/boris/connections.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/converters.py` & `boris-behav-obs-8.9.8/boris/converters.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/converters_ui.py` & `boris-behav-obs-8.9.8/boris/converters_ui.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/core.py` & `boris-behav-obs-8.9.8/boris/core.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/core.qrc` & `boris-behav-obs-8.9.8/boris/core.qrc`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/core.ui` & `boris-behav-obs-8.9.8/boris/core.ui`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/core_qrc.py` & `boris-behav-obs-8.9.8/boris/core_qrc.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/core_ui.py` & `boris-behav-obs-8.9.8/boris/core_ui.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/db_functions.py` & `boris-behav-obs-8.9.8/boris/db_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
   Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston,
   MA 02110-1301, USA.
 
 """
 
 import sqlite3
 import logging
+from typing import Optional, Tuple
 from . import config as cfg
 from . import project_functions
 
 
 def load_events_in_db(
     pj: dict,
     selected_subjects: list,
@@ -162,15 +163,15 @@
 
     db.commit()
     return cursor
 
 
 def load_aggregated_events_in_db(
     pj: dict, selected_subjects: list, selected_observations: list, selected_behaviors: list
-):
+) -> Tuple[bool, str, Optional[sqlite3.Connection]]:
     """
     populate a memory sqlite database with aggregated events from selected_observations, selected_subjects and selected_behaviors
 
     Args:
         pj (dict): project dictionary
         selected_observations (list):
         selected_subjects (list):
```

### Comparing `boris-behav-obs-8.9.6/boris/dialog.py` & `boris-behav-obs-8.9.8/boris/dialog.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/duration_widget.py` & `boris-behav-obs-8.9.8/boris/duration_widget.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/edit_event.py` & `boris-behav-obs-8.9.8/boris/edit_event.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/edit_event.ui` & `boris-behav-obs-8.9.8/boris/edit_event.ui`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/edit_event_ui.py` & `boris-behav-obs-8.9.8/boris/edit_event_ui.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/event_operations.py` & `boris-behav-obs-8.9.8/boris/event_operations.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/events_cursor.py` & `boris-behav-obs-8.9.8/boris/events_cursor.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/events_snapshots.py` & `boris-behav-obs-8.9.8/boris/events_snapshots.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,15 +20,15 @@
   MA 02110-1301, USA.
 
 """
 
 
 import logging
 import os
-import pathlib
+import pathlib as pl
 import subprocess
 from decimal import Decimal as dec
 
 from PyQt5.QtWidgets import QFileDialog, QInputDialog, QMessageBox
 
 from . import config as cfg
 from . import db_functions, dialog, project_functions, select_observations, select_subj_behav
@@ -224,33 +224,14 @@
 
                             media_path = project_functions.full_path(
                                 self.pj[cfg.OBSERVATIONS][obsId][cfg.FILE][nplayer][mediaFileIdx],
                                 self.projectFileName,
                             )
 
                             vframes = 1 if not time_interval else int(mediafile_fps * time_interval * 2)
-                            ffmpeg_command = (
-                                f'"{self.ffmpeg_bin}" '
-                                f"-ss {start:.3f} "
-                                f'-i "{media_path}" '
-                                f"-vframes {vframes} "
-                                f'"{exportDir}{os.sep}'
-                                f"{util.safeFileName(obsId)}"
-                                f"_PLAYER{nplayer}"
-                                f"_{util.safeFileName(subject)}"
-                                f"_{util.safeFileName(behavior)}"
-                                f'_{start:.3f}_%08d.{self.frame_bitmap_format.lower()}"'
-                            )
-
-                            logging.debug(f"ffmpeg command: {ffmpeg_command}")
-
-                            p = subprocess.Popen(
-                                ffmpeg_command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True
-                            )
-                            out, error = p.communicate()
 
                         if cfg.STATE in behavior_state:
                             if idx % 2 == 0:
 
                                 # check if stop is on same media file
                                 if (
                                     mediaFileIdx
@@ -297,34 +278,36 @@
                                     continue
 
                                 media_path = project_functions.full_path(
                                     self.pj[cfg.OBSERVATIONS][obsId][cfg.FILE][nplayer][mediaFileIdx],
                                     self.projectFileName,
                                 )
 
-                                extension = "png"
                                 vframes = int((stop - start) * mediafile_fps + time_interval * mediafile_fps * 2)
-                                ffmpeg_command = (
-                                    f'"{self.ffmpeg_bin}" -ss {start:.3f} '
-                                    f'-i "{media_path}" '
-                                    f"-vframes {vframes} "
-                                    f'"{exportDir}{os.sep}'
-                                    f"{util.safeFileName(obsId)}"
-                                    f"_PLAYER{nplayer}"
-                                    f"_{util.safeFileName(subject)}"
-                                    f"_{util.safeFileName(behavior)}"
-                                    f'_{start:.3f}_%08d.{self.frame_bitmap_format.lower()}"'
-                                )
 
-                                logging.debug(f"ffmpeg command: {ffmpeg_command}")
+                            else:
+                                continue
 
-                                p = subprocess.Popen(
-                                    ffmpeg_command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True
-                                )
-                                out, _ = p.communicate()
+                        ffmpeg_command = (
+                            f'"{self.ffmpeg_bin}" '
+                            f"-ss {start:.3f} "
+                            f'-i "{media_path}" '
+                            f"-vframes {vframes} "
+                            f'"{exportDir}{os.sep}'
+                            f"{util.safeFileName(obsId).replace(' ', '-')}"
+                            f"_PLAYER{nplayer}"
+                            f"_{util.safeFileName(subject).replace(' ', '-')}"
+                            f"_{util.safeFileName(behavior).replace(' ', '-')}"
+                            f'_{start:.3f}_%08d.{self.frame_bitmap_format.lower()}"'
+                        )
+
+                        logging.debug(f"ffmpeg command: {ffmpeg_command}")
+
+                        p = subprocess.Popen(ffmpeg_command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
+                        out, _ = p.communicate()
 
 
 def extract_events(self):
     """
     extract sub-sequences from media files corresponding to coded events with FFmpeg
     in case of point event, from -n to +n seconds are extracted (n is asked to user)
     """
@@ -346,39 +329,39 @@
         out += "<br>".join(live_images_obs_list)
         results = dialog.Results_dialog()
         results.setWindowTitle(cfg.programName)
         results.ptText.setReadOnly(True)
         results.ptText.appendHtml(out)
         results.pbSave.setVisible(False)
         results.pbCancel.setVisible(True)
-        if not results.exec_():
+        if results.exec_():
+            # remove live observations
+            selected_observations = [x for x in selected_observations if x not in live_images_obs_list]
+            if not selected_observations:
+                return
+        else:
             return
 
-    # remove live observations
-    selected_observations = [x for x in selected_observations if x not in live_images_obs_list]
-    if not selected_observations:
+    # check if state events are paired
+    not_ok, selected_observations = project_functions.check_state_events(self.pj, selected_observations)
+    if not_ok or not selected_observations:
         return
 
     parameters = select_subj_behav.choose_obs_subj_behav_category(
         self,
         selected_observations,
         start_coding=dec("NaN"),
         end_coding=dec("NaN"),
         flagShowIncludeModifiers=False,
         flagShowExcludeBehaviorsWoEvents=False,
     )
 
     if not parameters[cfg.SELECTED_SUBJECTS] or not parameters[cfg.SELECTED_BEHAVIORS]:
         return
 
-    # check if state events are paired
-    not_ok, selected_observations = project_functions.check_state_events(self.pj, selected_observations)
-    if not_ok or not selected_observations:
-        return
-
     # Ask for time interval around the event
     while True:
         text, ok = QInputDialog.getDouble(
             self, "Time interval around the events", "Time (in seconds):", 0.0, 0.0, 86400, 1
         )
         if not ok:
             return
@@ -391,151 +374,155 @@
     # ask for video / audio extraction
     items_to_extract, ok = QInputDialog.getItem(
         self, "Tracks to extract", "Tracks", ("Video and audio", "Only video", "Only audio"), 0, False
     )
     if not ok:
         return
 
-    exportDir = QFileDialog().getExistingDirectory(
+    export_dir = QFileDialog().getExistingDirectory(
         self,
         "Choose a directory to extract events",
         os.path.expanduser("~"),
         options=QFileDialog(self).ShowDirsOnly,
     )
-    if not exportDir:
+    if not export_dir:
         return
 
     cursor = db_functions.load_events_in_db(
         self.pj,
         parameters[cfg.SELECTED_SUBJECTS],
         selected_observations,
         parameters[cfg.SELECTED_BEHAVIORS],
         time_interval=cfg.TIME_FULL_OBS,
     )
 
+    """
     ffmpeg_extract_command = (
         '"{ffmpeg_bin}" -i "{input_}" -y -ss {start} -to {stop} {codecs} '
         ' "{dir_}{sep}{obsId}_{player}_{subject}_{behavior}_{globalStart}'
         '-{globalStop}{extension}" '
     )
+    """
+    ffmpeg_extract_command = '"{ffmpeg_bin}" -ss {start} -i "{input_}" -y -t {duration} {codecs} '
+    mem_command = ""
+    for obs_id in selected_observations:
 
-    for obsId in selected_observations:
-
-        for nplayer in self.pj[cfg.OBSERVATIONS][obsId][cfg.FILE]:
+        for nplayer in self.pj[cfg.OBSERVATIONS][obs_id][cfg.FILE]:
 
-            if not self.pj[cfg.OBSERVATIONS][obsId][cfg.FILE][nplayer]:
+            if not self.pj[cfg.OBSERVATIONS][obs_id][cfg.FILE][nplayer]:
                 continue
 
             duration1 = []  # in seconds
-            for mediaFile in self.pj[cfg.OBSERVATIONS][obsId][cfg.FILE][nplayer]:
-                duration1.append(self.pj[cfg.OBSERVATIONS][obsId][cfg.MEDIA_INFO][cfg.LENGTH][mediaFile])
+            for mediaFile in self.pj[cfg.OBSERVATIONS][obs_id][cfg.FILE][nplayer]:
+                duration1.append(self.pj[cfg.OBSERVATIONS][obs_id][cfg.MEDIA_INFO][cfg.LENGTH][mediaFile])
 
             for subject in parameters[cfg.SELECTED_SUBJECTS]:
 
                 for behavior in parameters[cfg.SELECTED_BEHAVIORS]:
 
                     cursor.execute(
                         "SELECT occurence FROM events WHERE observation = ? AND subject = ? AND code = ?",
-                        (obsId, subject, behavior),
+                        (obs_id, subject, behavior),
                     )
                     rows = [{"occurence": util.float2decimal(r["occurence"])} for r in cursor.fetchall()]
 
                     behavior_state = project_functions.event_type(behavior, self.pj[cfg.ETHOGRAM])
                     if cfg.STATE in behavior_state and len(rows) % 2:  # unpaired events
                         continue
 
                     for idx, row in enumerate(rows):
 
                         mediaFileIdx = [
                             idx1 for idx1, x in enumerate(duration1) if row["occurence"] >= sum(duration1[0:idx1])
                         ][-1]
 
-                        # check if media has video
-                        try:
-                            if self.pj[cfg.OBSERVATIONS][obsId][cfg.MEDIA_INFO][cfg.HAS_VIDEO][
-                                self.pj[cfg.OBSERVATIONS][obsId][cfg.FILE][nplayer][mediaFileIdx]
-                            ]:
-                                codecs = "-acodec copy -vcodec copy"
-                                # extract extension from video file
-                                extension = pathlib.Path(
-                                    self.pj[cfg.OBSERVATIONS][obsId][cfg.FILE][nplayer][mediaFileIdx]
-                                ).suffix
-                                if not extension:
-                                    extension = ".mp4"
-                            else:
-                                codecs = "-vn"
-                                extension = ".wav"
-
-                                logging.debug(
-                                    f"Media {self.pj[cfg.OBSERVATIONS][obsId][cfg.FILE][nplayer][mediaFileIdx]} does not have video"
-                                )
+                        if "VIDEO" in items_to_extract.upper():
+                            # check if media has video
+                            has_video = False
+                            try:
+                                has_video = self.pj[cfg.OBSERVATIONS][obs_id][cfg.MEDIA_INFO][cfg.HAS_VIDEO][
+                                    self.pj[cfg.OBSERVATIONS][obs_id][cfg.FILE][nplayer][mediaFileIdx]
+                                ]
+                            except:
+                                has_video = False
+                            if not has_video:
+                                if (
+                                    dialog.MessageDialog(
+                                        cfg.programName,
+                                        f"The media file {self.pj[cfg.OBSERVATIONS][obs_id][cfg.FILE][nplayer][mediaFileIdx]} does not have a video stream",
+                                        ["Continue", "Abort"],
+                                    )
+                                    == "Abort"
+                                ):
+                                    return
+                                else:
+                                    continue
 
-                        except Exception:
+                            new_extension = ".mp4"
+                            if items_to_extract == "Only video":
+                                codecs = "-an"
+                            else:
+                                codecs = ""
 
-                            logging.debug(
-                                f"has_video not found for: {self.pj[cfg.OBSERVATIONS][obsId][cfg.FILE][nplayer][mediaFileIdx]}"
-                            )
+                        if items_to_extract == "Only audio":
+                            # check if media has audio
+                            has_audio = False
+                            try:
+                                has_audio = self.pj[cfg.OBSERVATIONS][obs_id][cfg.MEDIA_INFO][cfg.HAS_AUDIO][
+                                    self.pj[cfg.OBSERVATIONS][obs_id][cfg.FILE][nplayer][mediaFileIdx]
+                                ]
+                            except:
+                                has_audio = False
+                            if not has_audio:
 
-                            continue
+                                if (
+                                    dialog.MessageDialog(
+                                        cfg.programName,
+                                        f"The media file {self.pj[cfg.OBSERVATIONS][obs_id][cfg.FILE][nplayer][mediaFileIdx]} does not have an audio stream",
+                                        ["Continue", "Abort"],
+                                    )
+                                    == "Abort"
+                                ):
+                                    return
+                                else:
+                                    continue
 
-                        globalStart = (
-                            dec("0.000") if row["occurence"] < timeOffset else round(row["occurence"] - timeOffset, 3)
-                        )
-                        start = round(
-                            row["occurence"]
-                            - timeOffset
-                            - util.float2decimal(sum(duration1[0:mediaFileIdx]))
-                            - self.pj[cfg.OBSERVATIONS][obsId][cfg.TIME_OFFSET],
-                            3,
-                        )
-                        if start < timeOffset:
-                            start = dec("0.000")
+                            new_extension = ".wav"
+                            codecs = "-vn"
 
                         if cfg.POINT in behavior_state:
 
-                            globalStop = round(row["occurence"] + timeOffset, 3)
-
-                            stop = round(
+                            globalStart = (
+                                dec("0.000")
+                                if row["occurence"] < timeOffset
+                                else round(row["occurence"] - timeOffset, 3)
+                            )
+                            start = round(
                                 row["occurence"]
-                                + timeOffset
+                                - (timeOffset if timeOffset else 1)  # if time offset is not set default = 1 s
                                 - util.float2decimal(sum(duration1[0:mediaFileIdx]))
-                                - self.pj[cfg.OBSERVATIONS][obsId][cfg.TIME_OFFSET],
+                                - self.pj[cfg.OBSERVATIONS][obs_id][cfg.TIME_OFFSET],
                                 3,
                             )
+                            if start < timeOffset:
+                                start = dec("0.000")
 
-                            ffmpeg_command = ffmpeg_extract_command.format(
-                                ffmpeg_bin=self.ffmpeg_bin,
-                                input_=project_functions.full_path(
-                                    self.pj[cfg.OBSERVATIONS][obsId][cfg.FILE][nplayer][mediaFileIdx],
-                                    self.projectFileName,
-                                ),
-                                start=start,
-                                stop=stop,
-                                codecs=codecs,
-                                globalStart=globalStart,
-                                globalStop=globalStop,
-                                dir_=exportDir,
-                                sep=os.sep,
-                                obsId=util.safeFileName(obsId),
-                                player="PLAYER{}".format(nplayer),
-                                subject=util.safeFileName(subject),
-                                behavior=util.safeFileName(behavior),
-                                extension=extension,
-                            )
-
-                            logging.debug(f"ffmpeg command: {ffmpeg_command}")
+                            globalStop = round(row["occurence"] + timeOffset, 3)
 
-                            p = subprocess.Popen(
-                                ffmpeg_command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True
+                            stop = round(
+                                row["occurence"]
+                                + (timeOffset if timeOffset else 1)  # if time offset is not set default = 1 s
+                                - util.float2decimal(sum(duration1[0:mediaFileIdx]))
+                                - self.pj[cfg.OBSERVATIONS][obs_id][cfg.TIME_OFFSET],
+                                3,
                             )
-                            out, _ = p.communicate()
 
                         if cfg.STATE in behavior_state:
-                            if idx % 2 == 0:
 
+                            if idx % 2 == 0:
                                 # check if stop is on same media file
                                 if (
                                     mediaFileIdx
                                     != [
                                         idx1
                                         for idx1, x in enumerate(duration1)
                                         if rows[idx + 1]["occurence"] >= sum(duration1[0:idx1])
@@ -550,50 +537,81 @@
                                         [cfg.OK, "Abort"],
                                     )
                                     if response == cfg.OK:
                                         continue
                                     if response == "Abort":
                                         return
 
+                                globalStart = (
+                                    dec("0.000")
+                                    if row["occurence"] < timeOffset
+                                    else round(row["occurence"] - timeOffset, 3)
+                                )
+                                start = round(
+                                    row["occurence"]
+                                    - timeOffset
+                                    - util.float2decimal(sum(duration1[0:mediaFileIdx]))
+                                    - self.pj[cfg.OBSERVATIONS][obs_id][cfg.TIME_OFFSET],
+                                    3,
+                                )
+                                if start < timeOffset:
+                                    start = dec("0.000")
+
                                 globalStop = round(rows[idx + 1]["occurence"] + timeOffset, 3)
 
                                 stop = round(
                                     rows[idx + 1]["occurence"]
                                     + timeOffset
-                                    - util.float2decimal(sum(duration1[0:mediaFileIdx])),
+                                    - util.float2decimal(sum(duration1[0:mediaFileIdx]))
+                                    - self.pj[cfg.OBSERVATIONS][obs_id][cfg.TIME_OFFSET],
                                     3,
                                 )
 
                                 # check if start after length of media
                                 if (
                                     start
-                                    > self.pj[cfg.OBSERVATIONS][obsId][cfg.MEDIA_INFO][cfg.LENGTH][
-                                        self.pj[cfg.OBSERVATIONS][obsId][cfg.FILE][nplayer][mediaFileIdx]
+                                    > self.pj[cfg.OBSERVATIONS][obs_id][cfg.MEDIA_INFO][cfg.LENGTH][
+                                        self.pj[cfg.OBSERVATIONS][obs_id][cfg.FILE][nplayer][mediaFileIdx]
                                     ]
                                 ):
                                     continue
 
-                                ffmpeg_command = ffmpeg_extract_command.format(
-                                    ffmpeg_bin=self.ffmpeg_bin,
-                                    input_=project_functions.full_path(
-                                        self.pj[cfg.OBSERVATIONS][obsId][cfg.FILE][nplayer][mediaFileIdx],
-                                        self.projectFileName,
-                                    ),
-                                    start=start,
-                                    stop=stop,
-                                    codecs=codecs,
-                                    globalStart=globalStart,
-                                    globalStop=globalStop,
-                                    dir_=exportDir,
-                                    sep=os.sep,
-                                    obsId=util.safeFileName(obsId),
-                                    player=f"PLAYER{nplayer}",
-                                    subject=util.safeFileName(subject),
-                                    behavior=util.safeFileName(behavior),
-                                    extension=extension,
-                                )
+                            else:
+                                continue
 
-                                logging.debug("ffmpeg command: {}".format(ffmpeg_command))
-                                p = subprocess.Popen(
-                                    ffmpeg_command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True
+                        new_file_name = pl.Path(export_dir) / pl.Path(
+                            f"{util.safeFileName(obs_id).replace(' ', '-')}_PLAYER{nplayer}_{util.safeFileName(subject).replace(' ', '-')}_{util.safeFileName(behavior)}_{globalStart}-{globalStop}"
+                        ).with_suffix(new_extension)
+                        if new_file_name.is_file():
+                            if mem_command not in (cfg.OVERWRITE_ALL, cfg.SKIP_ALL):
+                                mem_command = dialog.MessageDialog(
+                                    cfg.programName,
+                                    f"The file <b>{new_file_name}</b> already exists.",
+                                    [cfg.OVERWRITE, cfg.OVERWRITE_ALL, cfg.SKIP, cfg.SKIP_ALL, cfg.CANCEL],
                                 )
-                                out, error = p.communicate()
+                            if mem_command == cfg.CANCEL:
+                                return
+                            if "SKIP" in mem_command.upper():
+                                continue
+
+                        ffmpeg_command = ffmpeg_extract_command.format(
+                            ffmpeg_bin=self.ffmpeg_bin,
+                            input_=project_functions.full_path(
+                                self.pj[cfg.OBSERVATIONS][obs_id][cfg.FILE][nplayer][mediaFileIdx],
+                                self.projectFileName,
+                            ),
+                            start=start,
+                            duration=stop - start,
+                            codecs=codecs,
+                        )
+
+                        logging.debug(f"ffmpeg command: {ffmpeg_command} '{new_file_name}'")
+
+                        p = subprocess.Popen(
+                            f"{ffmpeg_command} '{new_file_name}'",
+                            stdout=subprocess.PIPE,
+                            stderr=subprocess.PIPE,
+                            shell=True,
+                        )
+                        out, _ = p.communicate()
+
+    self.statusbar.showMessage(f"Media sequence extracted in {export_dir}", 0)
```

### Comparing `boris-behav-obs-8.9.6/boris/exclusion_matrix.py` & `boris-behav-obs-8.9.8/boris/exclusion_matrix.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/export_events.py` & `boris-behav-obs-8.9.8/boris/export_events.py`

 * *Files 0% similar despite different names*

```diff
@@ -764,15 +764,14 @@
         )
 
         cursor = db_functions.load_events_in_db(
             self.pj,
             parameters[cfg.SELECTED_SUBJECTS],
             selected_observations,
             parameters[cfg.SELECTED_BEHAVIORS],
-            time_interval=cfg.TIME_FULL_OBS,
         )
 
         cursor.execute(
             (
                 "SELECT COUNT(DISTINCT subject) FROM events "
                 "WHERE observation = ? AND subject IN ({}) AND type = 'STATE' ".format(
                     ",".join(["?"] * len(parameters[cfg.SELECTED_SUBJECTS]))
@@ -794,15 +793,18 @@
             "tiers? <exists>\n"
             f"size = {subjectsNum}\n"
             "item []:\n"
         )
 
         subject_index = 0
         for subject in parameters[cfg.SELECTED_SUBJECTS]:
-            if subject not in [x[cfg.EVENT_SUBJECT_FIELD_IDX] for x in self.pj[cfg.OBSERVATIONS][obs_id][cfg.EVENTS]]:
+            if subject not in [
+                x[cfg.EVENT_SUBJECT_FIELD_IDX] if x[cfg.EVENT_SUBJECT_FIELD_IDX] else cfg.NO_FOCAL_SUBJECT
+                for x in self.pj[cfg.OBSERVATIONS][obs_id][cfg.EVENTS]
+            ]:
                 continue
 
             intervalsMin, intervalsMax = 0, total_media_duration
 
             # STATE events
             cursor.execute(
                 (
```

### Comparing `boris-behav-obs-8.9.6/boris/export_observation.py` & `boris-behav-obs-8.9.8/boris/export_observation.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/geometric_measurement.py` & `boris-behav-obs-8.9.8/boris/geometric_measurement.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/gui_utilities.py` & `boris-behav-obs-8.9.8/boris/gui_utilities.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/icons/logo_eye.ico` & `boris-behav-obs-8.9.8/boris/icons/logo_eye.ico`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/image_overlay.py` & `boris-behav-obs-8.9.8/boris/image_overlay.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/import_observations.py` & `boris-behav-obs-8.9.8/boris/import_observations.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/irr.py` & `boris-behav-obs-8.9.8/boris/irr.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/latency.py` & `boris-behav-obs-8.9.8/boris/latency.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/map_creator.py` & `boris-behav-obs-8.9.8/boris/map_creator.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/media_file.py` & `boris-behav-obs-8.9.8/boris/media_file.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/menu_options.py` & `boris-behav-obs-8.9.8/boris/menu_options.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/modifiers_coding_map.py` & `boris-behav-obs-8.9.8/boris/modifiers_coding_map.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/mpv.py` & `boris-behav-obs-8.9.8/boris/mpv.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/mpv2.py` & `boris-behav-obs-8.9.8/boris/mpv2.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/observation.py` & `boris-behav-obs-8.9.8/boris/observation.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/observation.ui` & `boris-behav-obs-8.9.8/boris/observation.ui`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/observation_operations.py` & `boris-behav-obs-8.9.8/boris/observation_operations.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/observation_ui.py` & `boris-behav-obs-8.9.8/boris/observation_ui.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/observations_list.py` & `boris-behav-obs-8.9.8/boris/observations_list.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/otx_parser.py` & `boris-behav-obs-8.9.8/boris/otx_parser.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/param_panel.py` & `boris-behav-obs-8.9.8/boris/param_panel.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/param_panel.ui` & `boris-behav-obs-8.9.8/boris/param_panel.ui`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/param_panel_ui.py` & `boris-behav-obs-8.9.8/boris/param_panel_ui.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/player_dock_widget.py` & `boris-behav-obs-8.9.8/boris/player_dock_widget.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/plot_data_module.py` & `boris-behav-obs-8.9.8/boris/plot_data_module.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/plot_events.py` & `boris-behav-obs-8.9.8/boris/plot_events.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/plot_events_rt.py` & `boris-behav-obs-8.9.8/boris/plot_events_rt.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/plot_spectrogram_rt.py` & `boris-behav-obs-8.9.8/boris/plot_spectrogram_rt.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/plot_waveform_rt.py` & `boris-behav-obs-8.9.8/boris/plot_waveform_rt.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/portion/__init__.py` & `boris-behav-obs-8.9.8/boris/portion/__init__.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/portion/const.py` & `boris-behav-obs-8.9.8/boris/portion/const.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/portion/dict.py` & `boris-behav-obs-8.9.8/boris/portion/dict.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/portion/func.py` & `boris-behav-obs-8.9.8/boris/portion/func.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/portion/interval.py` & `boris-behav-obs-8.9.8/boris/portion/interval.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/portion/io.py` & `boris-behav-obs-8.9.8/boris/portion/io.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/preferences.py` & `boris-behav-obs-8.9.8/boris/preferences.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/preferences.ui` & `boris-behav-obs-8.9.8/boris/preferences.ui`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/preferences_ui.py` & `boris-behav-obs-8.9.8/boris/preferences_ui.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/project.py` & `boris-behav-obs-8.9.8/boris/project.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/project.ui` & `boris-behav-obs-8.9.8/boris/project.ui`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/project_functions.py` & `boris-behav-obs-8.9.8/boris/project_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -549,15 +549,15 @@
     cursor = db_connector.cursor()
     flag_ok = True
     msg = ""
     mem_command = ""
     for obs_id in selected_observations:
         if pj[cfg.OBSERVATIONS][obs_id][cfg.TYPE] == cfg.LIVE:
             out = ""
-            if parameters["time"] in ("limit to events", "full obs"):
+            if parameters["time"] in (cfg.TIME_EVENTS, cfg.TIME_FULL_OBS):
                 cursor.execute(
                     (
                         "SELECT subject, behavior, start, stop, type, modifiers FROM aggregated_events "
                         "WHERE observation = ? "
                         "AND subject in ({}) "
                         "AND behavior in ({}) "
                         "ORDER BY start"
@@ -568,15 +568,15 @@
                     [
                         obs_id,
                     ]
                     + parameters[cfg.SELECTED_SUBJECTS]
                     + parameters[cfg.SELECTED_BEHAVIORS],
                 )
 
-            else:  # 'time interval'
+            else:  # arbitrary 'time interval'
                 cursor.execute(
                     (
                         "SELECT subject, behavior, start, stop, type, modifiers FROM aggregated_events "
                         "WHERE observation = ? "
                         "AND (start BETWEEN ? AND ?) "
                         "AND subject in ({}) "
                         "AND behavior in ({}) "
@@ -640,15 +640,15 @@
                 for media_file in pj[cfg.OBSERVATIONS][obs_id][cfg.FILE][nplayer]:
                     try:
                         end = init + pj[cfg.OBSERVATIONS][obs_id][cfg.MEDIA_INFO][cfg.LENGTH][media_file]
                     except KeyError:
                         return False, f"The length for media file {media_file} is not available"
                     out = ""
 
-                    if parameters["time"] in ("limit to events", "full obs"):
+                    if parameters["time"] in (cfg.TIME_EVENTS, cfg.TIME_FULL_OBS):
                         cursor.execute(
                             (
                                 "SELECT subject, behavior, start, stop, type, modifiers FROM aggregated_events "
                                 "WHERE observation = ? "
                                 "AND (start BETWEEN ? AND ?) "
                                 "AND subject in ({}) "
                                 "AND behavior in ({}) "
@@ -662,15 +662,15 @@
                                 init,
                                 end,
                             ]
                             + parameters[cfg.SELECTED_SUBJECTS]
                             + parameters[cfg.SELECTED_BEHAVIORS],
                         )
 
-                    else:
+                    else:  # arbitrary 'time interval'
 
                         cursor.execute(
                             (
                                 "SELECT subject, behavior, type, start, stop, modifiers FROM aggregated_events "
                                 "WHERE observation = ? "
                                 "AND (start BETWEEN ? AND ?) "
                                 "AND (start BETWEEN ? AND ?) "
```

### Comparing `boris-behav-obs-8.9.6/boris/project_import_export.py` & `boris-behav-obs-8.9.8/boris/project_import_export.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/project_server.py` & `boris-behav-obs-8.9.8/boris/project_server.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/project_ui.py` & `boris-behav-obs-8.9.8/boris/project_ui.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/select_modifiers.py` & `boris-behav-obs-8.9.8/boris/select_modifiers.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/select_observations.py` & `boris-behav-obs-8.9.8/boris/select_observations.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/select_subj_behav.py` & `boris-behav-obs-8.9.8/boris/select_subj_behav.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/state_events.py` & `boris-behav-obs-8.9.8/boris/state_events.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/subjects_pad.py` & `boris-behav-obs-8.9.8/boris/subjects_pad.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/synthetic_time_budget.py` & `boris-behav-obs-8.9.8/boris/synthetic_time_budget.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/time_budget_functions.py` & `boris-behav-obs-8.9.8/boris/time_budget_functions.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/time_budget_widget.py` & `boris-behav-obs-8.9.8/boris/time_budget_widget.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/transitions.py` & `boris-behav-obs-8.9.8/boris/transitions.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/utilities.py` & `boris-behav-obs-8.9.8/boris/utilities.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/version.py` & `boris-behav-obs-8.9.8/boris/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,9 +16,9 @@
   GNU General Public License for more details.
 
   You should have received a copy of the GNU General Public License
   along with this program; if not see <http://www.gnu.org/licenses/>.
 
 """
 
-__version__ = "8.9.6"
-__version_date__ = "BETA 2022-12-01"
+__version__ = "8.9.8"
+__version_date__ = "BETA 2022-12-13"
```

### Comparing `boris-behav-obs-8.9.6/boris/video_equalizer.py` & `boris-behav-obs-8.9.8/boris/video_equalizer.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/video_equalizer_ui.py` & `boris-behav-obs-8.9.8/boris/video_equalizer_ui.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris/video_operations.py` & `boris-behav-obs-8.9.8/boris/video_operations.py`

 * *Files identical despite different names*

### Comparing `boris-behav-obs-8.9.6/boris_behav_obs.egg-info/PKG-INFO` & `boris-behav-obs-8.9.8/boris_behav_obs.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,116 +1,119 @@
 Metadata-Version: 2.1
 Name: boris-behav-obs
-Version: 8.9.6
+Version: 8.9.8
 Summary: BORIS - Behavioral Observation Research Interactive Software
 Home-page: http://www.boris.unito.it
 Author: Olivier Friard - Marco Gamba
 Author-email: olivier.friard@unito.it
 License: UNKNOWN
 Project-URL: Documentation, https://boris.readthedocs.io/en/latest/
 Project-URL: Changelog, https://github.com/olivierfriard/BORIS/wiki/BORIS-change-log-v.8
 Project-URL: Source code, https://github.com/olivierfriard/BORIS
 Project-URL: Issues, https://github.com/olivierfriard/BORIS/issues
-Description: ===============================================================
-        Behavioral Observation Research Interactive Software (BORIS)
-        ===============================================================
-        
-        BORIS is an easy-to-use event logging software for video/audio coding or live observations.
-        
-        BORIS is a free and open-source software available for GNU/Linux and Windows.
-        
-        It provides also some analysis tools like time budget.
-        
-        The BORIS paper has more than `1000 citations in peer-reviewed scientific publications <http://www.boris.unito.it/pages/citations.html>`_.
-        
-        See http://www.boris.unito.it
-        
-        
-        .. image:: https://img.shields.io/badge/Made%20with-Python-1f425f.svg
-         :target: https://www.python.org/
-        
-        .. image:: https://static.pepy.tech/personalized-badge/boris-behav-obs?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads
-         :target: https://pepy.tech/project/boris-behav-obs
-        
-        
-        
-        
-        
-        
-        Documentation
-        -------------------------------------
-        
-        The official documentation is hosted here:
-        http://boris.readthedocs.io/
-        
-        The documentation provides a good starting point for learning how to use BORIS.
-        
-        Some video tutorials are available:
-        https://www.youtube.com/channel/UCo-Jyvzawwp0bRMEor4aLVQ
-        
-        
-        
-        
-        
-        Bug reports and feature requests
-        --------------------------------------
-        
-        To search for bugs, report them or request a feature, please use the github tracker:
-        https://github.com/olivierfriard/BORIS/issues
-        
-        
-        
-        
-        
-        Citing BORIS
-        --------------------------------------
-        
-        Please acknowledge and cite the use of this software and its authors when
-        results are used in publications or published elsewhere. You can use the
-        following BibTex entry
-        
-        ::
-        
-            @article {MEE3:MEE312584,
-            author = {Friard, Olivier and Gamba, Marco},
-            title = {BORIS: a free, versatile open-source event-logging software for video/audio coding and live observations},
-            journal = {Methods in Ecology and Evolution},
-            issn = {2041-210X},
-            url = {http://dx.doi.org/10.1111/2041-210X.12584},
-            doi = {10.1111/2041-210X.12584},
-            pages = {1324--1330},
-            keywords = {behavioural analysis, behaviour coding, coding scheme, ethology, observational data, ttime-budget},
-            year = {2016},
-            }
-        
-        
-        
-        
-        
-        
-        
-        
-        
-        Licence
-        -----------------------------
-        
-        Distributed with a `GPL v.3 license <LICENSE.TXT>`_
-        
-        
-        Copyright (C) 2012-2022 Olivier Friard
-        
-        
-        
-        
-        
 Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
+License-File: LICENSE.TXT
+
+===============================================================
+Behavioral Observation Research Interactive Software (BORIS)
+===============================================================
+
+BORIS is an easy-to-use event logging software for video/audio coding or live observations.
+
+BORIS is a free and open-source software available for GNU/Linux and Windows.
+
+It provides also some analysis tools like time budget.
+
+The BORIS paper has more than `1000 citations in peer-reviewed scientific publications <http://www.boris.unito.it/pages/citations.html>`_.
+
+See http://www.boris.unito.it
+
+
+.. image:: https://img.shields.io/badge/Made%20with-Python-1f425f.svg
+ :target: https://www.python.org/
+
+.. image:: https://static.pepy.tech/personalized-badge/boris-behav-obs?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads
+ :target: https://pepy.tech/project/boris-behav-obs
+
+
+
+
+
+
+Documentation
+-------------------------------------
+
+The official documentation is hosted here:
+http://boris.readthedocs.io/
+
+The documentation provides a good starting point for learning how to use BORIS.
+
+Some video tutorials are available:
+https://www.youtube.com/channel/UCo-Jyvzawwp0bRMEor4aLVQ
+
+
+
+
+
+Bug reports and feature requests
+--------------------------------------
+
+To search for bugs, report them or request a feature, please use the github tracker:
+https://github.com/olivierfriard/BORIS/issues
+
+
+
+
+
+Citing BORIS
+--------------------------------------
+
+Please acknowledge and cite the use of this software and its authors when
+results are used in publications or published elsewhere. You can use the
+following BibTex entry
+
+::
+
+    @article {MEE3:MEE312584,
+    author = {Friard, Olivier and Gamba, Marco},
+    title = {BORIS: a free, versatile open-source event-logging software for video/audio coding and live observations},
+    journal = {Methods in Ecology and Evolution},
+    issn = {2041-210X},
+    url = {http://dx.doi.org/10.1111/2041-210X.12584},
+    doi = {10.1111/2041-210X.12584},
+    pages = {1324--1330},
+    keywords = {behavioural analysis, behaviour coding, coding scheme, ethology, observational data, ttime-budget},
+    year = {2016},
+    }
+
+
+
+
+
+
+
+
+
+Licence
+-----------------------------
+
+Distributed with a `GPL v.3 license <LICENSE.TXT>`_
+
+
+Copyright (C) 2012-2022 Olivier Friard
+
+
+
+
+
+
```

### Comparing `boris-behav-obs-8.9.6/boris_behav_obs.egg-info/SOURCES.txt` & `boris-behav-obs-8.9.8/boris_behav_obs.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 boris/converters_ui.py
 boris/core.py
 boris/core.qrc
 boris/core.ui
 boris/core_qrc.py
 boris/core_ui.py
 boris/db_functions.py
-boris/dev.py
 boris/dialog.py
 boris/duration_widget.py
 boris/edit_event.py
 boris/edit_event.ui
 boris/edit_event_ui.py
 boris/event_operations.py
 boris/events_cursor.py
```

### Comparing `boris-behav-obs-8.9.6/setup.py` & `boris-behav-obs-8.9.8/setup.py`

 * *Files identical despite different names*

