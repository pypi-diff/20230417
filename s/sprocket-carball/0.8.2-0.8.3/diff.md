# Comparing `tmp/sprocket_carball-0.8.2.tar.gz` & `tmp/sprocket_carball-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sprocket_carball-0.8.2.tar", last modified: Sun Apr 16 23:09:39 2023, max compression
+gzip compressed data, was "sprocket_carball-0.8.3.tar", last modified: Sun Apr 16 23:13:01 2023, max compression
```

## Comparing `sprocket_carball-0.8.2.tar` & `sprocket_carball-0.8.3.tar`

### file list

```diff
@@ -1,258 +1,258 @@
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:09:39.073509 sprocket_carball-0.8.2/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        2 2023-04-16 06:27:02.000000 sprocket_carball-0.8.2/CARBALL_VERSION
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    11357 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/LICENSE
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      198 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/MANIFEST.in
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      552 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/NOTICE
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     6396 2023-04-16 23:09:39.073509 sprocket_carball-0.8.2/PKG-INFO
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     6039 2023-04-16 06:26:08.000000 sprocket_carball-0.8.2/README.md
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:09:39.009509 sprocket_carball-0.8.2/carball/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      223 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:09:39.009509 sprocket_carball-0.8.2/carball/analysis/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        2 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/PROTOBUF_VERSION
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    17254 2023-04-16 06:18:49.000000 sprocket_carball-0.8.2/carball/analysis/analysis_manager.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:09:39.009509 sprocket_carball-0.8.2/carball/analysis/cleaner/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/cleaner/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1383 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/cleaner/cleaner.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2295 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/cleaner/frame_cleaner.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:09:39.013509 sprocket_carball-0.8.2/carball/analysis/constants/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/constants/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      815 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/constants/basic_math.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     5721 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/constants/dropshot.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     6198 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/constants/field_constants.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1187 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/constants/playlist.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:09:39.013509 sprocket_carball-0.8.2/carball/analysis/events/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/events/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:09:39.013509 sprocket_carball-0.8.2/carball/analysis/events/boost_pad_detection/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/events/boost_pad_detection/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3707 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/events/boost_pad_detection/pickup_analysis.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:09:39.013509 sprocket_carball-0.8.2/carball/analysis/events/bump_detection/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/events/bump_detection/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1277 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/events/bump_detection/bump_analysis.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    15118 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/events/carry_detection.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:09:39.013509 sprocket_carball-0.8.2/carball/analysis/events/dropshot/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/events/dropshot/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1386 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/events/dropshot/ball.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      935 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/events/dropshot/damage.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     5568 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/events/event_creator.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:09:39.013509 sprocket_carball-0.8.2/carball/analysis/events/fifty_fifty/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/events/fifty_fifty/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     7419 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/events/fifty_fifty/fifty_analysis.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:09:39.017509 sprocket_carball-0.8.2/carball/analysis/events/hit_detection/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/events/hit_detection/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    11653 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/events/hit_detection/base_hit.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    11223 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/events/hit_detection/hit_analysis.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:09:39.017509 sprocket_carball-0.8.2/carball/analysis/events/hit_detection/hitbox/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    41555 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/events/hit_detection/hitbox/Vehicle Specifications v1.39 - Hitboxes, Handling.xlsx
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/events/hit_detection/hitbox/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1662 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/events/hit_detection/hitbox/car.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1973 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/events/hit_detection/hitbox/hitbox.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:09:39.017509 sprocket_carball-0.8.2/carball/analysis/events/hit_pressure/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/events/hit_pressure/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3373 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/events/hit_pressure/pressure_analysis.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:09:39.017509 sprocket_carball-0.8.2/carball/analysis/events/kickoff_detection/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/events/kickoff_detection/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    10002 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/events/kickoff_detection/kickoff_analysis.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:09:39.017509 sprocket_carball-0.8.2/carball/analysis/saltie_game/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/saltie_game/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:09:39.021509 sprocket_carball-0.8.2/carball/analysis/saltie_game/metadata/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      459 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/saltie_game/metadata/ApiDemo.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2531 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/saltie_game/metadata/ApiGame.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      383 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/saltie_game/metadata/ApiGoal.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      479 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/saltie_game/metadata/ApiMutators.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1473 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/saltie_game/metadata/ApiPlayer.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1406 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/saltie_game/metadata/ApiPlayerCameraSettings.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3124 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/saltie_game/metadata/ApiPlayerLoadout.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      681 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/saltie_game/metadata/ApiTeam.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/saltie_game/metadata/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     4703 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/saltie_game/saltie_game.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:09:39.025509 sprocket_carball-0.8.2/carball/analysis/simulator/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/simulator/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    11609 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/simulator/ball_simulator.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      855 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/simulator/bounce.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      238 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/simulator/map_constants.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:09:39.025509 sprocket_carball-0.8.2/carball/analysis/stats/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/stats/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:09:39.025509 sprocket_carball-0.8.2/carball/analysis/stats/ball_forward/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/stats/ball_forward/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1023 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/stats/ball_forward/distance_hit_ball_forward.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:09:39.025509 sprocket_carball-0.8.2/carball/analysis/stats/boost/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/stats/boost/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     6918 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/stats/boost/boost.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:09:39.025509 sprocket_carball-0.8.2/carball/analysis/stats/controls/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/stats/controls/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2829 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/stats/controls/controls.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:09:39.025509 sprocket_carball-0.8.2/carball/analysis/stats/demos/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/stats/demos/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1623 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/stats/demos/demos.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:09:39.029509 sprocket_carball-0.8.2/carball/analysis/stats/dribbles/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/stats/dribbles/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3342 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/stats/dribbles/ball_carry.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:09:39.029509 sprocket_carball-0.8.2/carball/analysis/stats/dropshot/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      343 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/stats/dropshot/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2082 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/stats/dropshot/ball_phase_times.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3902 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/stats/dropshot/damage.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2575 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/stats/dropshot/goals.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:09:39.029509 sprocket_carball-0.8.2/carball/analysis/stats/kickoffs/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/stats/kickoffs/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2211 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/stats/kickoffs/kickoff_stat.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:09:39.029509 sprocket_carball-0.8.2/carball/analysis/stats/possession/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/stats/possession/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3521 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/stats/possession/ball_distances.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    10214 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/stats/possession/per_possession.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2982 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/stats/possession/possession.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2243 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/stats/possession/turnovers.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:09:39.033509 sprocket_carball-0.8.2/carball/analysis/stats/rumble/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/stats/rumble/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3475 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/stats/rumble/goals.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     8977 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/stats/rumble/rumble.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     4033 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/stats/stats.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3336 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/stats/stats_list.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3851 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/stats/stats_manager.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:09:39.033509 sprocket_carball-0.8.2/carball/analysis/stats/tendencies/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/stats/tendencies/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1330 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/stats/tendencies/averages.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1583 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/stats/tendencies/hit_counts.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     6969 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/stats/tendencies/positional_tendencies.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2777 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/stats/tendencies/relative_position_tendencies.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1962 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/stats/tendencies/speed_tendencies.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     6502 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/stats/tendencies/team_tendencies.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:09:39.033509 sprocket_carball-0.8.2/carball/analysis/stats/utils/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/stats/utils/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1708 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/stats/utils/pandas_utils.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:09:39.037509 sprocket_carball-0.8.2/carball/analysis/utils/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/utils/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      316 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/utils/json_encoder.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1974 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/utils/numpy_manager.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2050 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/utils/pandas_manager.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      374 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/utils/proto_manager.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1265 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/analysis/utils/split_location.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2558 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/command_line.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:09:39.037509 sprocket_carball-0.8.2/carball/controls/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/controls/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2203 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/controls/controls.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3427 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/controls/rotations.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2568 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/decompile_replays.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:09:39.037509 sprocket_carball-0.8.2/carball/extras/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/extras/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1770 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/extras/per_goal_analysis.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:09:39.001509 sprocket_carball-0.8.2/carball/generated/
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:09:39.041509 sprocket_carball-0.8.2/carball/generated/api/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 06:27:31.000000 sprocket_carball-0.8.2/carball/generated/api/__init__.py
--rw-------   0 jacbaile  (1000) jacbaile  (1000)     5076 2023-04-16 06:27:31.000000 sprocket_carball-0.8.2/carball/generated/api/game_pb2.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:09:39.041509 sprocket_carball-0.8.2/carball/generated/api/metadata/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 06:27:31.000000 sprocket_carball-0.8.2/carball/generated/api/metadata/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     4653 2023-04-16 06:27:31.000000 sprocket_carball-0.8.2/carball/generated/api/metadata/camera_settings_pb2.py
--rw-------   0 jacbaile  (1000) jacbaile  (1000)    19305 2023-04-16 06:27:31.000000 sprocket_carball-0.8.2/carball/generated/api/metadata/game_metadata_pb2.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3635 2023-04-16 06:27:31.000000 sprocket_carball-0.8.2/carball/generated/api/metadata/mutators_pb2.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    12482 2023-04-16 06:27:31.000000 sprocket_carball-0.8.2/carball/generated/api/metadata/player_loadout_pb2.py
--rw-------   0 jacbaile  (1000) jacbaile  (1000)     2397 2023-04-16 06:27:31.000000 sprocket_carball-0.8.2/carball/generated/api/party_pb2.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1793 2023-04-16 06:27:31.000000 sprocket_carball-0.8.2/carball/generated/api/player_id_pb2.py
--rw-------   0 jacbaile  (1000) jacbaile  (1000)     8237 2023-04-16 06:27:31.000000 sprocket_carball-0.8.2/carball/generated/api/player_pb2.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:09:39.045509 sprocket_carball-0.8.2/carball/generated/api/stats/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 06:27:31.000000 sprocket_carball-0.8.2/carball/generated/api/stats/__init__.py
--rw-------   0 jacbaile  (1000) jacbaile  (1000)     3714 2023-04-16 06:27:31.000000 sprocket_carball-0.8.2/carball/generated/api/stats/ball_stats_pb2.py
--rw-------   0 jacbaile  (1000) jacbaile  (1000)     1383 2023-04-16 06:27:31.000000 sprocket_carball-0.8.2/carball/generated/api/stats/data_frame_pb2.py
--rw-------   0 jacbaile  (1000) jacbaile  (1000)    18134 2023-04-16 06:27:31.000000 sprocket_carball-0.8.2/carball/generated/api/stats/dropshot_pb2.py
--rw-------   0 jacbaile  (1000) jacbaile  (1000)    31534 2023-04-16 06:27:31.000000 sprocket_carball-0.8.2/carball/generated/api/stats/events_pb2.py
--rw-------   0 jacbaile  (1000) jacbaile  (1000)     5766 2023-04-16 06:27:31.000000 sprocket_carball-0.8.2/carball/generated/api/stats/extra_mode_stats_pb2.py
--rw-------   0 jacbaile  (1000) jacbaile  (1000)     6701 2023-04-16 06:27:31.000000 sprocket_carball-0.8.2/carball/generated/api/stats/game_stats_pb2.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1837 2023-04-16 06:27:31.000000 sprocket_carball-0.8.2/carball/generated/api/stats/goal_pb2.py
--rw-------   0 jacbaile  (1000) jacbaile  (1000)    18809 2023-04-16 06:27:31.000000 sprocket_carball-0.8.2/carball/generated/api/stats/kickoff_pb2.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     7823 2023-04-16 06:27:31.000000 sprocket_carball-0.8.2/carball/generated/api/stats/per_possession_stats_pb2.py
--rw-------   0 jacbaile  (1000) jacbaile  (1000)    34767 2023-04-16 06:27:31.000000 sprocket_carball-0.8.2/carball/generated/api/stats/player_stats_pb2.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     7450 2023-04-16 06:27:31.000000 sprocket_carball-0.8.2/carball/generated/api/stats/rumble_pb2.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    21715 2023-04-16 06:27:31.000000 sprocket_carball-0.8.2/carball/generated/api/stats/stats_pb2.py
--rw-------   0 jacbaile  (1000) jacbaile  (1000)     7909 2023-04-16 06:27:31.000000 sprocket_carball-0.8.2/carball/generated/api/stats/team_stats_pb2.py
--rw-------   0 jacbaile  (1000) jacbaile  (1000)     3568 2023-04-16 06:27:31.000000 sprocket_carball-0.8.2/carball/generated/api/team_pb2.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:09:39.049509 sprocket_carball-0.8.2/carball/generated/binaries/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 06:27:31.000000 sprocket_carball-0.8.2/carball/generated/binaries/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:09:39.049509 sprocket_carball-0.8.2/carball/json_parser/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/json_parser/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:09:39.053509 sprocket_carball-0.8.2/carball/json_parser/actor/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      435 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/json_parser/actor/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1649 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/json_parser/actor/ball.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1210 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/json_parser/actor/base.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     4316 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/json_parser/actor/boost.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1053 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/json_parser/actor/camera.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3497 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/json_parser/actor/car.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1719 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/json_parser/actor/dropshot.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1034 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/json_parser/actor/game_event.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      388 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/json_parser/actor/game_info.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1386 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/json_parser/actor/jump.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     4207 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/json_parser/actor/player.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1122 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/json_parser/actor/rumble.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      466 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/json_parser/actor/team.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3761 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/json_parser/actor_parsing.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1374 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/json_parser/bots.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2021 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/json_parser/dropshot.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    12747 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/json_parser/frame_parser.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    13147 2023-04-16 06:04:04.000000 sprocket_carball-0.8.2/carball/json_parser/game.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1614 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/json_parser/game_info.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      932 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/json_parser/goal.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    11640 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/json_parser/player.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:09:39.057509 sprocket_carball-0.8.2/carball/json_parser/sanity_check/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/json_parser/sanity_check/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:09:39.057509 sprocket_carball-0.8.2/carball/json_parser/sanity_check/base_checks/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/json_parser/sanity_check/base_checks/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1261 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/json_parser/sanity_check/base_checks/base_check.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      117 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/json_parser/sanity_check/base_checks/game_check.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      298 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/json_parser/sanity_check/base_checks/player_check.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:09:39.057509 sprocket_carball-0.8.2/carball/json_parser/sanity_check/checks/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/json_parser/sanity_check/checks/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      496 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/json_parser/sanity_check/checks/ball_data_frame_check.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1037 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/json_parser/sanity_check/checks/player_attributes_check.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      813 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/json_parser/sanity_check/checks/player_data_frame_check.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:09:39.057509 sprocket_carball-0.8.2/carball/json_parser/sanity_check/errors/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/json_parser/sanity_check/errors/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      275 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/json_parser/sanity_check/errors/errors.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1459 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/json_parser/sanity_check/sanity_check.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1195 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/json_parser/team.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:09:39.061509 sprocket_carball-0.8.2/carball/tests/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/tests/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3666 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/tests/analysis_test.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:09:39.061509 sprocket_carball-0.8.2/carball/tests/benchmarking/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/tests/benchmarking/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1577 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/tests/benchmarking/benchmarking.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      124 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/tests/conftest.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:09:39.061509 sprocket_carball-0.8.2/carball/tests/docs/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/tests/docs/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1610 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/tests/docs/data_frame_docs.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2641 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/tests/export_test.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2791 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/tests/game_creation_test.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:09:39.065509 sprocket_carball-0.8.2/carball/tests/metadata/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/tests/metadata/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1100 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/tests/metadata/camera_settings_test.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      796 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/tests/metadata/command_line_test.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      668 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/tests/metadata/error_test.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2809 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/tests/metadata/leader_test.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      635 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/tests/metadata/offline_test.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      819 2023-04-15 17:31:55.000000 sprocket_carball-0.8.2/carball/tests/read_pandas_test.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:09:39.069509 sprocket_carball-0.8.2/carball/tests/stats/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:56.000000 sprocket_carball-0.8.2/carball/tests/stats/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     6280 2023-04-15 17:31:56.000000 sprocket_carball-0.8.2/carball/tests/stats/boost_test.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      494 2023-04-15 17:31:56.000000 sprocket_carball-0.8.2/carball/tests/stats/demo_test.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    16228 2023-04-15 17:31:56.000000 sprocket_carball-0.8.2/carball/tests/stats/dribble_test.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     8308 2023-04-15 17:31:56.000000 sprocket_carball-0.8.2/carball/tests/stats/dropshot_test.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2911 2023-04-15 17:31:56.000000 sprocket_carball-0.8.2/carball/tests/stats/fifty_fifty_test.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     6753 2023-04-15 17:31:56.000000 sprocket_carball-0.8.2/carball/tests/stats/hit_test.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     5648 2023-04-15 17:31:56.000000 sprocket_carball-0.8.2/carball/tests/stats/kickoff_test.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    10956 2023-04-15 17:31:56.000000 sprocket_carball-0.8.2/carball/tests/stats/rumble_test.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      814 2023-04-15 17:31:56.000000 sprocket_carball-0.8.2/carball/tests/stats/team_test.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      574 2023-04-15 17:31:56.000000 sprocket_carball-0.8.2/carball/tests/tiles_test.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    12330 2023-04-15 17:31:56.000000 sprocket_carball-0.8.2/carball/tests/utils.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      375 2023-04-15 17:31:56.000000 sprocket_carball-0.8.2/init.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)       62 2023-04-16 23:09:05.000000 sprocket_carball-0.8.2/requirements.txt
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)       38 2023-04-16 23:09:39.073509 sprocket_carball-0.8.2/setup.cfg
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1963 2023-04-16 23:09:16.000000 sprocket_carball-0.8.2/setup.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:09:39.069509 sprocket_carball-0.8.2/sprocket_carball.egg-info/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     6396 2023-04-16 23:09:38.000000 sprocket_carball-0.8.2/sprocket_carball.egg-info/PKG-INFO
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     8464 2023-04-16 23:09:38.000000 sprocket_carball-0.8.2/sprocket_carball.egg-info/SOURCES.txt
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)        1 2023-04-16 23:09:38.000000 sprocket_carball-0.8.2/sprocket_carball.egg-info/dependency_links.txt
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)       54 2023-04-16 23:09:38.000000 sprocket_carball-0.8.2/sprocket_carball.egg-info/entry_points.txt
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)       61 2023-04-16 23:09:38.000000 sprocket_carball-0.8.2/sprocket_carball.egg-info/requires.txt
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)       14 2023-04-16 23:09:38.000000 sprocket_carball-0.8.2/sprocket_carball.egg-info/top_level.txt
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:09:39.069509 sprocket_carball-0.8.2/utils/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:56.000000 sprocket_carball-0.8.2/utils/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2544 2023-04-15 17:31:56.000000 sprocket_carball-0.8.2/utils/create_proto.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2610 2023-04-15 17:31:56.000000 sprocket_carball-0.8.2/utils/import_fixer.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:13:01.245394 sprocket_carball-0.8.3/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        2 2023-04-16 06:27:02.000000 sprocket_carball-0.8.3/CARBALL_VERSION
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    11357 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/LICENSE
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      198 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/MANIFEST.in
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      552 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/NOTICE
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     6488 2023-04-16 23:13:01.245394 sprocket_carball-0.8.3/PKG-INFO
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     6131 2023-04-16 23:11:46.000000 sprocket_carball-0.8.3/README.md
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:13:01.193394 sprocket_carball-0.8.3/carball/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      223 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/__init__.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:13:01.193394 sprocket_carball-0.8.3/carball/analysis/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        2 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/PROTOBUF_VERSION
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    17254 2023-04-16 06:18:49.000000 sprocket_carball-0.8.3/carball/analysis/analysis_manager.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:13:01.193394 sprocket_carball-0.8.3/carball/analysis/cleaner/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/cleaner/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1383 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/cleaner/cleaner.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2295 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/cleaner/frame_cleaner.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:13:01.193394 sprocket_carball-0.8.3/carball/analysis/constants/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/constants/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      815 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/constants/basic_math.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     5721 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/constants/dropshot.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     6198 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/constants/field_constants.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1187 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/constants/playlist.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:13:01.193394 sprocket_carball-0.8.3/carball/analysis/events/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/events/__init__.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:13:01.193394 sprocket_carball-0.8.3/carball/analysis/events/boost_pad_detection/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/events/boost_pad_detection/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3707 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/events/boost_pad_detection/pickup_analysis.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:13:01.193394 sprocket_carball-0.8.3/carball/analysis/events/bump_detection/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/events/bump_detection/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1277 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/events/bump_detection/bump_analysis.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    15118 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/events/carry_detection.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:13:01.193394 sprocket_carball-0.8.3/carball/analysis/events/dropshot/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/events/dropshot/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1386 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/events/dropshot/ball.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      935 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/events/dropshot/damage.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     5568 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/events/event_creator.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:13:01.197394 sprocket_carball-0.8.3/carball/analysis/events/fifty_fifty/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/events/fifty_fifty/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     7419 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/events/fifty_fifty/fifty_analysis.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:13:01.197394 sprocket_carball-0.8.3/carball/analysis/events/hit_detection/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/events/hit_detection/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    11653 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/events/hit_detection/base_hit.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    11223 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/events/hit_detection/hit_analysis.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:13:01.197394 sprocket_carball-0.8.3/carball/analysis/events/hit_detection/hitbox/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    41555 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/events/hit_detection/hitbox/Vehicle Specifications v1.39 - Hitboxes, Handling.xlsx
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/events/hit_detection/hitbox/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1662 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/events/hit_detection/hitbox/car.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1973 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/events/hit_detection/hitbox/hitbox.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:13:01.197394 sprocket_carball-0.8.3/carball/analysis/events/hit_pressure/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/events/hit_pressure/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3373 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/events/hit_pressure/pressure_analysis.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:13:01.197394 sprocket_carball-0.8.3/carball/analysis/events/kickoff_detection/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/events/kickoff_detection/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    10002 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/events/kickoff_detection/kickoff_analysis.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:13:01.197394 sprocket_carball-0.8.3/carball/analysis/saltie_game/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/saltie_game/__init__.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:13:01.201394 sprocket_carball-0.8.3/carball/analysis/saltie_game/metadata/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      459 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/saltie_game/metadata/ApiDemo.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2531 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/saltie_game/metadata/ApiGame.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      383 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/saltie_game/metadata/ApiGoal.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      479 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/saltie_game/metadata/ApiMutators.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1473 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/saltie_game/metadata/ApiPlayer.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1406 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/saltie_game/metadata/ApiPlayerCameraSettings.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3124 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/saltie_game/metadata/ApiPlayerLoadout.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      681 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/saltie_game/metadata/ApiTeam.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/saltie_game/metadata/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     4703 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/saltie_game/saltie_game.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:13:01.201394 sprocket_carball-0.8.3/carball/analysis/simulator/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/simulator/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    11609 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/simulator/ball_simulator.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      855 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/simulator/bounce.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      238 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/simulator/map_constants.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:13:01.205394 sprocket_carball-0.8.3/carball/analysis/stats/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/stats/__init__.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:13:01.205394 sprocket_carball-0.8.3/carball/analysis/stats/ball_forward/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/stats/ball_forward/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1023 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/stats/ball_forward/distance_hit_ball_forward.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:13:01.205394 sprocket_carball-0.8.3/carball/analysis/stats/boost/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/stats/boost/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     6918 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/stats/boost/boost.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:13:01.205394 sprocket_carball-0.8.3/carball/analysis/stats/controls/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/stats/controls/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2829 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/stats/controls/controls.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:13:01.205394 sprocket_carball-0.8.3/carball/analysis/stats/demos/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/stats/demos/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1623 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/stats/demos/demos.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:13:01.205394 sprocket_carball-0.8.3/carball/analysis/stats/dribbles/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/stats/dribbles/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3342 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/stats/dribbles/ball_carry.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:13:01.209394 sprocket_carball-0.8.3/carball/analysis/stats/dropshot/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      343 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/stats/dropshot/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2082 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/stats/dropshot/ball_phase_times.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3902 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/stats/dropshot/damage.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2575 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/stats/dropshot/goals.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:13:01.209394 sprocket_carball-0.8.3/carball/analysis/stats/kickoffs/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/stats/kickoffs/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2211 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/stats/kickoffs/kickoff_stat.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:13:01.209394 sprocket_carball-0.8.3/carball/analysis/stats/possession/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/stats/possession/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3521 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/stats/possession/ball_distances.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    10214 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/stats/possession/per_possession.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2982 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/stats/possession/possession.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2243 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/stats/possession/turnovers.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:13:01.209394 sprocket_carball-0.8.3/carball/analysis/stats/rumble/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/stats/rumble/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3475 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/stats/rumble/goals.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     8977 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/stats/rumble/rumble.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     4033 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/stats/stats.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3336 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/stats/stats_list.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3851 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/stats/stats_manager.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:13:01.213394 sprocket_carball-0.8.3/carball/analysis/stats/tendencies/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/stats/tendencies/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1330 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/stats/tendencies/averages.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1583 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/stats/tendencies/hit_counts.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     6969 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/stats/tendencies/positional_tendencies.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2777 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/stats/tendencies/relative_position_tendencies.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1962 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/stats/tendencies/speed_tendencies.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     6502 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/stats/tendencies/team_tendencies.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:13:01.213394 sprocket_carball-0.8.3/carball/analysis/stats/utils/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/stats/utils/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1708 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/stats/utils/pandas_utils.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:13:01.213394 sprocket_carball-0.8.3/carball/analysis/utils/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/utils/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      316 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/utils/json_encoder.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1974 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/utils/numpy_manager.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2050 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/utils/pandas_manager.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      374 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/utils/proto_manager.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1265 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/analysis/utils/split_location.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2558 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/command_line.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:13:01.217394 sprocket_carball-0.8.3/carball/controls/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/controls/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2203 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/controls/controls.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3427 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/controls/rotations.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2586 2023-04-16 23:12:44.000000 sprocket_carball-0.8.3/carball/decompile_replays.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:13:01.217394 sprocket_carball-0.8.3/carball/extras/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/extras/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1770 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/extras/per_goal_analysis.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:13:01.181394 sprocket_carball-0.8.3/carball/generated/
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:13:01.217394 sprocket_carball-0.8.3/carball/generated/api/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 06:27:31.000000 sprocket_carball-0.8.3/carball/generated/api/__init__.py
+-rw-------   0 jacbaile  (1000) jacbaile  (1000)     5076 2023-04-16 06:27:31.000000 sprocket_carball-0.8.3/carball/generated/api/game_pb2.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:13:01.221394 sprocket_carball-0.8.3/carball/generated/api/metadata/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 06:27:31.000000 sprocket_carball-0.8.3/carball/generated/api/metadata/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     4653 2023-04-16 06:27:31.000000 sprocket_carball-0.8.3/carball/generated/api/metadata/camera_settings_pb2.py
+-rw-------   0 jacbaile  (1000) jacbaile  (1000)    19305 2023-04-16 06:27:31.000000 sprocket_carball-0.8.3/carball/generated/api/metadata/game_metadata_pb2.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3635 2023-04-16 06:27:31.000000 sprocket_carball-0.8.3/carball/generated/api/metadata/mutators_pb2.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    12482 2023-04-16 06:27:31.000000 sprocket_carball-0.8.3/carball/generated/api/metadata/player_loadout_pb2.py
+-rw-------   0 jacbaile  (1000) jacbaile  (1000)     2397 2023-04-16 06:27:31.000000 sprocket_carball-0.8.3/carball/generated/api/party_pb2.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1793 2023-04-16 06:27:31.000000 sprocket_carball-0.8.3/carball/generated/api/player_id_pb2.py
+-rw-------   0 jacbaile  (1000) jacbaile  (1000)     8237 2023-04-16 06:27:31.000000 sprocket_carball-0.8.3/carball/generated/api/player_pb2.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:13:01.225394 sprocket_carball-0.8.3/carball/generated/api/stats/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 06:27:31.000000 sprocket_carball-0.8.3/carball/generated/api/stats/__init__.py
+-rw-------   0 jacbaile  (1000) jacbaile  (1000)     3714 2023-04-16 06:27:31.000000 sprocket_carball-0.8.3/carball/generated/api/stats/ball_stats_pb2.py
+-rw-------   0 jacbaile  (1000) jacbaile  (1000)     1383 2023-04-16 06:27:31.000000 sprocket_carball-0.8.3/carball/generated/api/stats/data_frame_pb2.py
+-rw-------   0 jacbaile  (1000) jacbaile  (1000)    18134 2023-04-16 06:27:31.000000 sprocket_carball-0.8.3/carball/generated/api/stats/dropshot_pb2.py
+-rw-------   0 jacbaile  (1000) jacbaile  (1000)    31534 2023-04-16 06:27:31.000000 sprocket_carball-0.8.3/carball/generated/api/stats/events_pb2.py
+-rw-------   0 jacbaile  (1000) jacbaile  (1000)     5766 2023-04-16 06:27:31.000000 sprocket_carball-0.8.3/carball/generated/api/stats/extra_mode_stats_pb2.py
+-rw-------   0 jacbaile  (1000) jacbaile  (1000)     6701 2023-04-16 06:27:31.000000 sprocket_carball-0.8.3/carball/generated/api/stats/game_stats_pb2.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1837 2023-04-16 06:27:31.000000 sprocket_carball-0.8.3/carball/generated/api/stats/goal_pb2.py
+-rw-------   0 jacbaile  (1000) jacbaile  (1000)    18809 2023-04-16 06:27:31.000000 sprocket_carball-0.8.3/carball/generated/api/stats/kickoff_pb2.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     7823 2023-04-16 06:27:31.000000 sprocket_carball-0.8.3/carball/generated/api/stats/per_possession_stats_pb2.py
+-rw-------   0 jacbaile  (1000) jacbaile  (1000)    34767 2023-04-16 06:27:31.000000 sprocket_carball-0.8.3/carball/generated/api/stats/player_stats_pb2.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     7450 2023-04-16 06:27:31.000000 sprocket_carball-0.8.3/carball/generated/api/stats/rumble_pb2.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    21715 2023-04-16 06:27:31.000000 sprocket_carball-0.8.3/carball/generated/api/stats/stats_pb2.py
+-rw-------   0 jacbaile  (1000) jacbaile  (1000)     7909 2023-04-16 06:27:31.000000 sprocket_carball-0.8.3/carball/generated/api/stats/team_stats_pb2.py
+-rw-------   0 jacbaile  (1000) jacbaile  (1000)     3568 2023-04-16 06:27:31.000000 sprocket_carball-0.8.3/carball/generated/api/team_pb2.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:13:01.225394 sprocket_carball-0.8.3/carball/generated/binaries/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 06:27:31.000000 sprocket_carball-0.8.3/carball/generated/binaries/__init__.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:13:01.229394 sprocket_carball-0.8.3/carball/json_parser/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/json_parser/__init__.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:13:01.233394 sprocket_carball-0.8.3/carball/json_parser/actor/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      435 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/json_parser/actor/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1649 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/json_parser/actor/ball.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1210 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/json_parser/actor/base.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     4316 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/json_parser/actor/boost.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1053 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/json_parser/actor/camera.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3497 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/json_parser/actor/car.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1719 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/json_parser/actor/dropshot.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1034 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/json_parser/actor/game_event.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      388 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/json_parser/actor/game_info.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1386 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/json_parser/actor/jump.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     4207 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/json_parser/actor/player.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1122 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/json_parser/actor/rumble.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      466 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/json_parser/actor/team.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3761 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/json_parser/actor_parsing.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1374 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/json_parser/bots.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2021 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/json_parser/dropshot.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    12747 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/json_parser/frame_parser.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    13147 2023-04-16 06:04:04.000000 sprocket_carball-0.8.3/carball/json_parser/game.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1614 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/json_parser/game_info.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      932 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/json_parser/goal.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    11640 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/json_parser/player.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:13:01.233394 sprocket_carball-0.8.3/carball/json_parser/sanity_check/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/json_parser/sanity_check/__init__.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:13:01.233394 sprocket_carball-0.8.3/carball/json_parser/sanity_check/base_checks/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/json_parser/sanity_check/base_checks/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1261 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/json_parser/sanity_check/base_checks/base_check.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      117 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/json_parser/sanity_check/base_checks/game_check.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      298 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/json_parser/sanity_check/base_checks/player_check.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:13:01.233394 sprocket_carball-0.8.3/carball/json_parser/sanity_check/checks/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/json_parser/sanity_check/checks/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      496 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/json_parser/sanity_check/checks/ball_data_frame_check.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1037 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/json_parser/sanity_check/checks/player_attributes_check.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      813 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/json_parser/sanity_check/checks/player_data_frame_check.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:13:01.233394 sprocket_carball-0.8.3/carball/json_parser/sanity_check/errors/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/json_parser/sanity_check/errors/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      275 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/json_parser/sanity_check/errors/errors.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1459 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/json_parser/sanity_check/sanity_check.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1195 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/json_parser/team.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:13:01.237394 sprocket_carball-0.8.3/carball/tests/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/tests/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3666 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/tests/analysis_test.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:13:01.237394 sprocket_carball-0.8.3/carball/tests/benchmarking/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/tests/benchmarking/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1577 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/tests/benchmarking/benchmarking.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      124 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/tests/conftest.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:13:01.237394 sprocket_carball-0.8.3/carball/tests/docs/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/tests/docs/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1610 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/tests/docs/data_frame_docs.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2641 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/tests/export_test.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2791 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/tests/game_creation_test.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:13:01.241394 sprocket_carball-0.8.3/carball/tests/metadata/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/tests/metadata/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1100 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/tests/metadata/camera_settings_test.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      796 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/tests/metadata/command_line_test.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      668 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/tests/metadata/error_test.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2809 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/tests/metadata/leader_test.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      635 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/tests/metadata/offline_test.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      819 2023-04-15 17:31:55.000000 sprocket_carball-0.8.3/carball/tests/read_pandas_test.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:13:01.245394 sprocket_carball-0.8.3/carball/tests/stats/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:56.000000 sprocket_carball-0.8.3/carball/tests/stats/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     6280 2023-04-15 17:31:56.000000 sprocket_carball-0.8.3/carball/tests/stats/boost_test.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      494 2023-04-15 17:31:56.000000 sprocket_carball-0.8.3/carball/tests/stats/demo_test.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    16228 2023-04-15 17:31:56.000000 sprocket_carball-0.8.3/carball/tests/stats/dribble_test.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     8308 2023-04-15 17:31:56.000000 sprocket_carball-0.8.3/carball/tests/stats/dropshot_test.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2911 2023-04-15 17:31:56.000000 sprocket_carball-0.8.3/carball/tests/stats/fifty_fifty_test.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     6753 2023-04-15 17:31:56.000000 sprocket_carball-0.8.3/carball/tests/stats/hit_test.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     5648 2023-04-15 17:31:56.000000 sprocket_carball-0.8.3/carball/tests/stats/kickoff_test.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    10956 2023-04-15 17:31:56.000000 sprocket_carball-0.8.3/carball/tests/stats/rumble_test.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      814 2023-04-15 17:31:56.000000 sprocket_carball-0.8.3/carball/tests/stats/team_test.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      574 2023-04-15 17:31:56.000000 sprocket_carball-0.8.3/carball/tests/tiles_test.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    12330 2023-04-15 17:31:56.000000 sprocket_carball-0.8.3/carball/tests/utils.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      375 2023-04-15 17:31:56.000000 sprocket_carball-0.8.3/init.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)       62 2023-04-16 23:09:05.000000 sprocket_carball-0.8.3/requirements.txt
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)       38 2023-04-16 23:13:01.245394 sprocket_carball-0.8.3/setup.cfg
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1963 2023-04-16 23:12:54.000000 sprocket_carball-0.8.3/setup.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:13:01.245394 sprocket_carball-0.8.3/sprocket_carball.egg-info/
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     6488 2023-04-16 23:13:01.000000 sprocket_carball-0.8.3/sprocket_carball.egg-info/PKG-INFO
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     8464 2023-04-16 23:13:01.000000 sprocket_carball-0.8.3/sprocket_carball.egg-info/SOURCES.txt
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)        1 2023-04-16 23:13:01.000000 sprocket_carball-0.8.3/sprocket_carball.egg-info/dependency_links.txt
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)       54 2023-04-16 23:13:01.000000 sprocket_carball-0.8.3/sprocket_carball.egg-info/entry_points.txt
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)       61 2023-04-16 23:13:01.000000 sprocket_carball-0.8.3/sprocket_carball.egg-info/requires.txt
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)       14 2023-04-16 23:13:01.000000 sprocket_carball-0.8.3/sprocket_carball.egg-info/top_level.txt
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-16 23:13:01.245394 sprocket_carball-0.8.3/utils/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:56.000000 sprocket_carball-0.8.3/utils/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2544 2023-04-15 17:31:56.000000 sprocket_carball-0.8.3/utils/create_proto.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2610 2023-04-15 17:31:56.000000 sprocket_carball-0.8.3/utils/import_fixer.py
```

### Comparing `sprocket_carball-0.8.2/LICENSE` & `sprocket_carball-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/NOTICE` & `sprocket_carball-0.8.3/NOTICE`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/PKG-INFO` & `sprocket_carball-0.8.3/sprocket_carball.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sprocket_carball
-Version: 0.8.2
+Name: sprocket-carball
+Version: 0.8.3
 Summary: Rocket League replay parsing and analysis.
 Home-page: https://github.com/SprocketBot/carball
 Author: Sprocket Dev Team
 Author-email: asaxplayinghorse@gmail.com
 License: Apache 2.0
 Keywords: rocket-league
 Description-Content-Type: text/markdown
@@ -51,14 +51,21 @@
 git clone https://github.com/SprocketBot/carball
 cd carball/
 ./utils/install_protobuf.sh
 python init.py
 sudo python setup.py install
 ```
 
+Finally, to publish the package on PyPI
+
+```
+python setup.py sdist
+twine upload dist/*
+```
+
 ##### Mac
 In MacOS Catalina, zsh replaced bash as the default shell, which may cause permission issues when trying to run `install-protoc.sh` in the above fashion. Simply invoking bash should resolve this issue, like so:
 ```
 git clone https://github.com/SprocketBot/carball
 cd carball/
 bash ./_travis/install-protoc.sh
 python init.py
```

### Comparing `sprocket_carball-0.8.2/README.md` & `sprocket_carball-0.8.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,21 @@
 git clone https://github.com/SprocketBot/carball
 cd carball/
 ./utils/install_protobuf.sh
 python init.py
 sudo python setup.py install
 ```
 
+Finally, to publish the package on PyPI
+
+```
+python setup.py sdist
+twine upload dist/*
+```
+
 ##### Mac
 In MacOS Catalina, zsh replaced bash as the default shell, which may cause permission issues when trying to run `install-protoc.sh` in the above fashion. Simply invoking bash should resolve this issue, like so:
 ```
 git clone https://github.com/SprocketBot/carball
 cd carball/
 bash ./_travis/install-protoc.sh
 python init.py
```

### Comparing `sprocket_carball-0.8.2/carball/analysis/analysis_manager.py` & `sprocket_carball-0.8.3/carball/analysis/analysis_manager.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/analysis/cleaner/cleaner.py` & `sprocket_carball-0.8.3/carball/analysis/cleaner/cleaner.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/analysis/cleaner/frame_cleaner.py` & `sprocket_carball-0.8.3/carball/analysis/cleaner/frame_cleaner.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/analysis/constants/basic_math.py` & `sprocket_carball-0.8.3/carball/analysis/constants/basic_math.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/analysis/constants/dropshot.py` & `sprocket_carball-0.8.3/carball/analysis/constants/dropshot.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/analysis/constants/field_constants.py` & `sprocket_carball-0.8.3/carball/analysis/constants/field_constants.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/analysis/constants/playlist.py` & `sprocket_carball-0.8.3/carball/analysis/constants/playlist.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/analysis/events/boost_pad_detection/pickup_analysis.py` & `sprocket_carball-0.8.3/carball/analysis/events/boost_pad_detection/pickup_analysis.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/analysis/events/bump_detection/bump_analysis.py` & `sprocket_carball-0.8.3/carball/analysis/events/bump_detection/bump_analysis.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/analysis/events/carry_detection.py` & `sprocket_carball-0.8.3/carball/analysis/events/carry_detection.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/analysis/events/dropshot/ball.py` & `sprocket_carball-0.8.3/carball/analysis/events/dropshot/ball.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/analysis/events/dropshot/damage.py` & `sprocket_carball-0.8.3/carball/analysis/events/dropshot/damage.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/analysis/events/event_creator.py` & `sprocket_carball-0.8.3/carball/analysis/events/event_creator.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/analysis/events/fifty_fifty/fifty_analysis.py` & `sprocket_carball-0.8.3/carball/analysis/events/fifty_fifty/fifty_analysis.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/analysis/events/hit_detection/base_hit.py` & `sprocket_carball-0.8.3/carball/analysis/events/hit_detection/base_hit.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/analysis/events/hit_detection/hit_analysis.py` & `sprocket_carball-0.8.3/carball/analysis/events/hit_detection/hit_analysis.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/analysis/events/hit_detection/hitbox/Vehicle Specifications v1.39 - Hitboxes, Handling.xlsx` & `sprocket_carball-0.8.3/carball/analysis/events/hit_detection/hitbox/Vehicle Specifications v1.39 - Hitboxes, Handling.xlsx`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/analysis/events/hit_detection/hitbox/car.py` & `sprocket_carball-0.8.3/carball/analysis/events/hit_detection/hitbox/car.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/analysis/events/hit_detection/hitbox/hitbox.py` & `sprocket_carball-0.8.3/carball/analysis/events/hit_detection/hitbox/hitbox.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/analysis/events/hit_pressure/pressure_analysis.py` & `sprocket_carball-0.8.3/carball/analysis/events/hit_pressure/pressure_analysis.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/analysis/events/kickoff_detection/kickoff_analysis.py` & `sprocket_carball-0.8.3/carball/analysis/events/kickoff_detection/kickoff_analysis.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/analysis/saltie_game/metadata/ApiGame.py` & `sprocket_carball-0.8.3/carball/analysis/saltie_game/metadata/ApiGame.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/analysis/saltie_game/metadata/ApiPlayer.py` & `sprocket_carball-0.8.3/carball/analysis/saltie_game/metadata/ApiPlayer.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/analysis/saltie_game/metadata/ApiPlayerCameraSettings.py` & `sprocket_carball-0.8.3/carball/analysis/saltie_game/metadata/ApiPlayerCameraSettings.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/analysis/saltie_game/metadata/ApiPlayerLoadout.py` & `sprocket_carball-0.8.3/carball/analysis/saltie_game/metadata/ApiPlayerLoadout.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/analysis/saltie_game/metadata/ApiTeam.py` & `sprocket_carball-0.8.3/carball/analysis/saltie_game/metadata/ApiTeam.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/analysis/saltie_game/saltie_game.py` & `sprocket_carball-0.8.3/carball/analysis/saltie_game/saltie_game.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/analysis/simulator/ball_simulator.py` & `sprocket_carball-0.8.3/carball/analysis/simulator/ball_simulator.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/analysis/simulator/bounce.py` & `sprocket_carball-0.8.3/carball/analysis/simulator/bounce.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/analysis/stats/ball_forward/distance_hit_ball_forward.py` & `sprocket_carball-0.8.3/carball/analysis/stats/ball_forward/distance_hit_ball_forward.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/analysis/stats/boost/boost.py` & `sprocket_carball-0.8.3/carball/analysis/stats/boost/boost.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/analysis/stats/controls/controls.py` & `sprocket_carball-0.8.3/carball/analysis/stats/controls/controls.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/analysis/stats/demos/demos.py` & `sprocket_carball-0.8.3/carball/analysis/stats/demos/demos.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/analysis/stats/dribbles/ball_carry.py` & `sprocket_carball-0.8.3/carball/analysis/stats/dribbles/ball_carry.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/analysis/stats/dropshot/ball_phase_times.py` & `sprocket_carball-0.8.3/carball/analysis/stats/dropshot/ball_phase_times.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/analysis/stats/dropshot/damage.py` & `sprocket_carball-0.8.3/carball/analysis/stats/dropshot/damage.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/analysis/stats/dropshot/goals.py` & `sprocket_carball-0.8.3/carball/analysis/stats/dropshot/goals.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/analysis/stats/kickoffs/kickoff_stat.py` & `sprocket_carball-0.8.3/carball/analysis/stats/kickoffs/kickoff_stat.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/analysis/stats/possession/ball_distances.py` & `sprocket_carball-0.8.3/carball/analysis/stats/possession/ball_distances.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/analysis/stats/possession/per_possession.py` & `sprocket_carball-0.8.3/carball/analysis/stats/possession/per_possession.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/analysis/stats/possession/possession.py` & `sprocket_carball-0.8.3/carball/analysis/stats/possession/possession.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/analysis/stats/possession/turnovers.py` & `sprocket_carball-0.8.3/carball/analysis/stats/possession/turnovers.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/analysis/stats/rumble/goals.py` & `sprocket_carball-0.8.3/carball/analysis/stats/rumble/goals.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/analysis/stats/rumble/rumble.py` & `sprocket_carball-0.8.3/carball/analysis/stats/rumble/rumble.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/analysis/stats/stats.py` & `sprocket_carball-0.8.3/carball/analysis/stats/stats.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/analysis/stats/stats_list.py` & `sprocket_carball-0.8.3/carball/analysis/stats/stats_list.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/analysis/stats/stats_manager.py` & `sprocket_carball-0.8.3/carball/analysis/stats/stats_manager.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/analysis/stats/tendencies/averages.py` & `sprocket_carball-0.8.3/carball/analysis/stats/tendencies/averages.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/analysis/stats/tendencies/hit_counts.py` & `sprocket_carball-0.8.3/carball/analysis/stats/tendencies/hit_counts.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/analysis/stats/tendencies/positional_tendencies.py` & `sprocket_carball-0.8.3/carball/analysis/stats/tendencies/positional_tendencies.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/analysis/stats/tendencies/relative_position_tendencies.py` & `sprocket_carball-0.8.3/carball/analysis/stats/tendencies/relative_position_tendencies.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/analysis/stats/tendencies/speed_tendencies.py` & `sprocket_carball-0.8.3/carball/analysis/stats/tendencies/speed_tendencies.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/analysis/stats/tendencies/team_tendencies.py` & `sprocket_carball-0.8.3/carball/analysis/stats/tendencies/team_tendencies.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/analysis/stats/utils/pandas_utils.py` & `sprocket_carball-0.8.3/carball/analysis/stats/utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/analysis/utils/numpy_manager.py` & `sprocket_carball-0.8.3/carball/analysis/utils/numpy_manager.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/analysis/utils/pandas_manager.py` & `sprocket_carball-0.8.3/carball/analysis/utils/pandas_manager.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/analysis/utils/split_location.py` & `sprocket_carball-0.8.3/carball/analysis/utils/split_location.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/command_line.py` & `sprocket_carball-0.8.3/carball/command_line.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/controls/controls.py` & `sprocket_carball-0.8.3/carball/controls/controls.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/controls/rotations.py` & `sprocket_carball-0.8.3/carball/controls/rotations.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/decompile_replays.py` & `sprocket_carball-0.8.3/carball/decompile_replays.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 import os
-from boxcars_py import parse_replay
+from sprocket_boxcars_py import parse_replay
 
 from carball.analysis.analysis_manager import AnalysisManager
 from carball.controls.controls import ControlsCreator
 from carball.extras.per_goal_analysis import PerGoalAnalysis
 from carball.json_parser.game import Game
 from carball.json_parser.sanity_check.sanity_check import SanityChecker
 
@@ -51,15 +51,16 @@
     # get_controls(game)  # TODO: enable and optimise.
     if sanity_check is not None:
         sanity_check.check_game(game)
     if analysis_per_goal:
         analysis = PerGoalAnalysis(game)
     else:
         analysis = AnalysisManager(game)
-    analysis.create_analysis(calculate_intensive_events=calculate_intensive_events, clean=clean)
+    analysis.create_analysis(
+        calculate_intensive_events=calculate_intensive_events, clean=clean)
 
     if controls is not None:
         controls.get_controls(game)
 
     return analysis
```

### Comparing `sprocket_carball-0.8.2/carball/extras/per_goal_analysis.py` & `sprocket_carball-0.8.3/carball/extras/per_goal_analysis.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/generated/api/game_pb2.py` & `sprocket_carball-0.8.3/carball/generated/api/game_pb2.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/generated/api/metadata/camera_settings_pb2.py` & `sprocket_carball-0.8.3/carball/generated/api/metadata/camera_settings_pb2.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/generated/api/metadata/game_metadata_pb2.py` & `sprocket_carball-0.8.3/carball/generated/api/metadata/game_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/generated/api/metadata/mutators_pb2.py` & `sprocket_carball-0.8.3/carball/generated/api/metadata/mutators_pb2.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/generated/api/metadata/player_loadout_pb2.py` & `sprocket_carball-0.8.3/carball/generated/api/metadata/player_loadout_pb2.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/generated/api/party_pb2.py` & `sprocket_carball-0.8.3/carball/generated/api/party_pb2.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/generated/api/player_id_pb2.py` & `sprocket_carball-0.8.3/carball/generated/api/player_id_pb2.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/generated/api/player_pb2.py` & `sprocket_carball-0.8.3/carball/generated/api/player_pb2.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/generated/api/stats/ball_stats_pb2.py` & `sprocket_carball-0.8.3/carball/generated/api/stats/ball_stats_pb2.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/generated/api/stats/data_frame_pb2.py` & `sprocket_carball-0.8.3/carball/generated/api/stats/data_frame_pb2.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/generated/api/stats/dropshot_pb2.py` & `sprocket_carball-0.8.3/carball/generated/api/stats/dropshot_pb2.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/generated/api/stats/events_pb2.py` & `sprocket_carball-0.8.3/carball/generated/api/stats/events_pb2.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/generated/api/stats/extra_mode_stats_pb2.py` & `sprocket_carball-0.8.3/carball/generated/api/stats/extra_mode_stats_pb2.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/generated/api/stats/game_stats_pb2.py` & `sprocket_carball-0.8.3/carball/generated/api/stats/game_stats_pb2.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/generated/api/stats/goal_pb2.py` & `sprocket_carball-0.8.3/carball/generated/api/stats/goal_pb2.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/generated/api/stats/kickoff_pb2.py` & `sprocket_carball-0.8.3/carball/generated/api/stats/kickoff_pb2.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/generated/api/stats/per_possession_stats_pb2.py` & `sprocket_carball-0.8.3/carball/generated/api/stats/per_possession_stats_pb2.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/generated/api/stats/player_stats_pb2.py` & `sprocket_carball-0.8.3/carball/generated/api/stats/player_stats_pb2.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/generated/api/stats/rumble_pb2.py` & `sprocket_carball-0.8.3/carball/generated/api/stats/rumble_pb2.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/generated/api/stats/stats_pb2.py` & `sprocket_carball-0.8.3/carball/generated/api/stats/stats_pb2.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/generated/api/stats/team_stats_pb2.py` & `sprocket_carball-0.8.3/carball/generated/api/stats/team_stats_pb2.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/generated/api/team_pb2.py` & `sprocket_carball-0.8.3/carball/generated/api/team_pb2.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/json_parser/actor/ball.py` & `sprocket_carball-0.8.3/carball/json_parser/actor/ball.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/json_parser/actor/base.py` & `sprocket_carball-0.8.3/carball/json_parser/actor/base.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/json_parser/actor/boost.py` & `sprocket_carball-0.8.3/carball/json_parser/actor/boost.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/json_parser/actor/camera.py` & `sprocket_carball-0.8.3/carball/json_parser/actor/camera.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/json_parser/actor/car.py` & `sprocket_carball-0.8.3/carball/json_parser/actor/car.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/json_parser/actor/dropshot.py` & `sprocket_carball-0.8.3/carball/json_parser/actor/dropshot.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/json_parser/actor/game_event.py` & `sprocket_carball-0.8.3/carball/json_parser/actor/game_event.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/json_parser/actor/jump.py` & `sprocket_carball-0.8.3/carball/json_parser/actor/jump.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/json_parser/actor/player.py` & `sprocket_carball-0.8.3/carball/json_parser/actor/player.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/json_parser/actor/rumble.py` & `sprocket_carball-0.8.3/carball/json_parser/actor/rumble.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/json_parser/actor_parsing.py` & `sprocket_carball-0.8.3/carball/json_parser/actor_parsing.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/json_parser/bots.py` & `sprocket_carball-0.8.3/carball/json_parser/bots.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/json_parser/dropshot.py` & `sprocket_carball-0.8.3/carball/json_parser/dropshot.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/json_parser/frame_parser.py` & `sprocket_carball-0.8.3/carball/json_parser/frame_parser.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/json_parser/game.py` & `sprocket_carball-0.8.3/carball/json_parser/game.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/json_parser/game_info.py` & `sprocket_carball-0.8.3/carball/json_parser/game_info.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/json_parser/goal.py` & `sprocket_carball-0.8.3/carball/json_parser/goal.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/json_parser/player.py` & `sprocket_carball-0.8.3/carball/json_parser/player.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/json_parser/sanity_check/base_checks/base_check.py` & `sprocket_carball-0.8.3/carball/json_parser/sanity_check/base_checks/base_check.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/json_parser/sanity_check/checks/player_attributes_check.py` & `sprocket_carball-0.8.3/carball/json_parser/sanity_check/checks/player_attributes_check.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/json_parser/sanity_check/checks/player_data_frame_check.py` & `sprocket_carball-0.8.3/carball/json_parser/sanity_check/checks/player_data_frame_check.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/json_parser/sanity_check/sanity_check.py` & `sprocket_carball-0.8.3/carball/json_parser/sanity_check/sanity_check.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/json_parser/team.py` & `sprocket_carball-0.8.3/carball/json_parser/team.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/tests/analysis_test.py` & `sprocket_carball-0.8.3/carball/tests/analysis_test.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/tests/benchmarking/benchmarking.py` & `sprocket_carball-0.8.3/carball/tests/benchmarking/benchmarking.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/tests/docs/data_frame_docs.py` & `sprocket_carball-0.8.3/carball/tests/docs/data_frame_docs.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/tests/export_test.py` & `sprocket_carball-0.8.3/carball/tests/export_test.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/tests/game_creation_test.py` & `sprocket_carball-0.8.3/carball/tests/game_creation_test.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/tests/metadata/camera_settings_test.py` & `sprocket_carball-0.8.3/carball/tests/metadata/camera_settings_test.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/tests/metadata/command_line_test.py` & `sprocket_carball-0.8.3/carball/tests/metadata/command_line_test.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/tests/metadata/error_test.py` & `sprocket_carball-0.8.3/carball/tests/metadata/error_test.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/tests/metadata/leader_test.py` & `sprocket_carball-0.8.3/carball/tests/metadata/leader_test.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/tests/metadata/offline_test.py` & `sprocket_carball-0.8.3/carball/tests/metadata/offline_test.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/tests/read_pandas_test.py` & `sprocket_carball-0.8.3/carball/tests/read_pandas_test.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/tests/stats/boost_test.py` & `sprocket_carball-0.8.3/carball/tests/stats/boost_test.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/tests/stats/dribble_test.py` & `sprocket_carball-0.8.3/carball/tests/stats/dribble_test.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/tests/stats/dropshot_test.py` & `sprocket_carball-0.8.3/carball/tests/stats/dropshot_test.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/tests/stats/fifty_fifty_test.py` & `sprocket_carball-0.8.3/carball/tests/stats/fifty_fifty_test.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/tests/stats/hit_test.py` & `sprocket_carball-0.8.3/carball/tests/stats/hit_test.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/tests/stats/kickoff_test.py` & `sprocket_carball-0.8.3/carball/tests/stats/kickoff_test.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/tests/stats/rumble_test.py` & `sprocket_carball-0.8.3/carball/tests/stats/rumble_test.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/tests/stats/team_test.py` & `sprocket_carball-0.8.3/carball/tests/stats/team_test.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/tests/tiles_test.py` & `sprocket_carball-0.8.3/carball/tests/tiles_test.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/carball/tests/utils.py` & `sprocket_carball-0.8.3/carball/tests/utils.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/setup.py` & `sprocket_carball-0.8.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         initialize_project()
         # this needs to be last
         install.run(self)
 
 
 setup(
     name='sprocket_carball',
-    version='0.8.2',
+    version='0.8.3',
     packages=setuptools.find_packages(),
     include_package_data=True,
     install_requires=['pandas', 'protobuf==3.6.1',
                       'xlrd==1.1.0', 'numpy', 'sprocket-boxcars-py'],
     url='https://github.com/SprocketBot/carball',
     keywords=['rocket-league'],
     license='Apache 2.0',
```

### Comparing `sprocket_carball-0.8.2/sprocket_carball.egg-info/PKG-INFO` & `sprocket_carball-0.8.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sprocket-carball
-Version: 0.8.2
+Name: sprocket_carball
+Version: 0.8.3
 Summary: Rocket League replay parsing and analysis.
 Home-page: https://github.com/SprocketBot/carball
 Author: Sprocket Dev Team
 Author-email: asaxplayinghorse@gmail.com
 License: Apache 2.0
 Keywords: rocket-league
 Description-Content-Type: text/markdown
@@ -51,14 +51,21 @@
 git clone https://github.com/SprocketBot/carball
 cd carball/
 ./utils/install_protobuf.sh
 python init.py
 sudo python setup.py install
 ```
 
+Finally, to publish the package on PyPI
+
+```
+python setup.py sdist
+twine upload dist/*
+```
+
 ##### Mac
 In MacOS Catalina, zsh replaced bash as the default shell, which may cause permission issues when trying to run `install-protoc.sh` in the above fashion. Simply invoking bash should resolve this issue, like so:
 ```
 git clone https://github.com/SprocketBot/carball
 cd carball/
 bash ./_travis/install-protoc.sh
 python init.py
```

### Comparing `sprocket_carball-0.8.2/sprocket_carball.egg-info/SOURCES.txt` & `sprocket_carball-0.8.3/sprocket_carball.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/utils/create_proto.py` & `sprocket_carball-0.8.3/utils/create_proto.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.2/utils/import_fixer.py` & `sprocket_carball-0.8.3/utils/import_fixer.py`

 * *Files identical despite different names*

