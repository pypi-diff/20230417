# Comparing `tmp/auraboros-0.8.0a0.tar.gz` & `tmp/auraboros-0.9.0a0.tar.gz`

## Comparing `auraboros-0.8.0a0.tar` & `auraboros-0.9.0a0.tar`

### file list

```diff
@@ -1,81 +1,86 @@
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/Pipfile
--rw-r--r--   0        0        0    63551 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/Pipfile.lock
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/README.md
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/.vscode/launch.json
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/.vscode/settings.json
--rw-r--r--   0        0        0  1171204 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/assets/fonts/misaki_gothic.ttf
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/assets/imgs/enemy_a.piskel
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/assets/imgs/enemy_a.png
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/assets/imgs/enemy_b.piskel
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/assets/imgs/enemy_b.png
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/assets/imgs/explosion_a.piskel
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/assets/imgs/explosion_a.png
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/assets/imgs/explosion_b.png
--rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/assets/imgs/fighter_a.piskel
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/assets/imgs/fighter_a.png
--rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/assets/imgs/icon.ico
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/assets/imgs/laser1.png
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/assets/imgs/scoutdisk.piskel
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/assets/imgs/scoutdisk.png
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/assets/imgs/shot1.piskel
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/assets/imgs/shot1.png
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/assets/imgs/shot2.piskel
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/assets/imgs/shot2.png
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/assets/imgs/shot3.png
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/assets/imgs/shot4.png
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/assets/imgs/shot5.piskel
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/assets/imgs/shot5.png
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/assets/imgs/shot6.piskel
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/assets/imgs/shot6.png
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/assets/imgs/shot7.png
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/assets/imgs/shot8.png
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/assets/imgs/terrain_rock.png
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/assets/level_data/debug1/level.json
--rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/assets/level_data/debug1/patterns.json
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/assets/level_data/stage1/level.json
--rw-r--r--   0        0        0     3498 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/assets/level_data/stage1/patterns.json
--rw-r--r--   0        0        0    78688 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/assets/sounds/deathse2.wav
--rw-r--r--   0        0        0   191648 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/assets/sounds/deathse3.wav
--rw-r--r--   0        0        0    28264 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/assets/sounds/deathse4.wav
--rw-r--r--   0        0        0    21586 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/assets/sounds/explosion1.wav
--rw-r--r--   0        0        0   352960 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/assets/sounds/explosion2.wav
--rw-r--r--   0        0        0   150572 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/assets/sounds/laser.wav
--rw-r--r--   0        0        0   150610 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/assets/sounds/laser2.wav
--rw-r--r--   0        0        0    21360 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/assets/sounds/shot1.wav
--rw-r--r--   0        0        0  5177872 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/assets/sounds/music/bgm1.wav
--rw-r--r--   0        0        0   789664 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/assets/sounds/music/gameover.wav
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/docs/Makefile
--rwxr-xr-x   0        0        0      769 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/docs/make.bat
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/docs/source/conf.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/docs/source/index.rst
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/docs/source/locale/de/LC_MESSAGES/index.po
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/docs/source/locale/ja/LC_MESSAGES/index.po
--rw-r--r--   0        0        0    43792 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/examples/eightrail.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/examples/example.py
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/examples/helloworld/engine.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/examples/helloworld/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/src/auraboros/__init__.py
--rw-r--r--   0        0        0     5203 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/src/auraboros/animation.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/src/auraboros/engine.py
--rw-r--r--   0        0        0    10881 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/src/auraboros/entity.py
--rw-r--r--   0        0        0     5626 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/src/auraboros/gameinput.py
--rw-r--r--   0        0        0     9333 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/src/auraboros/gamelevel.py
--rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/src/auraboros/gamescene.py
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/src/auraboros/gametext.py
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/src/auraboros/global_.py
--rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/src/auraboros/schedule.py
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/src/auraboros/sound.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/src/auraboros/terrain.py
--rw-r--r--   0        0        0    15249 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/src/auraboros/ui.py
--rw-r--r--   0        0        0     4649 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/src/auraboros/utilities.py
--rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/src/debugs/gamemenu.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/src/debugs/init_for_dev.py
--rw-r--r--   0        0        0     5500 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/src/debugs/keyboard.py
--rw-r--r--   0        0        0  1171204 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/src/debugs/assets/fonts/misaki_gothic.ttf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/tests/__init__.py
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/tests/test_gameinput.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/tests/test_ui.py
--rw-r--r--   0        0        0     4254 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/LICENSE
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/pyproject.toml
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 auraboros-0.8.0a0/PKG-INFO
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/Pipfile
+-rw-r--r--   0        0        0    63551 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/Pipfile.lock
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/README.md
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/.vscode/launch.json
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/.vscode/settings.json
+-rw-r--r--   0        0        0  1171204 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/fonts/misaki_gothic.ttf
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/imgs/enemy_a.piskel
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/imgs/enemy_a.png
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/imgs/enemy_b.piskel
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/imgs/enemy_b.png
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/imgs/explosion_a.piskel
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/imgs/explosion_a.png
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/imgs/explosion_b.png
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/imgs/fighter_a.piskel
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/imgs/fighter_a.png
+-rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/imgs/icon.ico
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/imgs/laser1.png
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/imgs/scoutdisk.piskel
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/imgs/scoutdisk.png
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/imgs/shot1.piskel
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/imgs/shot1.png
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/imgs/shot2.piskel
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/imgs/shot2.png
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/imgs/shot3.png
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/imgs/shot4.png
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/imgs/shot5.piskel
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/imgs/shot5.png
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/imgs/shot6.piskel
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/imgs/shot6.png
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/imgs/shot7.png
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/imgs/shot8.png
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/imgs/terrain_rock.png
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/level_data/debug1/level.json
+-rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/level_data/debug1/patterns.json
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/level_data/stage1/level.json
+-rw-r--r--   0        0        0     3498 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/level_data/stage1/patterns.json
+-rw-r--r--   0        0        0    78688 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/sounds/deathse2.wav
+-rw-r--r--   0        0        0   191648 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/sounds/deathse3.wav
+-rw-r--r--   0        0        0    28264 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/sounds/deathse4.wav
+-rw-r--r--   0        0        0    21586 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/sounds/explosion1.wav
+-rw-r--r--   0        0        0   352960 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/sounds/explosion2.wav
+-rw-r--r--   0        0        0   150572 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/sounds/laser.wav
+-rw-r--r--   0        0        0   150610 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/sounds/laser2.wav
+-rw-r--r--   0        0        0    21360 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/sounds/shot1.wav
+-rw-r--r--   0        0        0  5177872 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/sounds/music/bgm1.wav
+-rw-r--r--   0        0        0   789664 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/sounds/music/gameover.wav
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/docs/Makefile
+-rwxr-xr-x   0        0        0      769 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/docs/make.bat
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/docs/source/conf.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/docs/source/index.rst
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/docs/source/locale/de/LC_MESSAGES/index.po
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/docs/source/locale/ja/LC_MESSAGES/index.po
+-rw-r--r--   0        0        0    43792 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/examples/eightrail.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/examples/example.py
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/examples/helloworld/engine.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/examples/helloworld/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/src/auraboros/__init__.py
+-rw-r--r--   0        0        0     5391 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/src/auraboros/animation.py
+-rw-r--r--   0        0        0     5196 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/src/auraboros/animation2.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/src/auraboros/engine.py
+-rw-r--r--   0        0        0    10881 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/src/auraboros/entity.py
+-rw-r--r--   0        0        0     5827 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/src/auraboros/gameinput.py
+-rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/src/auraboros/gameinput2.py
+-rw-r--r--   0        0        0     9333 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/src/auraboros/gamelevel.py
+-rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/src/auraboros/gamescene.py
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/src/auraboros/gametext.py
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/src/auraboros/global_.py
+-rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/src/auraboros/schedule.py
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/src/auraboros/schedule2.py
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/src/auraboros/sound.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/src/auraboros/terrain.py
+-rw-r--r--   0        0        0    15249 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/src/auraboros/ui.py
+-rw-r--r--   0        0        0     4649 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/src/auraboros/utilities.py
+-rw-r--r--   0        0        0     6401 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/src/debugs/animation.py
+-rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/src/debugs/gamemenu.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/src/debugs/init_for_dev.py
+-rw-r--r--   0        0        0     5500 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/src/debugs/keyboard.py
+-rw-r--r--   0        0        0  1171204 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/src/debugs/assets/fonts/misaki_gothic.ttf
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/src/debugs/assets/imgs/testsprite.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/tests/__init__.py
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/tests/test_gameinput.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/tests/test_ui.py
+-rw-r--r--   0        0        0     4254 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/LICENSE
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/pyproject.toml
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/PKG-INFO
```

### Comparing `auraboros-0.8.0a0/Pipfile.lock` & `auraboros-0.9.0a0/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `auraboros-0.8.0a0/.vscode/launch.json` & `auraboros-0.9.0a0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `auraboros-0.8.0a0/assets/fonts/misaki_gothic.ttf` & `auraboros-0.9.0a0/assets/fonts/misaki_gothic.ttf`

 * *Files identical despite different names*

### Comparing `auraboros-0.8.0a0/assets/imgs/enemy_a.piskel` & `auraboros-0.9.0a0/assets/imgs/enemy_a.piskel`

 * *Files identical despite different names*

### Comparing `auraboros-0.8.0a0/assets/imgs/enemy_a.png` & `auraboros-0.9.0a0/assets/imgs/enemy_a.png`

 * *Files identical despite different names*

### Comparing `auraboros-0.8.0a0/assets/imgs/enemy_b.piskel` & `auraboros-0.9.0a0/assets/imgs/enemy_b.piskel`

 * *Files identical despite different names*

### Comparing `auraboros-0.8.0a0/assets/imgs/enemy_b.png` & `auraboros-0.9.0a0/assets/imgs/enemy_b.png`

 * *Files identical despite different names*

### Comparing `auraboros-0.8.0a0/assets/imgs/explosion_a.piskel` & `auraboros-0.9.0a0/assets/imgs/explosion_a.piskel`

 * *Files identical despite different names*

### Comparing `auraboros-0.8.0a0/assets/imgs/explosion_a.png` & `auraboros-0.9.0a0/assets/imgs/explosion_a.png`

 * *Files identical despite different names*

### Comparing `auraboros-0.8.0a0/assets/imgs/explosion_b.png` & `auraboros-0.9.0a0/assets/imgs/explosion_b.png`

 * *Files identical despite different names*

### Comparing `auraboros-0.8.0a0/assets/imgs/fighter_a.piskel` & `auraboros-0.9.0a0/assets/imgs/fighter_a.piskel`

 * *Files identical despite different names*

### Comparing `auraboros-0.8.0a0/assets/imgs/fighter_a.png` & `auraboros-0.9.0a0/assets/imgs/fighter_a.png`

 * *Files identical despite different names*

### Comparing `auraboros-0.8.0a0/assets/imgs/icon.ico` & `auraboros-0.9.0a0/assets/imgs/icon.ico`

 * *Files identical despite different names*

### Comparing `auraboros-0.8.0a0/assets/imgs/scoutdisk.piskel` & `auraboros-0.9.0a0/assets/imgs/scoutdisk.piskel`

 * *Files identical despite different names*

### Comparing `auraboros-0.8.0a0/assets/imgs/scoutdisk.png` & `auraboros-0.9.0a0/assets/imgs/scoutdisk.png`

 * *Files identical despite different names*

### Comparing `auraboros-0.8.0a0/assets/imgs/shot6.piskel` & `auraboros-0.9.0a0/assets/imgs/shot6.piskel`

 * *Files identical despite different names*

### Comparing `auraboros-0.8.0a0/assets/imgs/terrain_rock.png` & `auraboros-0.9.0a0/assets/imgs/terrain_rock.png`

 * *Files identical despite different names*

### Comparing `auraboros-0.8.0a0/assets/level_data/debug1/patterns.json` & `auraboros-0.9.0a0/assets/level_data/debug1/patterns.json`

 * *Files identical despite different names*

### Comparing `auraboros-0.8.0a0/assets/level_data/stage1/patterns.json` & `auraboros-0.9.0a0/assets/level_data/stage1/patterns.json`

 * *Files identical despite different names*

### Comparing `auraboros-0.8.0a0/assets/sounds/deathse2.wav` & `auraboros-0.9.0a0/assets/sounds/deathse2.wav`

 * *Files identical despite different names*

### Comparing `auraboros-0.8.0a0/assets/sounds/deathse3.wav` & `auraboros-0.9.0a0/assets/sounds/deathse3.wav`

 * *Files identical despite different names*

### Comparing `auraboros-0.8.0a0/assets/sounds/deathse4.wav` & `auraboros-0.9.0a0/assets/sounds/deathse4.wav`

 * *Files identical despite different names*

### Comparing `auraboros-0.8.0a0/assets/sounds/explosion1.wav` & `auraboros-0.9.0a0/assets/sounds/explosion1.wav`

 * *Files identical despite different names*

### Comparing `auraboros-0.8.0a0/assets/sounds/explosion2.wav` & `auraboros-0.9.0a0/assets/sounds/explosion2.wav`

 * *Files identical despite different names*

### Comparing `auraboros-0.8.0a0/assets/sounds/laser.wav` & `auraboros-0.9.0a0/assets/sounds/laser.wav`

 * *Files identical despite different names*

### Comparing `auraboros-0.8.0a0/assets/sounds/laser2.wav` & `auraboros-0.9.0a0/assets/sounds/laser2.wav`

 * *Files identical despite different names*

### Comparing `auraboros-0.8.0a0/assets/sounds/shot1.wav` & `auraboros-0.9.0a0/assets/sounds/shot1.wav`

 * *Files identical despite different names*

### Comparing `auraboros-0.8.0a0/assets/sounds/music/bgm1.wav` & `auraboros-0.9.0a0/assets/sounds/music/bgm1.wav`

 * *Files identical despite different names*

### Comparing `auraboros-0.8.0a0/assets/sounds/music/gameover.wav` & `auraboros-0.9.0a0/assets/sounds/music/gameover.wav`

 * *Files identical despite different names*

### Comparing `auraboros-0.8.0a0/docs/Makefile` & `auraboros-0.9.0a0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `auraboros-0.8.0a0/docs/make.bat` & `auraboros-0.9.0a0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `auraboros-0.8.0a0/docs/source/conf.py` & `auraboros-0.9.0a0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `auraboros-0.8.0a0/docs/source/locale/de/LC_MESSAGES/index.po` & `auraboros-0.9.0a0/docs/source/locale/de/LC_MESSAGES/index.po`

 * *Files identical despite different names*

### Comparing `auraboros-0.8.0a0/docs/source/locale/ja/LC_MESSAGES/index.po` & `auraboros-0.9.0a0/docs/source/locale/ja/LC_MESSAGES/index.po`

 * *Files identical despite different names*

### Comparing `auraboros-0.8.0a0/examples/eightrail.py` & `auraboros-0.9.0a0/examples/eightrail.py`

 * *Files identical despite different names*

### Comparing `auraboros-0.8.0a0/examples/helloworld/engine.py` & `auraboros-0.9.0a0/examples/helloworld/engine.py`

 * *Files identical despite different names*

### Comparing `auraboros-0.8.0a0/src/auraboros/animation.py` & `auraboros-0.9.0a0/src/auraboros/animation.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,17 +31,17 @@
         self._anim_frames = value
         self.image = self.anim_frames[self.anim_frame_id]
 
     @property
     def frame_num(self):
         return len(self.anim_frames)
 
-    def draw_while_playing(self, screen: pygame.surface.Surface):
-        if self.is_playing:
-            screen.blit(self.image, self.rect)
+    # def draw_while_playing(self, screen: pygame.surface.Surface):
+    #     if self.is_playing:
+    #         screen.blit(self.image, self.rect)
 
     @schedule_instance_method_interval(
         "anim_interval",
     )
     def update_frame_at_interval(self):
         self.update_frame()
 
@@ -63,15 +63,15 @@
     def set_current_frame_to_image(self):
         self.image = self.anim_frames[self.anim_frame_id]
 
     def set_current_frame_id(self, id: int):
         self.anim_frame_id = id
 
     def let_play_animation(self):
-        """Active update and draw function"""
+        """Active update and draw function WITH RESET animation"""
         self.is_playing = True
         self.is_finished = False
         self.reset_animation()
 
     def let_continue_animation(self):
         """Active update and draw function without reset animation"""
         self.is_playing = True
@@ -80,21 +80,25 @@
         self.is_playing = False
 
     def reset_animation(self):
         self.anim_frame_id = 0
         self._anim_frame_progress = 0
         self._loop_counter = 0
         self._do_reset_anim_interval_counter = True
+        self.set_current_frame_to_image()
 
-    def draw(self, screen):
-        self.draw_while_playing(screen)
+    # def draw(self, screen):
+    #     self.draw_while_playing(screen)
 
     def update(self, dt):
         self.update_frame_at_interval()
 
+    def render_current_frame(self) -> pygame.surface.Surface:
+        return self.anim_frames[self.anim_frame_id]
+
 
 class AnimationFactory(MutableMapping):
     """
     Examples:
         class ExampleAnimation(AnimationImage):
             pass
         a = AnimationFactory()
```

### Comparing `auraboros-0.8.0a0/src/auraboros/engine.py` & `auraboros-0.9.0a0/src/auraboros/engine.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,32 +3,32 @@
 
 # from typing import TYPE_CHECKING
 # if TYPE_CHECKING:
 
 import pygame
 
 from .global_ import init  # noqa
-from .schedule import IntervalCounter
+from .schedule2 import Schedule
 from .gamescene import SceneManager
 from . import global_
 
 
 clock = pygame.time.Clock()
 
 
 def run(scene_manager: SceneManager, fps_num=60):
     fps = fps_num
     running = True
     while running:
-        dt = clock.tick(fps)/1000  # dt means delta time
-
+        clock.tick(fps)
+        Schedule.execute()
         global_.screen.fill((0, 0, 0))
         for event in pygame.event.get():
             running = scene_manager.event(event)
 
-        scene_manager.update(dt)
+        scene_manager.update()
         scene_manager.draw(global_.screen)
         pygame.transform.scale(global_.screen, global_.w_size_unscaled,
                                pygame.display.get_surface())
         pygame.display.update()
-        IntervalCounter.tick(dt)
+        # IntervalCounter.tick(dt)
     pygame.quit()
```

### Comparing `auraboros-0.8.0a0/src/auraboros/entity.py` & `auraboros-0.9.0a0/src/auraboros/entity.py`

 * *Files identical despite different names*

### Comparing `auraboros-0.8.0a0/src/auraboros/gameinput.py` & `auraboros-0.9.0a0/src/auraboros/gameinput.py`

 * *Files 8% similar despite different names*

```diff
@@ -73,15 +73,20 @@
             return self.keyaction_dict[key_const]["keyup"]()
 
     def register_keyaction(
             self,
             key_const,
             delay, interval,
             keydown: Callable = lambda: None, keyup: Callable = lambda: None):
-
+        """
+        Args:
+            key_const: pygame.localsから参照する登録するキーの定数。
+            delay (int): milliseconds
+            interval (int): milliseconds
+        """
         self.keyaction_dict[key_const] = KeyActionItem({
             "keydown": keydown, "keyup": keyup,
             "delay": delay, "interval": interval,
             "is_pressed": False,
             "_delay_counter": 0, "_interval_counter": 0,
             "_first_input_finished": False,
             "keydown_deactivated": False,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `auraboros-0.8.0a0/src/auraboros/gamelevel.py` & `auraboros-0.9.0a0/src/auraboros/gamelevel.py`

 * *Files identical despite different names*

### Comparing `auraboros-0.8.0a0/src/auraboros/gamescene.py` & `auraboros-0.9.0a0/src/auraboros/gamescene.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 
 from dataclasses import dataclass
-from typing import Optional, Union
+# from typing import Optional, Union
 
 import pygame
 
 from .animation import AnimationImage
-from .gameinput import KeyboardManager, Joystick2
+from .gameinput2 import KeyboardManager
 
 
 @dataclass
 class Scene(object):
 
     def __init__(self, manager):
         from .gamelevel import Level
         self.manager = manager
         self.gameworld: Level = None
         self.keyboard: KeyboardManager = KeyboardManager()
-        self._joystick: Joystick2 = None
+        # self._joystick: Joystick2 = None
         self.visual_effects: list[AnimationImage] = []
         attrs_of_class = set(dir(self.__class__)) - set(dir(Scene))
         for attr_name in attrs_of_class:
             attrs_of_object = set(
                 getattr(self, attr_name).__class__.__mro__) - {object, }
             is_gameworld = Level in attrs_of_object
             if is_gameworld:
                 getattr(self, attr_name).scene = self
 
-    @property
-    def joystick(self) -> Optional[Joystick2]:
-        return self._joystick
-
-    @joystick.setter
-    def joystick(self, value: Union[Joystick2, None]):
-        self._joystick = value
+    # @property
+    # def joystick(self) -> Optional[Joystick2]:
+    #     return self._joystick
+
+    # @joystick.setter
+    # def joystick(self, value: Union[Joystick2, None]):
+    #     self._joystick = value
 
     def event(self, event: pygame.event):
         pass
 
     def draw(self, screen: pygame.surface.Surface):
         pass
 
-    def update(self, dt):
+    def update(self, ):
         pass
 
 
 class SceneManager:
     def __init__(self):
         self.scenes: list[Scene] = []
         self._current: int = 0
@@ -62,31 +62,31 @@
         if event.type == pygame.QUIT:
             return False
         if self.current == -1:
             return False
         self.scenes[self.current].event(event)
         if self.scenes[self.current].keyboard.current_setup is not None:
             self.scenes[self.current].keyboard.current_setup.event(event)
-        if self.scenes[self.current].joystick is not None:
-            self.scenes[self.current].joystick.event(event)
+        # if self.scenes[self.current].joystick is not None:
+        #     self.scenes[self.current].joystick.event(event)
         return True
 
     def is_current_scene_has_gameworld(self) -> bool:
         if self.scenes[self.current].gameworld is None:
             return False
         else:
             return True
 
-    def update(self, dt):
-        self.scenes[self.current].update(dt)
+    def update(self):
+        self.scenes[self.current].update()
         if self.is_current_scene_has_gameworld():
             if not self.scenes[self.current].gameworld.pause:
-                [entity.update(dt)
+                [entity.update()
                  for entity in self.scenes[self.current].gameworld.entities]
-        [visual_effect.update(dt)
+        [visual_effect.update()
          for visual_effect in self.scenes[self.current].visual_effects]
 
     def draw(self, screen: pygame.surface.Surface):
         self.scenes[self.current].draw(screen)
         if self.is_current_scene_has_gameworld():
             if not self.scenes[self.current].gameworld.pause:
                 [entity.draw(screen)
```

### Comparing `auraboros-0.8.0a0/src/auraboros/gametext.py` & `auraboros-0.9.0a0/src/auraboros/gametext.py`

 * *Files identical despite different names*

### Comparing `auraboros-0.8.0a0/src/auraboros/global_.py` & `auraboros-0.9.0a0/src/auraboros/global_.py`

 * *Files identical despite different names*

### Comparing `auraboros-0.8.0a0/src/auraboros/schedule.py` & `auraboros-0.9.0a0/src/auraboros/schedule.py`

 * *Files identical despite different names*

### Comparing `auraboros-0.8.0a0/src/auraboros/sound.py` & `auraboros-0.9.0a0/src/auraboros/sound.py`

 * *Files identical despite different names*

### Comparing `auraboros-0.8.0a0/src/auraboros/ui.py` & `auraboros-0.9.0a0/src/auraboros/ui.py`

 * *Files identical despite different names*

### Comparing `auraboros-0.8.0a0/src/auraboros/utilities.py` & `auraboros-0.9.0a0/src/auraboros/utilities.py`

 * *Files identical despite different names*

### Comparing `auraboros-0.8.0a0/src/debugs/gamemenu.py` & `auraboros-0.9.0a0/src/debugs/gamemenu.py`

 * *Files identical despite different names*

### Comparing `auraboros-0.8.0a0/src/debugs/keyboard.py` & `auraboros-0.9.0a0/src/debugs/keyboard.py`

 * *Files identical despite different names*

### Comparing `auraboros-0.8.0a0/src/debugs/assets/fonts/misaki_gothic.ttf` & `auraboros-0.9.0a0/src/debugs/assets/fonts/misaki_gothic.ttf`

 * *Files identical despite different names*

### Comparing `auraboros-0.8.0a0/tests/test_gameinput.py` & `auraboros-0.9.0a0/tests/test_gameinput.py`

 * *Files identical despite different names*

### Comparing `auraboros-0.8.0a0/tests/test_ui.py` & `auraboros-0.9.0a0/tests/test_ui.py`

 * *Files identical despite different names*

### Comparing `auraboros-0.8.0a0/.gitignore` & `auraboros-0.9.0a0/.gitignore`

 * *Files identical despite different names*

### Comparing `auraboros-0.8.0a0/LICENSE` & `auraboros-0.9.0a0/LICENSE`

 * *Files identical despite different names*

